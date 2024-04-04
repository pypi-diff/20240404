# Comparing `tmp/mngs-1.1.1.tar.gz` & `tmp/mngs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mngs-1.1.1.tar", last modified: Thu Mar 14 01:04:13 2024, max compression
+gzip compressed data, was "mngs-1.2.0.tar", last modified: Thu Apr  4 08:47:32 2024, max compression
```

## Comparing `mngs-1.1.1.tar` & `mngs-1.2.0.tar`

### file list

```diff
@@ -1,178 +1,193 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.296864 mngs-1.1.1/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2024-02-03 10:31:02.000000 mngs-1.1.1/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.1.1/MANIFEST.in
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      955 2024-03-14 01:04:13.296864 mngs-1.1.1/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.1.1/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-03-14 01:04:13.296864 mngs-1.1.1/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.1.1/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.270864 mngs-1.1.1/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.272864 mngs-1.1.1/src/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      455 2024-03-14 01:00:26.000000 mngs-1.1.1/src/mngs/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.274864 mngs-1.1.1/src/mngs/dsp/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12036 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/HilbertTransformationTorch.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      148 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      911 2024-02-20 21:59:18.000000 mngs-1.1.1/src/mngs/dsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6660 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/_load_BIDS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1712 2024-02-20 21:58:40.000000 mngs-1.1.1/src/mngs/dsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5550 2024-02-14 09:04:19.000000 mngs-1.1.1/src/mngs/dsp/demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    14356 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/feature_extractors.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4473 2024-02-07 00:39:16.000000 mngs-1.1.1/src/mngs/dsp/fft.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    14678 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      816 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2868 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/referencing.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      734 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/sampling.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12019 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/dsp/transform.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.277864 mngs-1.1.1/src/mngs/general/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1065 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/TimeStamper.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1427 2024-03-11 23:31:41.000000 mngs-1.1.1/src/mngs/general/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.1.1/src/mngs/general/_close.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/_shell.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3797 2024-03-08 21:22:32.000000 mngs-1.1.1/src/mngs/general/_start.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/_xml2dict.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1054 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/calc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3956 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/converters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/cuda_collect_env.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2144 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/debug.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/email.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/latex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.1.1/src/mngs/general/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/mat2py.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    21137 2024-03-12 09:03:16.000000 mngs-1.1.1/src/mngs/general/misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/pandas.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.1.1/src/mngs/general/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.1.1/src/mngs/general/repro.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-11 03:32:28.000000 mngs-1.1.1/src/mngs/general/save.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/general/torch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.277864 mngs-1.1.1/src/mngs/gists/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/gists/_SigMacro_processFigure_S.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/gists/_SigMacro_toBlue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/gists/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.278864 mngs-1.1.1/src/mngs/io/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-02-04 02:18:33.000000 mngs-1.1.1/src/mngs/io/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.1.1/src/mngs/io/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.1.1/src/mngs/io/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-11 03:32:28.000000 mngs-1.1.1/src/mngs/io/save.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.278864 mngs-1.1.1/src/mngs/linalg/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/linalg/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/linalg/_misc.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.279864 mngs-1.1.1/src/mngs/ml/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/ClassificationReporter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/ClassifierServer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3077 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/EarlyStopping.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/LearningCurveLogger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/__Classifiers.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.1.1/src/mngs/ml/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.280864 mngs-1.1.1/src/mngs/ml/act/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/act/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/act/_define.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.280864 mngs-1.1.1/src/mngs/ml/clustering/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.1.1/src/mngs/ml/clustering/_UMAP.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.1.1/src/mngs/ml/clustering/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.1.1/src/mngs/ml/clustering/_umap.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.281864 mngs-1.1.1/src/mngs/ml/layer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/layer/_Pass.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/layer/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/layer/_switch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.281864 mngs-1.1.1/src/mngs/ml/loss/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/loss/MultiTaskLoss.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/loss/_L1L2Losses.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/loss/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.282864 mngs-1.1.1/src/mngs/ml/metrics/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.1.1/src/mngs/ml/metrics/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.1.1/src/mngs/ml/metrics/_bACC.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.282864 mngs-1.1.1/src/mngs/ml/optim/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.282864 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.283864 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/optim/_get_set.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.284864 mngs-1.1.1/src/mngs/ml/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.1.1/src/mngs/ml/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.1.1/src/mngs/ml/plt/_conf_mat.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.1.1/src/mngs/ml/plt/_learning_curve.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3451 2024-03-13 03:13:57.000000 mngs-1.1.1/src/mngs/ml/plt/_optuna_study.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.285864 mngs-1.1.1/src/mngs/ml/plt/aucs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/plt/aucs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/plt/aucs/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/plt/aucs/pre_rec_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/plt/aucs/roc_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/silhoute_score_block.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.285864 mngs-1.1.1/src/mngs/ml/sk/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.1.1/src/mngs/ml/sk/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1854 2024-03-13 01:04:31.000000 mngs-1.1.1/src/mngs/ml/sk/_clf.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.1.1/src/mngs/ml/sk/_to_sktime.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.287864 mngs-1.1.1/src/mngs/ml/utils/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/utils/_DefaultDataset.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.1.1/src/mngs/ml/utils/_LabelEncoder.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.1.1/src/mngs/ml/utils/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.1.1/src/mngs/ml/utils/_check_params.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/utils/_format_samples_for_sktime.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.1.1/src/mngs/ml/utils/_merge_labels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/utils/_sliding_window_data_augmentation.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/utils/_under_sample.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/ml/utils/_verify_n_gpus.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.289864 mngs-1.1.1/src/mngs/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/nn/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.290864 mngs-1.1.1/src/mngs/os/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.1.1/src/mngs/os/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1342 2024-03-02 10:35:45.000000 mngs-1.1.1/src/mngs/os/_mv.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.292864 mngs-1.1.1/src/mngs/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      390 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/_add_hue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/_annotated_heatmap.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5710 2024-03-07 15:07:44.000000 mngs-1.1.1/src/mngs/plt/_configure_mpl.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/_draw_a_cube.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/_get_RGBA_from_colormap.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/_mk_colorbar.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/_mk_patches.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9875 2024-02-04 02:05:41.000000 mngs-1.1.1/src/mngs/plt/_subplots.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.294864 mngs-1.1.1/src/mngs/plt/ax/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      436 2024-03-07 12:38:36.000000 mngs-1.1.1/src/mngs/plt/ax/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_circular_hist.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_extend.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_fill_between.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.1.1/src/mngs/plt/ax/_hide_spines.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_map_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_panel.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_sci_note.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      322 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_set_n_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.1.1/src/mngs/plt/ax/_set_pos.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/ax/_set_size.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/colors.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/plt/get_mpl_color.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.294864 mngs-1.1.1/src/mngs/resource/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/resource/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/resource/get.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/resource/limit_RAM.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.296864 mngs-1.1.1/src/mngs/stats/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      462 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_bonferroni_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_brunner_munzel_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_calc_partial_corr.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_corr_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_fdr_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_multicompair.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_nocorrelation_test.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_smirnov_grubbs.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.1.1/src/mngs/stats/_to_asterisks.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-03-14 01:04:13.272864 mngs-1.1.1/src/mngs.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      955 2024-03-14 01:04:13.000000 mngs-1.1.1/src/mngs.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4588 2024-03-14 01:04:13.000000 mngs-1.1.1/src/mngs.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-03-14 01:04:13.000000 mngs-1.1.1/src/mngs.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      332 2024-03-14 01:04:13.000000 mngs-1.1.1/src/mngs.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-03-14 01:04:13.000000 mngs-1.1.1/src/mngs.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.896993 mngs-1.2.0/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2024-02-03 10:31:02.000000 mngs-1.2.0/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.2.0/MANIFEST.in
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-04 08:47:32.896993 mngs-1.2.0/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.2.0/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-04 08:47:32.896993 mngs-1.2.0/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.0/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.876993 mngs-1.2.0/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.878993 mngs-1.2.0/src/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      482 2024-04-04 08:47:16.000000 mngs-1.2.0/src/mngs/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.879993 mngs-1.2.0/src/mngs/dsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.2.0/src/mngs/dsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      300 2024-04-04 08:41:51.000000 mngs-1.2.0/src/mngs/dsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3783 2024-04-03 02:08:42.000000 mngs-1.2.0/src/mngs/dsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      338 2024-04-02 12:33:00.000000 mngs-1.2.0/src/mngs/dsp/_ensure_3d.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1455 2024-04-03 21:02:11.000000 mngs-1.2.0/src/mngs/dsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.2.0/src/mngs/dsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1710 2024-04-04 08:07:31.000000 mngs-1.2.0/src/mngs/dsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1749 2024-04-04 02:34:34.000000 mngs-1.2.0/src/mngs/dsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2848 2024-04-03 20:26:59.000000 mngs-1.2.0/src/mngs/dsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2791 2024-04-02 11:21:03.000000 mngs-1.2.0/src/mngs/dsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1232 2024-04-04 02:23:09.000000 mngs-1.2.0/src/mngs/dsp/filt.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.2.0/src/mngs/dsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.881993 mngs-1.2.0/src/mngs/general/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1065 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1494 2024-04-02 10:35:31.000000 mngs-1.2.0/src/mngs/general/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.2.0/src/mngs/general/_close.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8880 2024-04-04 02:22:41.000000 mngs-1.2.0/src/mngs/general/_converters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.2.0/src/mngs/general/_norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/_shell.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3822 2024-03-25 01:12:15.000000 mngs-1.2.0/src/mngs/general/_start.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/cuda_collect_env.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2144 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/debug.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/email.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.0/src/mngs/general/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22093 2024-04-01 10:51:59.000000 mngs-1.2.0/src/mngs/general/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.0/src/mngs/general/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.2.0/src/mngs/general/repro.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.0/src/mngs/general/save.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/torch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.881993 mngs-1.2.0/src/mngs/gists/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/gists/_SigMacro_processFigure_S.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/gists/_SigMacro_toBlue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/gists/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.882993 mngs-1.2.0/src/mngs/io/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-02-04 02:18:33.000000 mngs-1.2.0/src/mngs/io/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.0/src/mngs/io/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.0/src/mngs/io/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.0/src/mngs/io/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.882993 mngs-1.2.0/src/mngs/linalg/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/linalg/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/linalg/_misc.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.883993 mngs-1.2.0/src/mngs/ml/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/ClassificationReporter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/ClassifierServer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.2.0/src/mngs/ml/EarlyStopping.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/LearningCurveLogger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/__Classifiers.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.2.0/src/mngs/ml/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.883993 mngs-1.2.0/src/mngs/ml/act/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/act/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/act/_define.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.884993 mngs-1.2.0/src/mngs/ml/clustering/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.2.0/src/mngs/ml/clustering/_UMAP.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.2.0/src/mngs/ml/clustering/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.2.0/src/mngs/ml/clustering/_umap.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.884993 mngs-1.2.0/src/mngs/ml/layer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/layer/_Pass.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/layer/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/layer/_switch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/loss/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/loss/MultiTaskLoss.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/loss/_L1L2Losses.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/loss/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/metrics/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.2.0/src/mngs/ml/metrics/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.2.0/src/mngs/ml/metrics/_bACC.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/optim/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.886993 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/_get_set.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.887993 mngs-1.2.0/src/mngs/ml/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.2.0/src/mngs/ml/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.2.0/src/mngs/ml/plt/_conf_mat.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.2.0/src/mngs/ml/plt/_learning_curve.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.2.0/src/mngs/ml/plt/_optuna_study.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.888993 mngs-1.2.0/src/mngs/ml/plt/aucs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/pre_rec_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/roc_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/silhoute_score_block.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.888993 mngs-1.2.0/src/mngs/ml/sk/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.2.0/src/mngs/ml/sk/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.2.0/src/mngs/ml/sk/_clf.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.2.0/src/mngs/ml/sk/_to_sktime.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.889993 mngs-1.2.0/src/mngs/ml/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_DefaultDataset.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.2.0/src/mngs/ml/utils/_LabelEncoder.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.2.0/src/mngs/ml/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.2.0/src/mngs/ml/utils/_check_params.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_format_samples_for_sktime.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.2.0/src/mngs/ml/utils/_merge_labels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_sliding_window_data_augmentation.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_under_sample.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_verify_n_gpus.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.890993 mngs-1.2.0/src/mngs/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/mngs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/mngs/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.891993 mngs-1.2.0/src/mngs/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.0/src/mngs/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3998 2024-04-02 14:06:31.000000 mngs-1.2.0/src/mngs/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.0/src/mngs/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-02 12:48:08.000000 mngs-1.2.0/src/mngs/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.0/src/mngs/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.0/src/mngs/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.0/src/mngs/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9428 2024-04-02 09:35:04.000000 mngs-1.2.0/src/mngs/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      838 2024-04-02 13:16:20.000000 mngs-1.2.0/src/mngs/nn/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.891993 mngs-1.2.0/src/mngs/os/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.2.0/src/mngs/os/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1342 2024-03-02 10:35:45.000000 mngs-1.2.0/src/mngs/os/_mv.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.892993 mngs-1.2.0/src/mngs/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.2.0/src/mngs/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_add_hue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_annotated_heatmap.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5710 2024-03-07 15:07:44.000000 mngs-1.2.0/src/mngs/plt/_configure_mpl.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_draw_a_cube.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_get_RGBA_from_colormap.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_mk_colorbar.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_mk_patches.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9875 2024-02-04 02:05:41.000000 mngs-1.2.0/src/mngs/plt/_subplots.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.2.0/src/mngs/plt/_tpl.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.893993 mngs-1.2.0/src/mngs/plt/ax/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      436 2024-03-07 12:38:36.000000 mngs-1.2.0/src/mngs/plt/ax/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_circular_hist.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_extend.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_fill_between.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.2.0/src/mngs/plt/ax/_hide_spines.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_map_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_panel.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_sci_note.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      395 2024-03-29 22:04:00.000000 mngs-1.2.0/src/mngs/plt/ax/_set_n_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.2.0/src/mngs/plt/ax/_set_pos.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_set_size.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/colors.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/get_mpl_color.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.894993 mngs-1.2.0/src/mngs/resource/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/resource/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/resource/get.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/resource/limit_RAM.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.895993 mngs-1.2.0/src/mngs/stats/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.2.0/src/mngs/stats/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_bonferroni_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_brunner_munzel_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_calc_partial_corr.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_corr_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_fdr_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.2.0/src/mngs/stats/_general.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_multicompair.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_nocorrelation_test.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_smirnov_grubbs.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_to_asterisks.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.895993 mngs-1.2.0/src/mngs/torch/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.2.0/src/mngs/torch/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.2.0/src/mngs/torch/_apply_to.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.895993 mngs-1.2.0/src/mngs.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4901 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      375 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/top_level.txt
```

### Comparing `mngs-1.1.1/LICENSE` & `mngs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/setup.py` & `mngs-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/dsp/filters.py` & `mngs-1.2.0/src/mngs/ml/LearningCurveLogger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,448 +1,467 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Time-stamp: "2024-01-20 14:17:34 (ywatanabe)"
-
-import numpy as np
-import pandas as pd
-import scipy.ndimage
-import torch
-
-
-def gaussian_filter1d(xx, radius):
-    """
-    Apply a one-dimensional Gaussian filter to an input array, tensor, or DataFrame.
-
-    Arguments:
-        xx (numpy.ndarray, torch.Tensor, or pandas.DataFrame): The input data to filter. It can be a 1D or 2D array/tensor/DataFrame.
-        radius (int): The radius of the Gaussian kernel. The standard deviation of the Gaussian kernel is implicitly set to 1.
-
-    Returns:
-        numpy.ndarray, torch.Tensor, or pandas.DataFrame: The filtered data, with the same type as the input.
-
-    Data Types:
-        Input can be either numpy.ndarray, torch.Tensor, or pandas.DataFrame. Output will match the input data type.
-
-    Data Shapes:
-        - Input xx: If 1D, shape (n,), if 2D, shape (m, n)
-        - Output: Same shape as input xx
-
-    References:
-        - SciPy documentation for gaussian_filter1d: https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.gaussian_filter1d.html
-    """
-    sigma = 1
-    truncate = radius / sigma
-
-    # Convert input to NumPy array if it is a pandas DataFrame or PyTorch tensor
-    if isinstance(xx, pd.DataFrame):
-        values = xx.values
-        result = scipy.ndimage.gaussian_filter1d(
-            values, sigma, truncate=truncate
-        )
-        return pd.DataFrame(result, index=xx.index, columns=xx.columns)
-    elif isinstance(xx, torch.Tensor):
-        values = xx.numpy()
-        result = scipy.ndimage.gaussian_filter1d(
-            values, sigma, truncate=truncate
-        )
-        return torch.from_numpy(result)
-    else:
-        # Assume input is a NumPy array
-        return scipy.ndimage.gaussian_filter1d(xx, sigma, truncate=truncate)
 
