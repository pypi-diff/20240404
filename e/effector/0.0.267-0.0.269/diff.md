# Comparing `tmp/effector-0.0.267.tar.gz` & `tmp/effector-0.0.269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/effector/effector/dist/.tmp-cjqkquml/effector-0.0.267.tar", last modified: Fri Mar 29 14:36:14 2024, max compression
+gzip compressed data, was "/home/runner/work/effector/effector/dist/.tmp-ozne8som/effector-0.0.269.tar", last modified: Thu Apr  4 09:13:07 2024, max compression
```

## Comparing `effector-0.0.267.tar` & `effector-0.0.269.tar`

### file list

```diff
@@ -1,220 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-29 14:36:08.000000 effector-0.0.267/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-29 14:36:08.000000 effector-0.0.267/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-29 14:36:08.000000 effector-0.0.267/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-29 14:36:08.000000 effector-0.0.267/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 14:36:08.000000 effector-0.0.267/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-29 14:36:14.000000 effector-0.0.267/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-29 14:36:08.000000 effector-0.0.267/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/data/Bike-Sharing-Dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-03-29 14:36:08.000000 effector-0.0.267/data/Bike-Sharing-Dataset/Readme.txt
--rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-03-29 14:36:08.000000 effector-0.0.267/data/Bike-Sharing-Dataset/day.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1156736 2024-03-29 14:36:08.000000 effector-0.0.267/data/Bike-Sharing-Dataset/hour.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/data/California-Housing/
--rw-r--r--   0 runner    (1001) docker     (127)  1423529 2024-03-29 14:36:08.000000 effector-0.0.267/data/California-Housing/housing.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/data/Diabetes-Dataset/
--rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-03-29 14:36:08.000000 effector-0.0.267/data/Diabetes-Dataset/diabetes.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/data/cervical-cancer/
--rw-r--r--   0 runner    (1001) docker     (127)   102059 2024-03-29 14:36:08.000000 effector-0.0.267/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/data/titanic/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-29 14:36:08.000000 effector-0.0.267/data/titanic/gender_submission.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-03-29 14:36:08.000000 effector-0.0.267/data/titanic/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61194 2024-03-29 14:36:08.000000 effector-0.0.267/data/titanic/train.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-29 14:36:08.000000 effector-0.0.267/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/Guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/Guides/wrap_models.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/
--rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    74048 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   104555 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/
--rw-r--r--   0 runner    (1001) docker     (127)    28642 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/
--rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    85909 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    25706 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    15115 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31929 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    25683 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    82693 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    93083 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    78989 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    70340 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27158 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    93033 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    61147 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    61778 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23713 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25432 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    41075 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/
--rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    95212 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    45458 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    63502 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    64573 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    61231 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    77057 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    33786 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    44470 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    48588 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18315 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24421 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    27083 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24762 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/global_effect_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/regional_effect_intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)    25907 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_global_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    98424 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_global_rhale.png
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png
--rw-r--r--   0 runner    (1001) docker     (127)   100395 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_regional_pdp_weekends.png
--rw-r--r--   0 runner    (1001) docker     (127)    73994 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_regional_pdp_workingdays.png
--rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_regional_rhale_weekends.png
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/bike_sharing_regional_rhale_workingdays.png
--rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/concept_example_black_box.png
--rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/concept_example_dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)    89602 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/concept_example_global_effect_feat_1_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    57999 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)   132369 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/effector_intro.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/github-mark-white.png
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/github-mark-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/github-mark.png
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-29 14:36:08.000000 effector-0.0.267/docs/docs/static/github-mark.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/docs/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-29 14:36:08.000000 effector-0.0.267/docs/javascript/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-29 14:36:08.000000 effector-0.0.267/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/effector/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-29 14:36:08.000000 effector-0.0.267/effector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-03-29 14:36:08.000000 effector-0.0.267/effector/bin_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-29 14:36:08.000000 effector-0.0.267/effector/binning_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-03-29 14:36:08.000000 effector-0.0.267/effector/global_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-03-29 14:36:08.000000 effector-0.0.267/effector/global_effect_ale.py
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-03-29 14:36:08.000000 effector-0.0.267/effector/global_effect_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-03-29 14:36:08.000000 effector-0.0.267/effector/global_effect_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-29 14:36:08.000000 effector-0.0.267/effector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-03-29 14:36:08.000000 effector-0.0.267/effector/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-03-29 14:36:08.000000 effector-0.0.267/effector/partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-03-29 14:36:08.000000 effector-0.0.267/effector/regional_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-03-29 14:36:08.000000 effector-0.0.267/effector/regional_effect_ale.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-29 14:36:08.000000 effector-0.0.267/effector/regional_effect_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-03-29 14:36:08.000000 effector-0.0.267/effector/regional_effect_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-03-29 14:36:08.000000 effector-0.0.267/effector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-29 14:36:08.000000 effector-0.0.267/effector/utils_integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-29 14:36:08.000000 effector-0.0.267/effector/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/effector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-29 14:36:14.000000 effector-0.0.267/effector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-03-29 14:36:14.000000 effector-0.0.267/effector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 14:36:14.000000 effector-0.0.267/effector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-29 14:36:14.000000 effector-0.0.267/effector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 14:36:14.000000 effector-0.0.267/effector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 14:36:08.000000 effector-0.0.267/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/real-examples/
--rw-r--r--   0 runner    (1001) docker     (127)   427021 2024-03-29 14:36:08.000000 effector-0.0.267/real-examples/01_bike_sharing_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-29 14:36:08.000000 effector-0.0.267/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-29 14:36:08.000000 effector-0.0.267/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 14:36:14.000000 effector-0.0.267/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/synthetic-examples/
--rw-r--r--   0 runner    (1001) docker     (127)   753343 2024-03-29 14:36:08.000000 effector-0.0.267/synthetic-examples/01_linear_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   791350 2024-03-29 14:36:08.000000 effector-0.0.267/synthetic-examples/02_global_effect_methods_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1081136 2024-03-29 14:36:08.000000 effector-0.0.267/synthetic-examples/03_regional_effects_synthetic_f.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1437013 2024-03-29 14:36:08.000000 effector-0.0.267/synthetic-examples/04_regional_effects_real_f.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:14.000000 effector-0.0.267/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 14:36:08.000000 effector-0.0.267/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-03-29 14:36:08.000000 effector-0.0.267/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-29 14:36:08.000000 effector-0.0.267/tests/test_functional_gam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-29 14:36:08.000000 effector-0.0.267/tests/test_functional_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-29 14:36:08.000000 effector-0.0.267/tests/test_regional_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-29 14:36:08.000000 effector-0.0.267/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-04 09:12:58.000000 effector-0.0.269/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 09:12:58.000000 effector-0.0.269/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 09:12:58.000000 effector-0.0.269/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-04 09:12:58.000000 effector-0.0.269/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 09:12:58.000000 effector-0.0.269/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-04 09:13:07.000000 effector-0.0.269/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-04 09:12:58.000000 effector-0.0.269/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/Bike-Sharing-Dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-04 09:12:58.000000 effector-0.0.269/data/Bike-Sharing-Dataset/Readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-04-04 09:12:58.000000 effector-0.0.269/data/Bike-Sharing-Dataset/day.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1156736 2024-04-04 09:12:58.000000 effector-0.0.269/data/Bike-Sharing-Dataset/hour.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/California-Housing/
+-rw-r--r--   0 runner    (1001) docker     (127)  1423529 2024-04-04 09:12:58.000000 effector-0.0.269/data/California-Housing/housing.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/Diabetes-Dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-04-04 09:12:58.000000 effector-0.0.269/data/Diabetes-Dataset/diabetes.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/cervical-cancer/
+-rw-r--r--   0 runner    (1001) docker     (127)   102059 2024-04-04 09:12:58.000000 effector-0.0.269/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/titanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-04 09:12:58.000000 effector-0.0.269/data/titanic/gender_submission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-04-04 09:12:58.000000 effector-0.0.269/data/titanic/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61194 2024-04-04 09:12:58.000000 effector-0.0.269/data/titanic/train.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 09:12:58.000000 effector-0.0.269/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/Guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/Guides/wrap_models.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74048 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   104555 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    28642 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85909 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25706 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15115 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31929 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25683 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82693 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93083 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78989 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70340 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27158 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93033 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61147 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61778 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23713 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25432 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41075 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95212 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45458 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63502 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64573 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61231 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77057 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33786 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44470 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48588 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18315 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24421 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27083 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24762 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/global_effect_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/regional_effect_intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    25907 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98424 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_rhale.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100395 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_weekends.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73994 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_workingdays.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_weekends.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_workingdays.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_black_box.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89602 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_global_effect_feat_1_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57999 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)   132369 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/effector_intro.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 09:12:58.000000 effector-0.0.269/docs/javascript/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-04 09:12:58.000000 effector-0.0.269/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/effector/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 09:12:58.000000 effector-0.0.269/effector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-04 09:12:58.000000 effector-0.0.269/effector/bin_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-04 09:12:58.000000 effector-0.0.269/effector/binning_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect_ale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-04 09:12:58.000000 effector-0.0.269/effector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-04 09:12:58.000000 effector-0.0.269/effector/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-04-04 09:12:58.000000 effector-0.0.269/effector/partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect_ale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-04-04 09:12:58.000000 effector-0.0.269/effector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-04 09:12:58.000000 effector-0.0.269/effector/utils_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-04 09:12:58.000000 effector-0.0.269/effector/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 09:12:58.000000 effector-0.0.269/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/real-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   427021 2024-04-04 09:12:58.000000 effector-0.0.269/real-examples/01_bike_sharing_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 09:12:58.000000 effector-0.0.269/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 09:12:58.000000 effector-0.0.269/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:13:07.000000 effector-0.0.269/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/synthetic-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   753343 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/01_linear_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   791350 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/02_global_effect_methods_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1081136 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/03_regional_effects_synthetic_f.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1437013 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/04_regional_effects_real_f.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:12:58.000000 effector-0.0.269/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_functional_gam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_functional_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_regional_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_unit.py
```

### Comparing `effector-0.0.267/.github/workflows/publish_documentation.yml` & `effector-0.0.269/.github/workflows/publish_documentation.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/.github/workflows/publish_to_pypi.yml` & `effector-0.0.269/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/.gitignore` & `effector-0.0.269/.gitignore`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/LICENSE` & `effector-0.0.269/LICENSE`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/PKG-INFO` & `effector-0.0.269/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: effector
-Version: 0.0.267
+Version: 0.0.269
 Summary: A Python library for global and regional effects
 Author-email: Vasilis Gkolemis <ntipakos@gmail.com>
