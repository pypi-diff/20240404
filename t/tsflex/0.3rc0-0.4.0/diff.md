# Comparing `tmp/tsflex-0.3rc0.tar.gz` & `tmp/tsflex-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsflex-0.3rc0.tar", max compression
+gzip compressed data, was "tsflex-0.4.0.tar", max compression
```

## Comparing `tsflex-0.3rc0.tar` & `tsflex-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0     1116 2022-08-13 15:11:54.911308 tsflex-0.3rc0/LICENSE
--rw-r--r--   0        0        0     7332 2022-08-13 15:11:54.911308 tsflex-0.3rc0/README.md
--rw-r--r--   0        0        0     1196 2022-08-20 20:37:30.922302 tsflex-0.3rc0/pyproject.toml
--rw-r--r--   0        0        0      552 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/__init__.py
--rw-r--r--   0        0        0      210 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/chunking/__init__.py
--rw-r--r--   0        0        0    14239 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/chunking/chunking.py
--rw-r--r--   0        0        0      741 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/features/__init__.py
--rw-r--r--   0        0        0     5529 2022-08-19 14:43:37.109614 tsflex-0.3rc0/tsflex/features/dynamicstridefc.py
--rw-r--r--   0        0        0    12546 2022-08-20 08:30:47.567050 tsflex-0.3rc0/tsflex/features/feature.py
--rw-r--r--   0        0        0    35794 2022-08-20 19:29:34.213376 tsflex-0.3rc0/tsflex/features/feature_collection.py
--rw-r--r--   0        0        0     4163 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/features/function_wrapper.py
--rw-r--r--   0        0        0    13133 2022-08-14 15:24:36.127422 tsflex-0.3rc0/tsflex/features/integrations.py
--rw-r--r--   0        0        0     5782 2022-08-20 08:30:47.567050 tsflex-0.3rc0/tsflex/features/logger.py
--rw-r--r--   0        0        0      268 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/features/segmenter/__init__.py
--rw-r--r--   0        0        0    30620 2022-08-20 20:34:48.483362 tsflex-0.3rc0/tsflex/features/segmenter/strided_rolling.py
--rw-r--r--   0        0        0     2985 2022-08-20 08:30:47.567050 tsflex-0.3rc0/tsflex/features/segmenter/strided_rolling_factory.py
--rw-r--r--   0        0        0     7784 2022-08-20 19:37:17.164875 tsflex-0.3rc0/tsflex/features/utils.py
--rw-r--r--   0        0        0      477 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/processing/__init__.py
--rw-r--r--   0        0        0     2526 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/processing/logger.py
--rw-r--r--   0        0        0    10981 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/processing/series_pipeline.py
--rw-r--r--   0        0        0    14668 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/processing/series_processor.py
--rw-r--r--   0        0        0     3081 2022-08-13 15:11:55.043307 tsflex-0.3rc0/tsflex/processing/utils.py
--rw-r--r--   0        0        0      106 2022-08-13 15:11:55.047307 tsflex-0.3rc0/tsflex/utils/__init__.py
--rw-r--r--   0        0        0     2044 2022-08-14 15:24:36.127422 tsflex-0.3rc0/tsflex/utils/attribute_parsing.py
--rw-r--r--   0        0        0      513 2022-08-13 15:11:55.047307 tsflex-0.3rc0/tsflex/utils/classes.py
--rw-r--r--   0        0        0     5544 2022-08-14 15:24:36.127422 tsflex-0.3rc0/tsflex/utils/data.py
--rw-r--r--   0        0        0     3288 2022-08-13 15:11:55.047307 tsflex-0.3rc0/tsflex/utils/logging.py
--rw-r--r--   0        0        0     2147 2022-08-13 15:11:55.047307 tsflex-0.3rc0/tsflex/utils/time.py
--rw-r--r--   0        0        0     8403 2022-08-20 20:37:38.744705 tsflex-0.3rc0/setup.py
--rw-r--r--   0        0        0     8334 2022-08-20 20:37:38.745982 tsflex-0.3rc0/PKG-INFO
+-rw-r--r--   0        0        0     1116 2022-08-28 08:28:04.839396 tsflex-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7610 2024-04-04 10:02:10.189904 tsflex-0.4.0/README.md
+-rw-r--r--   0        0        0     3727 2024-04-04 10:10:12.274958 tsflex-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      550 2024-04-04 10:10:26.534989 tsflex-0.4.0/tsflex/__init__.py
+-rw-r--r--   0        0        0      204 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/chunking/__init__.py
+-rw-r--r--   0        0        0    14232 2023-07-27 09:12:06.183647 tsflex-0.4.0/tsflex/chunking/chunking.py
+-rw-r--r--   0        0        0      741 2022-08-28 08:28:05.043403 tsflex-0.4.0/tsflex/features/__init__.py
+-rw-r--r--   0        0        0    12571 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/features/feature.py
+-rw-r--r--   0        0        0    60309 2024-04-04 10:02:10.197904 tsflex-0.4.0/tsflex/features/feature_collection.py
+-rw-r--r--   0        0        0     4915 2023-07-27 09:12:06.183647 tsflex-0.4.0/tsflex/features/function_wrapper.py
+-rw-r--r--   0        0        0    13183 2023-07-27 09:12:06.183647 tsflex-0.4.0/tsflex/features/integrations.py
+-rw-r--r--   0        0        0     6244 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/features/logger.py
+-rw-r--r--   0        0        0      268 2022-10-03 06:35:44.434440 tsflex-0.4.0/tsflex/features/segmenter/__init__.py
+-rw-r--r--   0        0        0    31247 2024-04-04 10:02:10.197904 tsflex-0.4.0/tsflex/features/segmenter/strided_rolling.py
+-rw-r--r--   0        0        0     2980 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/features/segmenter/strided_rolling_factory.py
+-rw-r--r--   0        0        0     9037 2024-04-04 10:02:10.197904 tsflex-0.4.0/tsflex/features/utils.py
+-rw-r--r--   0        0        0      477 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/processing/__init__.py
+-rw-r--r--   0        0        0     2747 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/processing/logger.py
+-rw-r--r--   0        0        0    10979 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/processing/series_pipeline.py
+-rw-r--r--   0        0        0    14744 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/processing/series_processor.py
+-rw-r--r--   0        0        0     3071 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/processing/utils.py
+-rw-r--r--   0        0        0      106 2022-08-28 08:28:05.043403 tsflex-0.4.0/tsflex/utils/__init__.py
+-rw-r--r--   0        0        0     2063 2023-01-20 16:02:23.812887 tsflex-0.4.0/tsflex/utils/attribute_parsing.py
+-rw-r--r--   0        0        0      513 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/utils/classes.py
+-rw-r--r--   0        0        0     5644 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/utils/data.py
+-rw-r--r--   0        0        0     3288 2023-01-20 16:02:31.572985 tsflex-0.4.0/tsflex/utils/logging.py
+-rw-r--r--   0        0        0     2148 2023-01-20 16:02:31.576985 tsflex-0.4.0/tsflex/utils/time.py
+-rw-r--r--   0        0        0     8949 1970-01-01 00:00:00.000000 tsflex-0.4.0/PKG-INFO
```

### Comparing `tsflex-0.3rc0/LICENSE` & `tsflex-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsflex-0.3rc0/README.md` & `tsflex-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # <p align="center"> <a href="https://predict-idlab.github.io/tsflex"><img alt="tsflex" src="https://raw.githubusercontent.com/predict-idlab/tsflex/main/docs/_static/logo.png" width="66%"></a></p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/tsflex.svg)](https://pypi.org/project/tsflex/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/tsflex?label=conda)](https://anaconda.org/conda-forge/tsflex)
 [![support-version](https://img.shields.io/pypi/pyversions/tsflex)](https://img.shields.io/pypi/pyversions/tsflex)
 [![codecov](https://img.shields.io/codecov/c/github/predict-idlab/tsflex?logo=codecov)](https://codecov.io/gh/predict-idlab/tsflex)
-[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/tsflex?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/tsflex/context:python)
-[![Downloads](https://pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex)
+[![CodeQL](https://github.com/predict-idlab/tsflex/actions/workflows/codeql.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/codeql.yml)
+[![Downloads](https://static.pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
 [![Documentation](https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml)
 [![Testing](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml)
 
 <!-- ![Downloads](https://img.shields.io/conda/dn/conda-forge/tsflex?logo=anaconda) -->
 
-> *tsflex* is a toolkit for _**flex**ible **t**ime **s**eries_ [processing](https://predict-idlab.github.io/tsflex/processing) & [feature extraction](https://predict-idlab.github.io/tsflex/features), that is efficient and makes few assumptions about sequence data.
+> _tsflex_ is a toolkit for _**flex**ible **t**ime **s**eries_ [processing](https://predict-idlab.github.io/tsflex/processing) & [feature extraction](https://predict-idlab.github.io/tsflex/features), that is efficient and makes few assumptions about sequence data.
 
 #### Useful links
 
 - [Paper](https://www.sciencedirect.com/science/article/pii/S2352711021001904)
 - [Documentation](https://predict-idlab.github.io/tsflex/)
 - [Example (machine learning) notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples)
 
 #### Installation
 
-| | command|
-|:--------------|:--------------|
-| [**pip**](https://pypi.org/project/tsflex/) | `pip install tsflex` | 
+|                                                      | command                               |
+| :--------------------------------------------------- | :------------------------------------ |
+| [**pip**](https://pypi.org/project/tsflex/)          | `pip install tsflex`                  |
 | [**conda**](https://anaconda.org/conda-forge/tsflex) | `conda install -c conda-forge tsflex` |
 
 ## Usage
 
 _tsflex_ is built to be intuitive, so we encourage you to copy-paste this code and toy with some parameters!
 
 ### <a href="https://predict-idlab.github.io/tsflex/features/#getting-started">Feature extraction</a>
@@ -59,50 +59,53 @@
 | signal | columns | sample rate |
 |:-------|:-------|------------------:|
 | df_tmp | ["TMP"]| 4Hz |
 | df_acc | ["ACC_x", "ACC_y", "ACC_z" ]| 32Hz |
 | df_ibi | ["IBI"]| irregularly sampled |
 
 ### <a href="https://predict-idlab.github.io/tsflex/processing/index.html#getting-started">Processing</a>
+
 [Working example in our docs](https://predict-idlab.github.io/tsflex/processing/index.html#working-example)
 
 ## Why tsflex? ✨
 
-* `Flexible`:
-    * handles multivariate/multimodal time series
-    * versatile function support
-      => **integrates** with many packages for:
-      * processing (e.g., [scipy.signal](https://docs.scipy.org/doc/scipy/reference/tutorial/signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/tsa.html#time-series-filters))
-      * feature extraction (e.g., [numpy](https://numpy.org/doc/stable/reference/routines.html), [scipy.stats](https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [seglearn](https://dmbee.github.io/seglearn/feature_functions.html)¹, [tsfresh](https://tsfresh.readthedocs.io/en/latest/text/list_of_features.html)¹, [tsfel](https://tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)¹)
-    * feature extraction handles **multiple strides & window sizes**
-* `Efficient`:<br>
-  * view-based operations for processing & feature extraction => extremely **low memory peak** & **fast execution time**<br>
-    * see: [feature extraction benchmark visualization](https://predict-idlab.github.io/tsflex/#benchmark)
-* `Intuitive`:<br>
-  * maintains the sequence-index of the data
-  * feature extraction constructs interpretable output column names
-  * intuitive API
-* `Few assumptions` about the sequence data:
-  * no assumptions about sampling rate
-  * able to deal with multivariate asynchronous data<br>i.e. data with small time-offsets between the modalities
-* `Advanced functionalities`:
-  * apply [FeatureCollection.**reduce**](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.reduce) after feature selection for faster inference
-  * use **function execution time logging** to discover processing and feature extraction bottlenecks
-  * embedded [SeriesPipeline](http://predict-idlab.github.io/tsflex/processing/#tsflex.processing.SeriesPipeline.serialize) & [FeatureCollection](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.serialize) **serialization**
-  * time series [**chunking**](https://predict-idlab.github.io/tsflex/chunking/index.html)
+- `Flexible`:
+  - handles multivariate/multimodal time series
+  - versatile function support
+    => **integrates** with many packages for:
+    - processing (e.g., [scipy.signal](https://docs.scipy.org/doc/scipy/reference/tutorial/signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/tsa.html#time-series-filters))
+    - feature extraction (e.g., [numpy](https://numpy.org/doc/stable/reference/routines.html), [scipy.stats](https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [antropy](https://raphaelvallat.com/antropy/build/html/api.html), [nolds](https://cschoel.github.io/nolds/nolds.html#algorithms), [seglearn](https://dmbee.github.io/seglearn/feature_functions.html)¹, [tsfresh](https://tsfresh.readthedocs.io/en/latest/text/list_of_features.html)¹, [tsfel](https://tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)¹)
+  - feature extraction handles **multiple strides & window sizes**
+- `Efficient`:<br>
+  - view-based operations for processing & feature extraction => extremely **low memory peak** & **fast execution time**<br>
+    - see: [feature extraction benchmark visualization](https://predict-idlab.github.io/tsflex/#benchmark)
+- `Intuitive`:<br>
+  - maintains the sequence-index of the data
+  - feature extraction constructs interpretable output column names
+  - intuitive API
+- `Few assumptions` about the sequence data:
+  - no assumptions about sampling rate
+  - able to deal with multivariate asynchronous data<br>i.e. data with small time-offsets between the modalities
+- `Advanced functionalities`:
+  - apply [FeatureCollection.**reduce**](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.reduce) after feature selection for faster inference
+  - use **function execution time logging** to discover processing and feature extraction bottlenecks
+  - embedded [SeriesPipeline](http://predict-idlab.github.io/tsflex/processing/#tsflex.processing.SeriesPipeline.serialize) & [FeatureCollection](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.serialize) **serialization**
+  - time series [**chunking**](https://predict-idlab.github.io/tsflex/chunking/index.html)
 
 ¹ These integrations are shown in [integration-example notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples).
+
 ## Future work 🔨
 
-* scikit-learn integration for both processing and feature extraction<br>
+- scikit-learn integration for both processing and feature extraction<br>
   **note**: is actively developed upon [sklearn integration](https://github.com/predict-idlab/tsflex/tree/sklearn_integration) branch.
-* Support time series segmentation (exposing under the hood strided-rolling functionality) - [see this issue](https://github.com/predict-idlab/tsflex/issues/15)
-* Support for multi-indexed dataframes
+- Support time series segmentation (exposing under the hood strided-rolling functionality) - [see this issue](https://github.com/predict-idlab/tsflex/issues/15)
+- Support for multi-indexed dataframes
 
 => Also see the [enhancement issues](https://github.com/predict-idlab/tsflex/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement+)
+
 ## Contributing 👪
 
 We are thrilled to see your contributions to further enhance `tsflex`.<br>
 See [this guide](CONTRIBUTING.md) for more instructions on how to contribute.
 
 ## Referencing our package
```

#### html2text {}

```diff
@@ -2,87 +2,90 @@
                                    _[_t_s_f_l_e_x_]
 [![PyPI Latest Release](https://img.shields.io/pypi/v/tsflex.svg)](https://
 pypi.org/project/tsflex/) [![Conda Latest Release](https://img.shields.io/
 conda/vn/conda-forge/tsflex?label=conda)](https://anaconda.org/conda-forge/
 tsflex) [![support-version](https://img.shields.io/pypi/pyversions/tsflex)]
 (https://img.shields.io/pypi/pyversions/tsflex) [![codecov](https://
 img.shields.io/codecov/c/github/predict-idlab/tsflex?logo=codecov)](https://
-codecov.io/gh/predict-idlab/tsflex) [![Code quality](https://img.shields.io/
-lgtm/grade/python/github/predict-idlab/tsflex?label=code%20quality&logo=lgtm)]
-(https://lgtm.com/projects/g/predict-idlab/tsflex/context:python) [![Downloads]
-(https://pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex) [![PRs
+codecov.io/gh/predict-idlab/tsflex) [![CodeQL](https://github.com/predict-
+idlab/tsflex/actions/workflows/codeql.yml/badge.svg)](https://github.com/
+predict-idlab/tsflex/actions/workflows/codeql.yml) [![Downloads](https://
+static.pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex) [![PRs
 Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
 makeapullrequest.com) [![Documentation](https://github.com/predict-idlab/
 tsflex/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/
 predict-idlab/tsflex/actions/workflows/deploy-docs.yml) [![Testing](https://
 github.com/predict-idlab/tsflex/actions/workflows/test.yml/badge.svg)](https://
-github.com/predict-idlab/tsflex/actions/workflows/test.yml) > *tsflex* is a
+github.com/predict-idlab/tsflex/actions/workflows/test.yml) > _tsflex_ is a
 toolkit for _**flex**ible **t**ime **s**eries_ [processing](https://predict-
 idlab.github.io/tsflex/processing) & [feature extraction](https://predict-
 idlab.github.io/tsflex/features), that is efficient and makes few assumptions
 about sequence data. #### Useful links - [Paper](https://www.sciencedirect.com/
 science/article/pii/S2352711021001904) - [Documentation](https://predict-
 idlab.github.io/tsflex/) - [Example (machine learning) notebooks](https://
 github.com/predict-idlab/tsflex/tree/main/examples) #### Installation | |
-command| |:--------------|:--------------| | [**pip**](https://pypi.org/
-project/tsflex/) | `pip install tsflex` | | [**conda**](https://anaconda.org/
-conda-forge/tsflex) | `conda install -c conda-forge tsflex` | ## Usage _tsflex_
-is built to be intuitive, so we encourage you to copy-paste this code and toy
-with some parameters! ### _F_e_a_t_u_r_e_ _e_x_t_r_a_c_t_i_o_n ```python import pandas as pd;
-import numpy as np; import scipy.stats as ss from tsflex.features import
+command | | :--------------------------------------------------- | :-----------
+------------------------- | | [**pip**](https://pypi.org/project/tsflex/) |
+`pip install tsflex` | | [**conda**](https://anaconda.org/conda-forge/tsflex) |
+`conda install -c conda-forge tsflex` | ## Usage _tsflex_ is built to be
+intuitive, so we encourage you to copy-paste this code and toy with some
+parameters! ### _F_e_a_t_u_r_e_ _e_x_t_r_a_c_t_i_o_n ```python import pandas as pd; import numpy
+as np; import scipy.stats as ss from tsflex.features import
 MultipleFeatureDescriptors, FeatureCollection from tsflex.utils.data import
 load_empatica_data # 1. Load sequence-indexed data (in this case a time-index)
 df_tmp, df_acc, df_ibi = load_empatica_data(['tmp', 'acc', 'ibi']) # 2.
 Construct your feature extraction configuration fc = FeatureCollection
 ( MultipleFeatureDescriptors( functions=[np.min, np.mean, np.std, ss.skew,
 ss.kurtosis], series_names=["TMP", "ACC_x", "ACC_y", "IBI"], windows=["15min",
 "30min"], strides="15min", ) ) # 3. Extract features fc.calculate(data=[df_tmp,
 df_acc, df_ibi], approve_sparsity=True) ``` Note that the feature extraction is
 performed on multivariate data with varying sample rates. | signal | columns |
 sample rate | |:-------|:-------|------------------:| | df_tmp | ["TMP"]| 4Hz |
 | df_acc | ["ACC_x", "ACC_y", "ACC_z" ]| 32Hz | | df_ibi | ["IBI"]| irregularly
 sampled | ### _P_r_o_c_e_s_s_i_n_g [Working example in our docs](https://predict-
 idlab.github.io/tsflex/processing/index.html#working-example) ## Why tsflex?
-â¨ * `Flexible`: * handles multivariate/multimodal time series * versatile
-function support => **integrates** with many packages for: * processing (e.g.,
+â¨ - `Flexible`: - handles multivariate/multimodal time series - versatile
+function support => **integrates** with many packages for: - processing (e.g.,
 [scipy.signal](https://docs.scipy.org/doc/scipy/reference/tutorial/
 signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/
-tsa.html#time-series-filters)) * feature extraction (e.g., [numpy](https://
+tsa.html#time-series-filters)) - feature extraction (e.g., [numpy](https://
 numpy.org/doc/stable/reference/routines.html), [scipy.stats](https://
-docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [seglearn](https://
+docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [antropy](https://
+raphaelvallat.com/antropy/build/html/api.html), [nolds](https://
+cschoel.github.io/nolds/nolds.html#algorithms), [seglearn](https://
 dmbee.github.io/seglearn/feature_functions.html)Â¹, [tsfresh](https://
 tsfresh.readthedocs.io/en/latest/text/list_of_features.html)Â¹, [tsfel](https:/
-/tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)Â¹) * feature
-extraction handles **multiple strides & window sizes** * `Efficient`:
-* view-based operations for processing & feature extraction => extremely **low
+/tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)Â¹) - feature
+extraction handles **multiple strides & window sizes** - `Efficient`:
+- view-based operations for processing & feature extraction => extremely **low
 memory peak** & **fast execution time**
-* see: [feature extraction benchmark visualization](https://predict-
-idlab.github.io/tsflex/#benchmark) * `Intuitive`:
-* maintains the sequence-index of the data * feature extraction constructs
-interpretable output column names * intuitive API * `Few assumptions` about the
-sequence data: * no assumptions about sampling rate * able to deal with
+- see: [feature extraction benchmark visualization](https://predict-
+idlab.github.io/tsflex/#benchmark) - `Intuitive`:
+- maintains the sequence-index of the data - feature extraction constructs
+interpretable output column names - intuitive API - `Few assumptions` about the
+sequence data: - no assumptions about sampling rate - able to deal with
 multivariate asynchronous data
-i.e. data with small time-offsets between the modalities * `Advanced
-functionalities`: * apply [FeatureCollection.**reduce**](https://predict-
+i.e. data with small time-offsets between the modalities - `Advanced
+functionalities`: - apply [FeatureCollection.**reduce**](https://predict-
 idlab.github.io/tsflex/features/
 index.html#tsflex.features.FeatureCollection.reduce) after feature selection
-for faster inference * use **function execution time logging** to discover
-processing and feature extraction bottlenecks * embedded [SeriesPipeline](http:
+for faster inference - use **function execution time logging** to discover
+processing and feature extraction bottlenecks - embedded [SeriesPipeline](http:
 //predict-idlab.github.io/tsflex/processing/
 #tsflex.processing.SeriesPipeline.serialize) & [FeatureCollection](https://
 predict-idlab.github.io/tsflex/features/
-index.html#tsflex.features.FeatureCollection.serialize) **serialization** *
+index.html#tsflex.features.FeatureCollection.serialize) **serialization** -
 time series [**chunking**](https://predict-idlab.github.io/tsflex/chunking/
 index.html) Â¹ These integrations are shown in [integration-example notebooks]
 (https://github.com/predict-idlab/tsflex/tree/main/examples). ## Future work
-ð¨ * scikit-learn integration for both processing and feature extraction
+ð¨ - scikit-learn integration for both processing and feature extraction
 **note**: is actively developed upon [sklearn integration](https://github.com/
-predict-idlab/tsflex/tree/sklearn_integration) branch. * Support time series
+predict-idlab/tsflex/tree/sklearn_integration) branch. - Support time series
 segmentation (exposing under the hood strided-rolling functionality) - [see
-this issue](https://github.com/predict-idlab/tsflex/issues/15) * Support for
+this issue](https://github.com/predict-idlab/tsflex/issues/15) - Support for
 multi-indexed dataframes => Also see the [enhancement issues](https://
 github.com/predict-idlab/tsflex/
 issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement+) ## Contributing ðª We are
 thrilled to see your contributions to further enhance `tsflex`.
 See [this guide](CONTRIBUTING.md) for more instructions on how to contribute.
 ## Referencing our package If you use `tsflex` in a scientific publication, we
 would highly appreciate citing us as: ```bibtex @article
```

### Comparing `tsflex-0.3rc0/tsflex/chunking/chunking.py` & `tsflex-0.4.0/tsflex/chunking/chunking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """(Advanced) tsflex utilities for chunking sequence data."""
 
 __author__ = "Jonas Van Der Donckt"
 
 from datetime import timedelta
-from typing import Dict, List, Union, Tuple, Optional
+from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 
 from ..utils.attribute_parsing import AttributeParser, DataType
 from ..utils.data import to_series_list
 from ..utils.time import parse_time_arg
 
@@ -50,17 +50,17 @@
             for s in series_list
         }
 
     # Assert the names reside in fs_dict
     assert all([str(s.name) in fs_dict for s in series_list])
 
     # Some range asserts
-    assert sub_chunk_overlap.total_seconds() >= 0, f"sub_chunk_overlap_s must be > 0"
+    assert sub_chunk_overlap.total_seconds() >= 0, "sub_chunk_overlap_s must be > 0"
     if max_chunk_dur is not None:
-        assert max_chunk_dur.total_seconds() > 0, f"max_chunk_dur_ must be > 0"
+        assert max_chunk_dur.total_seconds() > 0, "max_chunk_dur_ must be > 0"
 
     # Variable in which the same time-range chunks are stored
     # Each list item can be seen as (t_start_chunk, t_end_chunk, chunk_list)
     same_range_chunks: List[Tuple[pd.Timestamp, pd.Timestamp, List[pd.Series]]] = []
 
     def print_verbose_time(sig, t_begin, t_end, msg=""):
         fmt = "%Y-%m-%d %H:%M"
@@ -123,15 +123,15 @@
         # Set the first and last timestamp to True
         gaps.iloc[[0, -1]] = True
         gaps: List[pd.Timestamp] = series[gaps].index.to_list()
         if verbose:
             print("-" * 10, " detected gaps", "-" * 10)
             print(*gaps, sep="\n")
 
-        for (t_begin_c, t_end_c) in zip(gaps, gaps[1:]):
+        for t_begin_c, t_end_c in zip(gaps, gaps[1:]):
             # The t_end is the t_start of the new time range -> hence [:-1]
             # => cut on [t_start_c(hunk), t_end_c(hunk)[
             sig_chunk = series[t_begin_c:t_end_c]
             if t_end_c < gaps[-1]:
                 # Note: we doe not adjust when t_end_c = gaps[-1]
                 #   (as gaps-[-1] is not really a gap)
                 sig_chunk = sig_chunk[:-1]
@@ -245,37 +245,37 @@
     df_acc  # cols ['ACC_x', 'ACC_y`, 'ACC_z`, 'ACC_SMV`] - 32 Hz
     df_gyro # cols ['gyro_x', 'gyro_y`, 'gyro_z`, 'gyro_area`] - 100 Hz
     chunk_data({'acc': df_acc, 'g': df_gyro}, fs_dict={'acc': 32, 'g': 100})
     ```
     <br>
 
     .. Note::
-        If `chunk_range_margin` / `min_chunk_dur` / `max_chunk_dur` / 
+        If `chunk_range_margin` / `min_chunk_dur` / `max_chunk_dur` /
         `sub_chunk_overlap` is a int/float, it will be interpreted as numerical
         sequence range  and a numerical-indexed `data` will be assumed.
         **These attributes must be all either time-based or numerical and match
         the data its index dtype**
 
     Parameters
     -----------
     data: Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]], Dict[str, pd.DataFrame]]
         The sequence data which will be chunked. Each item in `data` must have a
         monotonically increasing index. We assume that each `item` in data
-        has a _nearly-constant_ sample frequency (when there are no gaps) and all 
+        has a _nearly-constant_ sample frequency (when there are no gaps) and all
         indices have the same dtype.
     fs_dict: Dict[str, int], optional
         The sample frequency dict. If set, this dict must at least withhold all the keys
         from the items in `data`.
         .. note::
             if you passed a **_DataFrame-dict_** (i.e., a dict with key=str;
             value=DataFrame) to `data`, then you can **use** the **corresponding
             dataframe str-key** to describe the `fs` for all the DataFrame its columns
             with the `fs_dict` attribute. See also the example above
     chunk_range_margin: Union[float, str, pd.Timedelta], optional
-        The allowed margin for each `ts` chunk their start and end time to be seen as 
+        The allowed margin for each `ts` chunk their start and end time to be seen as
         same time-range chunks with other `ts`. If `None` the margin will be set as:
 
             2 / min(fs_dict.intersection(data.names).values())
 
         Which is equivalent to twice the min-fs (= max-period) of the passed `data`,
         by default None.\n
         * if `pd.Timedelta`, it will be interpreted as a time-range margin
```

### Comparing `tsflex-0.3rc0/tsflex/features/__init__.py` & `tsflex-0.4.0/tsflex/features/__init__.py`

 * *Files identical despite different names*

### Comparing `tsflex-0.3rc0/tsflex/features/feature.py` & `tsflex-0.4.0/tsflex/features/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,51 +3,51 @@
 
 FeatureDescriptor and MultipleFeatureDescriptors class for creating time-series
 features.
 
 """
 
 import itertools
-from typing import Callable, List, Optional, Union, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from .function_wrapper import FuncWrapper
 from ..utils.attribute_parsing import AttributeParser, DataType
 from ..utils.classes import FrozenClass
 from ..utils.data import to_list, to_tuple
 from ..utils.time import parse_time_arg
+from .function_wrapper import FuncWrapper
 
 
 class FeatureDescriptor(FrozenClass):
     """A FeatureDescriptor object, containing all feature information.
 
     Parameters
     ----------
     function : Union[FuncWrapper, Callable]
         The function that calculates the feature(s).
         The prototype of the function should match: \n
 
             function(*series: Union[np.array, pd.Series])
                 -> Union[Any, List[Any]]
 
-        Note that when the input type is ``pd.Series``, the function should be wrapped in
-        a `FuncWrapper` with `input_type` = ``pd.Series``.
+        Note that when the input type is ``pd.Series``, the function should be wrapped
+          in a `FuncWrapper` with `input_type` = ``pd.Series``.
 
     series_name : Union[str, Tuple[str, ...]]
         The names of the series on which the feature function should be applied.
         This argument should match the `function` its input; \n
         * If `series_name` is a string (or tuple of a single string), then
             `function` should require just one series as input.
         * If `series_name` is a tuple of strings, then `function` should
             require `len(tuple)` series as input **and in exactly the same order**
 
     window : Union[float, str, pd.Timedelta], optional
         The window size. By default None. This argument supports multiple types: \n
-        * If None, the `segment_start_idxs` and `segment_end_idxs` will need to be 
+        * If None, the `segment_start_idxs` and `segment_end_idxs` will need to be
           passed.
         * If the type is an `float` or an `int`, its value represents the series
             - its window **range** when a **non time-indexed** series is passed.
             - its window in **number of samples**, when a **time-indexed** series is
               passed (must then be and `int`)
         * If the window's type is a `pd.Timedelta`, the window size represents
           the window-time-range. The passed data **must have a time-index**.
@@ -55,30 +55,30 @@
           must have a time-index**.
         .. Note::
             - When the `segment_start_idxs` and `segment_end_idxs` are both passed to
               the `FeatureCollection.calculate` method, this window argument is ignored.
               Note that this is the only case when it is allowed to pass None for the
               window argument.
             - When the window argument is None, than the stride argument should be None
-              as well (as it makes no sense to pass a stride value when the window is 
+              as well (as it makes no sense to pass a stride value when the window is
               None).
 
     stride : Union[float, str, pd.Timedelta, List[Union[float, str, pd.Timedelta]]], optional
         The stride size(s). By default None. This argument supports multiple types: \n
         * If None, the stride will need to be passed to `FeatureCollection.calculate`.
         * If the type is an `float` or an `int`, its value represents the series
             - its stride **range** when a **non time-indexed** series is passed.
             - the stride in **number of samples**, when a **time-indexed** series
               is passed (must then be and `int`)
         * If the stride's type is a `pd.Timedelta`, the stride size represents
           the stride-time delta. The passed data **must have a time-index**.
         * If a `str`, it must represent a stride-time-delta-string. The **passed data
           must have a time-index**. \n
-        * If a `List[Union[float, str, pd.Timedelta]]`, then the set intersection of the
-          strides will be used (e.g., stride=[2,3] -> index: 0, 2, 3, 6, 8, 9, ...)
+        * If a `List[Union[float, str, pd.Timedelta]]`, then the set intersection,of the
+          strides will be used (e.g., stride=[2,3] -> index: 0, 2, 3, 4, 6, 8, 9, ...)
         .. Note::
             - The stride argument of `FeatureCollection.calculate` takes precedence over
               this value when set (i.e., not None value for `stride` passed to the
               `calculate` method).
             - The stride argument should be None when the window argument is None (as it
               makes no sense to pass a stride value when the window is None).
 
@@ -247,15 +247,17 @@
 
     """
 
     def __init__(
         self,
         functions: Union[FuncWrapper, Callable, List[Union[FuncWrapper, Callable]]],
         series_names: Union[str, Tuple[str, ...], List[str], List[Tuple[str, ...]]],
-        windows: Optional[Union[float, str, pd.Timedelta, List[Union[float, str, pd.Timedelta]]]] = None,
+        windows: Optional[
+            Union[float, str, pd.Timedelta, List[Union[float, str, pd.Timedelta]]]
+        ] = None,
         strides: Optional[
             Union[float, str, pd.Timedelta, List[Union[float, str, pd.Timedelta]]]
         ] = None,
     ):
         # Cast functions to FuncWrapper, this avoids creating multiple
         # FuncWrapper objects for the same function in the FeatureDescriptor
         def to_func_wrapper(f: Callable):
```

### Comparing `tsflex-0.3rc0/tsflex/features/feature_collection.py` & `tsflex-0.4.0/tsflex/features/feature_collection.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,41 +3,49 @@
 Methods, next to `FeatureCollection.calculate()`, worth looking at: \n
 * `FeatureCollection.serialize()` - serialize the FeatureCollection to a file
 * `FeatureCollection.reduce()` - reduce the number of features after feature selection
 
 """
 
 from __future__ import annotations
-import warnings
 
+import warnings
 
 __author__ = "Jonas Van Der Donckt, Emiel Deprost, Jeroen Van Der Donckt"
 
+import logging
 import os
+import time
+import traceback
 import uuid
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union, Any
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import dill
-import traceback
 import numpy as np
 import pandas as pd
 from multiprocess import Pool
+from pandas.api.types import is_datetime64_any_dtype
 from tqdm.auto import tqdm
 
-from .feature import FeatureDescriptor, MultipleFeatureDescriptors
-from .logger import logger
-from .segmenter import StridedRollingFactory, StridedRolling
-from .utils import _determine_bounds, _check_start_end_array
 from ..features.function_wrapper import FuncWrapper
 from ..utils.attribute_parsing import AttributeParser
-from ..utils.data import to_list, to_series_list, flatten
-from ..utils.logging import delete_logging_handlers, add_logging_handler
+from ..utils.data import flatten, to_list, to_series_list
+from ..utils.logging import add_logging_handler, delete_logging_handlers
 from ..utils.time import parse_time_arg, timedelta_to_str
+from .feature import FeatureDescriptor, MultipleFeatureDescriptors
+from .logger import logger
+from .segmenter import StridedRolling, StridedRollingFactory
+from .utils import (
+    _check_start_end_array,
+    _determine_bounds,
+    _log_func_execution,
+    _process_func_output,
+)
 
 
 class FeatureCollection:
     """Create a FeatureCollection.
 
     Parameters
     ----------
@@ -109,47 +117,49 @@
 
         Returns
         -------
         int
             The number of output features in this feature collection.
 
         """
-        return sum(
-            fd.get_nb_output_features() 
-            for fd in flatten(self._feature_desc_dict.values())
-        )
+        fd_list: Iterable[FeatureDescriptor] = flatten(self._feature_desc_dict.values())
+        return sum(fd.get_nb_output_features() for fd in fd_list)
 
     def _get_nb_output_features_without_window(self) -> int:
         """Return the number of output features in this feature collection, without
         using the window as a unique identifier.
 
-        This is relevant for when the window value(s) are overriden by passing 
+        This is relevant for when the window value(s) are overridden by passing
         `segment_start_idxs` and `segment_end_idxs` to the `calculate` method.
 
         Returns
         -------
         int:
             The number of output features in this feature collection without using the
             window as a unique identifier.
 
-        """ 
+        """
         return len(
             set(
                 (series, o)
                 for (series, _), fd_list in self._feature_desc_dict.items()
                 for fd in fd_list
                 for o in fd.function.output_names
             )
         )
 
+    def _get_nb_feat_funcs(self) -> int:
+        return sum(map(len, self._feature_desc_dict.values()))
+
     @staticmethod
     def _get_collection_key(
         feature: FeatureDescriptor,
-    ) -> Tuple[Tuple[str, ...], Union[pd.Timedelta, float]]:
-        # Note: `window` property can be either a pd.Timedelta or a float
+    ) -> Tuple[Tuple[str, ...], Union[pd.Timedelta, float, None]]:
+        # Note: `window` property can be either a pd.Timedelta or a float or None
+        # assert feature.window is not None
         return feature.series_name, feature.window
 
     def _check_feature_descriptors(
         self,
         skip_none: bool,
         calc_stride: Optional[Union[float, pd.Timedelta, None]] = None,
     ):
@@ -158,26 +168,29 @@
         If this condition is not met, a warning will be raised.
 
         Parameters
         ----------
         skip_none: bool
             Whether to include None stride values in the checks.
         calc_stride: Union[float, pd.Timedelta, None], optional
-            The `FeatureCollection.calculate` stride, by default None. This stride
-            takes precedence over a `FeatureDescriptor` its stride when not None.
+            The `FeatureCollection.calculate` its stride argument, by default None.
+            This stride takes precedence over a `FeatureDescriptor` its stride when
+            it is not None.
 
         """
         dtype_set = set()
         for series_names, win in self._feature_desc_dict.keys():
             for fd in self._feature_desc_dict[(series_names, win)]:
-                str = calc_stride if calc_stride is not None else fd.stride
-                if skip_none and str is None:
+                stride = calc_stride if calc_stride is not None else fd.stride
+                if skip_none and stride is None:
                     dtype_set.add(AttributeParser.determine_type(win))
                 else:
-                    dtype_set.add(AttributeParser.determine_type([win] + to_list(str)))
+                    dtype_set.add(
+                        AttributeParser.determine_type([win] + to_list(stride))
+                    )
 
         if len(dtype_set) > 1:
             warnings.warn(
                 "There are multiple FeatureDescriptor window-stride "
                 + f"datatypes present in this FeatureCollection, i.e.: {dtype_set}",
                 category=RuntimeWarning,
             )
@@ -254,43 +267,117 @@
             else:
                 raise TypeError(f"type: {type(feature)} is not supported - {feature}")
 
         # After adding the features, check whether the descriptors are compatible
         self._check_feature_descriptors(skip_none=True)
 
     @staticmethod
-    def _executor(idx: int):
-        # global get_stroll_func
+    def _executor_stroll(idx: int) -> pd.DataFrame:
+        """Executor function for the StridedRolling.apply_func method.
+
+        Strided rolling feature calculation occurs when either;
+        - a `window` and `stride` argument are stored in the `FeatureDescriptor` object
+        - the `window` is stored in the `FeatureDescriptor` object and the `stride`
+          argument is passed to the `calculate` method, potentially overriding the
+          `stride`
+        - segment indices are passed to the `calculate` method
+        - a `group_by_consecutive` argument is passed to the `calculate` method (since
+          we calculate the segment indices for the consecutive groups)
+
+        This method uses the global `get_stroll_func` function, which returns the
+        StridedRolling object and the function that needs to be applied to the
+        StridedRolling object. Using a global function is necessary to facilitate
+        multiprocessing.
+        """
+        # Uses the global get_stroll_func
         stroll, function = get_stroll_func(idx)
-        return stroll.apply_func(function)
+        return stroll.apply_func(function)  # execution time is logged in apply_func
+
+    @staticmethod
+    def _executor_grouped(idx: int) -> pd.DataFrame:
+        """Executor function for grouped feature calculation.
 
-    # def _get_stroll(self, kwargs):
-        # return StridedRollingFactory.get_segmenter(**kwargs)
+        Grouped feature calculation occurs when either;
+        - a `group_by_all` argument is passed to the `calculate` method
+        - a `DataFrameGroupBy` is passed as `data` argument to the `calculate` method
+
+        Note that passing a `group_by_consecutive` argument to the `calculate` method
+        will not use this executor function, but will use the `_executor_stroll` as
+        executor function (since we calculate the segment indices for the consecutive
+        groups).
+
+        This method uses the global `get_group_func` function, which returns a
+        pd.DataFrame (containing only the necessary data for the function) and the
+        function that needs to be applied to the pd.DataFrame. In addition, the global
+        `group_indices` and `group_id_name` are used to access the grouped data and the
+        group id name respectively. Using a global function is necessary to facilitate
+        multiprocessing.
+        """
+        # Uses the global get_group_func, group_indices, and group_id_name
+        data, function = get_group_func(idx)
+        group_ids = group_indices.keys()  # group_ids are the keys of the group_indices
+        cols_tuple = tuple(data.columns.values)
+
+        t_start = time.perf_counter()
+
+        # Wrap the function to handle multiple inputs and convert the inputs to numpy
+        # array if necessary
+        f = function
+        if function.input_type is np.array:
+
+            def f(x: pd.DataFrame):
+                # pass the inputs as positional arguments of numpy array type
+                return function(*[x[c].values for c in cols_tuple])
+
+        else:  # function.input_type is pd.Series
+
+            def f(x: pd.DataFrame):
+                # pass the inputs as positional arguments of pd.Series type
+                return function(*[x[c] for c in cols_tuple])
+
+        # Function execution over the grouped data (accessed by using the group_indices)
+        out = np.array(list(map(f, [data.iloc[idx] for idx in group_indices.values()])))
+
+        # Aggregate function output in a dictionary
+        output_names = [
+            StridedRolling.construct_output_index(
+                cols_tuple, feat_name, win_str="manual"
+            )
+            for feat_name in function.output_names
+        ]
+        feat_out = _process_func_output(out, group_ids, output_names, str(function))
+
+        # Log the function execution time
+        _log_func_execution(
+            t_start, function, cols_tuple, "manual", "manual", output_names
+        )
+
+        return pd.DataFrame(feat_out, index=group_ids).rename_axis(index=group_id_name)
 
     def _stroll_feat_generator(
         self,
         series_dict: Dict[str, pd.Series],
         calc_stride: Union[List[Union[float, pd.Timedelta]], None],
         segment_start_idxs: Union[np.ndarray, None],
         segment_end_idxs: Union[np.ndarray, None],
         start_idx: Any,
         end_idx: Any,
         window_idx: str,
         include_final_window: bool,
         approve_sparsity: bool,
-    ) -> List[Tuple[StridedRolling, FuncWrapper]]:
+    ) -> Callable[[int], Tuple[StridedRolling, FuncWrapper]]:
         # --- Future work ---
         # We could also make the StridedRolling creation multithreaded
         # Very low priority because the STROLL __init__ is rather efficient!
         keys_wins_strides = list(self._feature_desc_dict.keys())
         lengths = np.cumsum(
             [len(self._feature_desc_dict[k]) for k in keys_wins_strides]
         )
 
-        def get_stroll_function(idx):
+        def get_stroll_function(idx) -> Tuple[StridedRolling, FuncWrapper]:
             key_idx = np.searchsorted(lengths, idx, "right")  # right bc idx starts at 0
             key, win = keys_wins_strides[key_idx]
 
             feature = self._feature_desc_dict[keys_wins_strides[key_idx]][
                 idx - lengths[key_idx]
             ]
             stride = feature.stride if calc_stride is None else calc_stride
@@ -306,97 +393,523 @@
                 end_idx=end_idx,
                 window_idx=window_idx,
                 include_final_window=include_final_window,
                 approve_sparsity=approve_sparsity,
                 func_data_type=function.input_type,
             )
             stroll = StridedRollingFactory.get_segmenter(**stroll_arg_dict)
-            # stroll = self._get_stroll(stroll_arg_dict)
             return stroll, function
 
         return get_stroll_function
 
-    def _get_stroll_feat_length(self) -> int:
-        return sum(
-            len(self._feature_desc_dict[k]) for k in self._feature_desc_dict.keys()
-        )
+    def _group_feat_generator(
+        self,
+        grouped_df: pd.api.typing.DataFrameGroupBy,
+    ) -> Callable[[int], Tuple[pd.api.typing.DataFrameGroupBy, FuncWrapper,],]:
+        """Return a function that returns the necessary columns of the grouped data and
+        the function that needs to be applied to the grouped data.
+
+        Note that the function does not return groups, but rather the necessary columns
+        of the grouped data (i.e. the data on which the function needs to be applied).
+        To access the groups, the global `group_indices` and `group_id_name` are used.
+        """
+        keys_wins = list(self._feature_desc_dict.keys())
+        lengths = np.cumsum([len(self._feature_desc_dict[k]) for k in keys_wins])
+
+        def get_group_function(
+            idx,
+        ) -> Tuple[pd.api.typing.DataFrameGroupBy, FuncWrapper,]:
+            key_idx = np.searchsorted(lengths, idx, "right")  # right bc idx starts at 0
+            key, win = keys_wins[key_idx]
+
+            feature = self._feature_desc_dict[keys_wins[key_idx]][
+                idx - lengths[key_idx]
+            ]
+            function: FuncWrapper = feature.function
+            return grouped_df.obj[list(key)], function
+
+        return get_group_function
 
-    def _check_no_multiple_windows(self):
+    def _check_no_multiple_windows(self, error_case: str):
+        """Check whether there are no multiple windows in the feature collection.
+
+        Parameters
+        ----------
+        error_case : str
+            The case in which no multiple windows are allowed.
+
+        """
         assert (
-            self._get_nb_output_features_without_window() == self.get_nb_output_features()
-        ), "Each output name - series_input combination must have 1 or None window"
+            self._get_nb_output_features_without_window()
+            == self.get_nb_output_features()
+        ), (
+            error_case
+            + "; each output name - series_input combination can only have 1 window"
+            + " (or None)"
+        )
+
+    @staticmethod
+    def _data_to_series_dict(
+        data: Union[pd.DataFrame, pd.Series, List[Union[pd.Series, pd.DataFrame]]],
+        required_series: List[str],
+    ) -> Dict[str, pd.Series]:
+        series_dict: Dict[str, pd.Series] = {}
+        for s in to_series_list(data):
+            if not s.index.is_monotonic_increasing:
+                warnings.warn(
+                    f"The index of series '{s.name}' is not monotonic increasing. "
+                    + "The series will be sorted by the index.",
+                    RuntimeWarning,
+                )
+                s = s.sort_index(ascending=True, inplace=False, ignore_index=False)
+
+            # Assert the assumptions we make!
+            assert s.index.is_monotonic_increasing
+
+            if s.name in required_series:
+                series_dict[str(s.name)] = s
+
+        return series_dict
 
     @staticmethod
     def _process_segment_idxs(
         segment_idxs: Union[list, np.ndarray, pd.Series, pd.Index]
     ) -> np.ndarray:
         if hasattr(segment_idxs, "values"):
             segment_idxs = segment_idxs.values
         segment_idxs = np.asarray(segment_idxs)
         if segment_idxs.ndim > 1:
             segment_idxs = segment_idxs.squeeze()  # remove singleton dimensions
         return segment_idxs
 
-    def calculate(
+    @staticmethod
+    def _group_by_all(
+        series_dict: Dict[str, pd.Series], col_name: str = None
+    ) -> pd.api.typing.DataFrameGroupBy:
+        """Group all `column_name` values and return the grouped data.
+
+        GroupBy ignores all rows with NaN values for the column on which we group.
+
+        Parameters
+        ----------
+        series_dict : Dict[str, pd.Series]
+            Input data.
+        col_name : str
+            The column name on which the grouping will need to take place.
+
+        Returns
+        -------
+        pd.api.typing.DataFrameGroupBy
+            A `DataFrameGroupBy` object, with the group names as keys and the indices
+            as values.
+
+        """
+        df = pd.DataFrame(series_dict)
+        assert col_name in df.columns
+
+        # Check if there are nan values in the column on which we group
+        if df[col_name].isna().any():
+            warnings.warn(
+                f"NaN values were found in the column '{col_name}' (when expanding the "
+                + f"data to a pd.DataFrame which contains {df.columns}. "
+                + "Rows with NaN values for the grouping column will be ignored.",
+                RuntimeWarning,
+            )
+
+        # GroupBy ignores all rows with NaN values for the column on which we group
+        return df.groupby(col_name)
+
+    def _calculate_group_by_all(
+        self,
+        grouped_data: pd.api.typing.DataFrameGroupBy,
+        return_df: Optional[bool],
+        show_progress: Optional[bool],
+        n_jobs: Optional[int],
+        f_handler: Optional[logging.FileHandler],
+    ) -> Union[List[pd.DataFrame], pd.DataFrame]:
+        """Calculate features on each group of the grouped data.
+
+        Parameters
+        ----------
+        grouped_data : pd.api.typing.DataFrameGroupBy
+            The grouped data.
+        return_df: bool, optional
+            Whether the output needs to be a DataFrame or a list thereof.
+        show_progress: bool, optional
+            Whether to show a progress bar.
+        n_jobs: int, optional
+            The number of jobs to run in parallel.
+        f_handler: logging.FileHandler, optional
+            The file handler that is used to log the function execution times.
+
+        .. Note::
+            Is comparable to following pseudo-SQL code:
+            ```sql
+            SELECT func(x)
+            FROM `data`
+            GROUP BY ...
+            ```
+            where `func` is the FeatureDescriptor function and `x` is the name
+            on which the FeatureDescriptor operates. The group by is already done by
+            passing a `DataFrameGroupBy` object to this method.
+        """
+        global group_indices, group_id_name, get_group_func
+        group_indices = grouped_data.indices  # dict - group_id as key; indices as value
+        # since in future versions of pandas grouper will be deprecated
+        group_attr = "_grouper" if hasattr(grouped_data, "_grouper") else "grouper"
+        group_id_name = getattr(grouped_data, group_attr).names  # name of group col(s)
+        get_group_func = self._group_feat_generator(grouped_data)
+
+        # sort_output_index can be set to False, since we want to keep the same order as
+        # the group_indices
+        return self._calculate_feature_list(
+            self._executor_grouped, n_jobs, show_progress, return_df, False, f_handler
+        )
+
+    @staticmethod
+    def _group_by_consecutive(
+        df: Union[pd.Series, pd.DataFrame], col_name: str = None
+    ) -> pd.DataFrame:
+        """Group consecutive `col_name` values in a single DataFrame.
+
+        This is especially useful if you want to represent sparse data in a more
+        compact format.
+
+        Parameters
+        ----------
+        df : Union[pd.Series, pd.DataFrame]
+            Input data.
+        col_name : str, optional
+            If a dataFrame is passed, you will need to specify the `col_name` on which
+            the consecutive-grouping will need to take place.
+
+        Returns
+        -------
+        pd.DataFrame
+            A new `DataFrame` view, with columns:
+            [`start`, `end`, `col_name`], representing the
+            start- and endtime of the consecutive range, and the col_name's consecutive
+            values.
+        """
+        if type(df) == pd.Series:
+            col_name = df.name
+            df = df.to_frame()
+
+        assert col_name in df.columns
+        assert col_name not in [
+            "start",
+            "end",
+        ], "Grouping column cannot be 'start' or 'end'"
+
+        # Check if there are nan values in the column on which we group
+        if df[col_name].isna().any():
+            warnings.warn(
+                f"NaN values were found in the column '{col_name}' (when expanding the "
+                + f"data to a pd.DataFrame which contains {df.columns}. "
+                + "Rows with NaN values for the grouping column will be ignored.",
+                RuntimeWarning,
+            )
+
+        # Drop all rows with NaN values for the column on which we group
+        df.dropna(subset=[col_name], inplace=True)
+
+        df_cum = (
+            (df[col_name] != df[col_name].shift(1))
+            .astype("int")
+            .cumsum()
+            .rename("value_grp")
+            .to_frame()
+        )
+        df_cum["sequence_idx"] = df.index
+        df_cum[col_name] = df[col_name]
+
+        df_cum_grouped = df_cum.groupby("value_grp")
+        df_grouped = pd.DataFrame(
+            {
+                "start": df_cum_grouped["sequence_idx"].first(),
+                "end": df_cum_grouped["sequence_idx"].last(),
+                col_name: df_cum_grouped[col_name].first(),
+            }
+        ).reset_index(drop=True)
+
+        return df_grouped
+
+    def _calculate_group_by_consecutive(
         self,
         data: Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]]],
+        group_by: str,
+        return_df: Optional[bool] = False,
+        **calculate_kwargs,
+    ) -> Union[List[pd.DataFrame], pd.DataFrame]:
+        """Calculate features on each consecutive group of the data.
+
+        Parameters
+        ----------
+        data : Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]]]
+            Must be time-indexed!
+        group_by: str
+            Name of column by which to group values.
+        return_df: bool, optional
+            Whether the output needs to be a DataFrame or a list thereof, by default
+            False. If `True` the output dataframes will be merged to a DataFrame with an
+            outer merge.
+        **calculate_kwargs:
+            Keyword arguments that will be passed to the `calculate` method.
+
+        .. Note::
+            Is comparable to following pseudo-SQL code:
+            ```sql
+            SELECT func(x)
+            FROM `data`
+            GROUP BY `group_by`
+            ```
+            where `func` is the FeatureDescriptor function and `x` is the name
+            on which the FeatureDescriptor operates. Note however that the grouping is
+            done on consecutive values of `group_by` (i.e. `group_by` values that are
+            the same and are next to each other are grouped together).
+        """
+        # 0. Transform to dataframe
+        series_dict = FeatureCollection._data_to_series_dict(
+            data, self.get_required_series() + [group_by]
+        )
+        df = pd.DataFrame(series_dict)
+        # 1. Group by `group_by` column
+        consecutive_grouped_by_df = self._group_by_consecutive(df, col_name=group_by)
+        # 2. Get start and end idxs of consecutive groups
+        start_segment_idxs = consecutive_grouped_by_df["start"]
+        end_segment_idxs = start_segment_idxs.shift(-1)
+        # fill the nan value with the last end idx
+        end_segment_idxs.iloc[-1] = consecutive_grouped_by_df["end"].iloc[-1]
+        # because segment end idxs are exclusive, we need to add an offset to the last
+        # end idx so that all data gets used
+        segment_vals = end_segment_idxs.values
+        if is_datetime64_any_dtype(segment_vals):
+            segment_vals[-1] += pd.Timedelta(days=1)
+        else:
+            segment_vals[-1] += 1
+        # 3. Calculate features
+        try:
+            # Filter out the warnings that are raised when segment indices are passed
+            # (since users expect irregular window sizes when grouping)
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore", category=RuntimeWarning, message="^.*segment indexes.*$"
+                )
+                warnings.filterwarnings(
+                    "ignore", category=RuntimeWarning, message="^.*gaps.*$"
+                )
+                # 3.1. Calculate features using the groupby segment idxs
+                calc_results = self.calculate(
+                    data=df,
+                    segment_start_idxs=start_segment_idxs,
+                    segment_end_idxs=end_segment_idxs,
+                    **calculate_kwargs,
+                )
+
+            # 3.2 Concatenate results and add the group_by column as well as the
+            # start and end idxs of the segments
+            calc_result = pd.concat(calc_results, join="outer", copy=False, axis=1)
+            calc_result.reset_index(inplace=True, drop=True)
+            calc_result[group_by] = consecutive_grouped_by_df[group_by]
+            calc_result["__start"] = consecutive_grouped_by_df["start"]
+            calc_result["__end"] = consecutive_grouped_by_df["end"]
+
+            if return_df:
+                return calc_result
+            else:
+                return [calc_result[col] for col in calc_result.columns]
+
+        except Exception as e:
+            raise RuntimeError(
+                f"An exception was raised during feature extraction:\n{e}"
+            )
+
+    @staticmethod
+    def _process_njobs(n_jobs: Union[int, None], nb_funcs: int) -> int:
+        """Process the number of jobs to run in parallel.
+
+        On Windows no multiprocessing is supported, see
+        https://github.com/predict-idlab/tsflex/issues/51
+
+        Parameters
+        ----------
+        n_jobs : Union[int, None]
+            The number of jobs to run in parallel.
+        nb_funcs : int
+            The number of feature functions.
+
+        Returns
+        -------
+        int
+            The number of jobs to run in parallel.
+
+        """
+        if os.name == "nt":  # On Windows no multiprocessing is supported
+            n_jobs = 1
+        elif n_jobs is None:
+            n_jobs = os.cpu_count()
+        return min(n_jobs, nb_funcs)
+
+    def _calculate_feature_list(
+        self,
+        executor: Callable[[int], pd.DataFrame],
+        n_jobs: Union[int, None],
+        show_progress: bool,
+        return_df: bool,
+        sort_output_index: bool,
+        f_handler: logging.FileHandler,
+    ) -> Union[List[pd.DataFrame], pd.DataFrame]:
+        """Calculate the features for the given executor.
+
+        Parameters
+        ----------
+        executor : Callable[[int], pd.DataFrame]
+            The executor function that will be used to calculate the features.
+        n_jobs : Union[int, None]
+            The number of jobs to run in parallel.
+        show_progress : bool
+            Whether to show a progress bar.
+        return_df : bool
+            Whether to return a DataFrame or a list of DataFrames.
+        sort_output_index : bool
+            Whether to sort the output index. Note that this is only relevant when
+            `return_df` is set to `True`.
+        f_handler : logging.FileHandler
+            The file handler that is used to log the function execution times.
+
+        Returns
+        -------
+        Union[List[pd.DataFrame], pd.DataFrame]
+            The calculated features.
+
+        """
+        nb_feat_funcs = self._get_nb_feat_funcs()
+        n_jobs = FeatureCollection._process_njobs(n_jobs, nb_feat_funcs)
+
+        calculated_feature_list: List[pd.DataFrame] = None
+
+        if n_jobs in [0, 1]:
+            # No multiprocessing
+            idxs = range(nb_feat_funcs)
+            if show_progress:
+                idxs = tqdm(idxs)
+            try:
+                calculated_feature_list = [executor(idx) for idx in idxs]
+            except Exception:
+                traceback.print_exc()
+        else:
+            # Multiprocessing
+            with Pool(processes=n_jobs) as pool:
+                results = pool.imap_unordered(executor, range(nb_feat_funcs))
+                if show_progress:
+                    results = tqdm(results, total=nb_feat_funcs)
+                try:
+                    calculated_feature_list = [f for f in results]
+                except Exception:
+                    traceback.print_exc()
+                    pool.terminate()
+                finally:
+                    # Close & join because: https://github.com/uqfoundation/pathos/issues/131
+                    pool.close()
+                    pool.terminate()
+                    pool.join()
+
+        # Close the file handler (this avoids PermissionError: [WinError 32])
+        if f_handler is not None:
+            f_handler.close()
+            logger.removeHandler(f_handler)
+
+        if calculated_feature_list is None:
+            raise RuntimeError(
+                "Feature Extraction halted due to error while extracting one "
+                + "(or multiple) feature(s)! See stack trace above."
+            )
+
+        if return_df:
+            # Concatenate & sort the columns
+            df = pd.concat(
+                calculated_feature_list,
+                axis=1,
+                join="outer",
+                copy=False,
+                sort=sort_output_index,
+            )
+            return df.reindex(sorted(df.columns), axis=1)
+        else:
+            return calculated_feature_list
+
+    def calculate(
+        self,
+        data: Union[
+            pd.Series,
+            pd.DataFrame,
+            List[Union[pd.Series, pd.DataFrame]],
+            pd.core.groupby.DataFrameGroupby,
+        ],
         stride: Optional[Union[float, str, pd.Timedelta, List, None]] = None,
-        segment_start_idxs: Optional[Union[list, np.ndarray, pd.Series, pd.Index]] = None,
+        segment_start_idxs: Optional[
+            Union[list, np.ndarray, pd.Series, pd.Index]
+        ] = None,
         segment_end_idxs: Optional[Union[list, np.ndarray, pd.Series, pd.Index]] = None,
         return_df: Optional[bool] = False,
         window_idx: Optional[str] = "end",
         include_final_window: Optional[bool] = False,
+        group_by_all: Optional[str] = None,  # TODO: support multiple columns
+        group_by_consecutive: Optional[str] = None,  # TODO: support multiple columns
         bound_method: Optional[str] = "inner",
         approve_sparsity: Optional[bool] = False,
         show_progress: Optional[bool] = False,
         logging_file_path: Optional[Union[str, Path]] = None,
         n_jobs: Optional[int] = None,
     ) -> Union[List[pd.DataFrame], pd.DataFrame]:
         """Calculate features on the passed data.
 
         Parameters
         ----------
-        data : Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]]]
+        data : Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]], pd.core.groupby.DataFrameGroupby]
             Dataframe or Series or list thereof, with all the required data for the
             feature calculation. \n
             **Assumptions**: \n
             * each Series / DataFrame must have a sortable index. This index represents
             the sequence position of the corresponding values, the index can be either
             numeric or a ``pd.DatetimeIndex``.
-            * each Series / DataFrame index must be comparable.with all others
+            * each Series / DataFrame index must be comparable with all others
             * we assume that each series-name / dataframe-column-name is unique.
+            Can also be a `DataFrameGroupBy` object, in which case the expected
+            behaviour is similar to grouping by all values in `group_by_all` (i.e.,
+            for each group, the features are calculated on the group's data).
         stride: Union[float, str, pd.Timedelta, List[Union[float, str, pd.Timedelta], None], optional
             The stride size. By default None. This argument supports multiple types: \n
             * If None, the stride of the `FeatureDescriptor` objects will be used.
-            * If the type is an `float` or an `int`, its value represents the series
+            * If the type is an `float` or an `int`, its value represents the series:\n
                 - its stride **range** when a **non time-indexed** series is passed.
                 - the stride in **number of samples**, when a **time-indexed** series
                 is passed (must then be and `int`)
             * If the stride's type is a `pd.Timedelta`, the stride size represents
             the stride-time delta. The passed data **must have a time-index**.
-            * If a `str`, it must represent a stride-time-delta-string. The **passed data
-            must have a time-index**. \n
+            * If a `str`, it must represent a stride-time-delta-string. Hence, the
+            **passed data must have a time-index**. \n
             .. Note::
                 When set, this stride argument takes precedence over the stride property
                 of the `FeatureDescriptor`s in this `FeatureCollection` (i.e., when a
                 not None value for `stride` passed to this method).
         segment_start_idxs: Union[list, np.ndarray, pd.Series, pd.Index], optional
             The start indices of the segments. If None, the start indices will be
-            computed from the data using either
+            computed from the data using either:\n
             - the `segment_end_idxs` - the `window` size property of the
                 `FeatureDescriptor` in this `FeatureCollection` (if `segment_end_idxs`
                 is not None)
             - strided-window rolling on the data using `window` and `stride` of the
                 `FeatureDescriptor` in this `FeatureCollection` (if `segment_end_idxs`
                  is also None). (Note that the `stride` argument of this method takes
                  precedence over the `stride` property of the `FeatureDescriptor`s).
             By default None.
         segment_end_idxs: Union[list, np.ndarray, pd.Series, pd.Index], optional
             The end indices for the segmented windows. If None, the end indices will be
-            computed from the data using either
+            computed from the data using either:\n
             - the `segment_start_idxs` + the `window` size property of the
                 `FeatureDescriptor` in this `FeatureCollection` (if `segment_start_idxs`
                 is not None)
             - strided-window rolling on the data using `window` and `stride` of the
                 `FeatureDescriptor` in this `FeatureCollection` (if `segment_start_idxs`
                  is also None). (Note that the `stride` argument of this method takes
                  precedence over the `stride` property of the `FeatureDescriptor`s).
@@ -415,15 +928,15 @@
         return_df : bool, optional
             Whether the output needs to be a DataFrame or a list thereof, by default
             False. If `True` the output dataframes will be merged to a DataFrame with an
             outer merge.
         window_idx : str, optional
             The window's index position which will be used as index for the
             feature_window aggregation. Must be either of: `["begin", "middle", "end"]`.
-            by default "end". All features in this collection will use the same
+            by **default "end"**. All features in this collection will use the same
             window_idx.
 
             ..Note::
                 `window_idx`="end" uses the window's end (= right open bound) as
                 output index. \n
                 `window_idx`="begin" uses the window's start idx (= left closed bound)
                 as output index.
@@ -447,14 +960,51 @@
 
                 - the stride is the sampling rate of the data (or stride = 1 for
                 sample-based configurations).<br>
                 **Remark**: that when `include_final_window` is set to False, the last
                 window (which is a full) window will not be included!
                 - *(len * sampling_rate - window_size) % stride = 0*. Remark that the
                   above case is a base case of this.
+        group_by_all : str, optional
+            The name of the column by which to perform grouping. For each group, the
+            features will be calculated. The output that is returned contains this
+            `group_by` column as index to allow identifying the groups.
+            If this parameter is used, the parameters `stride`, `segment_start_idxs`,
+            `segment_end_idxs`, `window_idx` and `include_final_window` will be ignored.
+            Rows with NaN values for this column will not be considered (as pandas
+            ignores these rows when grouping).
+            .. note::
+                This is similar as passing a `DataFrameGroupBy` object as `data`
+                argument to the `calculate` method, where the `DataFrameGroupBy` object
+                is created by calling `data.groupby(group_by_all)`.
+        group_by_consecutive: str, optional
+            The name of the column by which to perform consecutive grouping. A
+            consecutive group is a group of values that are the same and are next to
+            each other. For each consecutive group, the features will be calculated.
+            The output that is returned contains this `group_by` column to allow
+            identifying the groups, and also contains fields [`__start`, "__end"] which
+            contain start and end time range for each result row.
+            If this parameter is used, the parameters `stride`, `segment_start_idxs`,
+            `segment_end_idxs`, `window_idx` and `include_final_window` will be ignored.
+            Rows with NaN values for this column will not be considered (as we deem NaN
+            not as a groupable value).
+            Note that for consecutive grouping, groups can appear multiple times if they
+            appear in different time-gaps.
+
+            Example output:
+            .. example::
+        ```python
+                    number_sold__sum__w=manual  store    __start      __end
+                0          845                  0     2019-01-01 2019-01-01
+                1          357                  3     2019-01-02 2019-01-02
+                2          904                  6     2019-01-03 2019-01-03
+                3          599                  3     2019-01-04 2019-01-05
+                4          871                  0     2019-01-06 2019-01-06
+                ...                           ...    ...        ...        ...
+        ```
         bound_method: str, optional
             The start-end bound methodology which is used to generate the slice ranges
             when ``data`` consists of multiple series / columns.
             Must be either of: `["inner", "inner-outer", "outer"]`, by default "inner".
 
             * if ``inner``, the inner-bounds of the series are returned.
             * if ``inner-outer``, the left-inner and right-outer bounds of the series
@@ -473,25 +1023,25 @@
             to the given file path. See also the `tsflex.features.logger` module.
         n_jobs : int, optional
             The number of processes used for the feature calculation. If `None`, then
             the number returned by _os.cpu_count()_ is used, by default None. \n
             If n_jobs is either 0 or 1, the code will be executed sequentially without
             creating a process pool. This is very useful when debugging, as the stack
             trace will be more comprehensible.
-            .. note:
+            .. note::
                 Multiprocessed execution is not supported on Windows. Even when,
                 `n_jobs` is set > 1, the feature extraction will still be executed
                 sequentially.
                 Why do we not support multiprocessing on Windows; see this issue
                 https://github.com/predict-idlab/tsflex/issues/51
 
             .. tip::
                 It takes on avg. _300ms_ to schedule everything with
                 multiprocessing. So if your sequential feature extraction code runs
-                faster than ~1.5s, it might not be worth it to parallelize the process
+                faster than ~1s, it might not be worth it to parallelize the process
                 (and thus better leave `n_jobs` to 0 or 1).
 
         Returns
         -------
         Union[List[pd.DataFrame], pd.DataFrame]
             The calculated features.
 
@@ -507,40 +1057,148 @@
           retrieved by calling `logger.get_feature_logs(logging_file_path)`.
           Be aware that the `logging_file_path` gets cleared before the logger pushes
           logged messages. Hence, one should use a separate logging file for each
           constructed processing and feature instance with this library.
 
 
         """
+
+        # Check valid data
+        if isinstance(data, list):
+            assert all(
+                isinstance(d, (pd.Series, pd.DataFrame)) for d in data
+            ), "All elements of the data list must be either a Series or a DataFrame!"
+        else:
+            assert isinstance(
+                data, (pd.Series, pd.DataFrame, pd.core.groupby.DataFrameGroupBy)
+            ), "The data must be either a Series, a DataFrame or a DataFrameGroupBy!"
+
+        # check valid group_by
+        assert group_by_all is None or group_by_consecutive is None, (
+            "Only max one of the following parameters can be set: "
+            + "`group_by_all` or `group_by_consecutive`"
+        )
+        assert not (
+            (group_by_all is not None or group_by_consecutive is not None)
+            and isinstance(data, pd.core.groupby.DataFrameGroupBy)
+        ), (
+            "Cannot use `group_by_all` or `group_by_consecutive` when `data` is"
+            + " already a grouped DataFrame!"
+        )
+
         # Delete other logging handlers
         delete_logging_handlers(logger)
         # Add logging handler (if path provided)
+        f_handler = None
         if logging_file_path:
             f_handler = add_logging_handler(logger, logging_file_path)
 
+        if (
+            group_by_all
+            or group_by_consecutive
+            or isinstance(data, pd.core.groupby.DataFrameGroupBy)
+        ):
+            self._check_no_multiple_windows(
+                error_case="When using the groupby behavior"
+            )
+
+            # The grouping column must be part of the required series
+            if group_by_all:
+                # group_by_consecutive should be None (checked by asserts above)
+                # data should not be a grouped DataFrame (checked by asserts above)
+                assert (
+                    group_by_all not in self.get_required_series()
+                ), "The `group_by_all` column cannot be part of the required series!"
+            elif group_by_consecutive:
+                # group_by_all should be None (checked by asserts above)
+                # data should not be a grouped DataFrame (checked by asserts above)
+                assert group_by_consecutive not in self.get_required_series(), (
+                    "The `group_by_consecutive` column cannot be part of the required "
+                    + "series!"
+                )
+                # __start and __end should not be part of the output names
+                assert "__start" not in self.get_required_series()
+                assert "__end" not in self.get_required_series()
+
+            # if any of the following params are not None, warn that they won't be of use
+            # in the grouped calculation
+            ignored_params = [
+                ("stride", None),
+                ("segment_start_idxs", None),
+                ("segment_end_idxs", None),
+                ("window_idx", "end"),
+                ("include_final_window", False),
+            ]
+            local_params = locals()
+
+            for ip, default_value in ignored_params:
+                if local_params[ip] is not default_value:
+                    warnings.warn(
+                        f"Parameter `{ip}` will be ignored in case of GroupBy feature"
+                        + " calculation."
+                    )
+
+            if group_by_consecutive:
+                # Strided rollling feature extraction will take place
+                return self._calculate_group_by_consecutive(
+                    data,
+                    group_by_consecutive,
+                    return_df,
+                    bound_method=bound_method,
+                    approve_sparsity=approve_sparsity,
+                    show_progress=show_progress,
+                    logging_file_path=logging_file_path,
+                    n_jobs=n_jobs,
+                )
+            else:
+                # Grouped feature extraction will take place
+                if not isinstance(data, pd.core.groupby.generic.DataFrameGroupBy):
+                    # group_by_all should not be None (checked by asserts above)
+                    # 0. Transform to dataframe
+                    series_dict = FeatureCollection._data_to_series_dict(
+                        data, self.get_required_series() + [group_by_all]
+                    )
+                    # 1. Group by `group_by_all` column
+                    data = self._group_by_all(series_dict, col_name=group_by_all)
+
+                return self._calculate_group_by_all(
+                    data,  # should be a DataFrameGroupBy
+                    return_df,
+                    show_progress=show_progress,
+                    n_jobs=n_jobs,
+                    f_handler=f_handler,
+                )
+
+        # Sort output index if segment indices are not provided
+        sort_output_index = segment_start_idxs is None and segment_end_idxs is None
+
         # Convert to numpy array (if necessary)
         if segment_start_idxs is not None:
-            segment_start_idxs = FeatureCollection._process_segment_idxs(segment_start_idxs)
+            segment_start_idxs = FeatureCollection._process_segment_idxs(
+                segment_start_idxs
+            )
         if segment_end_idxs is not None:
             segment_end_idxs = FeatureCollection._process_segment_idxs(segment_end_idxs)
 
         if segment_start_idxs is not None and segment_end_idxs is not None:
             # Check if segment indices have same length and whether every start idx
             # <= end idx
             _check_start_end_array(segment_start_idxs, segment_end_idxs)
-            # Check if there is only 1 or None window value for every output name - 
+            # Check if there is either 1 or No(ne) window value for every output name -
             # input_series combination
-            self._check_no_multiple_windows()
+            self._check_no_multiple_windows(
+                error_case="When using both `segment_start_idxs` and `segment_end_idxs`"
+            )
 
         if segment_start_idxs is None or segment_end_idxs is None:
             assert all(
                 fd.window is not None
                 for fd in flatten(self._feature_desc_dict.values())
             ), (
-                "Each feature descriptor must have a window when not both"
+                "Each feature descriptor must have a window when not both "
                 + "segment_start_idxs and segment_end_idxs are provided"
             )
 
         if stride is None and segment_start_idxs is None and segment_end_idxs is None:
             assert all(
                 fd.stride is not None
                 for fd in flatten(self._feature_desc_dict.values())
@@ -553,130 +1211,58 @@
         ):
             raise ValueError(
                 "The stride and any segment index argument cannot be set together! "
                 + "At least one of both should be None."
             )
 
         if stride is not None:
+            # Verify whether the stride complies with the input data dtype
             stride = [
                 parse_time_arg(s) if isinstance(s, str) else s for s in to_list(stride)
             ]
             self._check_feature_descriptors(skip_none=False, calc_stride=stride)
 
         # Convert the data to a series_dict
-        series_dict: Dict[str, pd.Series] = {}
-        for s in to_series_list(data):
-            if not s.index.is_monotonic_increasing:
-                # TODO -> maybe raise a warning?
-                s = s.sort_index(ascending=True, inplace=False, ignore_index=False)
-
-            # Assert the assumptions we make!
-            assert s.index.is_monotonic_increasing
-
-            if s.name in self.get_required_series():
-                series_dict[str(s.name)] = s
+        series_dict = FeatureCollection._data_to_series_dict(
+            data, self.get_required_series()
+        )
 
         # Determine the bounds of the series dict items and slice on them
-        # TODO: is dit wel nodig hier? want we doen dat ook in de strided rolling
+        # TODO: is dit wel nodig `hier? want we doen dat ook in de strided rolling
         start, end = _determine_bounds(bound_method, list(series_dict.values()))
         series_dict = {
             n: s.loc[
                 s.index.dtype.type(start) : s.index.dtype.type(end)
             ]  # TODO: check memory efficiency of ths
             for n, s, in series_dict.items()
         }
 
-        # Trim the segment indices (if necessary)
-        # TODO: currently commented this as this also happens in StridedRolling
-        # if segment_start_idxs is not None:
-        #     start_ = start; end_ = end
-        #     if isinstance(start, pd.Timestamp) and start.tz is not None:
-        #         assert isinstance(end, pd.Timestamp) and end.tz == start.tz
-        #         start_ = start_.tz_convert(None)
-        #         end_ = end_.tz_convert(None)
-        #     mask = (segment_start_idxs >= start_) & (segment_start_idxs <= end_)
-        #     segment_start_idxs = segment_start_idxs[mask]
-        # if segment_end_idxs is not None:
-        #     start_ = start; end_ = end
-        #     if isinstance(start, pd.Timestamp) and start.tz is not None:
-        #         assert isinstance(end, pd.Timestamp) and end.tz == start.tz
-        #         start_ = start_.tz_convert(None)
-        #         end_ = end_.tz_convert(None)
-        #     mask = (segment_end_idxs >= start_) & (segment_end_idxs <= end_)
-        #     segment_end_idxs = segment_end_idxs[mask]
-        # if segment_start_idxs is not None and segment_end_idxs is not None:
-        #     # Check if segment indices have same length and whether every start idx
-        #     # <= end idx
-        #     _check_start_end_array(segment_start_idxs, segment_end_idxs)
-
         # Note: this variable has a global scope so this is shared in multiprocessing
-        # TODO: try to make this more efficient
+        # TODO: try to make this more efficient (but is not really the bottleneck)
         global get_stroll_func
         get_stroll_func = self._stroll_feat_generator(
             series_dict,
             calc_stride=stride,
             segment_start_idxs=segment_start_idxs,
             segment_end_idxs=segment_end_idxs,
             start_idx=start,
             end_idx=end,
             window_idx=window_idx,
             include_final_window=include_final_window,
             approve_sparsity=approve_sparsity,
         )
-        nb_stroll_funcs = self._get_stroll_feat_length()
-
-        if (
-            os.name == "nt"
-        ):  # On Windows no multiprocessing is supported, see https://github.com/predict-idlab/tsflex/issues/51
-            n_jobs = 1
-        elif n_jobs is None:
-            n_jobs = os.cpu_count()
-        n_jobs = min(n_jobs, nb_stroll_funcs)
-
-        calculated_feature_list = None
-        if n_jobs in [0, 1]:
-            idxs = range(nb_stroll_funcs)
-            if show_progress:
-                idxs = tqdm(idxs)
-            try:
-                calculated_feature_list = [self._executor(idx) for idx in idxs]
-            except:
-                traceback.print_exc()
-        else:
-            with Pool(processes=n_jobs) as pool:
-                results = pool.imap_unordered(self._executor, range(nb_stroll_funcs))
-                if show_progress:
-                    results = tqdm(results, total=nb_stroll_funcs)
-                try:
-                    calculated_feature_list = [f for f in results]
-                except:
-                    traceback.print_exc()
-                    pool.terminate()
-                finally:
-                    # Close & join because: https://github.com/uqfoundation/pathos/issues/131
-                    pool.close()
-                    pool.join()
 
-        # Close the file handler (this avoids PermissionError: [WinError 32])
-        if logging_file_path:
-            f_handler.close()
-            logger.removeHandler(f_handler)
-
-        if calculated_feature_list is None:
-            raise RuntimeError(
-                "Feature Extraction halted due to error while extracting one "
-                + "(or multiple) feature(s)! See stack trace above."
-            )
-
-        if return_df:
-            # concatenate & sort the columns
-            df = pd.concat(calculated_feature_list, axis=1, join="outer", copy=False)
-            return df.reindex(sorted(df.columns), axis=1)
-        else:
-            return calculated_feature_list
+        return self._calculate_feature_list(
+            self._executor_stroll,
+            n_jobs,
+            show_progress,
+            return_df,
+            sort_output_index,
+            f_handler,
+        )
 
     def serialize(self, file_path: Union[str, Path]):
         """Serialize this FeatureCollection instance.
 
         Parameters
         ----------
         file_path : Union[str, Path]
@@ -723,35 +1309,31 @@
         # dict in which we store all the { output_col_name : (UUID, FeatureDescriptor) }
         # items of our current FeatureCollection object
         manual_window = False
         if any(c.endswith("w=manual") for c in feat_cols_to_keep):
             assert all(c.endswith("w=manual") for c in feat_cols_to_keep)
             # As the windows are created manual, the FeatureCollection cannot contain
             # multiple windows for the same output name - input_series combination
-            self._check_no_multiple_windows()
+            self._check_no_multiple_windows(
+                error_case="When reducing a FeatureCollection with manual windows"
+            )
             manual_window = True
         feat_col_fd_mapping: Dict[str, Tuple[str, FeatureDescriptor]] = {}
         for (s_names, window), fd_list in self._feature_desc_dict.items():
             window = "manual" if manual_window else self._ws_to_str(window)
             for fd in fd_list:
                 # As a single FeatureDescriptor can have multiple output col names, we
                 # create a unique identifier for each FeatureDescriptor (on which we
                 # will apply set-like operations later on to only retain all the unique
                 # FeatureDescriptors)
                 uuid_str = str(uuid.uuid4())
                 for output_name in fd.function.output_names:
                     # Reconstruct the feature column name
-                    feat_col_name = "__".join(
-                        [
-                            "|".join(s_names)
-                            if isinstance(s_names, tuple)
-                            else s_names,
-                            output_name,
-                            f"w={window}",
-                        ]
+                    feat_col_name = StridedRolling.construct_output_index(
+                        series_keys=s_names, feat_name=output_name, win_str=window
                     )
                     feat_col_fd_mapping[feat_col_name] = (uuid_str, fd)
 
         assert all(fc in feat_col_fd_mapping for fc in feat_cols_to_keep)
 
         # Collect (uuid, FeatureDescriptor) for the feat_cols_to_keep
         fd_subset: List[Tuple[str, FeatureDescriptor]] = [
@@ -770,28 +1352,29 @@
                     if uuid_str not in seen_uuids and not seen_uuids.add(uuid_str)
                 }
             ]
         )
 
     @staticmethod
     def _ws_to_str(window_or_stride: Any) -> str:
+        """Convert the window/stride value to a (shortend) string representation."""
         if isinstance(window_or_stride, pd.Timedelta):
             return timedelta_to_str(window_or_stride)
         else:
             return str(window_or_stride)
 
     def __repr__(self) -> str:
         """Representation string of a FeatureCollection."""
         feature_keys = sorted(set(k[0] for k in self._feature_desc_dict.keys()))
         output_str = ""
         for feature_key in feature_keys:
             output_str += f"{'|'.join(feature_key)}: ("
             keys = (x for x in self._feature_desc_dict.keys() if x[0] == feature_key)
             for _, win_size in keys:
-                output_str += f"\n\twin: "
+                output_str += "\n\twin: "
                 win_str = self._ws_to_str(win_size)
                 output_str += f"{win_str:<6}: ["
                 for feat_desc in self._feature_desc_dict[feature_key, win_size]:
                     stride_str = feat_desc.stride
                     if stride_str is not None:
                         stride_str = [self._ws_to_str(s) for s in stride_str]
                     output_str += f"\n\t\t{feat_desc._func_str}"
```

### Comparing `tsflex-0.3rc0/tsflex/features/function_wrapper.py` & `tsflex-0.4.0/tsflex/features/function_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 """FuncWrapper class for object-oriented representation of a function."""
 
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
 
+import functools
+from typing import Any, Callable, List, Optional, Union
+
 import numpy as np
 import pandas as pd
 
-from typing import Callable, List, Union, Any, Optional
-from ..utils.data import SUPPORTED_STROLL_TYPES
-from ..utils.classes import FrozenClass
 from .. import __pdoc__
+from ..utils.classes import FrozenClass
+from ..utils.data import SUPPORTED_STROLL_TYPES
 
 __pdoc__["FuncWrapper.__call__"] = True
 
 
+def _get_name(func: Callable) -> str:
+    """Get the name of the function.
+
+    Parameters
+    ----------
+    func: Callable
+        The function whose name has to be returned, should be either a function or an
+        object that is callable.
+
+    Returns
+    -------
+    str
+        The name of ``func`` in case of a function, or
+        - the name of the wrapped function in case of functools.partial.
+        - the name of the class in case of a callable object.
+
+    """
+    assert callable(func), f"The given argument {func} is not callable!"
+    try:
+        return func.__name__
+    except AttributeError:
+        if isinstance(func, functools.partial):
+            return func.func.__name__
+        return type(func).__name__
+
+
 class FuncWrapper(FrozenClass):
     """Function wrapper.
 
     A function wrapper which takes a numpy array / pandas series as input and returns
     one or multiple values. It also defines the names of the function outputs, and
     stores the function its keyword arguments.
 
@@ -39,18 +67,18 @@
         segmented windows, by default False.
         .. Info::
             A vectorized function should take one or multiple series that each have the
             shape (nb. segmented windows, window size).
             For example a vectorized version of `np.max` is
             ``FuncWrapper(np.max, vectorized=True, axis=1)``.
         .. Note::
-            * A function can only be applied in vectorized manner when the required 
+            * A function can only be applied in vectorized manner when the required
               series are REGULARLY sampled (and have the same index in case of multiple
               required series).
-            * The `input_type` should be `np.array` when `vectorized` is True. It does 
+            * The `input_type` should be `np.array` when `vectorized` is True. It does
               not make sense to use a `pd.Series`, as the index should be regularly
               sampled (see requirement above).
     **kwargs: dict, optional
         Keyword arguments which will be also passed to the `function`
 
     Raises
     ------
@@ -72,15 +100,15 @@
         self.kwargs: dict = kwargs
 
         if isinstance(output_names, list):
             self.output_names = output_names
         elif isinstance(output_names, str):
             self.output_names = [output_names]
         elif not output_names:
-            self.output_names = [self.func.__name__]
+            self.output_names = [_get_name(func)]
         else:
             raise TypeError(f"`output_names` is unexpected type {type(output_names)}")
 
         assert input_type in SUPPORTED_STROLL_TYPES, "Invalid input_type!"
         assert not (
             vectorized & (input_type is not np.array)
         ), "The input_type must be np.array if vectorized is True!"
@@ -88,15 +116,15 @@
         self.vectorized = vectorized
 
         self._freeze()
 
     def __repr__(self) -> str:
         """Return repr string."""
         return (
-            f"{self.__class__.__name__}({self.func.__name__}, {self.output_names},"
+            f"{self.__class__.__name__}({_get_name(self.func)}, {self.output_names},"
             f" {self.kwargs})"
         )
 
     def __call__(self, *series: Union[np.ndarray, pd.Series]) -> Any:
         """Call wrapped function with passed data.
 
         Parameters
```

### Comparing `tsflex-0.3rc0/tsflex/features/integrations.py` & `tsflex-0.4.0/tsflex/features/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Wrappers for seamless integration of feature functions from other packages."""
 
 __author__ = "Jeroen Van Der Donckt, Jonas Van Der Donckt"
 
 import importlib
-import pandas as pd
+from typing import Callable, Dict, List, Optional, Union
+
 import numpy as np
+import pandas as pd
 
-from typing import Callable, Optional, List, Dict, Union
-from .feature import FuncWrapper
-from .utils import _get_name
+from .function_wrapper import FuncWrapper, _get_name
 
 
 # ------------------------------------- SEGLEARN -------------------------------------
 def seglearn_wrapper(func: Callable, func_name: Optional[str] = None) -> FuncWrapper:
     """Wrapper enabling compatibility with seglearn functions.
-    
-    As [seglearn feature-functions](https://github.com/dmbee/seglearn/blob/master/seglearn/feature_functions.py) 
-    are vectorized along the first axis (axis=0), we need to expand our window-data.  
-    This wrapper converts `1D np.array` to a `2D np.array` with all the window-data in 
+
+    As [seglearn feature-functions](https://github.com/dmbee/seglearn/blob/master/seglearn/feature_functions.py)
+    are vectorized along the first axis (axis=0), we need to expand our window-data.
+    This wrapper converts `1D np.array` to a `2D np.array` with all the window-data in
     `axis=1`.
 
     Parameters
     ----------
     func: Callable
         The seglearn function.
     func_name: str, optional
@@ -30,43 +30,44 @@
 
     Returns
     -------
     FuncWrapper
         The wrapped seglearn function that is compatible with tsflex.
 
     """
+
     def wrap_func(x: np.ndarray):
         out = func(x.reshape(1, len(x)))
         return out.flatten()
 
     wrap_func.__name__ = "[seglearn_wrapped]__" + _get_name(func)
     output_names = _get_name(func) if func_name is None else func_name
     # A bit hacky (hard coded), bc hist is only func that returns multiple values
     if hasattr(func, "bins"):
         output_names = [output_names + f"_bin{idx}" for idx in range(1, func.bins + 1)]
     return FuncWrapper(wrap_func, output_names=output_names)
 
 
-def seglearn_feature_dict_wrapper(features_dict: Dict) -> List[Callable]:
+def seglearn_feature_dict_wrapper(features_dict: Dict) -> List[FuncWrapper]:
     """Wrapper enabling compatibility with seglearn feature dictionaries.
 
-    seglearn represents a collection of features as a dictionary. 
+    seglearn represents a collection of features as a dictionary.
 
-    By using this wrapper, we can plug in the features (that are present in the 
-    dictionary) in a tsflex ``FeatureCollection``. 
+    By using this wrapper, we can plug in the features (that are present in the
+    dictionary) in a tsflex ``FeatureCollection``.
     This enables to easily extract (a collection of) seglearn features while leveraging
     the flexibility of tsflex.
 
     .. Note::
         This wrapper wraps the output of seglearn functions that return feature
-        dictionaries;  
-        - [base_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.base_features)  
-        - [emg_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.emg_features)  
-        - [hudgins_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.hudgins_features)  
-        - [all_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.all_features)  
+        dictionaries;
+        - [base_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.base_features)
+        - [emg_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.emg_features)
+        - [hudgins_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.hudgins_features)
+        - [all_features()](https://dmbee.github.io/seglearn/feature_functions.html#seglearn.feature_functions.all_features)
 
     Example
     -------
     ```python
     from tsflex.features import FeatureCollection, MultipleFeatureDescriptors
     from tsflex.features.integrations import seglearn_feature_dict_wrapper
     from seglearn.feature_functions import base_features
@@ -87,27 +88,27 @@
         The seglearn collection of features (which is a dict).
 
     Returns
     -------
     List[Callable]
         List of the (wrapped) seglearn functions that are now directly compatible with
         with tsflex.
- 
+
     """
     return [seglearn_wrapper(func) for func in features_dict.values()]
-    
+
 
 # -------------------------------------- TSFEL --------------------------------------
 def tsfel_feature_dict_wrapper(features_dict: Dict) -> List[Callable]:
     """Wrapper enabling compatibility with tsfel feature extraction configurations.
 
     tsfel represents a collection of features as a dictionary, see more [here](https://tsfel.readthedocs.io/en/latest/descriptions/get_started.html#set-up-the-feature-extraction-config-file).
 
-    By using this wrapper, we can plug in the features (that are present in the 
-    tsfel feature extraction configuration) in a tsflex ``FeatureCollection``. 
+    By using this wrapper, we can plug in the features (that are present in the
+    tsfel feature extraction configuration) in a tsflex ``FeatureCollection``.
     This enables to easily extract (a collection of) tsfel features while leveraging
     the flexibility of tsflex.
 
     .. Note::
         This wrapper wraps the output of tsfel its `get_features_by_domain` or
         `get_features_by_tag`. <br>
         See more [here](https://github.com/fraunhoferportugal/tsfel/blob/master/tsfel/feature_extraction/features_settings.py).
@@ -135,23 +136,28 @@
         The tsfel collection of features (which is a dict).
 
     Returns
     -------
     List[Callable]
         List of the (wrapped) tsfel functions that are now directly compatible with
         with tsflex.
- 
+
     """
-    def get_output_names(config: dict):  
+
+    def get_output_names(config: dict):
         """Create the output_names based on the configuration."""
         nb_outputs = config["n_features"]
         func_name = config["function"].split(".")[-1]
-        if isinstance(nb_outputs, str) and isinstance(config["parameters"][nb_outputs], int):
+        if isinstance(nb_outputs, str) and isinstance(
+            config["parameters"][nb_outputs], int
+        ):
             nb_outputs = config["parameters"][nb_outputs]
-        if func_name == "lpcc":  # Because https://github.com/fraunhoferportugal/tsfel/issues/103
+        if (
+            func_name == "lpcc"
+        ):  # Because https://github.com/fraunhoferportugal/tsfel/issues/103
             nb_outputs += 1
         if isinstance(nb_outputs, int):
             if nb_outputs == 1:
                 return func_name
             else:
                 return [func_name + f"_{idx}" for idx in range(1, nb_outputs + 1)]
         output_param = eval(config["parameters"][nb_outputs])
@@ -170,62 +176,63 @@
 
 # ------------------------------------- TSFRESH -------------------------------------
 def tsfresh_combiner_wrapper(func: Callable, param: List[Dict]) -> FuncWrapper:
     """Wrapper enabling compatibility with tsfresh combiner functions.
 
     [tsfresh feature-funtions](https://github.com/blue-yonder/tsfresh/blob/main/tsfresh/feature_extraction/feature_calculators.py)
     are either of type `simple` or `combiner`.\n
-    * `simple`: feature calculators which calculate a single number  
+    * `simple`: feature calculators which calculate a single number
       **=> integrates natively with tsflex**
-    * `combiner`: feature calculates which calculate a bunch of features for a list of parameters. 
-       These features are returned as a list of (key, value) pairs for each input parameter.  
-       **=> requires wrapping the function to only extract the values of the returned tuples**  
+    * `combiner`: feature calculates which calculate a bunch of features for a list of parameters.
+       These features are returned as a list of (key, value) pairs for each input parameter.
+       **=> requires wrapping the function to only extract the values of the returned tuples**
 
     Parameters
     ----------
     func: Callable
         The tsfresh combiner function.
     param: List[Dict]
         List containing dictionaries with the parameter(s) for the combiner function.
-        This is exactly the same ``param`` as you would pass to a tsfresh combiner 
+        This is exactly the same ``param`` as you would pass to a tsfresh combiner
         function.
 
     Returns
     -------
     FuncWrapper
         The wrapped tsfresh combiner function that is compatible with tsflex.
 
     """
+
     def wrap_func(x: Union[np.ndarray, pd.Series]):
         out = func(x, param)
         return tuple(t[1] for t in out)
 
     wrap_func.__name__ = "[tsfresh-combiner_wrapped]__" + _get_name(func)
     input_type = pd.Series if hasattr(func, "index_type") else np.array
     return FuncWrapper(
         wrap_func,
         output_names=[func.__name__ + "_" + str(p) for p in param],
         input_type=input_type,
     )
 
 
-def tsfresh_settings_wrapper(settings: Dict) -> List[Callable]:
+def tsfresh_settings_wrapper(settings: Dict) -> List[Union[Callable, FuncWrapper]]:
     """Wrapper enabling compatibility with tsfresh feature extraction settings.
 
     [tsfresh feature extraction settings](https://tsfresh.readthedocs.io/en/latest/text/feature_extraction_settings.html)
     is how tsfresh represents a collection of features (as a dict).<br>
 
-    By using this wrapper, we can plug in the features (that are present in the 
-    tsfresh feature extraction settings) in a tsflex ``FeatureCollection``. 
+    By using this wrapper, we can plug in the features (that are present in the
+    tsfresh feature extraction settings) in a tsflex ``FeatureCollection``.
     This enables to easily extract (a collection of) tsfresh features while leveraging
     the flexibility of tsflex.
 
     .. Note::
-        This wrapper wraps the output of tsfresh its `MinimalFCParameters()`, 
-        `EfficientFCParameters()`, `IndexBasedFCParameters()`, 
+        This wrapper wraps the output of tsfresh its `MinimalFCParameters()`,
+        `EfficientFCParameters()`, `IndexBasedFCParameters()`,
         `TimeBasedFCParameters()`, or `ComprehensiveFCParameters()`. <br>
         See more [here](https://github.com/blue-yonder/tsfresh/blob/main/tsfresh/feature_extraction/settings.py).
 
     Example
     -------
     ```python
     from tsflex.features import FeatureCollection, MultipleFeatureDescriptors
@@ -245,23 +252,25 @@
     Parameters
     ----------
     settings: PicklableSettings
         The tsfresh base object for feature settings (which is a dict).
 
     Returns
     -------
-    List[Callable]
+    List[Union[Callable, FuncWrapper]]
         List of the (wrapped) tsfresh functions that are now directly compatible with
         with tsflex.
- 
+
     """
     functions = []
-    tsfresh_mod = importlib.import_module("tsfresh.feature_extraction.feature_calculators") 
+    tsfresh_mod = importlib.import_module(
+        "tsfresh.feature_extraction.feature_calculators"
+    )
     for func_name, param in settings.items():
-        func = getattr(tsfresh_mod, func_name) 
+        func = getattr(tsfresh_mod, func_name)
         if param is None:
             functions.append(func)
         elif getattr(func, "fctype") == "combiner":
             functions.append(tsfresh_combiner_wrapper(func, param))
         else:
             for kwargs in param:
                 functions.append(
@@ -272,15 +281,15 @@
     return functions
 
 
 # ----------------------------------- --CATCH22 -------------------------------------
 def catch22_wrapper(catch22_all: Callable) -> FuncWrapper:
     """Wrapper enabling compatibility with catch22.
 
-    [catch22](https://github.com/chlubba/catch22) is a collection of 22 time series 
+    [catch22](https://github.com/chlubba/catch22) is a collection of 22 time series
     features that are a high-performing subset of the over 7000 features in hctsa.
     -> [Python bindings](https://github.com/DynamicsAndNeuralSystems/pycatch22)
 
     By using this wrapper, we can plug the catch22 features in a tsflex
     ``FeatureCollection``.
     This enables to easily extract the catch22 features while leveraging the flexibility
     of tsflex.
@@ -312,15 +321,15 @@
         The `catch22_all` function from the `pycatch22` package.
 
     Returns
     -------
     FuncWrapper
         The wrapped `catch22_all` function that is compatible with tsflex.
         This FuncWrapper will output the 22 catch22 features.
- 
+
     """
     catch22_names = catch22_all([0])["names"]
 
     def wrap_catch22_all(x):
         return catch22_all(x)["values"]
 
     wrap_catch22_all.__name__ = "[wrapped]__" + _get_name(catch22_all)
```

### Comparing `tsflex-0.3rc0/tsflex/features/logger.py` & `tsflex-0.4.0/tsflex/features/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 FeatureCollection: its `logging_file_path` of the `calculate` method.
 
 """
 
 __author__ = "Jeroen Van Der Donckt"
 
 import logging
+import re
+
 import numpy as np
 import pandas as pd
-import re
 
 from ..utils.logging import logging_file_to_df, remove_inner_brackets
 from ..utils.time import timedelta_to_str
 
 # Package specific logger
 logger = logging.getLogger("feature_calculation_logger")
 logger.setLevel(logging.DEBUG)
@@ -26,48 +27,51 @@
 logger.addHandler(console)
 
 
 def _parse_message(message: str) -> list:
     """Parse the message of the logged info."""
     regex = r"\[(.*?)\]"
     matches = re.findall(regex, remove_inner_brackets(message))
-    assert len(matches) == 4
+    assert len(matches) == 5
     func = matches[0]
     key = matches[1].replace("'", "")
     window = matches[2].split(",")[0].strip()
     stride = ",".join(matches[2].split(",")[1:]).strip()
     if stride != "manual":
         stride = eval(stride)  # parse the tuple
-    duration_s = float(matches[3].rstrip(" seconds"))
-    return [func, key, window, stride, duration_s]
+    output_names = matches[3].replace("'", "")
+    duration_s = float(matches[4].rstrip(" seconds"))
+    return [func, key, window, stride, output_names, duration_s]
 
 
 def _parse_logging_execution_to_df(logging_file_path: str) -> pd.DataFrame:
     """Parse the logged messages into a dataframe that contains execution info.
 
     Parameters
     ----------
     logging_file_path: str
         The file path where the logged messages are stored. This is the file path that
         is passed to the `FeatureCollection` its `calculate` method.
 
-    Note
-    ----
-    This function only works when the `logging_file_path` used in a
-    `FeatureCollection` its `calculate` method is passed.
-
     Returns
     -------
     pd.DataFrame
-        A DataFrame with the features its function, input series names and
-        calculation duration.
+        A DataFrame with the features its function, input series names, output names,
+        and (%) calculation duration.
+
+    Note
+    ----
+    This function only works when the ``logging_file_path`` used in a
+    ``FeatureCollection`` its ``calculate`` method is passed.
 
     """
     df = logging_file_to_df(logging_file_path)
-    df[["function", "series_names", "window", "stride", "duration"]] = pd.DataFrame(
+    df[
+        ["function", "series_names", "window", "stride", "output_names", "duration"]
+    ] = pd.DataFrame(
         list(df["message"].apply(_parse_message)),
         index=df.index,
     )
     # Parse the window
     if (df["window"] == "manual").any():
         # All should be manual
         assert (df["window"] == "manual").all()
@@ -76,27 +80,28 @@
     else:
         df["window"] = pd.to_timedelta(df["window"]).apply(timedelta_to_str)
     # Parse the stride
     if (df["stride"] == "manual").any():
         # All should be manual
         assert (df["stride"] == "manual").all()
     elif (
-        df["stride"].apply(
-            lambda stride_tuple: np.char.isnumeric(stride_tuple).all()
-        ).all()
+        df["stride"]
+        .apply(lambda stride_tuple: np.char.isnumeric(stride_tuple).all())
+        .all()
     ):
         df["stride"] = df["stride"].apply(
             lambda stride_tuple: tuple(sorted(pd.to_numeric(s) for s in stride_tuple))
         )
     else:
         df["stride"] = df["stride"].apply(
             lambda stride_tuple: tuple(
                 timedelta_to_str(pd.to_timedelta(s)) for s in stride_tuple
             )
         )
+    df["duration %"] = (100 * (df["duration"] / df["duration"].sum())).round(2)
     return df.drop(columns=["name", "log_level", "message"])
 
 
 def get_feature_logs(logging_file_path: str) -> pd.DataFrame:
     """Get execution (time) info for each feature of a `FeatureCollection`.
 
     Parameters
@@ -105,15 +110,15 @@
         The file path where the logged messages are stored. This is the file path that
         is passed to the `FeatureCollection` its `calculate` method.
 
     Returns
     -------
     pd.DataFrame
         A DataFrame with the features its function, input series names and
-        calculation duration.
+        (%) calculation duration.
 
     """
     df = _parse_logging_execution_to_df(logging_file_path)
     df["duration"] = pd.to_timedelta(df["duration"], unit="s")
     return df
 
 
@@ -126,15 +131,16 @@
         The file path where the logged messages are stored. This is the file path that
         is passed to the `FeatureCollection` its `calculate` method.
 
     Returns
     -------
     pd.DataFrame
         A DataFrame with for each function (i.e., `function-(window,stride)`)
-        combination the mean (time), std (time), sum (time), and number of executions.
+        combination the mean (time), std (time), sum (time), sum (% time),
+        mean (% time),and number of executions.
 
     """
     df = _parse_logging_execution_to_df(logging_file_path)
     # Get the sorted functions in a list to use as key for sorting the groups
     sorted_funcs = (
         df.groupby(["function"])
         .agg({"duration": ["mean"]})
@@ -145,15 +151,20 @@
     def key_func(idx_level):
         if all(idx in sorted_funcs for idx in idx_level):
             return [sorted_funcs.index(idx) for idx in idx_level]
         return idx_level
 
     return (
         df.groupby(["function", "window", "stride"])
-        .agg({"duration": ["mean", "std", "sum", "count"]})
+        .agg(
+            {
+                "duration": ["sum", "mean", "std", "count"],
+                "duration %": ["sum", "mean"],
+            }
+        )
         .sort_index(key=key_func, ascending=False)
     )
 
 
 def get_series_names_stats(logging_file_path: str) -> pd.DataFrame:
     """Get execution (time) statistics for each `key-(window,stride)` combination.
 
@@ -162,17 +173,22 @@
     logging_file_path: str
         The file path where the logged messages are stored. This is the file path that
         is passed to the `FeatureCollection` its `calculate` method.
 
     Returns
     -------
     pd.DataFrame
-        A DataFrame with for each function the mean (time), std (time), sum (time), and
-        number of executions.
+        A DataFrame with for each function the mean (time), std (time), sum (time),
+        sum (% time), mean (% time), and number of executions.
 
     """
     df = _parse_logging_execution_to_df(logging_file_path)
     return (
         df.groupby(["series_names", "window", "stride"])
-        .agg({"duration": ["sum", "mean", "std", "count"]})
+        .agg(
+            {
+                "duration": ["sum", "mean", "std", "count"],
+                "duration %": ["sum", "mean"],
+            }
+        )
         .sort_values(by=("duration", "sum"), ascending=False)
     )
```

### Comparing `tsflex-0.3rc0/tsflex/features/segmenter/strided_rolling.py` & `tsflex-0.4.0/tsflex/features/segmenter/strided_rolling.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt"
 
 import time
 import warnings
 from abc import ABC, abstractmethod
 from collections import namedtuple
-from typing import Union, List, Tuple, Optional, TypeVar
+from typing import List, Optional, Tuple, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
-from ..function_wrapper import FuncWrapper
-from ..logger import logger
-from ..utils import _determine_bounds, _check_start_end_array
-from ...utils.data import SUPPORTED_STROLL_TYPES, to_series_list, to_list
-from ...utils.attribute_parsing import DataType, AttributeParser
+from ...utils.attribute_parsing import AttributeParser, DataType
+from ...utils.data import SUPPORTED_STROLL_TYPES, to_list, to_series_list, to_tuple
 from ...utils.time import timedelta_to_str
+from ..function_wrapper import FuncWrapper
+from ..utils import (
+    _check_start_end_array,
+    _determine_bounds,
+    _log_func_execution,
+    _process_func_output,
+)
 
 # Declare a type variable
 T = TypeVar("T")
 
 
 class StridedRolling(ABC):
     """Custom time-based sliding window with stride.
@@ -45,53 +49,54 @@
         Either an int, float, or ``pd.Timedelta``, representing the sliding window size
         in terms of the index (in case of a int or float) or the sliding window duration
         (in case of ``pd.Timedelta``).
     strides : Union[float, pd.Timedelta, List[Union[float, pd.Timedelta]]], optional
         Either a list of int, float, or ``pd.Timedelta``, representing the stride sizes
         in terms of the index (in case of a int or float) or the stride duration (in
         case of ``pd.Timedelta``). By default None.
-    segment_start_idxs: np.ndarray, optional  # TODO is this a numpy array?
+    segment_start_idxs: np.ndarray, optional
         The start indices for the segmented windows. If not provided, the start indices
-        will be computed from the data using the passed ``strides``. By default None.
+        will be computed from the data using the passed ``strides`` or by using the
+        ``segment_end_idxs`` (if not none) + ``window``. By default None.
     segment_end_idxs: np.ndarray, optional
-        The end indices for the segmented windows. You can only pass an array to this
-        argument when you pass an array to `segment_start_idxs` as well (read more in
-        note below). If not provided, the end indices will be computed from the data
-        using the passed ``strides``. By default None.
+        The end indices for the segmented windows. If not provided, the end indices will
+        be computed from either (1) the data using the passed ``window`` + ``strides``
+        or (2) the ``segment_start_idxs`` + ``window``, By default None.
         .. Note::
-            You can only pass an array for `segment_end_idxs` when an array is passed
-            for `segment_start_idxs` that has th following properties;
-                - both should have equal length
-                - all values in ``segment_start_idxs`` should be <= ``segment_end_idxs``
+            When you pass arrays to both ``segment_start_idxs`` and
+            ``segment_end_idxs``, the corresponding index-values of these arrays will be
+            used as segment-ranges. As a result, the following properties must be met:\n
+              - both arrays should have equal length
+              - all values in ``segment_start_idxs`` should be <= ``segment_end_idxs``
     start_idx: Union[float, pd.Timestamp], optional
         The start-index which will be used for each series passed to `data`. This is
-        especially useful if multiple `StridedRolling` instances are created and the
+        especially useful if multiple ``StridedRolling`` instances are created and the
         user want to ensure same (start-)indexes for each of them.
     end_idx: Union[float, pd.Timestamp], optional
         The end-index which will be used as sliding end-limit for each series passed to
         `data`.
     func_data_type: Union[np.array, pd.Series], optional
         The data type of the stroll (either np.array or pd.Series), by default np.array.
         <br>
         .. Note::
             Make sure to only set this argument to pd.Series when this is really
             required, since pd.Series strided-rolling is significantly less efficient.
             For a np.array it is possible to create very efficient views, but there is
             no such thing as a pd.Series view. Thus, for each stroll, a new series is
-            created.
+            created, inducing a lot of non-feature calculation of overhead.
     window_idx : str, optional
         The window's index position which will be used as index for the
         feature_window aggregation. Must be either of: `["begin", "middle", "end"]`, by
         default "end".
     include_final_window: bool, optional
         Whether the final (possibly incomplete) window should be included in the
         strided-window segmentation, by default False.
 
         .. Note::
-            The remarks below apply when `include_final_window` is set to True.
+            The remarks below apply when ``include_final_window`` is set to True.
             The user should be aware that the last window *might* be incomplete, i.e.;
 
             - when equally sampled, the last window *might* be smaller than the
               the other windows.
             - when not equally sampled, the last window *might* not include all the
                 data points (as the begin-time + window-size comes after the last data
                 point).
@@ -112,17 +117,20 @@
 
     Notes
     -----
     * This instance withholds a **read-only**-view of the data its values.
 
     """
 
-    # Class variables which are used by sub-classes
+    # Class variables which are used by subclasses
     win_str_type: DataType
     reset_series_index_b4_segmenting: bool = False
+    OUTSIDE_DATA_BOUNDS_WARNING: str = (
+        "Some segment indexes are outside the range of the data its index."
+    )
 
     # Create the named tuple
     _NumpySeriesContainer = namedtuple(
         "SeriesContainer", ["name", "values", "start_indexes", "end_indexes"]
     )
 
     def __init__(
@@ -180,38 +188,38 @@
         # Especially useful when the index dtype differs from the win-stride-dtype
         # e.g. -> performing a int-based stroll on time-indexed data
         # Note: this is very niche and thus requires advanced knowledge
         # TODO: this code can be omitted if we remove TimeIndexSampleStridedRolling
         self._update_start_end_indices_to_stroll_type(series_list)
 
         # 2. Construct the index ranges
-        # Either use the passed segment indices or compute the start or end times of the 
+        # Either use the passed segment indices or compute the start or end times of the
         # segments. The segment indices have precedence over the stride (and window) for
         # index computation.
         if segment_start_idxs is not None or segment_end_idxs is not None:
             self.strides = None
             if segment_start_idxs is not None and segment_end_idxs is not None:
                 # When both the start and end points are passed, the window does not
                 # matter.
                 self.window = None
                 np_start_times = self._parse_segment_idxs(segment_start_idxs)
                 np_end_times = self._parse_segment_idxs(segment_end_idxs)
             elif segment_start_idxs is not None:  # segment_end_idxs is None
                 np_start_times = self._parse_segment_idxs(segment_start_idxs)
                 np_end_times = np_start_times + self._get_np_value(self.window)
-            elif segment_end_idxs is not None:  # segment_start_idxs is None
+            else:  # segment_end_idxs is not None and segment_start_idxs is None
                 np_end_times = self._parse_segment_idxs(segment_end_idxs)
                 np_start_times = np_end_times - self._get_np_value(self.window)
         else:
             np_start_times = self._construct_start_idxs()
             np_end_times = np_start_times + self._get_np_value(self.window)
 
         # Check the numpy start and end indices
         _check_start_end_array(np_start_times, np_end_times)
-        
+
         # 3. Create a new-index which will be used for DataFrame reconstruction
         # Note: the index-name of the first passed series will be re-used as index-name
         self.index = self._get_output_index(
             np_start_times, np_end_times, name=series_list[0].index.name
         )
 
         # 4. Store the series containers
@@ -226,49 +234,51 @@
                 if np.ptp(container.end_indexes - container.start_indexes) != 0:
                     warnings.warn(
                         f"There are gaps in the sequence of the {container.name}"
                         f"-series!",
                         RuntimeWarning,
                     )
 
-    def _calc_nb_feats_for_stride(self, stride) -> int:
-        """Calculate the number of features for a given stride."""
+    def _calc_nb_segments_for_stride(self, stride) -> int:
+        """Calculate the number of output items (segments) for a given single stride."""
         nb_feats = max((self.end - self.start - self.window) // stride + 1, 0)
         # Add 1 if there is still some data after (including) the last window its
         # start index - this is only added when `include_last_window` is True.
         nb_feats += self.include_final_window * (
             self.start + stride * nb_feats <= self.end
         )
         return nb_feats
 
     def _get_np_start_idx_for_stride(self, stride: T) -> np.ndarray:
-        """Compute the start index for the given stride."""
+        """Compute the start index for the given single stride."""
         # ---------- Efficient numpy code -------
         np_start = self._get_np_value(self.start)
         np_stride = self._get_np_value(stride)
         # Compute the start times (these remain the same for each series)
         return np.arange(
             start=np_start,
-            stop=np_start + self._calc_nb_feats_for_stride(stride) * np_stride,
+            stop=np_start + self._calc_nb_segments_for_stride(stride) * np_stride,
             step=np_stride,
         )
 
     def _construct_start_idxs(self) -> np.ndarray:
         """Construct the start indices of the segments (for all stride values).
-        
+
         To realize this, we compute the start idxs for each stride and then merge them
-        together (without duplicates) in a sorted array. 
+        together (without duplicates) in a sorted array.
         """
         start_idxs = []
         for stride in self.strides:
             start_idxs += [self._get_np_start_idx_for_stride(stride)]
         # note - np.unique also sorts the array
         return np.unique(np.concatenate(start_idxs))
 
-    def _get_output_index(self, start_idxs: np.ndarray, end_idxs: Union[np.ndarray, None], name: str) -> pd.Index:
+    def _get_output_index(
+        self, start_idxs: np.ndarray, end_idxs: Union[np.ndarray, None], name: str
+    ) -> pd.Index:
         """Construct the output index."""
         if self.window_idx == "end":
             return pd.Index(end_idxs, name=name)
         elif self.window_idx == "middle":
             return pd.Index(
                 start_idxs + ((end_idxs - start_idxs) / 2),
                 name=name,
@@ -280,28 +290,29 @@
                 f"window index {self.window_idx} must be either of: "
                 "['end', 'middle', 'begin']"
             )
 
     def _construct_series_containers(
         self, series_list, np_start_times, np_end_times
     ) -> List[StridedRolling._NumpySeriesContainer]:
-
         series_containers: List[StridedRolling._NumpySeriesContainer] = []
         for series in series_list:
             if not self.reset_series_index_b4_segmenting:
                 np_idx_times = series.index.values
             else:
                 np_idx_times = np.arange(len(series))
+                # note: using pd.RangeIndex instead of arange gives the same performance
 
             series_name = series.name
-            if self.data_type is np.array:
+            if self.data_type is np.array:  # FuncWrapper.input_type is np.array
                 # create a non-writeable view of the series
-                series = series.values
+                series = series.values  # np.array will be stored in the SeriesContainer
                 series.flags.writeable = False
-            elif self.data_type is pd.Series:
+            elif self.data_type is pd.Series:  # FuncWrapper.input_type is pd.Series
+                # pd.Series will be stored in the SeriesContainer
                 series.values.flags.writeable = False
                 series.index.values.flags.writeable = False
             else:
                 raise ValueError("unsupported datatype")
 
             series_containers.append(
                 StridedRolling._NumpySeriesContainer(
@@ -346,25 +357,25 @@
         * If you want to calculate one-to-many, ``func`` should be
           a ``FuncWrapper`` instance and explicitly use
           the ``output_names`` attributes of its constructor.
 
         """
         feat_names = func.output_names
 
-        t_start = time.time()
+        t_start = time.perf_counter()
 
         # --- Future work ---
         # would be nice if we could optimize this double for loop with something
         # more vectorized
         #
         # As for now we use a map to apply the function (as this evaluates its
         # expression only once, whereas a list comprehension evaluates its expression
         # every time).
         # See more why: https://stackoverflow.com/a/59838723
-        out: np.array = None
+        out: np.array
         if func.vectorized:
             # Vectorized function execution
 
             ## IMPL 1
             ## Results in a high memory peak as a new np.array is created (and thus no
             ## view is being used)
             # out = np.asarray(
@@ -415,15 +426,18 @@
                         + "segmented window!"
                     )
                     assert np.all(
                         strides == strides[0]
                     ), "Vectorized functions require same number of samples as stride!"
                     views.append(
                         _sliding_strided_window_1d(
-                            sc.values[sc.start_indexes[0]:], windows[0], strides[0], len(self.index)
+                            sc.values[sc.start_indexes[0] :],
+                            windows[0],
+                            strides[0],
+                            len(self.index),
                         )
                     )
 
             # Assign empty array as output when there is no view to apply the vectorized
             # function on (this is the case when there is at least for one series no
             # feature windows)
             out = func(*views) if len(views) >= 1 else np.array([])
@@ -431,15 +445,15 @@
             out_type = type(out)
             out = np.asarray(out)
             # When multiple outputs are returned (= tuple) they should be transposed
             # when combining into an array
             out = out.T if out_type is tuple else out
 
         else:
-            # Sequential function execution (default)
+            # Function execution over slices (default)
             out = np.array(
                 list(
                     map(
                         func,
                         *[
                             [
                                 sc.values[sc.start_indexes[idx] : sc.end_indexes[idx]]
@@ -453,70 +467,56 @@
 
         # Check if the function output is valid.
         # This assertion will be raised when e.g. np.max is applied vectorized without
         # specifying axis=1.
         assert out.ndim > 0, "Vectorized function returned only 1 (non-array) value!"
 
         # Aggregate function output in a dictionary
-        feat_out = {}
-        if out.ndim == 1 and not len(out):
-            # When there are no features calculated (due to no feature windows)
-            assert not len(self.index)
-            for f_name in feat_names:
-                # Will be discarded (bc no index)
-                feat_out[self._create_feat_col_name(f_name)] = None
-        elif out.ndim == 1 or (out.ndim == 2 and out.shape[1] == 1):
-            assert len(feat_names) == 1, f"Func {func} returned more than 1 output!"
-            feat_out[self._create_feat_col_name(feat_names[0])] = out.flatten()
-        else:
-            assert out.ndim == 2 and out.shape[1] > 1
-            assert (
-                len(feat_names) == out.shape[1]
-            ), f"Func {func} returned incorrect number of outputs ({out.shape[1]})!"
-            for col_idx in range(out.shape[1]):
-                feat_out[self._create_feat_col_name(feat_names[col_idx])] = out[
-                    :, col_idx
-                ]
-
-        elapsed = time.time() - t_start
-        log_strides = "manual" if self.strides is None else tuple(map(str, self.strides))
+        output_names = list(map(self._create_feat_col_name, feat_names))
+        feat_out = _process_func_output(out, self.index, output_names, str(func))
+        # Log the function execution time
+        log_strides = (
+            "manual" if self.strides is None else tuple(map(str, self.strides))
+        )
         log_window = "manual" if self.window is None else self.window
-        logger.info(
-            f"Finished function [{func.func.__name__}] on "
-            f"{[self.series_key]} with window-stride "
-            f"[{log_window}, {log_strides}] in [{elapsed} seconds]!"
+        _log_func_execution(
+            t_start, func, self.series_key, log_window, log_strides, output_names
         )
 
-        return pd.DataFrame(index=self.index, data=feat_out)
-
-    def _update_start_end_indices_to_stroll_type(self, series_list: List[pd.Series]):
-        pass
+        return pd.DataFrame(feat_out, index=self.index)
 
     # --------------------------------- STATIC METHODS ---------------------------------
-    # @staticmethod
-    # def calc_nb_features(start, end, window, stride, include_final_window=False) -> int:
-    #     nb_feats = max((end - start - window) // stride + 1, 0)
-    #     # Add 1 if there is still some data after (including) the last window its
-    #     # start index - this is only added when `include_last_window` is True.
-    #     nb_feats += include_final_window * (start + stride * nb_feats <= end)
-    #     return nb_feats
-
     @staticmethod
     def _get_np_value(val):
         # Convert everything to int64
         if isinstance(val, pd.Timestamp):
             return val.to_datetime64()
         elif isinstance(val, pd.Timedelta):
             return val.to_timedelta64()
         else:
             return val
 
+    @staticmethod
+    def construct_output_index(
+        series_keys: Union[str, Tuple[str, ...]], feat_name: str, win_str: str
+    ) -> str:
+        series_keys = to_tuple(series_keys)
+        return f"{'|'.join(series_keys)}__{feat_name}__w={win_str}"
+
     # ----------------------------- OVERRIDE THESE METHODS -----------------------------
     @abstractmethod
+    def _update_start_end_indices_to_stroll_type(self, series_list: List[pd.Series]):
+        # NOTE: This method will only be implemented (with code != pass) in the
+        # TimeIndexSampleStridedRolling
+        raise NotImplementedError
+
+    @abstractmethod
     def _parse_segment_idxs(self, segment_idxs: np.ndarray) -> np.ndarray:
+        """Check the segment indexes array to lie between self.start and self.end and
+        convert it to the correct dtype (if necessary)."""
         raise NotImplementedError
 
     @abstractmethod
     def _create_feat_col_name(self, feat_name: str) -> str:
         raise NotImplementedError
 
 
@@ -530,26 +530,30 @@
         **kwargs,
     ):
         # Set the data type & call the super constructor
         self.win_str_type = DataType.SEQUENCE
         super().__init__(data, window, strides, *args, **kwargs)
 
     # ------------------------------- Overridden methods -------------------------------
+    def _update_start_end_indices_to_stroll_type(self, series_list: List[pd.Series]):
+        pass
+
     def _parse_segment_idxs(self, segment_idxs: np.ndarray) -> np.ndarray:
-        return segment_idxs[(segment_idxs >= self.start) & (segment_idxs <= self.end)]
+        if any((segment_idxs < self.start) | (segment_idxs > self.end)):
+            warnings.warn(self.OUTSIDE_DATA_BOUNDS_WARNING, RuntimeWarning)
+        return segment_idxs
 
     def _create_feat_col_name(self, feat_name: str) -> str:
-        # TODO -> this is not that loosely coupled if we want somewhere else in the code
-        #        to also reproduce col-name construction
-        win_str = "w="
         if self.window is not None:
-            win_str += str(self.window)
+            win_str = str(self.window)
         else:
-            win_str += "manual"
-        return f"{'|'.join(self.series_key)}__{feat_name}__{win_str}"
+            win_str = "manual"
+        return self.construct_output_index(
+            series_keys=self.series_key, feat_name=feat_name, win_str=win_str
+        )
 
 
 class TimeStridedRolling(StridedRolling):
     def __init__(
         self,
         data: Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]]],
         window: pd.Timedelta,
@@ -557,51 +561,61 @@
         *args,
         **kwargs,
     ):
         # Check that each series / dataframe has the same tz
         data = to_series_list(data)
         tz_index = data[0].index.tz
         for data_entry in to_series_list(data)[1:]:
-            assert data_entry.index.tz == tz_index
+            assert (
+                data_entry.index.tz == tz_index
+            ), "strided rolling input data must all have same timezone"
         self._tz_index = tz_index
         # Set the data type & call the super constructor
         self.win_str_type = DataType.TIME
         super().__init__(data, window, strides, *args, **kwargs)
 
-    # -------------------------------- Extended methdos --------------------------------
-    def _get_output_index(self, start_idxs: np.ndarray, end_idxs: np.ndarray, name: str) -> pd.Index:
+    # -------------------------------- Extended methods --------------------------------
+    def _get_output_index(
+        self, start_idxs: np.ndarray, end_idxs: np.ndarray, name: str
+    ) -> pd.Index:
         assert start_idxs.dtype.type == np.datetime64
         assert end_idxs.dtype.type == np.datetime64
+        if not len(start_idxs):  # to fix "datetime64 values must have a unit specified"
+            assert not len(end_idxs)
+            start_idxs = start_idxs.astype("datetime64[ns]")
+            end_idxs = end_idxs.astype("datetime64[ns]")
         start_idxs = pd.to_datetime(start_idxs, utc=True).tz_convert(self._tz_index)
         end_idxs = pd.to_datetime(end_idxs, utc=True).tz_convert(self._tz_index)
         return super()._get_output_index(start_idxs, end_idxs, name)
 
     # ------------------------------- Overridden methods -------------------------------
+    def _update_start_end_indices_to_stroll_type(self, series_list: List[pd.Series]):
+        pass
+
     def _parse_segment_idxs(self, segment_idxs: np.ndarray) -> np.ndarray:
-        if len(segment_idxs) == 0:
-            return segment_idxs.astype(np.datetime64)
-        start_ = self.start; end_ = self.end;
+        segment_idxs = segment_idxs.astype("datetime64")
+        start_, end_ = self.start, self.end
         if start_.tz is not None:
+            # Convert to UTC (allowing comparison with the segment_idxs)
             assert end_.tz is not None
             start_ = start_.tz_convert(None)
             end_ = end_.tz_convert(None)
-        valid_range = (segment_idxs >= start_) & (segment_idxs <= end_)
-        return segment_idxs[valid_range].astype(np.datetime64)
-
-    # TODO: how bad is it that we don't have freq information anymore?
-    # def _construct_output_index(self, series: pd.Series) -> pd.DatetimeIndex:
+        if any((segment_idxs < start_) | (segment_idxs > end_)):
+            warnings.warn(self.OUTSIDE_DATA_BOUNDS_WARNING, RuntimeWarning)
+        return segment_idxs
 
     def _create_feat_col_name(self, feat_name: str) -> str:
         # Convert win to time-string if available :)
-        win_str = "w="
         if self.window is not None:
-            win_str += timedelta_to_str(self.window)
+            win_str = timedelta_to_str(self.window)
         else:
-            win_str += "manual"
-        return f"{'|'.join(self.series_key)}__{feat_name}__{win_str}"
+            win_str = "manual"
+        return self.construct_output_index(
+            series_keys=self.series_key, feat_name=feat_name, win_str=win_str
+        )
 
 
 class TimeIndexSampleStridedRolling(SequenceStridedRolling):
     def __init__(
         self,
         # TODO -> update arguments
         data: Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]]],
@@ -617,14 +631,19 @@
             When `data` consists of multiple independently sampled series
             (e.g. feature functions which take multiple series as input),
             The time-**index of each series**: \n
             - must _roughly_ **share** the same **sample frequency**.
             - will be first time-aligned before transitioning to sample-segmentation by
               using the inner bounds
 
+        .. Note::
+            `TimeIndexSampleStridedRolling` **does not support** the
+            ``segment_start_idxs`` and ``segment_end_idxs`` arguments. Setting these
+            will raise a NotImplementedError.
+
         """
         if segment_start_idxs is not None or segment_end_idxs is not None:
             raise NotImplementedError(
                 "TimeIndexSampleStridedRolling is not implemented to support passing"
                 + "segment_start_idxs or segment_end_idxs"
             )
```

### Comparing `tsflex-0.3rc0/tsflex/features/segmenter/strided_rolling_factory.py` & `tsflex-0.4.0/tsflex/features/segmenter/strided_rolling_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 .. TODO::
     Also create a (SegmenterFactory) which the StridedRollingFactory implements
 
 """
 
 __author__ = "Jonas Van Der Donckt"
 
+from ...utils.attribute_parsing import AttributeParser, DataType
 from .strided_rolling import (
-    StridedRolling,
-    TimeStridedRolling,
     SequenceStridedRolling,
+    StridedRolling,
     TimeIndexSampleStridedRolling,
+    TimeStridedRolling,
 )
-from ...utils.attribute_parsing import AttributeParser, DataType
 
 
 class StridedRollingFactory:
     """Factory class for creating the appropriate StridedRolling segmenter."""
 
     _datatype_to_stroll = {
         DataType.TIME: TimeStridedRolling,
@@ -43,31 +43,31 @@
         **kwargs : dict, optional
             Additional keyword arguments, see the `StridedRolling` its documentation
             for more info.
 
         .. Note::
             When passing `time-based` data, but **int**-based window & stride params,
             the strided rolling will be `TimeIndexSampleStridedRolling`. This class
-            **assumes** that **all data series** _roughly_ have the 
-            **same sample frequency**, as  the windows and strides are interpreted in 
+            **assumes** that **all data series** _roughly_ have the
+            **same sample frequency**, as  the windows and strides are interpreted in
             terms of **number of samples**.
 
         Raises
         ------
         ValueError
-            When incompatible data & window-stride data types are passed (e.g. time 
+            When incompatible data & window-stride data types are passed (e.g. time
             window-stride args on sequence data-index).
 
         Returns
         -------
         StridedRolling
             The constructed StridedRolling instance.
 
         """
-        data_dtype = AttributeParser.determine_type(data)  
+        data_dtype = AttributeParser.determine_type(data)
         if strides is None:
             args_dtype = AttributeParser.determine_type(window)
         else:
             args_dtype = AttributeParser.determine_type([window] + strides)
 
         if window is None or data_dtype.value == args_dtype.value:
             return StridedRollingFactory._datatype_to_stroll[data_dtype](
```

### Comparing `tsflex-0.3rc0/tsflex/features/utils.py` & `tsflex-0.4.0/tsflex/features/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,66 @@
 """Utility functions for more convenient feature extraction."""
 
 __author__ = "Jeroen Van Der Donckt, Jonas Van Der Donckt"
 
-from typing import Callable, Any, Optional, List, Union, Tuple
+import time
+from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
-from .feature import FuncWrapper
+from .function_wrapper import FuncWrapper, _get_name
+from .logger import logger
 
+# Declare a type variable
+T = TypeVar("T")
 
 # ---------------------------------- PRIVATE METHODS ----------------------------------
+def _process_func_output(
+    out: np.ndarray, index: np.ndarray, output_names: List[str], func_str: str
+) -> Dict[str, np.ndarray]:
+    """Process the output of a feature function into a dictionary."""
+    feat_out = {}
+    if out.ndim == 1 and not len(out):
+        # When there are no features calculated (due to no feature windows)
+        assert not len(index)
+        for o_name in output_names:
+            # Will be discarded (bc no index)
+            feat_out[o_name] = None
+    elif out.ndim == 1 or (out.ndim == 2 and out.shape[1] == 1):
+        assert len(output_names) == 1, f"Func {func_str} returned more than 1 output!"
+        feat_out[output_names[0]] = out.flatten()
+    else:
+        assert out.ndim == 2 and out.shape[1] > 1
+        assert (
+            len(output_names) == out.shape[1]
+        ), f"Func {func_str} returned incorrect number of outputs ({out.shape[1]})!"
+        for col_idx in range(out.shape[1]):
+            feat_out[output_names[col_idx]] = out[:, col_idx]
+
+    return feat_out
+
+
+def _log_func_execution(
+    t_start: float,
+    func: FuncWrapper,
+    series_key: Tuple[str],
+    log_window: Optional[T],
+    log_strides: Optional[Union[str, Tuple[str]]],
+    output_names: List[str],
+):
+    """Log the execution time of a feature function."""
+    elapsed = time.perf_counter() - t_start
+
+    logger.info(
+        f"Finished function [{_get_name(func.func)}] on "
+        f"{[series_key]} with window-stride [{log_window}, {log_strides}] "
+        f"with output {output_names} in [{elapsed} seconds]!"
+    )
+
 
 def _determine_bounds(bound_method, series_list: List[pd.Series]) -> Tuple[Any, Any]:
     """Determine the bounds of the passed series.
 
     Parameters
     ----------
     bound_method: str
@@ -52,54 +98,32 @@
     else:
         raise ValueError(f"invalid bound method string passed {bound_method}")
 
 
 def _check_start_end_array(start_idxs: np.ndarray, end_idxs: np.ndarray):
     """Check if the start and end indices are valid.
 
-    These are vaild if they are of the same length and if the start indices are smaller
+    These are valid if they are of the same length and if the start indices are smaller
     than the end indices.
 
     Parameters
     ----------
     start_idxs: np.ndarray
         The start indices.
     end_idxs: np.ndarray
         The end indices.
     """
-    assert len(start_idxs) == len(end_idxs), (
-        "start_idxs and end_ixs must have equal length"
-    )
-    assert np.all(start_idxs <= end_idxs), (
-        "for all corresponding values: segment_start_idxs <= segment_end_idxs"
-    )
+    assert len(start_idxs) == len(
+        end_idxs
+    ), "start_idxs and end_ixs must have equal length"
+    assert np.all(
+        start_idxs <= end_idxs
+    ), "for all corresponding values: segment_start_idxs <= segment_end_idxs"
 
 
-def _get_name(func: Callable) -> str:
-    """Get the name of the function.
-
-    Parameters
-    ----------
-    func: Callable
-        The function whose name has to be returned, should be either a function or an
-        object that is callable.
-
-    Returns
-    -------
-    str
-        The name of ``func`` in case of a function or the name of the class in case
-        of a callable object.
-
-    """
-    assert callable(func), f"The given argument {func} is not callable!"
-    try:
-        return func.__name__
-    except:
-        return type(func).__name__
-
 def _get_funcwrapper_func_and_kwargs(func: FuncWrapper) -> Tuple[Callable, dict]:
     """Extract the function and keyword arguments from the given FuncWrapper.
 
     Parameters
     ----------
     func: FuncWrapper
         The FuncWrapper to extract the function and kwargs from.
@@ -113,15 +137,15 @@
     """
     assert isinstance(func, FuncWrapper)
 
     # Extract the function (is a Callable)
     function = func.func
 
     # Extract the keyword arguments
-    func_wrapper_kwargs = {}
+    func_wrapper_kwargs = dict()
     func_wrapper_kwargs["output_names"] = func.output_names
     func_wrapper_kwargs["input_type"] = func.input_type
     func_wrapper_kwargs["vectorized"] = func.vectorized
     func_wrapper_kwargs.update(func.kwargs)
 
     return function, func_wrapper_kwargs
 
@@ -168,45 +192,47 @@
         if any([len(s) < min_nb_samples for s in series]):
             if not isinstance(output_names, list) or len(output_names) == 1:
                 return error_val
             return tuple([error_val] * len(output_names))
         return func(*series, **kwargs)
 
     wrap_func.__name__ = "[robust]__" + _get_name(func)
-    if not "output_names" in func_wrapper_kwargs.keys():
+    if "output_names" not in func_wrapper_kwargs.keys():
         func_wrapper_kwargs["output_names"] = _get_name(func)
 
     return FuncWrapper(wrap_func, **func_wrapper_kwargs)
 
 
 # ---------------------------------- PUBLIC METHODS -----------------------------------
-
 def make_robust(
     funcs: Union[Callable, FuncWrapper, List[Union[Callable, FuncWrapper]]],
     min_nb_samples: Optional[int] = 1,
     error_val: Optional[Any] = np.nan,
     passthrough_nans: Optional[bool] = True,
 ) -> Union[FuncWrapper, List[FuncWrapper]]:
     """Decorate `funcs` into one or multiple robust FuncWrappers.
 
-     More specifically this method does:\n
+     More specifically this method does (in the following order):\n
      * `np.NaN` data input propagation / filtering
      *  `min_nb_samples` checking before feeding to `func`
         (if not met, returns `error_val`)\n
      Note: this wrapper is useful for functions that should be robust for empty or
      sparse windows and/or nans in the data.
 
     Parameters
     ----------
     funcs: Union[Callable, FuncWrapper, List[Union[Callable, FuncWrapper]]]
         The function which will be made robust.
     min_nb_samples: int, optional
-        The minimum number of samples that are needed for `func` to be applied, by
-        default 1.
-        successfully.
+        The minimum number of samples that are needed for `func` to be applied
+        successfully, by default 1.
+        .. Note::
+            The number of samples are determined after the `passthrough_nans` filter
+            took place.
+
     error_val: Any, optional
         The error *return* value if the `min_nb_samples` requirement is not met, by
         default `np.NaN`.
     passthrough_nans: bool, optional
         If set to true, `np.NaN` values, which occur in the data will be passed through.
         Otherwise, the `np.NaN` values will be masked out before being passed to `func`,
         by default True.
```

### Comparing `tsflex-0.3rc0/tsflex/processing/logger.py` & `tsflex-0.4.0/tsflex/processing/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 See Also
 --------
 SeriesPipeline : its `logging_file_path` of the `process` method.
 
 """
 
-__author__ = "Jeroen Van Der Donckt"
+__author__ = "Jeroen Van Der Donckt, Jonas Van Der Donckt"
 
 import logging
-import pandas as pd
 import re
 
+import pandas as pd
+
 from ..utils.logging import logging_file_to_df, remove_inner_brackets
 
 # Package specific logger
 logger = logging.getLogger("feature_processing_logger")
 logger.setLevel(logging.DEBUG)
 
 # Create logger which writes WARNING messages or higher to sys.stderr
@@ -24,47 +25,49 @@
 logger.addHandler(console)
 
 
 def _parse_message(message: str) -> list:
     """Parse the message of the logged info."""
     regex = r"\[(.*?)\]"
     matches = re.findall(regex, remove_inner_brackets(message))
-    assert len(matches) == 3
+    assert len(matches) == 4
     func = matches[0]
     series_names = matches[1].replace("'", "")
-    duration_s = float(matches[2].rstrip(" seconds"))
-    return [func, series_names, duration_s]
+    output_names = matches[2].replace("'", "")
+    duration_s = float(matches[3].rstrip(" seconds"))
+    return [func, series_names, output_names, duration_s]
 
 
 def _parse_logging_execution_to_df(logging_file_path: str) -> pd.DataFrame:
-    """Parse the logged messages into a dataframe that contains execution info.
+    """Parse the logged messages into a DataFrame that contains execution info.
 
     Parameters
     ----------
     logging_file_path: str
         The file path where the logged messages are stored. This is the file path that
-        is passed to the ``SeriesPipeline`` its process method.
+        is passed to the ``SeriesPipeline`` its ``process`` method.
 
     Returns
     -------
     pd.DataFrame
-        A DataFrame with the processor its method, series names and calculation 
-        duration.
+        A DataFrame with the processor its method, series names, output names, and
+        (%) calculation duration.
 
     Note
     ----
-    This function only works when the ``logging_file_path`` used in a
-    ``SeriesPipeline`` its ``process`` method is passed.
+    This function only works when the ``logging_file_path`` used in a ``SeriesPipeline``
+    its ``process`` method is passed.
 
     """
     df = logging_file_to_df(logging_file_path)
-    df[["function", "series_names", "duration"]] = pd.DataFrame(
+    df[["function", "series_names", "output_names", "duration"]] = pd.DataFrame(
         list(df["message"].apply(_parse_message)),
         index=df.index,
     )
+    df["duration %"] = (100 * (df["duration"] / df["duration"].sum())).round(2)
     return df.drop(columns=["name", "log_level", "message"])
 
 
 def get_processor_logs(logging_file_path: str) -> pd.DataFrame:
     """Get execution (time) info for each processor of a ``SeriesPipeline``.
 
     Parameters
@@ -72,13 +75,14 @@
     logging_file_path: str
         The file path where the logged messages are stored. This is the file path that
         is passed to the ``SeriesPipeline`` its ``process`` method.
 
     Returns
     -------
     pd.DataFrame
-        A DataFrame containing each processor its duration and its series names.
-    
+        A DataFrame containing each processor its series names, output names, and
+        (%) duration.
+
     """
     df = _parse_logging_execution_to_df(logging_file_path)
     df["duration"] = pd.to_timedelta(df["duration"], unit="s")
     return df
```

### Comparing `tsflex-0.3rc0/tsflex/processing/series_pipeline.py` & `tsflex-0.4.0/tsflex/processing/series_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import dill
 import pandas as pd
 
+from ..utils.data import flatten, series_dict_to_df, to_series_list
+from ..utils.logging import add_logging_handler, delete_logging_handlers
 from .logger import logger
 from .series_processor import SeriesProcessor
-from ..utils.data import series_dict_to_df, to_series_list, flatten
-from ..utils.logging import delete_logging_handlers, add_logging_handler
 
 
 class _ProcessingError(Exception):
     pass
 
 
 class SeriesPipeline:
@@ -76,15 +76,15 @@
         """
         if isinstance(processor, SeriesProcessor):
             self.processing_steps.append(processor)
         elif isinstance(processor, SeriesPipeline):
             self.processing_steps.extend(processor.processing_steps)
         else:
             raise TypeError(
-                f"Can only append SeriesProcessor or SeriesPipeline, "
+                "Can only append SeriesProcessor or SeriesPipeline, "
                 + f"not {type(processor)}"
             )
 
     def insert(
         self, idx: int, processor: Union[SeriesProcessor, SeriesPipeline]
     ) -> None:
         """Insert a ``SeriesProcessor`` at the given index in the pipeline.
@@ -105,15 +105,15 @@
         if isinstance(processor, SeriesProcessor):
             self.processing_steps.insert(idx, processor)
         elif isinstance(processor, SeriesPipeline):
             for i, ps in enumerate(processor.processing_steps):
                 self.insert(idx + i, ps)
         else:
             raise TypeError(
-                f"Can only insert a SeriesProcessor or SeriesPipeline, "
+                "Can only insert a SeriesProcessor or SeriesPipeline, "
                 + f"not {type(processor)}"
             )
 
     def process(
         self,
         data: Union[pd.Series, pd.DataFrame, List[Union[pd.Series, pd.DataFrame]]],
         return_df: Optional[bool] = False,
```

### Comparing `tsflex-0.3rc0/tsflex/processing/series_processor.py` & `tsflex-0.4.0/tsflex/processing/series_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code for time-series data (pre-)processing."""
 
 __author__ = "Jonas Van Der Donckt, Emiel Deprost, Jeroen Van Der Donckt"
 
 import time
-from typing import Callable, Dict, List, Union, Tuple
+from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from .. import __pdoc__
 from ..utils.classes import FrozenClass
+from ..utils.data import flatten, series_dict_to_df, to_list, to_tuple
 from .logger import logger
-from ..utils.data import series_dict_to_df, to_list, to_tuple, flatten
 
-__pdoc__['SeriesProcessor.__call__'] = True
+__pdoc__["SeriesProcessor.__call__"] = True
 
 
 def dataframe_func(func: Callable):
     """Decorate function to use a DataFrame instead of multiple series (as argument).
 
     This decorator can be used for functions that need to work on a whole
     `pd.DataFrame`. It will convert the required series into a DataFrame using an
@@ -105,14 +105,15 @@
     * a `pd.DataFrame` with (one) column name equal to the input series its name.
     * a list of `pd.Series` in which (exact) one series has the same name as the
       input series.
 
     Series (& columns) with other (column) names will be added to the series dict.
 
     """
+
     def __init__(
         self,
         function: Callable,
         series_names: Union[str, Tuple[str, ...], List[str], List[Tuple[str, ...]]],
         **kwargs,
     ):
         series_names = [to_tuple(names) for names in to_list(series_names)]
@@ -170,15 +171,15 @@
           This internal representation is constructed in the `process` method of the
           `SeriesPipeline`.
         * If you want to test or debug your `SeriesProcessor` object, just encapsulate
           your instance of this class in a `SeriesPipeline`. The latter allows more
           versatile input for its `process` method.
 
         """
-        t_start = time.time()
+        t_start = time.perf_counter()
 
         # Only selecting the series that are needed for this processing step
         # requested_dict = {}
         # try:
         #     for sig in self.get_required_series():
         #         requested_dict[sig] = series_dict[sig]
         # except KeyError as key:
@@ -210,18 +211,18 @@
             )
             # Check that the output of the function call produces unique columns / keys
             assert (
                 len(set(processed_output.keys()).intersection(func_output.keys())) == 0
             )
             processed_output.update(func_output)
 
-        elapsed = time.time() - t_start
+        elapsed = time.perf_counter() - t_start
         logger.info(
-            f"Finished function [{self.name}] on {self.series_names} in "
-            f"[{elapsed} seconds]!"
+            f"Finished function [{self.name}] on {self.series_names} with output "
+            f"{list(processed_output.keys())} in [{elapsed} seconds]!"
         )
 
         return processed_output
 
     def __repr__(self):
         """Return formal representation of object."""
         repr_str = self.name + (" " + str(self.kwargs))
@@ -231,14 +232,15 @@
     def __str__(self):
         """Return informal representation of object."""
         return self.__repr__()
 
 
 # ---------------------- utility functions for a SeriesProcessor ----------------------
 
+
 def _np_array_to_series(np_array: np.ndarray, series: pd.Series) -> pd.Series:
     """Convert the `np_array` into a pandas Series.
 
     Parameters
     ----------
     np_array: np.ndarray
         The numpy array that needs to be converted to a pandas Series.
@@ -346,15 +348,17 @@
         # Must be constructed from just 1 series
         # => the input series will be replaced by this array
         assert len(required_dict) == 1
         # Create a series with the same view
         input_series = list(required_dict.values())[0]
         return {str(input_series.name): _np_array_to_series(func_output, input_series)}
 
-    elif isinstance(func_output, list) and all([isinstance(el, pd.Series) for el in func_output]):
+    elif isinstance(func_output, list) and all(
+        [isinstance(el, pd.Series) for el in func_output]
+    ):
         # Convert the list of series into a series dict, using the same data reference
         # => if for any series in the list, series.name is in the required_dict, than
         #    the the original series will be replaced by this new series.
         # Assert that all outputs have different names
         assert len(set([s.name for s in func_output])) == len(func_output)
         assert all([isinstance(s.index, pd.DatetimeIndex) for s in func_output])
         return {s.name: s for s in func_output}
```

### Comparing `tsflex-0.3rc0/tsflex/processing/utils.py` & `tsflex-0.4.0/tsflex/processing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*- # TODO: rename file
 """(Advanced) utilities for the processing pipelines."""
 
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt"
 
 import os
 import traceback
-from typing import List, Any, Optional, Union
+from typing import Any, List, Optional, Union
 
 import pandas as pd
 from multiprocess import Pool
 from tqdm.auto import tqdm
 
 from .series_pipeline import SeriesPipeline
 
 
 def process_chunks_multithreaded(
-        same_range_chunks_list: List[List[Union[pd.Series, pd.DataFrame]]],
-        series_pipeline: SeriesPipeline,
-        show_progress: Optional[bool] = True,
-        n_jobs: Optional[int] = None,
-        **processing_kwargs,
+    same_range_chunks_list: List[List[Union[pd.Series, pd.DataFrame]]],
+    series_pipeline: SeriesPipeline,
+    show_progress: Optional[bool] = True,
+    n_jobs: Optional[int] = None,
+    **processing_kwargs,
 ) -> List[Any]:
     """Process `same_range_chunks_list` in a multithreaded manner, order is preserved.
 
     Parameters
     ----------
     same_range_chunks_list: List[List[Union[pd.Series, pd.DataFrame]]]
         A list of same-range-chunks, most likely the output of `chunk_data`.
@@ -67,15 +67,15 @@
     processed_out = None
     with Pool(processes=min(n_jobs, len(same_range_chunks_list))) as pool:
         results = pool.imap(_executor, same_range_chunks_list)
         if show_progress:
             results = tqdm(results, total=len(same_range_chunks_list))
         try:
             processed_out = [f for f in results]
-        except:
+        except Exception:
             traceback.print_exc()
             pool.terminate()
         finally:
             # Close & join because: https://github.com/uqfoundation/pathos/issues/131
             pool.close()
             pool.join()
     return processed_out
```

### Comparing `tsflex-0.3rc0/tsflex/utils/attribute_parsing.py` & `tsflex-0.4.0/tsflex/utils/attribute_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""AttributeParser class for for determining the datatype of the given data."""
+"""AttributeParser class for determining the datatype of the given data."""
 
-__author__ = 'Jonas Van Der Donckt'
+__author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt"
 
 import re
 from enum import IntEnum
 from typing import Any
 
 import pandas as pd
 
 from tsflex.utils.time import parse_time_arg
 
 
 class DataType(IntEnum):
-    """Emum class for supported data types."""
+    """Enum class for supported data types."""
 
     UNDEFINED = 0
     SEQUENCE = 1
     TIME = 2
 
 
 class AttributeParser:
@@ -31,15 +31,14 @@
         if data is None:
             return DataType.UNDEFINED
 
         elif isinstance(data, (pd.Series, pd.DataFrame)):
             dtype_str = str(data.index.dtype)
             if AttributeParser._datetime_regex.match(dtype_str) is not None:
                 return DataType.TIME
-
             elif any(r.match(dtype_str) for r in AttributeParser._numeric_regexes):
                 return DataType.SEQUENCE
 
         elif isinstance(data, (int, float)):
             return DataType.SEQUENCE
 
         elif isinstance(data, (str, pd.Timedelta)):
@@ -55,9 +54,9 @@
                 )
             return dtype_list[0]
 
         raise ValueError(f"Unsupported data type {type(data)}")
 
     @staticmethod
     def check_expected_type(data: Any, expected: DataType) -> bool:
-        """Check wether the given data has the expected datatype."""
+        """Check whether the given data has the expected datatype."""
         return AttributeParser.determine_type(data) == expected
```

### Comparing `tsflex-0.3rc0/tsflex/utils/classes.py` & `tsflex-0.4.0/tsflex/utils/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- # TODO: zetten we dat nu overal of niet?
 """Object-oriented utilities."""
 
-__author__ = 'Jonas Van Der Donckt'
+__author__ = "Jonas Van Der Donckt"
 
 
 class FrozenClass(object):
     """Superclass which allows subclasses to freeze at any time."""
 
     __is_frozen = False
```

### Comparing `tsflex-0.3rc0/tsflex/utils/data.py` & `tsflex-0.4.0/tsflex/utils/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Utility functions for internal data (representation) operations."""
 
 __author__ = "Jeroen Van Der Donckt, Jonas Van Der Donckt"
 
 import itertools
-from typing import Any, Dict, Iterable, Iterator, List, Union, Tuple
+import os
 from pathlib import Path
+from typing import Any, Dict, Iterable, Iterator, List, Tuple, Union
 
-import os
 import numpy as np
 import pandas as pd
 
 SUPPORTED_STROLL_TYPES = [np.array, pd.Series]
 
 
 def series_dict_to_df(series_dict: Dict[str, pd.Series]) -> pd.DataFrame:
@@ -105,15 +105,15 @@
 
 def to_list(x: Any) -> List:
     """Convert the input to a list if necessary.
 
     Parameters
     ----------
     x : Any
-        The input that needs to be convert to a list.
+        The input that needs to be converted into a list.
 
     Returns
     -------
     List
         A list of `x` if `x` wasn't a list yet, otherwise `x`.
 
     """
@@ -124,15 +124,15 @@
 
 def to_tuple(x: Any) -> Tuple[Any, ...]:
     """Convert the input to a tuple if necessary.
 
     Parameters
     ----------
     x : Any
-        The input that needs to be convert to a tuple.
+        The input that needs to be converted into a tuple.
 
     Returns
     -------
     List
         A tuple of `x` if `x` wasn't a tuple yet, otherwise `x`.
 
     """
@@ -155,35 +155,39 @@
         An iterator for the flattened data.
 
     """
     return itertools.chain.from_iterable(data)
 
 
 def load_empatica_data(f_names: Union[str, List[str]]) -> List[pd.DataFrame]:
-    """load example empatica data from the github repository.
+    """load example empatica data from the GitHub repository.
 
     Parameters
     ----------
     f_names : List[str]k
         The name-prefixes of the files, must be one or more from
 
             ["acc", "gsr", "tmp", "ibi"]
 
     Returns
     -------
     List[pd.DataFrame]
         Returns the empatica time-indexed data files in the same order as `f_names`
     """
-    dir = (
+    empatica_dir = (
         Path(__file__)
         .parent.parent.parent.joinpath("examples", "data", "empatica")
         .absolute()
     )
-    dir = str(dir) + "/"  # allows compatible + operation (as with the url)
+    empatica_dir = (
+        str(empatica_dir) + "/"
+    )  # allows compatible + operation (as with the url)
     url = "https://github.com/predict-idlab/tsflex/raw/main/examples/data/empatica/"
-    if not os.path.exists(dir):
-        dir = url  # fetch online if data not local
+    if not os.path.exists(empatica_dir):
+        empatica_dir = url  # fetch online if data not local
     f_names = [f_names] if isinstance(f_names, str) else f_names
     return [
-        pd.read_parquet(dir + f"{f_name.lower()}.parquet").set_index("timestamp")
+        pd.read_parquet(empatica_dir + f"{f_name.lower()}.parquet").set_index(
+            "timestamp"
+        )
         for f_name in f_names
     ]
```

### Comparing `tsflex-0.3rc0/tsflex/utils/logging.py` & `tsflex-0.4.0/tsflex/utils/logging.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Utility functions for logging operations."""
 
 __author__ = "Jeroen Van Der Donckt"
 
 import logging
 import warnings
-import pandas as pd
-
 from pathlib import Path
 from typing import Union
 
+import pandas as pd
+
 
 def remove_inner_brackets(message: str) -> str:
     """Remove the inner brackets i.e., [ or ], from a string, outer brackets are kept.
 
     Parameters
     ----------
     message: str
```

### Comparing `tsflex-0.3rc0/tsflex/utils/time.py` & `tsflex-0.4.0/tsflex/utils/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utility functions for time-related operations."""
 
-__author__ = 'Jonas Van Der Donckt'
+__author__ = "Jonas Van Der Donckt"
 
-import pandas as pd
 from typing import Union
 
+import pandas as pd
+
 
 def timedelta_to_str(td: pd.Timedelta) -> str:
     """Construct a tight string representation for the given timedelta arg.
 
     Parameters
     ----------
     td: pd.Timedelta
@@ -21,22 +22,22 @@
 
     """
     out_str = ""
 
     # Edge case if we deal with negative
     if td < pd.Timedelta(seconds=0):
         td *= -1
-        out_str += 'NEG'
+        out_str += "NEG"
 
     # Note: this must happen after the *= -1
     c = td.components
     if c.days > 0:
-        out_str += f'{c.days}D'
+        out_str += f"{c.days}D"
     if c.hours > 0 or c.minutes > 0 or c.seconds > 0 or c.milliseconds > 0:
-        out_str += '_' if len(out_str) else ""
+        out_str += "_" if len(out_str) else ""
 
     if c.hours > 0:
         out_str += f"{c.hours}h"
     if c.minutes > 0:
         out_str += f"{c.minutes}m"
     if c.seconds > 0 or c.milliseconds > 0:
         out_str += f"{c.seconds}"
```

### Comparing `tsflex-0.3rc0/setup.py` & `tsflex-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,160 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['tsflex',
- 'tsflex.chunking',
- 'tsflex.features',
- 'tsflex.features.segmenter',
- 'tsflex.processing',
- 'tsflex.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dill>=0.3.4,<0.4.0',
- 'multiprocess>=0.70.12,<0.71.0',
- 'numpy>=1.21.5,<2.0.0',
- 'pandas>=1.3.5,<2.0.0',
- 'tqdm>=4.62.3,<5.0.0']
-
-setup_kwargs = {
-    'name': 'tsflex',
-    'version': '0.3rc0',
-    'description': 'Toolkit for flexible processing & feature extraction on time-series data',
-    'long_description': '# <p align="center"> <a href="https://predict-idlab.github.io/tsflex"><img alt="tsflex" src="https://raw.githubusercontent.com/predict-idlab/tsflex/main/docs/_static/logo.png" width="66%"></a></p>\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/tsflex.svg)](https://pypi.org/project/tsflex/)\n[![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/tsflex?label=conda)](https://anaconda.org/conda-forge/tsflex)\n[![support-version](https://img.shields.io/pypi/pyversions/tsflex)](https://img.shields.io/pypi/pyversions/tsflex)\n[![codecov](https://img.shields.io/codecov/c/github/predict-idlab/tsflex?logo=codecov)](https://codecov.io/gh/predict-idlab/tsflex)\n[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/tsflex?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/tsflex/context:python)\n[![Downloads](https://pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)\n[![Documentation](https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml)\n[![Testing](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml)\n\n<!-- ![Downloads](https://img.shields.io/conda/dn/conda-forge/tsflex?logo=anaconda) -->\n\n> *tsflex* is a toolkit for _**flex**ible **t**ime **s**eries_ [processing](https://predict-idlab.github.io/tsflex/processing) & [feature extraction](https://predict-idlab.github.io/tsflex/features), that is efficient and makes few assumptions about sequence data.\n\n#### Useful links\n\n- [Paper](https://www.sciencedirect.com/science/article/pii/S2352711021001904)\n- [Documentation](https://predict-idlab.github.io/tsflex/)\n- [Example (machine learning) notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples)\n\n#### Installation\n\n| | command|\n|:--------------|:--------------|\n| [**pip**](https://pypi.org/project/tsflex/) | `pip install tsflex` | \n| [**conda**](https://anaconda.org/conda-forge/tsflex) | `conda install -c conda-forge tsflex` |\n\n## Usage\n\n_tsflex_ is built to be intuitive, so we encourage you to copy-paste this code and toy with some parameters!\n\n### <a href="https://predict-idlab.github.io/tsflex/features/#getting-started">Feature extraction</a>\n\n```python\nimport pandas as pd; import numpy as np; import scipy.stats as ss\nfrom tsflex.features import MultipleFeatureDescriptors, FeatureCollection\nfrom tsflex.utils.data import load_empatica_data\n\n# 1. Load sequence-indexed data (in this case a time-index)\ndf_tmp, df_acc, df_ibi = load_empatica_data([\'tmp\', \'acc\', \'ibi\'])\n\n# 2. Construct your feature extraction configuration\nfc = FeatureCollection(\n    MultipleFeatureDescriptors(\n          functions=[np.min, np.mean, np.std, ss.skew, ss.kurtosis],\n          series_names=["TMP", "ACC_x", "ACC_y", "IBI"],\n          windows=["15min", "30min"],\n          strides="15min",\n    )\n)\n\n# 3. Extract features\nfc.calculate(data=[df_tmp, df_acc, df_ibi], approve_sparsity=True)\n```\n\nNote that the feature extraction is performed on multivariate data with varying sample rates.\n| signal | columns | sample rate |\n|:-------|:-------|------------------:|\n| df_tmp | ["TMP"]| 4Hz |\n| df_acc | ["ACC_x", "ACC_y", "ACC_z" ]| 32Hz |\n| df_ibi | ["IBI"]| irregularly sampled |\n\n### <a href="https://predict-idlab.github.io/tsflex/processing/index.html#getting-started">Processing</a>\n[Working example in our docs](https://predict-idlab.github.io/tsflex/processing/index.html#working-example)\n\n## Why tsflex? ✨\n\n* `Flexible`:\n    * handles multivariate/multimodal time series\n    * versatile function support\n      => **integrates** with many packages for:\n      * processing (e.g., [scipy.signal](https://docs.scipy.org/doc/scipy/reference/tutorial/signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/tsa.html#time-series-filters))\n      * feature extraction (e.g., [numpy](https://numpy.org/doc/stable/reference/routines.html), [scipy.stats](https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [seglearn](https://dmbee.github.io/seglearn/feature_functions.html)¹, [tsfresh](https://tsfresh.readthedocs.io/en/latest/text/list_of_features.html)¹, [tsfel](https://tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)¹)\n    * feature extraction handles **multiple strides & window sizes**\n* `Efficient`:<br>\n  * view-based operations for processing & feature extraction => extremely **low memory peak** & **fast execution time**<br>\n    * see: [feature extraction benchmark visualization](https://predict-idlab.github.io/tsflex/#benchmark)\n* `Intuitive`:<br>\n  * maintains the sequence-index of the data\n  * feature extraction constructs interpretable output column names\n  * intuitive API\n* `Few assumptions` about the sequence data:\n  * no assumptions about sampling rate\n  * able to deal with multivariate asynchronous data<br>i.e. data with small time-offsets between the modalities\n* `Advanced functionalities`:\n  * apply [FeatureCollection.**reduce**](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.reduce) after feature selection for faster inference\n  * use **function execution time logging** to discover processing and feature extraction bottlenecks\n  * embedded [SeriesPipeline](http://predict-idlab.github.io/tsflex/processing/#tsflex.processing.SeriesPipeline.serialize) & [FeatureCollection](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.serialize) **serialization**\n  * time series [**chunking**](https://predict-idlab.github.io/tsflex/chunking/index.html)\n\n¹ These integrations are shown in [integration-example notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples).\n## Future work 🔨\n\n* scikit-learn integration for both processing and feature extraction<br>\n  **note**: is actively developed upon [sklearn integration](https://github.com/predict-idlab/tsflex/tree/sklearn_integration) branch.\n* Support time series segmentation (exposing under the hood strided-rolling functionality) - [see this issue](https://github.com/predict-idlab/tsflex/issues/15)\n* Support for multi-indexed dataframes\n\n=> Also see the [enhancement issues](https://github.com/predict-idlab/tsflex/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement+)\n## Contributing 👪\n\nWe are thrilled to see your contributions to further enhance `tsflex`.<br>\nSee [this guide](CONTRIBUTING.md) for more instructions on how to contribute.\n\n## Referencing our package\n\nIf you use `tsflex` in a scientific publication, we would highly appreciate citing us as:\n\n```bibtex\n@article{vanderdonckt2021tsflex,\n    author = {Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},\n    title = {tsflex: flexible time series processing \\& feature extraction},\n    journal = {SoftwareX},\n    year = {2021},\n    url = {https://github.com/predict-idlab/tsflex},\n    publisher={Elsevier}\n}\n```\n\nLink to the paper: https://www.sciencedirect.com/science/article/pii/S2352711021001904\n\n---\n\n<p align="center">\n👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>\n</p>\n',
-    'author': 'Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/predict-idlab/tsflex',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
+Metadata-Version: 2.1
+Name: tsflex
+Version: 0.4.0
+Summary: Toolkit for flexible processing & feature extraction on time-series data
+Home-page: https://github.com/predict-idlab/tsflex
+License: MIT
+Keywords: time-series,processing,feature-extraction,data-science,machine learning
+Author: Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
+Requires-Python: >=3.7.1,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dill (>=0.3.4,<0.4.0)
+Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
+Requires-Dist: numpy (>=1.21.5,<2.0.0) ; python_version < "3.8"
+Requires-Dist: numpy (>=1.22) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: numpy (>=1.24) ; python_version >= "3.11"
+Requires-Dist: pandas (>=1) ; python_version < "3.12"
+Requires-Dist: pandas (>=2) ; python_version >= "3.12"
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Project-URL: Documentation, https://predict-idlab.github.io/tsflex
+Project-URL: Repository, https://github.com/predict-idlab/tsflex
+Description-Content-Type: text/markdown
+
+# <p align="center"> <a href="https://predict-idlab.github.io/tsflex"><img alt="tsflex" src="https://raw.githubusercontent.com/predict-idlab/tsflex/main/docs/_static/logo.png" width="66%"></a></p>
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/tsflex.svg)](https://pypi.org/project/tsflex/)
+[![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/tsflex?label=conda)](https://anaconda.org/conda-forge/tsflex)
+[![support-version](https://img.shields.io/pypi/pyversions/tsflex)](https://img.shields.io/pypi/pyversions/tsflex)
+[![codecov](https://img.shields.io/codecov/c/github/predict-idlab/tsflex?logo=codecov)](https://codecov.io/gh/predict-idlab/tsflex)
+[![CodeQL](https://github.com/predict-idlab/tsflex/actions/workflows/codeql.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/codeql.yml)
+[![Downloads](https://static.pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
+[![Documentation](https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml)
+[![Testing](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml)
+
+<!-- ![Downloads](https://img.shields.io/conda/dn/conda-forge/tsflex?logo=anaconda) -->
+
+> _tsflex_ is a toolkit for _**flex**ible **t**ime **s**eries_ [processing](https://predict-idlab.github.io/tsflex/processing) & [feature extraction](https://predict-idlab.github.io/tsflex/features), that is efficient and makes few assumptions about sequence data.
+
+#### Useful links
+
+- [Paper](https://www.sciencedirect.com/science/article/pii/S2352711021001904)
+- [Documentation](https://predict-idlab.github.io/tsflex/)
+- [Example (machine learning) notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples)
+
+#### Installation
+
+|                                                      | command                               |
+| :--------------------------------------------------- | :------------------------------------ |
+| [**pip**](https://pypi.org/project/tsflex/)          | `pip install tsflex`                  |
+| [**conda**](https://anaconda.org/conda-forge/tsflex) | `conda install -c conda-forge tsflex` |
+
+## Usage
+
+_tsflex_ is built to be intuitive, so we encourage you to copy-paste this code and toy with some parameters!
+
+### <a href="https://predict-idlab.github.io/tsflex/features/#getting-started">Feature extraction</a>
+
+```python
+import pandas as pd; import numpy as np; import scipy.stats as ss
+from tsflex.features import MultipleFeatureDescriptors, FeatureCollection
+from tsflex.utils.data import load_empatica_data
+
+# 1. Load sequence-indexed data (in this case a time-index)
+df_tmp, df_acc, df_ibi = load_empatica_data(['tmp', 'acc', 'ibi'])
+
+# 2. Construct your feature extraction configuration
+fc = FeatureCollection(
+    MultipleFeatureDescriptors(
+          functions=[np.min, np.mean, np.std, ss.skew, ss.kurtosis],
+          series_names=["TMP", "ACC_x", "ACC_y", "IBI"],
+          windows=["15min", "30min"],
+          strides="15min",
+    )
+)
+
+# 3. Extract features
+fc.calculate(data=[df_tmp, df_acc, df_ibi], approve_sparsity=True)
+```
+
+Note that the feature extraction is performed on multivariate data with varying sample rates.
+| signal | columns | sample rate |
+|:-------|:-------|------------------:|
+| df_tmp | ["TMP"]| 4Hz |
+| df_acc | ["ACC_x", "ACC_y", "ACC_z" ]| 32Hz |
+| df_ibi | ["IBI"]| irregularly sampled |
+
+### <a href="https://predict-idlab.github.io/tsflex/processing/index.html#getting-started">Processing</a>
+
+[Working example in our docs](https://predict-idlab.github.io/tsflex/processing/index.html#working-example)
+
+## Why tsflex? ✨
+
+- `Flexible`:
+  - handles multivariate/multimodal time series
+  - versatile function support
+    => **integrates** with many packages for:
+    - processing (e.g., [scipy.signal](https://docs.scipy.org/doc/scipy/reference/tutorial/signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/tsa.html#time-series-filters))
+    - feature extraction (e.g., [numpy](https://numpy.org/doc/stable/reference/routines.html), [scipy.stats](https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [antropy](https://raphaelvallat.com/antropy/build/html/api.html), [nolds](https://cschoel.github.io/nolds/nolds.html#algorithms), [seglearn](https://dmbee.github.io/seglearn/feature_functions.html)¹, [tsfresh](https://tsfresh.readthedocs.io/en/latest/text/list_of_features.html)¹, [tsfel](https://tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)¹)
+  - feature extraction handles **multiple strides & window sizes**
+- `Efficient`:<br>
+  - view-based operations for processing & feature extraction => extremely **low memory peak** & **fast execution time**<br>
+    - see: [feature extraction benchmark visualization](https://predict-idlab.github.io/tsflex/#benchmark)
+- `Intuitive`:<br>
+  - maintains the sequence-index of the data
+  - feature extraction constructs interpretable output column names
+  - intuitive API
+- `Few assumptions` about the sequence data:
+  - no assumptions about sampling rate
+  - able to deal with multivariate asynchronous data<br>i.e. data with small time-offsets between the modalities
+- `Advanced functionalities`:
+  - apply [FeatureCollection.**reduce**](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.reduce) after feature selection for faster inference
+  - use **function execution time logging** to discover processing and feature extraction bottlenecks
+  - embedded [SeriesPipeline](http://predict-idlab.github.io/tsflex/processing/#tsflex.processing.SeriesPipeline.serialize) & [FeatureCollection](https://predict-idlab.github.io/tsflex/features/index.html#tsflex.features.FeatureCollection.serialize) **serialization**
+  - time series [**chunking**](https://predict-idlab.github.io/tsflex/chunking/index.html)
+
+¹ These integrations are shown in [integration-example notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples).
+
+## Future work 🔨
+
+- scikit-learn integration for both processing and feature extraction<br>
+  **note**: is actively developed upon [sklearn integration](https://github.com/predict-idlab/tsflex/tree/sklearn_integration) branch.
+- Support time series segmentation (exposing under the hood strided-rolling functionality) - [see this issue](https://github.com/predict-idlab/tsflex/issues/15)
+- Support for multi-indexed dataframes
+
+=> Also see the [enhancement issues](https://github.com/predict-idlab/tsflex/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement+)
+
+## Contributing 👪
+
+We are thrilled to see your contributions to further enhance `tsflex`.<br>
+See [this guide](CONTRIBUTING.md) for more instructions on how to contribute.
+
+## Referencing our package
+
+If you use `tsflex` in a scientific publication, we would highly appreciate citing us as:
+
+```bibtex
+@article{vanderdonckt2021tsflex,
+    author = {Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
+    title = {tsflex: flexible time series processing \& feature extraction},
+    journal = {SoftwareX},
+    year = {2021},
+    url = {https://github.com/predict-idlab/tsflex},
+    publisher={Elsevier}
 }
+```
+
+Link to the paper: https://www.sciencedirect.com/science/article/pii/S2352711021001904
+
+---
 
+<p align="center">
+👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>
+</p>
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,110 +1,115 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['tsflex',
-'tsflex.chunking', 'tsflex.features', 'tsflex.features.segmenter',
-'tsflex.processing', 'tsflex.utils'] package_data = \ {'': ['*']}
-install_requires = \ ['dill>=0.3.4,<0.4.0', 'multiprocess>=0.70.12,<0.71.0',
-'numpy>=1.21.5,<2.0.0', 'pandas>=1.3.5,<2.0.0', 'tqdm>=4.62.3,<5.0.0']
-setup_kwargs = { 'name': 'tsflex', 'version': '0.3rc0', 'description': 'Toolkit
-for flexible processing & feature extraction on time-series data',
-'long_description': '#
+Metadata-Version: 2.1 Name: tsflex Version: 0.4.0 Summary: Toolkit for flexible
+processing & feature extraction on time-series data Home-page: https://
+github.com/predict-idlab/tsflex License: MIT Keywords: time-
+series,processing,feature-extraction,data-science,machine learning Author:
+Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost Requires-Python:
+>=3.7.1,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: dill (>=0.3.4,<0.4.0) Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
+Requires-Dist: numpy (>=1.21.5,<2.0.0) ; python_version < "3.8" Requires-Dist:
+numpy (>=1.22) ; python_version >= "3.8" and python_version < "3.11" Requires-
+Dist: numpy (>=1.24) ; python_version >= "3.11" Requires-Dist: pandas (>=1) ;
+python_version < "3.12" Requires-Dist: pandas (>=2) ; python_version >= "3.12"
+Requires-Dist: tqdm (>=4.62.3,<5.0.0) Project-URL: Documentation, https://
+predict-idlab.github.io/tsflex Project-URL: Repository, https://github.com/
+predict-idlab/tsflex Description-Content-Type: text/markdown #
                                    _[_t_s_f_l_e_x_]
-\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/tsflex.svg)](https://
-pypi.org/project/tsflex/)\n[![Conda Latest Release](https://img.shields.io/
+[![PyPI Latest Release](https://img.shields.io/pypi/v/tsflex.svg)](https://
+pypi.org/project/tsflex/) [![Conda Latest Release](https://img.shields.io/
 conda/vn/conda-forge/tsflex?label=conda)](https://anaconda.org/conda-forge/
-tsflex)\n[![support-version](https://img.shields.io/pypi/pyversions/tsflex)]
-(https://img.shields.io/pypi/pyversions/tsflex)\n[![codecov](https://
+tsflex) [![support-version](https://img.shields.io/pypi/pyversions/tsflex)]
+(https://img.shields.io/pypi/pyversions/tsflex) [![codecov](https://
 img.shields.io/codecov/c/github/predict-idlab/tsflex?logo=codecov)](https://
-codecov.io/gh/predict-idlab/tsflex)\n[![Code quality](https://img.shields.io/
-lgtm/grade/python/github/predict-idlab/tsflex?label=code%20quality&logo=lgtm)]
-(https://lgtm.com/projects/g/predict-idlab/tsflex/context:python)\n[!
-[Downloads](https://pepy.tech/badge/tsflex)](https://pepy.tech/project/
-tsflex)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-
-brightgreen.svg?)](http://makeapullrequest.com)\n[![Documentation](https://
-github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml/badge.svg)]
-(https://github.com/predict-idlab/tsflex/actions/workflows/deploy-docs.yml)\n[!
-[Testing](https://github.com/predict-idlab/tsflex/actions/workflows/test.yml/
-badge.svg)](https://github.com/predict-idlab/tsflex/actions/workflows/
-test.yml)\n\n\n\n> *tsflex* is a toolkit for _**flex**ible **t**ime **s**eries_
-[processing](https://predict-idlab.github.io/tsflex/processing) & [feature
-extraction](https://predict-idlab.github.io/tsflex/features), that is efficient
-and makes few assumptions about sequence data.\n\n#### Useful links\n\n-
-[Paper](https://www.sciencedirect.com/science/article/pii/S2352711021001904)\n-
-[Documentation](https://predict-idlab.github.io/tsflex/)\n- [Example (machine
-learning) notebooks](https://github.com/predict-idlab/tsflex/tree/main/
-examples)\n\n#### Installation\n\n| | command|\n|:--------------|:-------------
--|\n| [**pip**](https://pypi.org/project/tsflex/) | `pip install tsflex` | \n|
-[**conda**](https://anaconda.org/conda-forge/tsflex) | `conda install -c conda-
-forge tsflex` |\n\n## Usage\n\n_tsflex_ is built to be intuitive, so we
-encourage you to copy-paste this code and toy with some parameters!\n\n###
-_F_e_a_t_u_r_e_ _e_x_t_r_a_c_t_i_o_n\n\n```python\nimport pandas as pd; import numpy as np;
-import scipy.stats as ss\nfrom tsflex.features import
-MultipleFeatureDescriptors, FeatureCollection\nfrom tsflex.utils.data import
-load_empatica_data\n\n# 1. Load sequence-indexed data (in this case a time-
-index)\ndf_tmp, df_acc, df_ibi = load_empatica_data([\'tmp\', \'acc\',
-\'ibi\'])\n\n# 2. Construct your feature extraction configuration\nfc =
-FeatureCollection(\n MultipleFeatureDescriptors(\n functions=[np.min, np.mean,
-np.std, ss.skew, ss.kurtosis],\n series_names=["TMP", "ACC_x", "ACC_y",
-"IBI"],\n windows=["15min", "30min"],\n strides="15min",\n )\n)\n\n# 3. Extract
-features\nfc.calculate(data=[df_tmp, df_acc, df_ibi],
-approve_sparsity=True)\n```\n\nNote that the feature extraction is performed on
-multivariate data with varying sample rates.\n| signal | columns | sample rate
-|\n|:-------|:-------|------------------:|\n| df_tmp | ["TMP"]| 4Hz |\n| df_acc
-| ["ACC_x", "ACC_y", "ACC_z" ]| 32Hz |\n| df_ibi | ["IBI"]| irregularly sampled
-|\n\n### _P_r_o_c_e_s_s_i_n_g\n[Working example in our docs](https://predict-
-idlab.github.io/tsflex/processing/index.html#working-example)\n\n## Why tsflex?
-â¨\n\n* `Flexible`:\n * handles multivariate/multimodal time series\n *
-versatile function support\n => **integrates** with many packages for:\n *
-processing (e.g., [scipy.signal](https://docs.scipy.org/doc/scipy/reference/
-tutorial/signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/
-tsa.html#time-series-filters))\n * feature extraction (e.g., [numpy](https://
+codecov.io/gh/predict-idlab/tsflex) [![CodeQL](https://github.com/predict-
+idlab/tsflex/actions/workflows/codeql.yml/badge.svg)](https://github.com/
+predict-idlab/tsflex/actions/workflows/codeql.yml) [![Downloads](https://
+static.pepy.tech/badge/tsflex)](https://pepy.tech/project/tsflex) [![PRs
+Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
+makeapullrequest.com) [![Documentation](https://github.com/predict-idlab/
+tsflex/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/
+predict-idlab/tsflex/actions/workflows/deploy-docs.yml) [![Testing](https://
+github.com/predict-idlab/tsflex/actions/workflows/test.yml/badge.svg)](https://
+github.com/predict-idlab/tsflex/actions/workflows/test.yml) > _tsflex_ is a
+toolkit for _**flex**ible **t**ime **s**eries_ [processing](https://predict-
+idlab.github.io/tsflex/processing) & [feature extraction](https://predict-
+idlab.github.io/tsflex/features), that is efficient and makes few assumptions
+about sequence data. #### Useful links - [Paper](https://www.sciencedirect.com/
+science/article/pii/S2352711021001904) - [Documentation](https://predict-
+idlab.github.io/tsflex/) - [Example (machine learning) notebooks](https://
+github.com/predict-idlab/tsflex/tree/main/examples) #### Installation | |
+command | | :--------------------------------------------------- | :-----------
+------------------------- | | [**pip**](https://pypi.org/project/tsflex/) |
+`pip install tsflex` | | [**conda**](https://anaconda.org/conda-forge/tsflex) |
+`conda install -c conda-forge tsflex` | ## Usage _tsflex_ is built to be
+intuitive, so we encourage you to copy-paste this code and toy with some
+parameters! ### _F_e_a_t_u_r_e_ _e_x_t_r_a_c_t_i_o_n ```python import pandas as pd; import numpy
+as np; import scipy.stats as ss from tsflex.features import
+MultipleFeatureDescriptors, FeatureCollection from tsflex.utils.data import
+load_empatica_data # 1. Load sequence-indexed data (in this case a time-index)
+df_tmp, df_acc, df_ibi = load_empatica_data(['tmp', 'acc', 'ibi']) # 2.
+Construct your feature extraction configuration fc = FeatureCollection
+( MultipleFeatureDescriptors( functions=[np.min, np.mean, np.std, ss.skew,
+ss.kurtosis], series_names=["TMP", "ACC_x", "ACC_y", "IBI"], windows=["15min",
+"30min"], strides="15min", ) ) # 3. Extract features fc.calculate(data=[df_tmp,
+df_acc, df_ibi], approve_sparsity=True) ``` Note that the feature extraction is
+performed on multivariate data with varying sample rates. | signal | columns |
+sample rate | |:-------|:-------|------------------:| | df_tmp | ["TMP"]| 4Hz |
+| df_acc | ["ACC_x", "ACC_y", "ACC_z" ]| 32Hz | | df_ibi | ["IBI"]| irregularly
+sampled | ### _P_r_o_c_e_s_s_i_n_g [Working example in our docs](https://predict-
+idlab.github.io/tsflex/processing/index.html#working-example) ## Why tsflex?
+â¨ - `Flexible`: - handles multivariate/multimodal time series - versatile
+function support => **integrates** with many packages for: - processing (e.g.,
+[scipy.signal](https://docs.scipy.org/doc/scipy/reference/tutorial/
+signal.html), [statsmodels.tsa](https://www.statsmodels.org/stable/
+tsa.html#time-series-filters)) - feature extraction (e.g., [numpy](https://
 numpy.org/doc/stable/reference/routines.html), [scipy.stats](https://
-docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [seglearn](https://
+docs.scipy.org/doc/scipy/reference/tutorial/stats.html), [antropy](https://
+raphaelvallat.com/antropy/build/html/api.html), [nolds](https://
+cschoel.github.io/nolds/nolds.html#algorithms), [seglearn](https://
 dmbee.github.io/seglearn/feature_functions.html)Â¹, [tsfresh](https://
 tsfresh.readthedocs.io/en/latest/text/list_of_features.html)Â¹, [tsfel](https:/
-/tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)Â¹)\n * feature
-extraction handles **multiple strides & window sizes**\n* `Efficient`:
-\n * view-based operations for processing & feature extraction => extremely
-**low memory peak** & **fast execution time**
-\n * see: [feature extraction benchmark visualization](https://predict-
-idlab.github.io/tsflex/#benchmark)\n* `Intuitive`:
-\n * maintains the sequence-index of the data\n * feature extraction constructs
-interpretable output column names\n * intuitive API\n* `Few assumptions` about
-the sequence data:\n * no assumptions about sampling rate\n * able to deal with
+/tsfel.readthedocs.io/en/latest/descriptions/feature_list.html)Â¹) - feature
+extraction handles **multiple strides & window sizes** - `Efficient`:
+- view-based operations for processing & feature extraction => extremely **low
+memory peak** & **fast execution time**
+- see: [feature extraction benchmark visualization](https://predict-
+idlab.github.io/tsflex/#benchmark) - `Intuitive`:
+- maintains the sequence-index of the data - feature extraction constructs
+interpretable output column names - intuitive API - `Few assumptions` about the
+sequence data: - no assumptions about sampling rate - able to deal with
 multivariate asynchronous data
-i.e. data with small time-offsets between the modalities\n* `Advanced
-functionalities`:\n * apply [FeatureCollection.**reduce**](https://predict-
+i.e. data with small time-offsets between the modalities - `Advanced
+functionalities`: - apply [FeatureCollection.**reduce**](https://predict-
 idlab.github.io/tsflex/features/
 index.html#tsflex.features.FeatureCollection.reduce) after feature selection
-for faster inference\n * use **function execution time logging** to discover
-processing and feature extraction bottlenecks\n * embedded [SeriesPipeline]
-(http://predict-idlab.github.io/tsflex/processing/
+for faster inference - use **function execution time logging** to discover
+processing and feature extraction bottlenecks - embedded [SeriesPipeline](http:
+//predict-idlab.github.io/tsflex/processing/
 #tsflex.processing.SeriesPipeline.serialize) & [FeatureCollection](https://
 predict-idlab.github.io/tsflex/features/
-index.html#tsflex.features.FeatureCollection.serialize) **serialization**\n *
+index.html#tsflex.features.FeatureCollection.serialize) **serialization** -
 time series [**chunking**](https://predict-idlab.github.io/tsflex/chunking/
-index.html)\n\nÂ¹ These integrations are shown in [integration-example
-notebooks](https://github.com/predict-idlab/tsflex/tree/main/examples).\n##
-Future work ð¨\n\n* scikit-learn integration for both processing and feature
-extraction
-\n **note**: is actively developed upon [sklearn integration](https://
-github.com/predict-idlab/tsflex/tree/sklearn_integration) branch.\n* Support
-time series segmentation (exposing under the hood strided-rolling
-functionality) - [see this issue](https://github.com/predict-idlab/tsflex/
-issues/15)\n* Support for multi-indexed dataframes\n\n=> Also see the
-[enhancement issues](https://github.com/predict-idlab/tsflex/
-issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement+)\n## Contributing ðª\n\nWe
-are thrilled to see your contributions to further enhance `tsflex`.
-\nSee [this guide](CONTRIBUTING.md) for more instructions on how to
-contribute.\n\n## Referencing our package\n\nIf you use `tsflex` in a
-scientific publication, we would highly appreciate citing us as:
-\n\n```bibtex\n@article{vanderdonckt2021tsflex,\n author = {Van Der Donckt,
-Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},\n
-title = {tsflex: flexible time series processing \\& feature extraction},\n
-journal = {SoftwareX},\n year = {2021},\n url = {https://github.com/predict-
-idlab/tsflex},\n publisher={Elsevier}\n}\n```\n\nLink to the paper: https://
-www.sciencedirect.com/science/article/pii/S2352711021001904\n\n---\n\n
-      \nð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost\n
-\n', 'author': 'Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost',
-'author_email': None, 'maintainer': None, 'maintainer_email': None, 'url':
-'https://github.com/predict-idlab/tsflex', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7.1,<3.11', } setup(**setup_kwargs)
+index.html) Â¹ These integrations are shown in [integration-example notebooks]
+(https://github.com/predict-idlab/tsflex/tree/main/examples). ## Future work
+ð¨ - scikit-learn integration for both processing and feature extraction
+**note**: is actively developed upon [sklearn integration](https://github.com/
+predict-idlab/tsflex/tree/sklearn_integration) branch. - Support time series
+segmentation (exposing under the hood strided-rolling functionality) - [see
+this issue](https://github.com/predict-idlab/tsflex/issues/15) - Support for
+multi-indexed dataframes => Also see the [enhancement issues](https://
+github.com/predict-idlab/tsflex/
+issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement+) ## Contributing ðª We are
+thrilled to see your contributions to further enhance `tsflex`.
+See [this guide](CONTRIBUTING.md) for more instructions on how to contribute.
+## Referencing our package If you use `tsflex` in a scientific publication, we
+would highly appreciate citing us as: ```bibtex @article
+{vanderdonckt2021tsflex, author = {Van Der Donckt, Jonas and Van Der Donckt,
+Jeroen and Deprost, Emiel and Van Hoecke, Sofie}, title = {tsflex: flexible
+time series processing \& feature extraction}, journal = {SoftwareX}, year =
+{2021}, url = {https://github.com/predict-idlab/tsflex}, publisher={Elsevier} }
+``` Link to the paper: https://www.sciencedirect.com/science/article/pii/
+S2352711021001904 ---
+        ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