+import re
+from collections import defaultdict
+from pprint import pprint
 
-def down_sample_1d(x, src_fs, tgt_fs):
-    factor = int(src_fs / tgt_fs)
-    assert factor == int(factor)
-    return scipy.signal.decimate(x, factor)
-
-
-#!/usr/bin/env python
-
-
-import time
-
-import matplotlib.pyplot as plt
-import numpy as np
+import matplotlib
+import mngs
 import pandas as pd
-import scipy.signal
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from obspy.imaging.cm import obspy_sequential
-from obspy.signal.tf_misfit import cwt
-
-
-class BandPassFilterTorch(nn.Module):
-    """
-    A PyTorch module that applies a bandpass filter to an input signal using FIR filter coefficients.
-
-    Attributes:
-        fs (int): The sampling frequency of the input signal.
-        order (int): The order of the filter. Defaults to the sampling frequency if not provided.
-        numtaps (int): The number of taps in the filter (order + 1).
-        filters (torch.Tensor): The FIR filter coefficients, shaped as (1, 1, numtaps).
-
-    Parameters:
-        order (int, optional): The order of the filter. Defaults to the sampling frequency if not provided.
-        low_hz (float): The lower cutoff frequency for the bandpass filter.
-        high_hz (float): The higher cutoff frequency for the bandpass filter.
-        fs (int): The sampling frequency of the input signal.
-        n_chs (int): The number of channels in the input signal.
-
-    Methods:
-        forward(x): Applies the bandpass filter to the input signal `x`.
-
-    Args:
-        x (torch.Tensor): The input signal to be filtered, shaped as (batch_size, n_chs, signal_length) for 3D input
-                          or (batch_size, signal_length) for 2D input.
-
-    Returns:
-        torch.Tensor: The filtered signal, with the same shape as the input signal.
-
-    References:
-        - SincNet implementation: https://raw.githubusercontent.com/mravanelli/SincNet/master/dnn_models.py
-        - FIR filter design: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.firwin.html
-    """
-
-    def __init__(self, order=None, low_hz=30, high_hz=60, fs=250, n_chs=19):
-        super().__init__()
-        self.fs = fs
-        # nyq = fs / 2
-        self.order = fs if order is None else order
-        self.numtaps = self.order + 1
-        filter_npy = scipy.signal.firwin(
-            self.numtaps,
-            [low_hz, high_hz],
-            pass_zero="bandpass",
-            fs=fs,
-        )
-
-        self.register_buffer(
-            "filters", torch.tensor(filter_npy).unsqueeze(0).unsqueeze(0)
-        )
-
-    def forward(self, x):
-        """
-            Apply the bandpass filter to the input signal.
-
-        The method applies a bandpass filter to the input signal using a FIR filter with the coefficients stored in the `filters` attribute. The filtering is performed in two passes to ensure zero-phase distortion: first forward and then backward.
-
-        Arguments:
-            x (torch.Tensor): The input signal tensor. If the input is 3D, it should have the shape (batch_size, n_chs, signal_length), where `n_chs` is the number of channels and `signal_length` is the length of the signal. If the input is 2D, it should have the shape (batch_size, signal_length).
-
-        Returns:
-            torch.Tensor: The filtered signal tensor. The output tensor will have the same shape as the input tensor.
-
-        Data Types:
-            Input: torch.Tensor (float32 or float64 typically, depending on the model's precision)
-            Output: torch.Tensor (same type as input)
-
-        Data Shapes:
-            Input: (batch_size, n_chs, signal_length) for 3D input or (batch_size, signal_length) for 2D input
-            Output: Same as input
-
-        References:
-            - Convolution operation: https://pytorch.org/docs/stable/generated/torch.nn.functional.conv1d.html
-            - Zero-phase filtering technique: https://en.wikipedia.org/wiki/Zero-phase_filtering
-        """
+import numpy as np
+import warnings
 