+Maintainer-email: Julia Herbinger <julia.herbinger@gmail.com>, Christos Diou <cdiou@hua.gr>, Giuseppe Casalicchio <giuseppe.casalicchio@gmail.com>
+License: MIT License
 Project-URL: documentation, https://xai-effector.github.io
 Project-URL: source, https://github.com/givasile/effector
 Project-URL: tracker, https://github.com/givasile/effector/issues
 Keywords: explainability,machine learning,deep learning,interpretability,feature effect
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tutorials
```

### Comparing `effector-0.0.267/README.md` & `effector-0.0.269/README.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/Bike-Sharing-Dataset/Readme.txt` & `effector-0.0.269/data/Bike-Sharing-Dataset/Readme.txt`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/Bike-Sharing-Dataset/day.csv` & `effector-0.0.269/data/Bike-Sharing-Dataset/day.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/Bike-Sharing-Dataset/hour.csv` & `effector-0.0.269/data/Bike-Sharing-Dataset/hour.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/California-Housing/housing.csv` & `effector-0.0.269/data/California-Housing/housing.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/Diabetes-Dataset/diabetes.csv` & `effector-0.0.269/data/Diabetes-Dataset/diabetes.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv` & `effector-0.0.269/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/titanic/gender_submission.csv` & `effector-0.0.269/data/titanic/gender_submission.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/titanic/test.csv` & `effector-0.0.269/data/titanic/test.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/data/titanic/train.csv` & `effector-0.0.269/data/titanic/train.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/Guides/wrap_models.md` & `effector-0.0.269/docs/docs/Tutorials/Guides/wrap_models.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png` & `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model.md` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png` & `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/api.md` & `effector-0.0.269/docs/docs/api.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/global_effect_intro.md` & `effector-0.0.269/docs/docs/global_effect_intro.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/index.md` & `effector-0.0.269/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/references.md` & `effector-0.0.269/docs/docs/references.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 ## Cite `Effector`
 
