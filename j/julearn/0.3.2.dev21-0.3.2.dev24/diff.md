# Comparing `tmp/julearn-0.3.2.dev21.tar.gz` & `tmp/julearn-0.3.2.dev24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julearn-0.3.2.dev21.tar", last modified: Wed Mar  6 17:04:17 2024, max compression
+gzip compressed data, was "julearn-0.3.2.dev24.tar", last modified: Thu Apr  4 14:42:17 2024, max compression
```

## Comparing `julearn-0.3.2.dev21.tar` & `julearn-0.3.2.dev24.tar`

### file list

```diff
@@ -1,283 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.855895 julearn-0.3.2.dev21/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.803895 julearn-0.3.2.dev21/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.811895 julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/documentation_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/feature_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.811895 julearn-0.3.2.dev21/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/check-stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-06 17:04:17.851895 julearn-0.3.2.dev21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.815895 julearn-0.3.2.dev21/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.803895 julearn-0.3.2.dev21/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.815895 julearn-0.3.2.dev21/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.815895 julearn-0.3.2.dev21/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.815895 julearn-0.3.2.dev21/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/_templates/function_warning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.815895 julearn-0.3.2.dev21/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/api/viz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/available_pipeline_steps.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.819895 julearn-0.3.2.dev21/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.819895 julearn-0.3.2.dev21/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/changes/newsfragments/224.misc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/changes/newsfragments/244.misc
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/changes/newsfragments/249.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/changes/newsfragments/251.misc
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.823895 julearn-0.3.2.dev21/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/corrected_ttest.png
--rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/final_estimator.png
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/iris_X.png
--rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/iris_df.png
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/iris_y.png
--rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_calm.png
--rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_confbias.png
--rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_generalization.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_it.png
--rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_ml.png
--rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/julearn_logo_mlit.png
--rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/multiple_scorers_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/plot_scores.png
--rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/scores_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/scores_run_cv_splitter.png
--rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/images/scores_run_cv_train.png
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.823895 julearn-0.3.2.dev21/docs/selected_deeper_topics/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/CBPM.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/confound_removal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/cross_validation_splitter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/hyperparameter_tuning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/model_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/stacked_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/selected_deeper_topics/target_transformers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.823895 julearn-0.3.2.dev21/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.823895 julearn-0.3.2.dev21/docs/what_really_need_know/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/what_really_need_know/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/what_really_need_know/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/what_really_need_know/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/what_really_need_know/model_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/what_really_need_know/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/what_really_need_know/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.827895 julearn-0.3.2.dev21/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.827895 julearn-0.3.2.dev21/examples/00_starting/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/plot_cm_acc_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/plot_example_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/plot_stratified_kfold_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/run_combine_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/run_grouped_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/00_starting/run_simple_binary_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.827895 julearn-0.3.2.dev21/examples/01_model_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/01_model_comparison/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/01_model_comparison/plot_simple_model_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.827895 julearn-0.3.2.dev21/examples/02_inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/02_inspection/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/02_inspection/plot_groupcv_inspect_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/02_inspection/plot_inspect_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/02_inspection/plot_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/02_inspection/run_binary_inspect_folds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.827895 julearn-0.3.2.dev21/examples/03_complex_models/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/03_complex_models/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/03_complex_models/run_apply_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/03_complex_models/run_example_pca_featsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/03_complex_models/run_hyperparameter_multiple_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/03_complex_models/run_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/03_complex_models/run_stacked_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.831895 julearn-0.3.2.dev21/examples/04_confounds/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/04_confounds/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/04_confounds/plot_confound_removal_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/04_confounds/run_return_confounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.831895 julearn-0.3.2.dev21/examples/05_customization/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/05_customization/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/05_customization/run_custom_scorers_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.831895 julearn-0.3.2.dev21/examples/99_docs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_cbpm_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_confound_removal_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_cv_splitters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_data_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_hyperparameters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_model_comparison_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_model_evaluation_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_model_inspection_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_pipeline_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_stacked_models_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/99_docs/run_target_transformer_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.831895 julearn-0.3.2.dev21/examples/XX_disabled/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/XX_disabled/dis_run_n_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/examples/XX_disabled/dis_run_target_confound_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.835895 julearn-0.3.2.dev21/julearn/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-06 17:04:17.000000 julearn-0.3.2.dev21/julearn/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.835895 julearn-0.3.2.dev21/julearn/base/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/base/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/base/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.835895 julearn-0.3.2.dev21/julearn/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/base/tests/test_base_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/base/tests/test_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.835895 julearn-0.3.2.dev21/julearn/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.839895 julearn-0.3.2.dev21/julearn/inspect/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/inspect/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.839895 julearn-0.3.2.dev21/julearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/continuous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.839895 julearn-0.3.2.dev21/julearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/tests/test_available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/tests/test_continous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/model_selection/tests/test_stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.839895 julearn-0.3.2.dev21/julearn/models/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/models/available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/models/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.839895 julearn-0.3.2.dev21/julearn/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/models/tests/test_available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/models/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/models/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.839895 julearn-0.3.2.dev21/julearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/target_pipeline_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/pipeline/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/test/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/test/test_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/test/test_target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/pipeline/test/test_target_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16338 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/scoring/available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/scoring/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/scoring/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/scoring/tests/test_available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/scoring/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/stats/corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/stats/tests/test_corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37962 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/tests/test_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.843895 julearn-0.3.2.dev21/julearn/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.847895 julearn-0.3.2.dev21/julearn/transformers/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/set_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.847895 julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_set_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/ju_column_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.847895 julearn-0.3.2.dev21/julearn/transformers/target/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.847895 julearn-0.3.2.dev21/julearn/transformers/target/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/tests/test_available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/tests/test_ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/tests/test_ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/target/tests/test_target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.847895 julearn-0.3.2.dev21/julearn/transformers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/tests/test_available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/tests/test_cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/tests/test_confounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/transformers/tests/test_jucolumntransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.851895 julearn-0.3.2.dev21/julearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.851895 julearn-0.3.2.dev21/julearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.851895 julearn-0.3.2.dev21/julearn/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14622 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/viz/_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.851895 julearn-0.3.2.dev21/julearn/viz/res/
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/julearn/viz/res/julearn_logo_generalization.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:04:17.851895 julearn-0.3.2.dev21/julearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-06 17:04:17.000000 julearn-0.3.2.dev21/julearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-03-06 17:04:17.000000 julearn-0.3.2.dev21/julearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:04:17.000000 julearn-0.3.2.dev21/julearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-06 17:04:17.000000 julearn-0.3.2.dev21/julearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-06 17:04:17.000000 julearn-0.3.2.dev21/julearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 17:04:17.855895 julearn-0.3.2.dev21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-06 17:04:06.000000 julearn-0.3.2.dev21/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.504727 julearn-0.3.2.dev24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.452727 julearn-0.3.2.dev24/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.460727 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/documentation_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/feature_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.460727 julearn-0.3.2.dev24/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/check-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-04 14:42:17.504727 julearn-0.3.2.dev24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.452727 julearn-0.3.2.dev24/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/function_warning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.468727 julearn-0.3.2.dev24/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/viz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/available_pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.468727 julearn-0.3.2.dev24/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.468727 julearn-0.3.2.dev24/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/224.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/244.misc
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/249.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/251.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/255.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/corrected_ttest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/final_estimator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/iris_X.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/iris_df.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/iris_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_calm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_confbias.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_generalization.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_it.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_ml.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_mlit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/multiple_scorers_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/plot_scores.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/scores_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/scores_run_cv_splitter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/scores_run_cv_train.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/selected_deeper_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/CBPM.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/confound_removal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/cross_validation_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/hyperparameter_tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/model_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/stacked_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/target_transformers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/sphinxext/gh_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/what_really_need_know/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/model_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/00_starting/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/plot_cm_acc_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/plot_example_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/plot_stratified_kfold_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/run_combine_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/run_grouped_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/run_simple_binary_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/01_model_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/01_model_comparison/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/01_model_comparison/plot_simple_model_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/02_inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/plot_groupcv_inspect_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/plot_inspect_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/plot_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/run_binary_inspect_folds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/03_complex_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_apply_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_example_pca_featsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_multiple_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_stacked_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/04_confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/04_confounds/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/04_confounds/plot_confound_removal_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/04_confounds/run_return_confounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/05_customization/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/05_customization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/05_customization/run_custom_scorers_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.484727 julearn-0.3.2.dev24/examples/99_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_cbpm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_confound_removal_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_cv_splitters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_data_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_hyperparameters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_model_comparison_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_model_evaluation_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_model_inspection_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_pipeline_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_stacked_models_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_target_transformer_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.484727 julearn-0.3.2.dev24/examples/XX_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/XX_disabled/dis_run_n_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/XX_disabled/dis_run_target_confound_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.484727 julearn-0.3.2.dev24/julearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/tests/test_base_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/tests/test_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/inspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/continuous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/tests/test_available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/tests/test_continous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/tests/test_stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/tests/test_available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/target_pipeline_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/pipeline/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16338 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/scoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/tests/test_available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/stats/corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/stats/tests/test_corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37962 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/tests/test_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/set_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_set_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/ju_column_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/target/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/target/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/transformers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_confounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_jucolumntransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/viz/_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/viz/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/viz/res/julearn_logo_generalization.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:42:17.504727 julearn-0.3.2.dev24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/tox.ini
```

### Comparing `julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/bug_report.yaml` & `julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/documentation_request.yaml` & `julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/documentation_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/ISSUE_TEMPLATE/feature_request.yaml` & `julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/workflows/ci-docs.yml` & `julearn-0.3.2.dev24/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/workflows/ci.yml` & `julearn-0.3.2.dev24/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/workflows/docs-preview.yml` & `julearn-0.3.2.dev24/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/workflows/docs.yml` & `julearn-0.3.2.dev24/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/workflows/lint.yml` & `julearn-0.3.2.dev24/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.github/workflows/pypi.yml` & `julearn-0.3.2.dev24/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.gitignore` & `julearn-0.3.2.dev24/.gitignore`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/.pre-commit-config.yaml` & `julearn-0.3.2.dev24/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/LICENSE.md` & `julearn-0.3.2.dev24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/PKG-INFO` & `julearn-0.3.2.dev24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev21
+Version: 0.3.2.dev24
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
```