-        dim = x.ndim
-        # sig_len_orig = x.shape[-1]
 
-        if dim == 3:
-            bs, n_chs, sig_len = x.shape
-            x = x.reshape(bs * n_chs, 1, sig_len)
+class LearningCurveLogger(object):
+    def __init__(
+        self,
+    ):
+        self.logged_dict = defaultdict(dict)
 
-        filted = F.conv1d(
-            x, self.filters.type_as(x), padding=int(self.numtaps / 2)
+        warnings.warn(
+            '\n"gt_label" will be removed in the feature. Please use "true_class" instead.\n',
+            DeprecationWarning,
         )
-        filted = filted.flip(dims=[-1])  # to backward
-        filted = F.conv1d(
-            filted, self.filters.type_as(x), padding=int(self.numtaps / 2)
-        )
-        filted = filted.flip(dims=[-1])  # reverse to the original order
-
-        filted = filted[..., 1:-1]
-        # print(self.order, filted.shape[-1])
-
-        if dim == 3:
-            filted = filted.reshape(bs, n_chs, -1)
-
-        return filted
-
-
-class BandPasserCPUTorch:
-    """
-    A class that applies a bandpass filter to an input signal using a Butterworth filter on the CPU.
-
-    Attributes:
-        sos (numpy.ndarray): The second-order sections representation of the filter.
-
-    Parameters:
-        low_hz (float): The lower cutoff frequency for the bandpass filter.
-        high_hz (float): The higher cutoff frequency for the bandpass filter.
-        fs (int): The sampling frequency of the input signal.
-
-    References:
-        - Butterworth filter: https://en.wikipedia.org/wiki/Butterworth_filter
-        - scipy.signal.butter: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.butter.html
-        - scipy.signal.sosfilt: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.sosfilt.html
-    """
 
-    def __init__(self, low_hz=100, high_hz=250, fs=1000):
-        from scipy.signal import butter, sosfilt
-
-        self.butter = butter
-        self.sosfilt = sosfilt
-
-        self.sos = self.mk_sos(low_hz, high_hz, fs)
-
-    def __call__(self, raw_sig):
-        """
-        Apply the bandpass filter to the input signal.
-
-        Parameters:
-            raw_sig (numpy.ndarray): The raw input signal. The shape of the array should be (n_samples,) for a 1D signal or (n_channels, n_samples) for a multi-channel signal.
-
-        Returns:
-            numpy.ndarray: The filtered signal. The shape of the array will be the same as the input signal.
-
-        Data Types:
-            Input: numpy.ndarray (typically float32 or float64)
-            Output: numpy.ndarray (same type as input)
-
-        Data Shapes:
-            Input: (n_samples,) or (n_channels, n_samples)
-            Output: Same as input
-
-        References:
-            - scipy.signal.sosfilt: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.sosfilt.html
+    def __call__(self, dict_to_log, step):
         """
-        filted = self.sosfilt(self.sos, raw_sig)
-        return filted
+        dict_to_log | str
+            Example:
+                dict_to_log = {
+                    "loss_plot": float(loss),
+                    "balanced_ACC_plot": float(bACC),
+                    "pred_proba": pred_proba.detach().cpu().numpy(),
+                    "true_class": T.cpu().numpy(),
+                    "i_fold": i_fold,
+                    "i_epoch": i_epoch,
+                    "i_global": i_global,
+                }
+
+        step | str
+            "Training", "Validation", or "Test"
+        """
+        ########################################
+        ## delete here in the future
+        ## rename "gt_label" to "true_class"
+        if "gt_label" in dict_to_log.keys():
+            dict_to_log["true_class"] = dict_to_log.pop("gt_label")
+            # del dict_to_log["gt_label"]
+        ########################################
+
+        # assert step in ["Training", "Validation", "Test"]
+
+        ## Initialize self.logged_dict
+        for k_to_log in dict_to_log.keys():
+            try:
+                self.logged_dict[step][k_to_log].append(dict_to_log[k_to_log])
+            except:
+                self.logged_dict[step].update({k_to_log: []})
+                self.logged_dict[step][k_to_log].append(dict_to_log[k_to_log])
+
+    @property
+    def dfs(self):
+        return self._to_dfs_pivot(
+            self.logged_dict,
+            pivot_column=None,
+        )
 
-    def mk_sos(self, low_hz, high_hz, fs, order=5):
+    def get_x_of_i_epoch(self, x, step, i_epoch):
         """
-        Create the second-order sections representation of the Butterworth filter.
-
-        Parameters:
-            low_hz (float): The lower cutoff frequency for the bandpass filter.
-            high_hz (float): The higher cutoff frequency for the bandpass filter.
-            fs (int): The sampling frequency of the input signal.
-            order (int): The order of the filter.
-
-        Returns:
-            numpy.ndarray: The second-order sections representation of the filter.
-
-        Data Types:
-            Return: numpy.ndarray (typically float64)
-
-        Data Shapes:
-            Return: (n_sections, 6) where n_sections is the number of second-order filter sections.
-
-        References:
-            - scipy.signal.butter: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.butter.html
+        lc_logger.get_x_of_i_epoch("true_label_diag", "Validation", 3)
         """
-        nyq = fs / 2.0
-        sos = self.butter(
-            order,
-            [low_hz / nyq, high_hz / nyq],
-            analog=False,
-            btype="band",
-            output="sos",
-        )
-        return sos
-
-
-# from here, not important
-
+        # assert step in ['Training', "Validation", "Test"]
+        indi = np.array(self.logged_dict[step]["i_epoch"]) == i_epoch
+        x_all_arr = np.array(self.logged_dict[step][x])
+        assert len(indi) == len(x_all_arr)
+        return x_all_arr[indi]
 
-class TimeKeeper:
-    """
-    A simple class to keep track of elapsed time.
-
-    Methods:
-        __call__(message=None): Print the elapsed time with an optional message.
-        start(): Reset the start time to the current time.
-    """
-
-    def __init__(
+    def plot_learning_curves(
         self,
+        plt,
+        plt_config_dict=None,
+        title=None,
+        max_n_ticks=4,
+        linewidth=1,
+        scattersize=50,
     ):
         """
-        Initialize the TimeKeeper with the current time as the start time.
-        """
-
-        self.start_time = time.time()
-
-    def __call__(self, message=None):
+        Plots learning curves from self.logged_dict
         """
-        Print the elapsed time since the start time with an optional message.
+        if plt_config_dict is not None:
+            mngs.plt.configure_mpl(plt, **plt_config_dict)
 
-        Parameters:
-            message (str, optional): An optional message to print before the elapsed time.
-        """
+        self.dfs_pivot_i_global = self._to_dfs_pivot(
+            self.logged_dict, pivot_column="i_global"
+        )
 
-        self.elapsed = time.time() - self.start_time
-        print(message)
-        print("elapsed time: {:.5f} [sec]".format(self.elapsed))
+        ########################################
+        ## Parameters
+        ########################################
+        COLOR_DICT = {
+            "Training": "blue",
+            "Validation": "green",
+            "Test": "red",
+        }
+
+        keys_to_plot = self._find_keys_to_plot(self.logged_dict)
+
+        ########################################
+        ## Plots
+        ########################################
+        fig, axes = plt.subplots(len(keys_to_plot), 1, sharex=True, sharey=False)
+        axes[-1].set_xlabel("Iteration#")
+        fig.text(0.5, 0.95, title, ha="center")
+
+        for i_plt, plt_k in enumerate(keys_to_plot):
+            ax = axes[i_plt]
+            ax.set_ylabel(self._rename_if_key_to_plot(plt_k))
+            ax.xaxis.set_major_locator(matplotlib.ticker.MaxNLocator(max_n_ticks))
+            ax.yaxis.set_major_locator(matplotlib.ticker.MaxNLocator(max_n_ticks))
+
+            if re.search("[aA][cC][cC]", plt_k):  # acc, ylim, yticks
+                ax.set_ylim(0, 1)
+                ax.set_yticks([0, 0.5, 1.0])
+
+            for step_k in self.dfs_pivot_i_global.keys():
+
+                if step_k == re.search("^[Tt]rain", step_k):  # line
+                    # if step_k == "Training":  # line
+                    ax.plot(
+                        self.dfs_pivot_i_global[step_k].index,
+                        self.dfs_pivot_i_global[step_k][plt_k],
+                        label=step_k,
+                        color=mngs.plt.colors.to_RGBA(COLOR_DICT[step_k], alpha=0.9),
+                        linewidth=linewidth,
+                    )
+                    ax.legend()
+
+                    ########################################
+                    ## Epoch starts points; just in "Training" not to b duplicated
+                    ########################################
+                    epoch_starts = abs(
+                        self.dfs_pivot_i_global[step_k]["i_epoch"]
+                        - self.dfs_pivot_i_global[step_k]["i_epoch"].shift(-1)
+                    )
+                    indi_global_epoch_starts = [0] + list(
+                        epoch_starts[epoch_starts == 1].index
+                    )
+
+                    for i_epoch, i_global_epoch_start in enumerate(
+                        indi_global_epoch_starts
+                    ):
+                        ax.axvline(
+                            x=i_global_epoch_start,
+                            ymin=-1e4,  # ax.get_ylim()[0],
+                            ymax=1e4,  # ax.get_ylim()[1],
+                            linestyle="--",
+                            color=mngs.plt.colors.to_RGBA("gray", alpha=0.5),
+                        )
+                        # ax.text(
+                        #     i_global_epoch_start,
+                        #     ax.get_ylim()[1] * 1.0,
+                        #     f"epoch#{i_epoch}",
+                        # )
+                    ########################################
+
+                if (step_k == "Validation") or (step_k == "Test"):  # scatter
+                    ax.scatter(
+                        self.dfs_pivot_i_global[step_k].index,
+                        self.dfs_pivot_i_global[step_k][plt_k],
+                        label=step_k,
+                        color=mngs.plt.colors.to_RGBA(COLOR_DICT[step_k], alpha=0.9),
+                        s=scattersize,
+                        alpha=0.9,
+                    )
+                    ax.legend()
+
+        return fig
+
+    def print(self, step):
+        df_pivot_i_epoch = self._to_dfs_pivot(self.logged_dict, pivot_column="i_epoch")
+        df_pivot_i_epoch_step = df_pivot_i_epoch[step]
+        df_pivot_i_epoch_step.columns = self._rename_if_key_to_plot(
+            df_pivot_i_epoch_step.columns
+        )
+        print("\n----------------------------------------\n")
+        print(f"\n{step}: (mean of batches)\n")
+        pprint(df_pivot_i_epoch_step)
+        print("\n----------------------------------------\n")
+
+    @staticmethod
+    def _find_keys_to_plot(logged_dict):
+        _steps_str = list(logged_dict.keys())
+        _, keys_to_plot = mngs.general.search(
+            "_plot",
+            list(logged_dict[_steps_str[0]].keys()),
+        )
+        return keys_to_plot
 
-    def start(
-        self,
-    ):
-        """
-        Reset the start time to the current time.
-        """
+    @staticmethod
+    def _rename_if_key_to_plot(keys):
+        def _rename_key_to_plot(key_to_plot):
+            # renamed = key_to_plot[:-5]
+            renamed = re.sub("_plot", "", key_to_plot).replace("_", " ")
+            # renamed = renamed.replace("_", " ")
+            capitalized = []
+            for s in renamed.split(" "):
+                if not re.search("^[A-Z]", s):
+                    capitalized.append(s.capitalize())
+                else:
+                    capitalized.append(s)
+            renamed = mngs.general.connect_strs(capitalized, filler=" ")
+            return renamed
+
+        if isinstance(keys, str):
+            keys = [keys]
+
+        out = []
+        for key in keys:
+            if key[-5:] == "_plot":
+                out.append(_rename_key_to_plot(key))
+            else:
+                out.append(key)
+
+        if len(out) == 1:
+            out = out[0]
+
+        return out
+
+    # @staticmethod
+    # def _to_dfs_pivot_i_global(logged_dict):
+    #     dfs_pivot_i_global = {}
+    #     for step in logged_dict.keys():
+    #         df_step = mngs.general.pandas.force_dataframe(logged_dict[step])
+    #         df_step_pvt_on_i_global = df_step.pivot_table(
+    #             columns="i_global", aggfunc="mean"
+    #         ).T
+    #         dfs_pivot_i_global[step] = df_step_pvt_on_i_global
+
+    #     return dfs_pivot_i_global
+
+    @staticmethod
+    def _to_dfs_pivot(logged_dict, pivot_column=None):
+        dfs_pivot = {}
+        for step in logged_dict.keys():
+            df_step = mngs.general.pandas.force_dataframe(logged_dict[step])
+            if pivot_column is not None:
+                dfs_pivot[step] = df_step.pivot_table(
+                    columns=pivot_column, aggfunc="mean"
+                ).T
+            else:
+                dfs_pivot[step] = df_step
 
-        self.start_time = time.time()
+        return dfs_pivot
 
 
 if __name__ == "__main__":
-    # Parameters
-    PASS_LOW_HZ = 40
-    PASS_HIGH_HZ = 80
-    T_sec = 50.0
-    fs = 250
-    freqs_hz = [30, 60, 100, 200, 1000]
-    n_chs = 19
-    bs = 64
-    i_batch_show = 0
-    i_ch_show = 0
-    sig_orig = np.array(
-        [
-            mngs.dsp.prepare_demo_data(
-                T_sec=T_sec, fs=fs, freqs_hz=freqs_hz, n_chs=n_chs
-            )
-            for _ in range(bs)
-        ]
-    )
-    print("sig_orig_shape: {}".format(sig_orig.shape))
-    tk = TimeKeeper()
-
-    # Original
-    title_orig = "Original, #{}, ch{} (Demo Freqs: {} Hz)".format(
-        i_batch_show, i_ch_show, freqs_hz
-    )
-    wv_out_orig = wavelet_np(
-        sig_orig[i_batch_show, i_ch_show],
-        fs,
-        f_min=1,
-        plot=True,
-        title=title_orig,
-    )
+    import warnings
 
-    # CPU Bandpass Filtering
-    bp_cpu = BandPasserCPUTorch(
-        low_hz=PASS_LOW_HZ, high_hz=PASS_HIGH_HZ, fs=fs
+    import matplotlib.pyplot as plt
+    import torch
+    import torch.nn as nn
+    from sklearn.metrics import balanced_accuracy_score
+    from torch.utils.data import DataLoader, TensorDataset
+    from torch.utils.data.dataset import Subset
+    from torchvision import datasets
+
+    import sys
+
+    ################################################################################
+    ## Sets tee
+    ################################################################################
+    sdir = mngs.io.path.mk_spath("")  # "/tmp/sdir/"
+    sys.stdout, sys.stderr = mngs.general.tee(sys, sdir)
+
+    ################################################################################
+    ## NN
+    ################################################################################
+    class Perceptron(nn.Module):
+        def __init__(self):
+            super().__init__()
+            self.l1 = nn.Linear(28 * 28, 50)
+            self.l2 = nn.Linear(50, 10)
+
+        def forward(self, x):
+            x = x.view(-1, 28 * 28)
+            x = self.l1(x)
+            x = self.l2(x)
+            return x
+
+    ################################################################################
+    ## Prepaires demo data
+    ################################################################################
+    ## Downloads
+    _ds_tra_val = datasets.MNIST("/tmp/mnist", train=True, download=True)
+    _ds_tes = datasets.MNIST("/tmp/mnist", train=False, download=True)
+
+    ## Training-Validation splitting
+    n_samples = len(_ds_tra_val)  # n_samples is 60000
+    train_size = int(n_samples * 0.8)  # train_size is 48000
+
+    subset1_indices = list(range(0, train_size))  # [0,1,.....47999]
+    subset2_indices = list(range(train_size, n_samples))  # [48000,48001,.....59999]
+
+    _ds_tra = Subset(_ds_tra_val, subset1_indices)
+    _ds_val = Subset(_ds_tra_val, subset2_indices)
+
+    ## to tensors
+    ds_tra = TensorDataset(
+        _ds_tra.dataset.data.to(torch.float32),
+        _ds_tra.dataset.targets,
     )
-    filted_cpu = sig_orig.copy()
-    ## calculation start ###
-    tk.start()
-    for i_batch in range(bs):
-        for i_ch in range(n_chs):
-            filted_cpu[i_batch, i_ch] = bp_cpu(filted_cpu[i_batch, i_ch])
-            tk(message="CPU")
-            ## calculation end ###
-    title_filt_cpu = "[CPU] Bandpass Filted, #{}, ch{} (Freqs: (Low_lim, High_lim) = ({}, {}) Hz) (time: {:.5f} [sec])".format(
-        i_batch_show, i_ch_show, PASS_LOW_HZ, PASS_HIGH_HZ, tk.elapsed
+    ds_val = TensorDataset(
+        _ds_val.dataset.data.to(torch.float32),
+        _ds_val.dataset.targets,
     )
-    _wv_out_filted_cpu = wavelet_np(
-        filted_cpu[i_batch_show, i_ch_show],
-        fs,
-        f_min=1,
-        plot=True,
-        title=title_filt_cpu,
+    ds_tes = TensorDataset(
+        _ds_tes.data.to(torch.float32),
+        _ds_tes.targets,
     )
 
-    # GPU Bandpass Filtering
-    BandPassFilterGPUTorch = BandPassFilterTorch
-    bp_gpu = BandPassFilterGPUTorch(
-        low_hz=PASS_LOW_HZ, high_hz=PASS_HIGH_HZ, fs=fs
-    ).cuda()
-    # sig_torch = torch.tensor(sig_orig).unsqueeze(0).unsqueeze(0).cuda()
-    sig_torch = torch.tensor(sig_orig).cuda()
-    ## calculation start ###
-    tk.start()
-    filted_gpu = bp_gpu(sig_torch)
-    tk(message="GPU")
-    ## calculation end ###
-    title_filt_gpu = "[GPU] Bandpass Filted, #{}, ch{} (Freqs: (Low_lim, High_lim) = ({}, {}) Hz) (time: {:.5f} [sec])".format(
-        i_batch_show, i_ch_show, PASS_LOW_HZ, PASS_HIGH_HZ, tk.elapsed
+    ## to dataloaders
+    batch_size = 64
+    dl_tra = DataLoader(
+        dataset=ds_tra,
+        batch_size=batch_size,
+        shuffle=True,
+        drop_last=True,
     )
-    _wv_out_filted_gpu = wavelet(
-        filted_gpu[i_batch_show, i_ch_show].cpu(),
-        fs,
-        f_min=1,
-        plot=True,
-        title=title_filt_gpu,
-    )
-
-
-from scipy.signal import butter, sosfilt, sosfreqz
-
-
-def bandpassfilter_np(data, lo_hz, hi_hz, fs, order=5):
-    """
-    Apply a Butterworth bandpass filter to a given data array.
-
-    Parameters:
-        data (ndarray): The input signal to be filtered.
-        lo_hz (float): The lower cutoff frequency of the bandpass filter in Hz.
-        hi_hz (float): The upper cutoff frequency of the bandpass filter in Hz.
-        fs (float): The sampling rate of the signal in Hz.
-        order (int): The order of the filter. Higher order means a sharper frequency cutoff,
-                     but the filter might become unstable. Defaults to 5.
-
-    Returns:
-        ndarray: The filtered signal.
-    """
-
-    def _mk_butter_bandpass(order=5):
-        """
-        Create a Butterworth bandpass filter using second-order sections representation.
-
-        Parameters:
-            order (int): The order of the filter.
-
-        Returns:
-            ndarray: Second-order sections representation of the Butterworth bandpass filter.
-        """
-
-        nyq = 0.5 * fs
-        low, high = lo_hz / nyq, hi_hz / nyq
-        sos = butter(
-            order, [low, high], analog=False, btype="band", output="sos"
-        )
-        return sos
-
-    def _butter_bandpass_filter(data):
-        """
-        Apply a Butterworth bandpass filter to a given data array.
-
-        Parameters:
-            data (ndarray): The input signal to be filtered.
-
-        Returns:
-            ndarray: The filtered signal.
-        """
-
-        sos = _mk_butter_bandpass()
-        y = sosfilt(sos, data)
-        return y
-
-    sos = _mk_butter_bandpass(order=order)
-    y = _butter_bandpass_filter(data)
-
-    return y
-
-    # EOF
 
+    dl_val = DataLoader(
+        dataset=ds_val,
+        batch_size=batch_size,
+        shuffle=False,
+        drop_last=True,
+    )
 
-# import scipy
+    dl_tes = DataLoader(
+        dataset=ds_tes,
+        batch_size=batch_size,
+        shuffle=False,
+        drop_last=True,
+    )
 
+    ################################################################################
+    ## Preparation
+    ################################################################################
+    model = Perceptron()
+    loss_func = nn.CrossEntropyLoss()
+    optimizer = torch.optim.SGD(model.parameters(), lr=1e-3)
+    softmax = nn.Softmax(dim=-1)
+
+    ################################################################################
+    ## Main
+    ################################################################################
+    lc_logger = LearningCurveLogger()
+    i_global = 0
+
+    n_classes = len(dl_tra.dataset.tensors[1].unique())
+    i_fold = 0
+    max_epochs = 3
+
+    for i_epoch in range(max_epochs):
+        step = "Validation"
+        for i_batch, batch in enumerate(dl_val):
+
+            X, T = batch
+            logits = model(X)
+            pred_proba = softmax(logits)
+            pred_class = pred_proba.argmax(dim=-1)
+            loss = loss_func(logits, T)
+
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", UserWarning)
+                bACC = balanced_accuracy_score(T, pred_class)
+
+            dict_to_log = {
+                "loss_plot": float(loss),
+                "balanced_ACC_plot": float(bACC),
+                "pred_proba": pred_proba.detach().cpu().numpy(),
+                "gt_label": T.cpu().numpy(),
+                # "true_class": T.cpu().numpy(),
+                "i_fold": i_fold,
+                "i_epoch": i_epoch,
+                "i_global": i_global,
+            }
+            lc_logger(dict_to_log, step)
+
+        lc_logger.print(step)
+
+        step = "Training"
+        for i_batch, batch in enumerate(dl_tra):
+            optimizer.zero_grad()
+
+            X, T = batch
+            logits = model(X)
+            pred_proba = softmax(logits)
+            pred_class = pred_proba.argmax(dim=-1)
+            loss = loss_func(logits, T)
+
+            loss.backward()
+            optimizer.step()
+
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", UserWarning)
+                bACC = balanced_accuracy_score(T, pred_class)
+
+            dict_to_log = {
+                "loss_plot": float(loss),
+                "balanced_ACC_plot": float(bACC),
+                "pred_proba": pred_proba.detach().cpu().numpy(),
+                "gt_label": T.cpu().numpy(),
+                # "true_class": T.cpu().numpy(),
+                "i_fold": i_fold,
+                "i_epoch": i_epoch,
+                "i_global": i_global,
+            }
+            lc_logger(dict_to_log, step)
+
+            i_global += 1
+
+        lc_logger.print(step)
+
+    step = "Test"
+    for i_batch, batch in enumerate(dl_tes):
+
+        X, T = batch
+        logits = model(X)
+        pred_proba = softmax(logits)
+        pred_class = pred_proba.argmax(dim=-1)
+        loss = loss_func(logits, T)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", UserWarning)
+            bACC = balanced_accuracy_score(T, pred_class)
+
+        dict_to_log = {
+            "loss_plot": float(loss),
+            "balanced_ACC_plot": float(bACC),
+            "pred_proba": pred_proba.detach().cpu().numpy(),
+            # "gt_label": T.cpu().numpy(),
+            "true_class": T.cpu().numpy(),
+            "i_fold": i_fold,
+            "i_epoch": i_epoch,
+            "i_global": i_global,
+        }
+        lc_logger(dict_to_log, step)
+
+    lc_logger.print(step)
+
+    plt_config_dict = dict(
+        # figsize=(8.7, 10),
+        figscale=2.5,
+        labelsize=16,
+        fontsize=12,
+        legendfontsize=12,
+        tick_size=0.8,
+        tick_width=0.2,
+    )
 
-# def gaussian_filter1d(xx, radius):
-#     # radius = round(truncate * sigma)
-#     sigma = 1
-#     truncate = radius / sigma
-#     return scipy.ndimage.gaussian_filter1d(xx, sigma, truncate=truncate)
+    fig = lc_logger.plot_learning_curves(
+        plt,
+        plt_config_dict=plt_config_dict,
+        title=f"fold#{i_fold}",
+        linewidth=1,
+        scattersize=50,
+    )
+    fig.show()
+    # mngs.general.save(fig, sdir + f"fold#{i_fold}.png")
```

### Comparing `mngs-1.1.1/src/mngs/dsp/mne.py` & `mngs-1.2.0/src/mngs/dsp/_mne.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-01-23 20:15:30 (ywatanabe)"
+# Time-stamp: "2024-04-04 19:34:41 (ywatanabe)"
 
 import mne
+import pandas as pd
+from mngs.dsp.PARAMS import EEG_MONTAGE_1020
 
 
-def to_dig_montage(channel_names):
+def get_eeg_pos(channel_names=EEG_MONTAGE_1020):
     # Load the standard 10-20 montage
     standard_montage = mne.channels.make_standard_montage("standard_1020")
+    standard_montage.ch_names = [
+        ch_name.upper() for ch_name in standard_montage.ch_names
+    ]
 
     # Get the positions of the electrodes in the standard montage
     positions = standard_montage.get_positions()
 
-    # Filter the positions to only include the desired channels
-    custom_ch_pos = {
-        ch: positions["ch_pos"][ch]
-        for ch in channel_names
-        if ch in positions["ch_pos"]
-    }
-
-    # Create a custom DigMontage
-    custom_montage = mne.channels.make_dig_montage(
-        ch_pos=custom_ch_pos,
-        nasion=positions["nasion"],
-        lpa=positions["lpa"],
-        rpa=positions["rpa"],
-    )
+    df = pd.DataFrame(positions["ch_pos"])[channel_names]
 
-    return custom_montage
+    df.set_index(pd.Series(["x", "y", "z"]))
+
+    return df
+
+
+if __name__ == "__main__":
+    print(get_eeg_pos())
```

### Comparing `mngs-1.1.1/src/mngs/general/TimeStamper.py` & `mngs-1.2.0/src/mngs/general/TimeStamper.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/__init__.py` & `mngs-1.2.0/src/mngs/general/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 
 # from .path import find_the_git_root_dir, get_this_fpath, mk_spath, split_fpath
 # from .load import get_data_path_from_a_package, load
 # from .save import is_listed_X, save, save_listed_dfs_as_csv, save_listed_scalars_as_csv
 from ..io.__init__ import *
 from ._close import close
+from ._converters import (
+    numpy_fn,
+    squeeze_if,
+    to_numpy,
+    to_torch,
+    torch_fn,
+    unsqueeze_if,
+)
+from ._norm import to_1_1, to_z, unbias
 from ._shell import run_shellcommand, run_shellscript
 from ._start import start
-from .calc import to_z
-from .converters import (
-    KeepPD,
-    my2array,
-    my2tensor,
-    three2two_dim,
-    two2three_dim,
-)
 from .cuda_collect_env import main as cuda_collect_env
 from .debug import *
 from .email import notify, send_gmail
 from .latex import add_hat_in_the_latex_style, to_the_latex_style
 from .mat2py import *
 from .misc import (
     _return_counting_process,
@@ -42,15 +43,18 @@
     mv_col,
     partial_at,
     pop_keys,
     print_block,
     search,
     squeeze_spaces,
     suppress_output,
+    symlink,
     take_the_closest,
+    to_even,
+    to_odd,
     unique,
     uq,
     wait_key,
 )
 from .pandas import (
     col_to_last,
     col_to_top,
```

### Comparing `mngs-1.1.1/src/mngs/general/_close.py` & `mngs-1.2.0/src/mngs/general/_close.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/_shell.py` & `mngs-1.2.0/src/mngs/general/_shell.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/_start.py` & `mngs-1.2.0/src/mngs/general/_start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-09 08:22:31 (ywatanabe)"
+# Time-stamp: "2024-03-25 12:12:15 (ywatanabe)"
 
 import inspect
 import os as _os
 from datetime import datetime
 from glob import glob
 from pprint import pprint
 from time import sleep
@@ -136,15 +136,17 @@
 if __name__ == "__main__":
     import sys
 
     import matplotlib.pyplot as plt
     import mngs
 
     # --------------------------------------------------------------------------- #
-    CONFIG, sys.stdout, sys.stderr, plt, cc = mngs.gen.start(sys, plt)
+    CONFIG, sys.stdout, sys.stderr, plt, cc = mngs.gen.start(
+        sys, plt, sdir=None
+    )
     # --------------------------------------------------------------------------- #
 
     # YOUR CODE HERE
     print("Hello world from mngs.")
 
     # --------------------------------------------------------------------------- #
     mngs.gen.close(CONFIG)
```

### Comparing `mngs-1.1.1/src/mngs/general/_xml2dict.py` & `mngs-1.2.0/src/mngs/general/_xml2dict.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/cuda_collect_env.py` & `mngs-1.2.0/src/mngs/general/cuda_collect_env.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/debug.py` & `mngs-1.2.0/src/mngs/general/debug.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/email.py` & `mngs-1.2.0/src/mngs/general/email.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/load.py` & `mngs-1.2.0/src/mngs/general/load.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/mat2py.py` & `mngs-1.2.0/src/mngs/general/mat2py.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/misc.py` & `mngs-1.2.0/src/mngs/general/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -723,7 +723,45 @@
 
 
 def mv_col(dataframe, column_name, position):
     temp_col = dataframe[column_name]
     dataframe.drop(labels=[column_name], axis=1, inplace=True)
     dataframe.insert(loc=position, column=column_name, value=temp_col)
     return dataframe
+
+
+def symlink(tgt, src, force=False):
+    if force:
+        try:
+            os.remove(src)
+        except FileNotFoundError:
+            pass
+
+    # Calculate the relative path from src to tgt
+    src_dir = os.path.dirname(src)
+    relative_tgt = os.path.relpath(tgt, src_dir)
+
+    os.symlink(relative_tgt, src)
+    print(
+        mngs.gen.ct(
+            f"\nSymlink was created: {src} -> {relative_tgt}\n", c="yellow"
+        )
+    )
+
+
+#     os.symlink(tgt, src)
+#     print(mngs.gen.ct(f"\nSymlink was created: {src} -> {tgt}\n", c="yellow"))
+# Symlink was created: ./scripts/ml/clf/sct_optuna/optuna_studies/optuna_study_stent_3_classes/best_trial -> /home/ywatanabe/proj/ecog_stent_sheep_visual/scripts/ml/clf/sct_optuna/RUNNING/2024Y-03M-29D-21h55m09s_IBSy/objective/Trial#00068/
+
+
+def to_even(n):
+    if n % 2 == 0:
+        return n
+    else:
+        return n - 1
+
+
+def to_odd(n):
+    if n % 2 == 0:
+        return n - 1
+    else:
+        return n
```

### Comparing `mngs-1.1.1/src/mngs/general/pandas.py` & `mngs-1.2.0/src/mngs/general/pandas.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/path.py` & `mngs-1.2.0/src/mngs/general/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/repro.py` & `mngs-1.2.0/src/mngs/general/repro.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/save.py` & `mngs-1.2.0/src/mngs/general/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/general/torch.py` & `mngs-1.2.0/src/mngs/general/torch.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/gists/_SigMacro_processFigure_S.py` & `mngs-1.2.0/src/mngs/gists/_SigMacro_processFigure_S.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/gists/_SigMacro_toBlue.py` & `mngs-1.2.0/src/mngs/gists/_SigMacro_toBlue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/io/load.py` & `mngs-1.2.0/src/mngs/io/load.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/io/path.py` & `mngs-1.2.0/src/mngs/io/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/io/save.py` & `mngs-1.2.0/src/mngs/io/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/linalg/_misc.py` & `mngs-1.2.0/src/mngs/linalg/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/ClassificationReporter.py` & `mngs-1.2.0/src/mngs/ml/ClassificationReporter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/ClassifierServer.py` & `mngs-1.2.0/src/mngs/ml/ClassifierServer.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/__Classifiers.py` & `mngs-1.2.0/src/mngs/ml/__Classifiers.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/clustering/_UMAP.py` & `mngs-1.2.0/src/mngs/ml/clustering/_UMAP.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/clustering/_umap.py` & `mngs-1.2.0/src/mngs/ml/clustering/_umap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/loss/MultiTaskLoss.py` & `mngs-1.2.0/src/mngs/ml/loss/MultiTaskLoss.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/loss/_L1L2Losses.py` & `mngs-1.2.0/src/mngs/ml/loss/_L1L2Losses.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/metrics/_bACC.py` & `mngs-1.2.0/src/mngs/ml/metrics/_bACC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py` & `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py` & `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py` & `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py` & `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py` & `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/optim/_get_set.py` & `mngs-1.2.0/src/mngs/ml/optim/_get_set.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/plt/_conf_mat.py` & `mngs-1.2.0/src/mngs/ml/plt/_conf_mat.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/plt/_learning_curve.py` & `mngs-1.2.0/src/mngs/ml/plt/_learning_curve.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/plt/_optuna_study.py` & `mngs-1.2.0/src/mngs/ml/plt/_optuna_study.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-13 14:13:54 (ywatanabe)"
+# Time-stamp: "2024-03-30 08:24:55 (ywatanabe)"
+import os
 
 
-def optuna_study(lpath, value_str):
+def optuna_study(lpath, value_str, sort=False):
     """
     Loads an Optuna study and generates various visualizations for each target metric.
 
     Parameters:
     - lpath (str): Path to the Optuna study database.
     - value_str (str): The name of the column to be used as the optimization target.
 
@@ -20,45 +21,59 @@
     import matplotlib.pyplot as plt
     import mngs
     import optuna
     import pandas as pd
 
     plt, CC = mngs.plt.configure_mpl(plt, fig_scale=3)
 
+    lpath = lpath.replace("./", "/")
+
     study = optuna.load_study(study_name=None, storage=lpath)
 
     sdir = lpath.replace("sqlite:///", "./").replace(".db", "/")
 
     # To get the best trial:
     best_trial = study.best_trial
     print(f"Best trial number: {best_trial.number}")
     print(f"Best trial value: {best_trial.value}")
     print(f"Best trial parameters: {best_trial.params}")
     print(f"Best trial user attributes: {best_trial.user_attrs}")
 
     # Merge the user attributes into the study history DataFrame
-    study_history = (
-        study.trials_dataframe()
-        .sort_values(["value"])
-        .rename(columns={"value": value_str})
+    study_history = study.trials_dataframe().rename(
+        columns={"value": value_str}
     )
 
+    if sort:
+        ascending = "MINIMIZE" in str(study.directions[0])  # [REVISED]
+        study_history = study_history.sort_values(
+            [value_str], ascending=ascending
+        )
+
     # Add user attributes to the study history DataFrame
     attrs_df = []
     for trial in study.trials:
         user_attrs = trial.user_attrs
         user_attrs = {k: v for k, v in user_attrs.items()}
         attrs_df.append({"number": trial.number, **user_attrs})
     attrs_df = pd.DataFrame(attrs_df).set_index("number")
 
     # Updates study history
     study_history = study_history.merge(
         attrs_df, left_index=True, right_index=True, how="left"
     ).set_index("number")
-    # study_history = mngs.gen.mv_col(study_history, "bACC", 1)
+    try:
+        study_history = mngs.gen.mv_col(study_history, "SDIR", 1)
+        study_history["SDIR"] = study_history["SDIR"].apply(
+            lambda x: str(x).replace("RUNNING", "FINISHED")
+        )
+        best_trial_dir = study_history["SDIR"].iloc[0]
+        mngs.gen.symlink(best_trial_dir, sdir + "best_trial", force=True)
+    except Exception as e:
+        print(e)
     mngs.io.save(study_history, sdir + "study_history.csv")
     print(study_history)
 
     # To visualize the optimization history:
     fig = optuna.visualization.plot_optimization_history(
         study, target_name=value_str
     )
@@ -93,10 +108,14 @@
     mngs.io.save(fig, sdir + "parallel_coordinate.png")
     mngs.io.save(fig, sdir + "parallel_coordinate.html")
     plt.close()
 
 
 if __name__ == "__main__":
     mngs.plt.configure_mpl(plt, fig_scale=3)
-    lpath = "sqlite:///scripts/ml/clf/sub_conv_transformer/optuna_studies/optuna_study_v032.db"
-    optuna_study(lpath, "Validation loss")
+    lpath = "sqlite:///scripts/ml/clf/sub_conv_transformer_optuna/optuna_studies/optuna_study_v001.db"
+    lpath = "sqlite:///scripts/ml/clf/rocket_optuna/optuna_studies/optuna_study_v001.db"
+    optuna_study(lpath, "Validation bACC")
     # scripts/ml/clf/sub_conv_transformer/optuna_studies/optuna_study_v032
+
+    lpath = "sqlite:///scripts/ml/clf/sub_conv_transformer_optuna/optuna_studies/optuna_study_v020.db"
+    mngs.ml.plt.optuna_study(lpath, "val_loss", sort=True)
```

### Comparing `mngs-1.1.1/src/mngs/ml/plt/aucs/example.py` & `mngs-1.2.0/src/mngs/ml/plt/aucs/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/plt/aucs/pre_rec_auc.py` & `mngs-1.2.0/src/mngs/ml/plt/aucs/pre_rec_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/plt/aucs/roc_auc.py` & `mngs-1.2.0/src/mngs/ml/plt/aucs/roc_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/silhoute_score_block.py` & `mngs-1.2.0/src/mngs/ml/silhoute_score_block.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/sk/_clf.py` & `mngs-1.2.0/src/mngs/ml/sk/_clf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-13 12:04:30 (ywatanabe)"
+# Time-stamp: "2024-03-23 17:36:05 (ywatanabe)"
 
 import numpy as np
 from sklearn.decomposition import PCA
 from sklearn.ensemble import GradientBoostingClassifier, RandomForestClassifier
 from sklearn.feature_selection import SelectKBest, f_classif
-from sklearn.linear_model import RidgeClassifierCV
+from sklearn.linear_model import LogisticRegression, RidgeClassifierCV
 from sklearn.pipeline import make_pipeline
 from sklearn.svm import SVC, LinearSVC
 from sktime.classification.deep_learning.cnn import CNNClassifier
 from sktime.classification.deep_learning.inceptiontime import (
     InceptionTimeClassifier,
 )
 from sktime.classification.deep_learning.lstmfcn import LSTMFCNClassifier
@@ -31,15 +31,18 @@
 # def rocket_pipeline(*args, **kwargs):
 #     return _rocket_pipeline
 
 
 def rocket_pipeline(*args, **kwargs):
     return make_pipeline(
         Rocket(*args, **kwargs),
-        RidgeClassifierCV(alphas=np.logspace(-3, 3, 10)),
+        LogisticRegression(
+            max_iter=1000
+        ),  # Increase max_iter if needed for convergence
+        # RidgeClassifierCV(alphas=np.logspace(-3, 3, 10)),
         # SVC(probability=True, kernel="linear"),
     )
 
 
 # def rocket_pipeline(*args, **kwargs):
 #     return make_pipeline(
 #         Rocket(*args, **kwargs),
```

### Comparing `mngs-1.1.1/src/mngs/ml/sk/_to_sktime.py` & `mngs-1.2.0/src/mngs/ml/sk/_to_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/utils/_DefaultDataset.py` & `mngs-1.2.0/src/mngs/ml/utils/_DefaultDataset.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/utils/_LabelEncoder.py` & `mngs-1.2.0/src/mngs/ml/utils/_LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/utils/_check_params.py` & `mngs-1.2.0/src/mngs/ml/utils/_check_params.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/utils/_format_samples_for_sktime.py` & `mngs-1.2.0/src/mngs/ml/utils/_format_samples_for_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/utils/_merge_labels.py` & `mngs-1.2.0/src/mngs/ml/utils/_merge_labels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/ml/utils/_under_sample.py` & `mngs-1.2.0/src/mngs/ml/utils/_under_sample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_BNet.py` & `mngs-1.2.0/src/mngs/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_BNet_Res.py` & `mngs-1.2.0/src/mngs/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_ChannelGainChanger.py` & `mngs-1.2.0/src/mngs/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_DropoutChannels.py` & `mngs-1.2.0/src/mngs/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_FreqGainChanger.py` & `mngs-1.2.0/src/mngs/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_MNet_1000.py` & `mngs-1.2.0/src/mngs/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_ResNet1D.py` & `mngs-1.2.0/src/mngs/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_SpatialAttention.py` & `mngs-1.2.0/src/mngs/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/nn/_SwapChannels.py` & `mngs-1.2.0/src/mngs/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/os/_mv.py` & `mngs-1.2.0/src/mngs/os/_mv.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_add_hue.py` & `mngs-1.2.0/src/mngs/plt/_add_hue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_annotated_heatmap.py` & `mngs-1.2.0/src/mngs/plt/_annotated_heatmap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_configure_mpl.py` & `mngs-1.2.0/src/mngs/plt/_configure_mpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_draw_a_cube.py` & `mngs-1.2.0/src/mngs/plt/_draw_a_cube.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_get_RGBA_from_colormap.py` & `mngs-1.2.0/src/mngs/plt/_get_RGBA_from_colormap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_mk_colorbar.py` & `mngs-1.2.0/src/mngs/plt/_mk_colorbar.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/_subplots.py` & `mngs-1.2.0/src/mngs/plt/_subplots.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_circular_hist.py` & `mngs-1.2.0/src/mngs/plt/ax/_circular_hist.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_extend.py` & `mngs-1.2.0/src/mngs/plt/ax/_extend.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_hide_spines.py` & `mngs-1.2.0/src/mngs/plt/ax/_hide_spines.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_map_ticks.py` & `mngs-1.2.0/src/mngs/plt/ax/_map_ticks.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_panel.py` & `mngs-1.2.0/src/mngs/plt/ax/_panel.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_sci_note.py` & `mngs-1.2.0/src/mngs/plt/ax/_sci_note.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/ax/_set_pos.py` & `mngs-1.2.0/src/mngs/plt/ax/_set_pos.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/colors.py` & `mngs-1.2.0/src/mngs/plt/colors.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/plt/get_mpl_color.py` & `mngs-1.2.0/src/mngs/plt/get_mpl_color.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/resource/get.py` & `mngs-1.2.0/src/mngs/resource/get.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/resource/limit_RAM.py` & `mngs-1.2.0/src/mngs/resource/limit_RAM.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_bonferroni_correction.py` & `mngs-1.2.0/src/mngs/stats/_bonferroni_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_brunner_munzel_test.py` & `mngs-1.2.0/src/mngs/stats/_brunner_munzel_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_corr_test.py` & `mngs-1.2.0/src/mngs/stats/_corr_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_fdr_correction.py` & `mngs-1.2.0/src/mngs/stats/_fdr_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_multicompair.py` & `mngs-1.2.0/src/mngs/stats/_multicompair.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_nocorrelation_test.py` & `mngs-1.2.0/src/mngs/stats/_nocorrelation_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs/stats/_smirnov_grubbs.py` & `mngs-1.2.0/src/mngs/stats/_smirnov_grubbs.py`

 * *Files identical despite different names*

### Comparing `mngs-1.1.1/src/mngs.egg-info/SOURCES.txt` & `mngs-1.2.0/src/mngs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,34 @@
 setup.py
 src/mngs/__init__.py
 src/mngs.egg-info/PKG-INFO
 src/mngs.egg-info/SOURCES.txt
 src/mngs.egg-info/dependency_links.txt
 src/mngs.egg-info/requires.txt
 src/mngs.egg-info/top_level.txt
-src/mngs/dsp/HilbertTransformationTorch.py
 src/mngs/dsp/PARAMS.py
 src/mngs/dsp/__init__.py
-src/mngs/dsp/_load_BIDS.py
+src/mngs/dsp/_demo_sig.py
+src/mngs/dsp/_ensure_3d.py
+src/mngs/dsp/_hilbert.py
+src/mngs/dsp/_mne.py
 src/mngs/dsp/_psd.py
-src/mngs/dsp/demo_sig.py
-src/mngs/dsp/feature_extractors.py
-src/mngs/dsp/fft.py
-src/mngs/dsp/filters.py
-src/mngs/dsp/mne.py
-src/mngs/dsp/referencing.py
-src/mngs/dsp/sampling.py
-src/mngs/dsp/transform.py
+src/mngs/dsp/_transform.py
+src/mngs/dsp/_wavelet.py
+src/mngs/dsp/add_noise.py
+src/mngs/dsp/filt.py
+src/mngs/dsp/ref.py
 src/mngs/general/TimeStamper.py
 src/mngs/general/__init__.py
 src/mngs/general/_close.py
+src/mngs/general/_converters.py
+src/mngs/general/_norm.py
 src/mngs/general/_shell.py
 src/mngs/general/_start.py
 src/mngs/general/_xml2dict.py
-src/mngs/general/calc.py
-src/mngs/general/converters.py
 src/mngs/general/cuda_collect_env.py
 src/mngs/general/debug.py
 src/mngs/general/email.py
 src/mngs/general/latex.py
 src/mngs/general/load.py
 src/mngs/general/mat2py.py
 src/mngs/general/misc.py
@@ -96,35 +95,46 @@
 src/mngs/ml/utils/__init__.py
 src/mngs/ml/utils/_check_params.py
 src/mngs/ml/utils/_format_samples_for_sktime.py
 src/mngs/ml/utils/_merge_labels.py
 src/mngs/ml/utils/_sliding_window_data_augmentation.py
 src/mngs/ml/utils/_under_sample.py
 src/mngs/ml/utils/_verify_n_gpus.py
+src/mngs/mngs/__init__.py
+src/mngs/mngs/setup.py
+src/mngs/nn/_AxiswiseDropout.py
 src/mngs/nn/_BNet.py
 src/mngs/nn/_BNet_Res.py
 src/mngs/nn/_ChannelGainChanger.py
 src/mngs/nn/_DropoutChannels.py
+src/mngs/nn/_Filters.py
 src/mngs/nn/_FreqGainChanger.py
+src/mngs/nn/_GaussianFilter.py
+src/mngs/nn/_Hilbert.py
 src/mngs/nn/_MNet_1000.py
+src/mngs/nn/_PSD.py
 src/mngs/nn/_ResNet1D.py
 src/mngs/nn/_SpatialAttention.py
+src/mngs/nn/_Spectrogram.py
 src/mngs/nn/_SwapChannels.py
+src/mngs/nn/_TransposeLayer.py
+src/mngs/nn/_Wavelet.py
 src/mngs/nn/__init__.py
 src/mngs/os/__init__.py
 src/mngs/os/_mv.py
 src/mngs/plt/__init__.py
 src/mngs/plt/_add_hue.py
 src/mngs/plt/_annotated_heatmap.py
 src/mngs/plt/_configure_mpl.py
 src/mngs/plt/_draw_a_cube.py
 src/mngs/plt/_get_RGBA_from_colormap.py
 src/mngs/plt/_mk_colorbar.py
 src/mngs/plt/_mk_patches.py
 src/mngs/plt/_subplots.py
+src/mngs/plt/_tpl.py
 src/mngs/plt/colors.py
 src/mngs/plt/get_mpl_color.py
 src/mngs/plt/ax/__init__.py
 src/mngs/plt/ax/_circular_hist.py
 src/mngs/plt/ax/_extend.py
 src/mngs/plt/ax/_fill_between.py
 src/mngs/plt/ax/_hide_spines.py
@@ -139,11 +149,14 @@
 src/mngs/resource/limit_RAM.py
 src/mngs/stats/__init__.py
 src/mngs/stats/_bonferroni_correction.py
 src/mngs/stats/_brunner_munzel_test.py
 src/mngs/stats/_calc_partial_corr.py
 src/mngs/stats/_corr_test.py
 src/mngs/stats/_fdr_correction.py
+src/mngs/stats/_general.py
 src/mngs/stats/_multicompair.py
 src/mngs/stats/_nocorrelation_test.py
 src/mngs/stats/_smirnov_grubbs.py
-src/mngs/stats/_to_asterisks.py
+src/mngs/stats/_to_asterisks.py
+src/mngs/torch/__init__.py
+src/mngs/torch/_apply_to.py
```