-TODO: Add citation information
+If you find `Effector` useful in your research, please consider citing the following papers:
+
+```bibtex
+@misc{gkolemis2024effector,
+      title={Effector: A Python package for regional explanations}, 
+      author={Vasilis Gkolemis and Christos Diou and Eirini Ntoutsi and Theodore Dalamagas and Bernd Bischl and Julia Herbinger and Giuseppe Casalicchio},
+      year={2024},
+      eprint={2404.02629},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
 
 ## Methods and Publications
 
 - [Friedman, Jerome H. "Greedy function approximation: a gradient boosting machine." Annals of statistics (2001): 1189-1232.](https://projecteuclid.org/euclid.aos/1013203451)
 - [Apley, Daniel W. "Visualizing the effects of predictor variables in black box supervised learning models." arXiv preprint arXiv:1612.08468 (2016).](https://arxiv.org/abs/1612.08468)
 - [Gkolemis, Vasilis, "RHALE: Robust and Heterogeneity-Aware Accumulated Local Effects"](https://ebooks.iospress.nl/doi/10.3233/FAIA230354)
 - [Gkolemis, Vasilis, "DALE: Decomposing Global Feature Effects Based on Feature Interactions"](https://proceedings.mlr.press/v189/gkolemis23a/gkolemis23a.pdf)
```