### Comparing `julearn-0.3.2.dev21/README.md` & `julearn-0.3.2.dev24/README.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/codecov.yml` & `julearn-0.3.2.dev24/codecov.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/Makefile` & `julearn-0.3.2.dev24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/_templates/class.rst` & `julearn-0.3.2.dev24/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/_templates/function_warning.rst` & `julearn-0.3.2.dev24/docs/_templates/function_warning.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/_templates/versions.html` & `julearn-0.3.2.dev24/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/base.rst` & `julearn-0.3.2.dev24/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/model_selection.rst` & `julearn-0.3.2.dev24/docs/api/model_selection.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/models.rst` & `julearn-0.3.2.dev24/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/scoring.rst` & `julearn-0.3.2.dev24/docs/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/transformers.rst` & `julearn-0.3.2.dev24/docs/api/transformers.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/utils.rst` & `julearn-0.3.2.dev24/docs/api/utils.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/api/viz.rst` & `julearn-0.3.2.dev24/docs/api/viz.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/available_pipeline_steps.rst` & `julearn-0.3.2.dev24/docs/available_pipeline_steps.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/conf.py` & `julearn-0.3.2.dev24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/configuration.rst` & `julearn-0.3.2.dev24/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/contributing.rst` & `julearn-0.3.2.dev24/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/examples.rst` & `julearn-0.3.2.dev24/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/faq.rst` & `julearn-0.3.2.dev24/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/getting_started.rst` & `julearn-0.3.2.dev24/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/corrected_ttest.png` & `julearn-0.3.2.dev24/docs/images/corrected_ttest.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/final_estimator.png` & `julearn-0.3.2.dev24/docs/images/final_estimator.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/iris_X.png` & `julearn-0.3.2.dev24/docs/images/iris_X.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/iris_df.png` & `julearn-0.3.2.dev24/docs/images/iris_df.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/iris_y.png` & `julearn-0.3.2.dev24/docs/images/iris_y.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_calm.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_calm.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_confbias.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_confbias.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_cv.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_generalization.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_it.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_it.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_ml.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_ml.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/julearn_logo_mlit.png` & `julearn-0.3.2.dev24/docs/images/julearn_logo_mlit.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/multiple_scorers_run_cv.png` & `julearn-0.3.2.dev24/docs/images/multiple_scorers_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/plot_scores.png` & `julearn-0.3.2.dev24/docs/images/plot_scores.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/scores_run_cv.png` & `julearn-0.3.2.dev24/docs/images/scores_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/scores_run_cv_splitter.png` & `julearn-0.3.2.dev24/docs/images/scores_run_cv_splitter.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/images/scores_run_cv_train.png` & `julearn-0.3.2.dev24/docs/images/scores_run_cv_train.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/index.rst` & `julearn-0.3.2.dev24/docs/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/links.inc` & `julearn-0.3.2.dev24/docs/links.inc`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/maintaining.rst` & `julearn-0.3.2.dev24/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/sphinxext/gh_substitutions.py` & `julearn-0.3.2.dev24/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/what_really_need_know/cross_validation.rst` & `julearn-0.3.2.dev24/docs/what_really_need_know/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/what_really_need_know/index.rst` & `julearn-0.3.2.dev24/docs/what_really_need_know/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/docs/whats_new.rst` & `julearn-0.3.2.dev24/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/00_starting/plot_cm_acc_multiclass.py` & `julearn-0.3.2.dev24/examples/00_starting/plot_cm_acc_multiclass.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/00_starting/plot_example_regression.py` & `julearn-0.3.2.dev24/examples/00_starting/plot_example_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/00_starting/plot_stratified_kfold_reg.py` & `julearn-0.3.2.dev24/examples/00_starting/plot_stratified_kfold_reg.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/00_starting/run_combine_pandas.py` & `julearn-0.3.2.dev24/examples/00_starting/run_combine_pandas.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/00_starting/run_grouped_cv.py` & `julearn-0.3.2.dev24/examples/00_starting/run_grouped_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/00_starting/run_simple_binary_classification.py` & `julearn-0.3.2.dev24/examples/00_starting/run_simple_binary_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/01_model_comparison/plot_simple_model_comparison.py` & `julearn-0.3.2.dev24/examples/01_model_comparison/plot_simple_model_comparison.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/02_inspection/plot_groupcv_inspect_svm.py` & `julearn-0.3.2.dev24/examples/02_inspection/plot_groupcv_inspect_svm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/02_inspection/plot_inspect_random_forest.py` & `julearn-0.3.2.dev24/examples/02_inspection/plot_inspect_random_forest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/02_inspection/plot_preprocess.py` & `julearn-0.3.2.dev24/examples/02_inspection/plot_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/02_inspection/run_binary_inspect_folds.py` & `julearn-0.3.2.dev24/examples/02_inspection/run_binary_inspect_folds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/03_complex_models/run_apply_to_target.py` & `julearn-0.3.2.dev24/examples/03_complex_models/run_apply_to_target.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/03_complex_models/run_example_pca_featsets.py` & `julearn-0.3.2.dev24/examples/03_complex_models/run_example_pca_featsets.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/03_complex_models/run_hyperparameter_multiple_grids.py` & `julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/03_complex_models/run_hyperparameter_tuning.py` & `julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/03_complex_models/run_stacked_models.py` & `julearn-0.3.2.dev24/examples/03_complex_models/run_stacked_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/04_confounds/plot_confound_removal_classification.py` & `julearn-0.3.2.dev24/examples/04_confounds/plot_confound_removal_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/04_confounds/run_return_confounds.py` & `julearn-0.3.2.dev24/examples/04_confounds/run_return_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/05_customization/run_custom_scorers_regression.py` & `julearn-0.3.2.dev24/examples/05_customization/run_custom_scorers_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_cbpm_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_cbpm_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_confound_removal_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_confound_removal_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_cv_splitters_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_cv_splitters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_data_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_data_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_hyperparameters_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_hyperparameters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_model_comparison_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_model_comparison_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_model_evaluation_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_model_evaluation_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_model_inspection_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_model_inspection_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_pipeline_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_pipeline_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_stacked_models_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_stacked_models_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/99_docs/run_target_transformer_docs.py` & `julearn-0.3.2.dev24/examples/99_docs/run_target_transformer_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/XX_disabled/dis_run_n_jobs.py` & `julearn-0.3.2.dev24/examples/XX_disabled/dis_run_n_jobs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/examples/XX_disabled/dis_run_target_confound_removal.py` & `julearn-0.3.2.dev24/examples/XX_disabled/dis_run_target_confound_removal.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/api.py` & `julearn-0.3.2.dev24/julearn/api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/base/column_types.py` & `julearn-0.3.2.dev24/julearn/base/column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/base/estimators.py` & `julearn-0.3.2.dev24/julearn/base/estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/base/tests/test_base_estimators.py` & `julearn-0.3.2.dev24/julearn/base/tests/test_base_estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/base/tests/test_column_types.py` & `julearn-0.3.2.dev24/julearn/base/tests/test_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/config.py` & `julearn-0.3.2.dev24/julearn/config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/conftest.py` & `julearn-0.3.2.dev24/julearn/conftest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/_cv.py` & `julearn-0.3.2.dev24/julearn/inspect/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/_pipeline.py` & `julearn-0.3.2.dev24/julearn/inspect/_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/_preprocess.py` & `julearn-0.3.2.dev24/julearn/inspect/_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/inspector.py` & `julearn-0.3.2.dev24/julearn/inspect/inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/tests/test_cv.py` & `julearn-0.3.2.dev24/julearn/inspect/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/tests/test_inspector.py` & `julearn-0.3.2.dev24/julearn/inspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/tests/test_pipeline.py` & `julearn-0.3.2.dev24/julearn/inspect/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/inspect/tests/test_preprocess.py` & `julearn-0.3.2.dev24/julearn/inspect/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/model_selection/available_searchers.py` & `julearn-0.3.2.dev24/julearn/model_selection/available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/model_selection/continuous_stratified_kfold.py` & `julearn-0.3.2.dev24/julearn/model_selection/continuous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/model_selection/stratified_bootstrap.py` & `julearn-0.3.2.dev24/julearn/model_selection/stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/model_selection/tests/test_available_searchers.py` & `julearn-0.3.2.dev24/julearn/model_selection/tests/test_available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/model_selection/tests/test_continous_stratified_kfold.py` & `julearn-0.3.2.dev24/julearn/model_selection/tests/test_continous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/model_selection/tests/test_stratified_bootstrap.py` & `julearn-0.3.2.dev24/julearn/model_selection/tests/test_stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/models/available_models.py` & `julearn-0.3.2.dev24/julearn/models/available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/models/dynamic.py` & `julearn-0.3.2.dev24/julearn/models/dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/models/tests/test_available_models.py` & `julearn-0.3.2.dev24/julearn/models/tests/test_available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/models/tests/test_dynamic.py` & `julearn-0.3.2.dev24/julearn/models/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/models/tests/test_models.py` & `julearn-0.3.2.dev24/julearn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/merger.py` & `julearn-0.3.2.dev24/julearn/pipeline/merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/pipeline_creator.py` & `julearn-0.3.2.dev24/julearn/pipeline/pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/target_pipeline.py` & `julearn-0.3.2.dev24/julearn/pipeline/target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/target_pipeline_creator.py` & `julearn-0.3.2.dev24/julearn/pipeline/target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/test/test_merger.py` & `julearn-0.3.2.dev24/julearn/pipeline/test/test_merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/test/test_pipeline_creator.py` & `julearn-0.3.2.dev24/julearn/pipeline/test/test_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/test/test_target_pipeline.py` & `julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/pipeline/test/test_target_pipeline_creator.py` & `julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/prepare.py` & `julearn-0.3.2.dev24/julearn/prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/scoring/available_scorers.py` & `julearn-0.3.2.dev24/julearn/scoring/available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/scoring/metrics.py` & `julearn-0.3.2.dev24/julearn/scoring/metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/scoring/tests/test_available_scorers.py` & `julearn-0.3.2.dev24/julearn/scoring/tests/test_available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/scoring/tests/test_metrics.py` & `julearn-0.3.2.dev24/julearn/scoring/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/stats/corrected_ttest.py` & `julearn-0.3.2.dev24/julearn/stats/corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/stats/tests/test_corrected_ttest.py` & `julearn-0.3.2.dev24/julearn/stats/tests/test_corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/tests/test_api.py` & `julearn-0.3.2.dev24/julearn/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/tests/test_config.py` & `julearn-0.3.2.dev24/julearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/tests/test_prepare.py` & `julearn-0.3.2.dev24/julearn/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/__init__.py` & `julearn-0.3.2.dev24/julearn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/available_transformers.py` & `julearn-0.3.2.dev24/julearn/transformers/available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/cbpm.py` & `julearn-0.3.2.dev24/julearn/transformers/cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/confound_remover.py` & `julearn-0.3.2.dev24/julearn/transformers/confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/change_column_types.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/drop_columns.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/filter_columns.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/set_column_types.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_change_column_types.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_drop_columns.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_filter_columns.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/dataframe/tests/test_set_column_types.py` & `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/ju_column_transformer.py` & `julearn-0.3.2.dev24/julearn/transformers/ju_column_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/__init__.py` & `julearn-0.3.2.dev24/julearn/transformers/target/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/available_target_transformers.py` & `julearn-0.3.2.dev24/julearn/transformers/target/available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/ju_target_transformer.py` & `julearn-0.3.2.dev24/julearn/transformers/target/ju_target_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/ju_transformed_target_model.py` & `julearn-0.3.2.dev24/julearn/transformers/target/ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/target_confound_remover.py` & `julearn-0.3.2.dev24/julearn/transformers/target/target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/tests/test_available_target_transformers.py` & `julearn-0.3.2.dev24/julearn/transformers/target/tests/test_available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/tests/test_ju_transformed_target_model.py` & `julearn-0.3.2.dev24/julearn/transformers/target/tests/test_ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/target/tests/test_target_confound_remover.py` & `julearn-0.3.2.dev24/julearn/transformers/target/tests/test_target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/tests/test_available_transformers.py` & `julearn-0.3.2.dev24/julearn/transformers/tests/test_available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/tests/test_cbpm.py` & `julearn-0.3.2.dev24/julearn/transformers/tests/test_cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/tests/test_confounds.py` & `julearn-0.3.2.dev24/julearn/transformers/tests/test_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/transformers/tests/test_jucolumntransformers.py` & `julearn-0.3.2.dev24/julearn/transformers/tests/test_jucolumntransformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/_cv.py` & `julearn-0.3.2.dev24/julearn/utils/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/checks.py` & `julearn-0.3.2.dev24/julearn/utils/checks.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/logging.py` & `julearn-0.3.2.dev24/julearn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/testing.py` & `julearn-0.3.2.dev24/julearn/utils/testing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/tests/test_logging.py` & `julearn-0.3.2.dev24/julearn/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/tests/test_version.py` & `julearn-0.3.2.dev24/julearn/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/typing.py` & `julearn-0.3.2.dev24/julearn/utils/typing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/utils/versions.py` & `julearn-0.3.2.dev24/julearn/utils/versions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn/viz/_scores.py` & `julearn-0.3.2.dev24/julearn/viz/_scores.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 y_units="screen",
                 text_align="center",
                 text="Please select a at least one model to display",
                 text_font_size="14pt",
             )
             p.add_layout(labels)
             return p
-        p.circle(
+        p.scatter(
             x=jitter("x", width=0.7, range=p.x_range),
             y="score",
             alpha=0.5,
             source=source,
             size=10,
             line_color="white",
             color=color,
@@ -381,15 +381,14 @@
         pn.Param(
             viewer.param.metric,
             name="Metric",
             show_name=True,
             widgets={
                 "metric": {
                     "type": pn.widgets.Select,
-                    "button_type": "primary",
                     "name": "",
                 }
             },
         )
     )
 
     widget_row.append(
```

### Comparing `julearn-0.3.2.dev21/julearn/viz/res/julearn_logo_generalization.png` & `julearn-0.3.2.dev24/julearn/viz/res/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/julearn.egg-info/PKG-INFO` & `julearn-0.3.2.dev24/julearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev21
+Version: 0.3.2.dev24
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
```

### Comparing `julearn-0.3.2.dev21/julearn.egg-info/SOURCES.txt` & `julearn-0.3.2.dev24/julearn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 docs/api/viz.rst
 docs/changes/contributors.inc
 docs/changes/newsfragments/.gitignore
 docs/changes/newsfragments/224.misc
 docs/changes/newsfragments/244.misc
 docs/changes/newsfragments/249.bugfix
 docs/changes/newsfragments/251.misc
+docs/changes/newsfragments/255.bugfix
 docs/images/corrected_ttest.png
 docs/images/final_estimator.png
 docs/images/iris_X.png
 docs/images/iris_df.png
 docs/images/iris_y.png
 docs/images/julearn_logo.png
 docs/images/julearn_logo_calm.png
```

### Comparing `julearn-0.3.2.dev21/pyproject.toml` & `julearn-0.3.2.dev24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev21/tox.ini` & `julearn-0.3.2.dev24/tox.ini`

 * *Files identical despite different names*