### Comparing `effector-0.0.267/docs/docs/regional_effect_intro.md` & `effector-0.0.269/docs/docs/regional_effect_intro.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_global_pdp.png` & `effector-0.0.269/docs/docs/static/bike_sharing_global_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png` & `effector-0.0.269/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_global_rhale.png` & `effector-0.0.269/docs/docs/static/bike_sharing_global_rhale.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png` & `effector-0.0.269/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_regional_pdp_weekends.png` & `effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_weekends.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_regional_pdp_workingdays.png` & `effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_workingdays.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_regional_rhale_weekends.png` & `effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_weekends.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/bike_sharing_regional_rhale_workingdays.png` & `effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_workingdays.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/concept_example_black_box.png` & `effector-0.0.269/docs/docs/static/concept_example_black_box.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/concept_example_dataset.png` & `effector-0.0.269/docs/docs/static/concept_example_dataset.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/concept_example_global_effect_feat_1_pdp.png` & `effector-0.0.269/docs/docs/static/concept_example_global_effect_feat_1_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png` & `effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png` & `effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/effector_intro.gif` & `effector-0.0.269/docs/docs/static/effector_intro.gif`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/github-mark-white.png` & `effector-0.0.269/docs/docs/static/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/github-mark-white.svg` & `effector-0.0.269/docs/docs/static/github-mark-white.svg`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/github-mark.png` & `effector-0.0.269/docs/docs/static/github-mark.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/docs/static/github-mark.svg` & `effector-0.0.269/docs/docs/static/github-mark.svg`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/docs/mkdocs.yml` & `effector-0.0.269/docs/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
           - Regional Effect in depth (a): Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
           - Regional Effect in depth (b): Tutorials/synthetic-examples/04_regional_effects_real_f.md
       - Real Datasets:
           - Bike Sharing: Tutorials/real-examples/01_bike_sharing_dataset.md
       - Guides:
           - Wrap black-models in common ML libraries: Tutorials/Guides/wrap_models.md
   - API: api.md
-  - Contributing: contributing.md
   - References: references.md
 
 
 theme:
   name: material
 
   font:
```

### Comparing `effector-0.0.267/effector/bin_splitting.py` & `effector-0.0.269/effector/bin_splitting.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/binning_methods.py` & `effector-0.0.269/effector/binning_methods.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/global_effect.py` & `effector-0.0.269/effector/global_effect.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/global_effect_ale.py` & `effector-0.0.269/effector/global_effect_ale.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/global_effect_pdp.py` & `effector-0.0.269/effector/global_effect_pdp.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/global_effect_shap.py` & `effector-0.0.269/effector/global_effect_shap.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/helpers.py` & `effector-0.0.269/effector/helpers.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/interaction.py` & `effector-0.0.269/effector/interaction.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/partitioning.py` & `effector-0.0.269/effector/partitioning.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/regional_effect.py` & `effector-0.0.269/effector/regional_effect.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/regional_effect_ale.py` & `effector-0.0.269/effector/regional_effect_ale.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/regional_effect_pdp.py` & `effector-0.0.269/effector/regional_effect_pdp.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/regional_effect_shap.py` & `effector-0.0.269/effector/regional_effect_shap.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/utils.py` & `effector-0.0.269/effector/utils.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/utils_integrate.py` & `effector-0.0.269/effector/utils_integrate.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector/visualization.py` & `effector-0.0.269/effector/visualization.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/effector.egg-info/PKG-INFO` & `effector-0.0.269/effector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: effector
-Version: 0.0.267
+Version: 0.0.269
 Summary: A Python library for global and regional effects
 Author-email: Vasilis Gkolemis <ntipakos@gmail.com>
+Maintainer-email: Julia Herbinger <julia.herbinger@gmail.com>, Christos Diou <cdiou@hua.gr>, Giuseppe Casalicchio <giuseppe.casalicchio@gmail.com>
+License: MIT License
 Project-URL: documentation, https://xai-effector.github.io
 Project-URL: source, https://github.com/givasile/effector
 Project-URL: tracker, https://github.com/givasile/effector/issues
 Keywords: explainability,machine learning,deep learning,interpretability,feature effect
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tutorials
```

### Comparing `effector-0.0.267/effector.egg-info/SOURCES.txt` & `effector-0.0.269/effector.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
 data/titanic/gender_submission.csv
 data/titanic/test.csv
 data/titanic/train.csv
 docs/README.md
 docs/mkdocs.yml
 docs/docs/api.md
-docs/docs/contributing.md
 docs/docs/global_effect_intro.md
 docs/docs/index.md
 docs/docs/installation.md
 docs/docs/references.md
 docs/docs/regional_effect_intro.md
 docs/docs/Tutorials/Guides/wrap_models.md
 docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
```

### Comparing `effector-0.0.267/pyproject.toml` & `effector-0.0.269/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 packages = ['effector']
 package-dir = {'effector'='effector'}
 
 [project]
 name = "effector"
 description = "A Python library for global and regional effects"
 authors = [{name = "Vasilis Gkolemis", email = "ntipakos@gmail.com"}]
+maintainers = [
+    {name = "Julia Herbinger", email = "julia.herbinger@gmail.com"},
+    {name = "Christos Diou", email = "cdiou@hua.gr"},
+    {name = "Giuseppe Casalicchio", email = "giuseppe.casalicchio@gmail.com"}
+]
+license = {text = "MIT License"}
 requires-python = ">=3.7"
 keywords = ["explainability", "machine learning", "deep learning", "interpretability", "feature effect"]
-version = "0.0.267"
+version = "0.0.269"
 readme = "README.md"
 dependencies = [
     "matplotlib",
     "numpy",
     "scipy",
     "tqdm",
     "shap"
```

### Comparing `effector-0.0.267/real-examples/01_bike_sharing_dataset.ipynb` & `effector-0.0.269/real-examples/01_bike_sharing_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/synthetic-examples/01_linear_model.ipynb` & `effector-0.0.269/synthetic-examples/01_linear_model.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/synthetic-examples/02_global_effect_methods_comparison.ipynb` & `effector-0.0.269/synthetic-examples/02_global_effect_methods_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/synthetic-examples/03_regional_effects_synthetic_f.ipynb` & `effector-0.0.269/synthetic-examples/03_regional_effects_synthetic_f.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/synthetic-examples/04_regional_effects_real_f.ipynb` & `effector-0.0.269/synthetic-examples/04_regional_effects_real_f.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/tests/test_functional.py` & `effector-0.0.269/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/tests/test_functional_gam.py` & `effector-0.0.269/tests/test_functional_gam.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/tests/test_functional_linear.py` & `effector-0.0.269/tests/test_functional_linear.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/tests/test_regional_methods.py` & `effector-0.0.269/tests/test_regional_methods.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.267/tests/test_unit.py` & `effector-0.0.269/tests/test_unit.py`

 * *Files identical despite different names*

