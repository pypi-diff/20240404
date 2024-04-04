# Comparing `tmp/effector-0.0.269.tar.gz` & `tmp/effector-0.0.270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/effector/effector/dist/.tmp-ozne8som/effector-0.0.269.tar", last modified: Thu Apr  4 09:13:07 2024, max compression
+gzip compressed data, was "/home/runner/work/effector/effector/dist/.tmp-j2b3aaaq/effector-0.0.270.tar", last modified: Thu Apr  4 09:16:42 2024, max compression
```

## Comparing `effector-0.0.269.tar` & `effector-0.0.270.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-04 09:12:58.000000 effector-0.0.269/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 09:12:58.000000 effector-0.0.269/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 09:12:58.000000 effector-0.0.269/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-04 09:12:58.000000 effector-0.0.269/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 09:12:58.000000 effector-0.0.269/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-04 09:13:07.000000 effector-0.0.269/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-04 09:12:58.000000 effector-0.0.269/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/Bike-Sharing-Dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-04 09:12:58.000000 effector-0.0.269/data/Bike-Sharing-Dataset/Readme.txt
--rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-04-04 09:12:58.000000 effector-0.0.269/data/Bike-Sharing-Dataset/day.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1156736 2024-04-04 09:12:58.000000 effector-0.0.269/data/Bike-Sharing-Dataset/hour.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/California-Housing/
--rw-r--r--   0 runner    (1001) docker     (127)  1423529 2024-04-04 09:12:58.000000 effector-0.0.269/data/California-Housing/housing.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/Diabetes-Dataset/
--rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-04-04 09:12:58.000000 effector-0.0.269/data/Diabetes-Dataset/diabetes.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/cervical-cancer/
--rw-r--r--   0 runner    (1001) docker     (127)   102059 2024-04-04 09:12:58.000000 effector-0.0.269/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/data/titanic/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-04 09:12:58.000000 effector-0.0.269/data/titanic/gender_submission.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-04-04 09:12:58.000000 effector-0.0.269/data/titanic/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61194 2024-04-04 09:12:58.000000 effector-0.0.269/data/titanic/train.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 09:12:58.000000 effector-0.0.269/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/Guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/Guides/wrap_models.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/
--rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    74048 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   104555 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/
--rw-r--r--   0 runner    (1001) docker     (127)    28642 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/
--rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    85909 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    25706 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    15115 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31929 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    25683 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    82693 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    93083 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    78989 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    70340 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27158 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    93033 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    61147 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    61778 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23713 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25432 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    41075 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/
--rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    95212 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    45458 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    63502 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    64573 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    61231 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    77057 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    33786 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    44470 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    48588 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18315 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24421 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    27083 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24762 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/global_effect_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/regional_effect_intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)    25907 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    98424 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_rhale.png
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png
--rw-r--r--   0 runner    (1001) docker     (127)   100395 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_weekends.png
--rw-r--r--   0 runner    (1001) docker     (127)    73994 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_workingdays.png
--rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_weekends.png
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_workingdays.png
--rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_black_box.png
--rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)    89602 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_global_effect_feat_1_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    57999 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)   132369 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/effector_intro.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark-white.png
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark.png
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-04 09:12:58.000000 effector-0.0.269/docs/docs/static/github-mark.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/docs/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 09:12:58.000000 effector-0.0.269/docs/javascript/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-04 09:12:58.000000 effector-0.0.269/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/effector/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 09:12:58.000000 effector-0.0.269/effector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-04 09:12:58.000000 effector-0.0.269/effector/bin_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-04 09:12:58.000000 effector-0.0.269/effector/binning_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect_ale.py
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-04 09:12:58.000000 effector-0.0.269/effector/global_effect_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-04 09:12:58.000000 effector-0.0.269/effector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-04 09:12:58.000000 effector-0.0.269/effector/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-04-04 09:12:58.000000 effector-0.0.269/effector/partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect_ale.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-04 09:12:58.000000 effector-0.0.269/effector/regional_effect_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-04-04 09:12:58.000000 effector-0.0.269/effector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-04 09:12:58.000000 effector-0.0.269/effector/utils_integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-04 09:12:58.000000 effector-0.0.269/effector/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 09:13:07.000000 effector-0.0.269/effector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 09:12:58.000000 effector-0.0.269/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/real-examples/
--rw-r--r--   0 runner    (1001) docker     (127)   427021 2024-04-04 09:12:58.000000 effector-0.0.269/real-examples/01_bike_sharing_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 09:12:58.000000 effector-0.0.269/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 09:12:58.000000 effector-0.0.269/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:13:07.000000 effector-0.0.269/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/synthetic-examples/
--rw-r--r--   0 runner    (1001) docker     (127)   753343 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/01_linear_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   791350 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/02_global_effect_methods_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1081136 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/03_regional_effects_synthetic_f.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1437013 2024-04-04 09:12:58.000000 effector-0.0.269/synthetic-examples/04_regional_effects_real_f.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:13:07.000000 effector-0.0.269/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:12:58.000000 effector-0.0.269/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_functional_gam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_functional_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_regional_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-04 09:12:58.000000 effector-0.0.269/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-04 09:16:35.000000 effector-0.0.270/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 09:16:35.000000 effector-0.0.270/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 09:16:35.000000 effector-0.0.270/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-04 09:16:35.000000 effector-0.0.270/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 09:16:35.000000 effector-0.0.270/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-04 09:16:42.000000 effector-0.0.270/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-04 09:16:35.000000 effector-0.0.270/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/data/Bike-Sharing-Dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-04 09:16:35.000000 effector-0.0.270/data/Bike-Sharing-Dataset/Readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-04-04 09:16:35.000000 effector-0.0.270/data/Bike-Sharing-Dataset/day.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1156736 2024-04-04 09:16:35.000000 effector-0.0.270/data/Bike-Sharing-Dataset/hour.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/data/California-Housing/
+-rw-r--r--   0 runner    (1001) docker     (127)  1423529 2024-04-04 09:16:35.000000 effector-0.0.270/data/California-Housing/housing.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/data/Diabetes-Dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-04-04 09:16:35.000000 effector-0.0.270/data/Diabetes-Dataset/diabetes.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/data/cervical-cancer/
+-rw-r--r--   0 runner    (1001) docker     (127)   102059 2024-04-04 09:16:35.000000 effector-0.0.270/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/data/titanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-04 09:16:35.000000 effector-0.0.270/data/titanic/gender_submission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-04-04 09:16:35.000000 effector-0.0.270/data/titanic/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61194 2024-04-04 09:16:35.000000 effector-0.0.270/data/titanic/train.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 09:16:35.000000 effector-0.0.270/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/Guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/Guides/wrap_models.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74048 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   104555 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    28642 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85909 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25706 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15115 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31929 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25683 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82693 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93083 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78989 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70340 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27158 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93033 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61147 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61778 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23713 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25432 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41075 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95212 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45458 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63502 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64573 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61231 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77057 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33786 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44470 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48588 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18315 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24421 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27083 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24762 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/global_effect_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/regional_effect_intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    25907 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_global_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98424 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_global_rhale.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100395 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_regional_pdp_weekends.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73994 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_regional_pdp_workingdays.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_regional_rhale_weekends.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/bike_sharing_regional_rhale_workingdays.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/concept_example_black_box.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/concept_example_dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89602 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/concept_example_global_effect_feat_1_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57999 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)   132369 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/effector_intro.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/github-mark-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/github-mark-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/github-mark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-04 09:16:35.000000 effector-0.0.270/docs/docs/static/github-mark.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/docs/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 09:16:35.000000 effector-0.0.270/docs/javascript/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-04 09:16:35.000000 effector-0.0.270/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/effector/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 09:16:35.000000 effector-0.0.270/effector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-04 09:16:35.000000 effector-0.0.270/effector/bin_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-04 09:16:35.000000 effector-0.0.270/effector/binning_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-04 09:16:35.000000 effector-0.0.270/effector/global_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-04 09:16:35.000000 effector-0.0.270/effector/global_effect_ale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-04-04 09:16:35.000000 effector-0.0.270/effector/global_effect_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-04 09:16:35.000000 effector-0.0.270/effector/global_effect_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-04 09:16:35.000000 effector-0.0.270/effector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-04 09:16:35.000000 effector-0.0.270/effector/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-04-04 09:16:35.000000 effector-0.0.270/effector/partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-04 09:16:35.000000 effector-0.0.270/effector/regional_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-04-04 09:16:35.000000 effector-0.0.270/effector/regional_effect_ale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-04 09:16:35.000000 effector-0.0.270/effector/regional_effect_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-04 09:16:35.000000 effector-0.0.270/effector/regional_effect_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-04-04 09:16:35.000000 effector-0.0.270/effector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-04 09:16:35.000000 effector-0.0.270/effector/utils_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-04 09:16:35.000000 effector-0.0.270/effector/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/effector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-04 09:16:42.000000 effector-0.0.270/effector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-04 09:16:42.000000 effector-0.0.270/effector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:16:42.000000 effector-0.0.270/effector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 09:16:42.000000 effector-0.0.270/effector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 09:16:42.000000 effector-0.0.270/effector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 09:16:35.000000 effector-0.0.270/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/real-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   427021 2024-04-04 09:16:35.000000 effector-0.0.270/real-examples/01_bike_sharing_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 09:16:35.000000 effector-0.0.270/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 09:16:35.000000 effector-0.0.270/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:16:42.000000 effector-0.0.270/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/synthetic-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   753343 2024-04-04 09:16:35.000000 effector-0.0.270/synthetic-examples/01_linear_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   791350 2024-04-04 09:16:35.000000 effector-0.0.270/synthetic-examples/02_global_effect_methods_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1081136 2024-04-04 09:16:35.000000 effector-0.0.270/synthetic-examples/03_regional_effects_synthetic_f.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1437013 2024-04-04 09:16:35.000000 effector-0.0.270/synthetic-examples/04_regional_effects_real_f.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:42.000000 effector-0.0.270/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:16:35.000000 effector-0.0.270/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-04 09:16:35.000000 effector-0.0.270/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 09:16:35.000000 effector-0.0.270/tests/test_functional_gam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-04 09:16:35.000000 effector-0.0.270/tests/test_functional_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-04 09:16:35.000000 effector-0.0.270/tests/test_regional_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-04 09:16:35.000000 effector-0.0.270/tests/test_unit.py
```

### Comparing `effector-0.0.269/.github/workflows/publish_documentation.yml` & `effector-0.0.270/.github/workflows/publish_documentation.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/.github/workflows/publish_to_pypi.yml` & `effector-0.0.270/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/.gitignore` & `effector-0.0.270/.gitignore`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/LICENSE` & `effector-0.0.270/LICENSE`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/PKG-INFO` & `effector-0.0.270/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effector
-Version: 0.0.269
+Version: 0.0.270
 Summary: A Python library for global and regional effects
 Author-email: Vasilis Gkolemis <ntipakos@gmail.com>
 Maintainer-email: Julia Herbinger <julia.herbinger@gmail.com>, Christos Diou <cdiou@hua.gr>, Giuseppe Casalicchio <giuseppe.casalicchio@gmail.com>
 License: MIT License
 Project-URL: documentation, https://xai-effector.github.io
 Project-URL: source, https://github.com/givasile/effector
 Project-URL: tracker, https://github.com/givasile/effector/issues
```

### Comparing `effector-0.0.269/README.md` & `effector-0.0.270/README.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/Bike-Sharing-Dataset/Readme.txt` & `effector-0.0.270/data/Bike-Sharing-Dataset/Readme.txt`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/Bike-Sharing-Dataset/day.csv` & `effector-0.0.270/data/Bike-Sharing-Dataset/day.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/Bike-Sharing-Dataset/hour.csv` & `effector-0.0.270/data/Bike-Sharing-Dataset/hour.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/California-Housing/housing.csv` & `effector-0.0.270/data/California-Housing/housing.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/Diabetes-Dataset/diabetes.csv` & `effector-0.0.270/data/Diabetes-Dataset/diabetes.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv` & `effector-0.0.270/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/titanic/gender_submission.csv` & `effector-0.0.270/data/titanic/gender_submission.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/titanic/test.csv` & `effector-0.0.270/data/titanic/test.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/data/titanic/train.csv` & `effector-0.0.270/data/titanic/train.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/Guides/wrap_models.md` & `effector-0.0.270/docs/docs/Tutorials/Guides/wrap_models.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png` & `effector-0.0.270/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model.md` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png` & `effector-0.0.270/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/api.md` & `effector-0.0.270/docs/docs/api.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/global_effect_intro.md` & `effector-0.0.270/docs/docs/global_effect_intro.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/index.md` & `effector-0.0.270/docs/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Home
 
-`Effector` is a python package for [global](./global_effect_intro/) and [regional](.regional_effect_intro/) feature effects.
+`Effector` is a python package for [global](./global_effect_intro/) and [regional](./regional_effect_intro/) feature effects.
 
 ## How to use
 
 ???+ success "You need a dataset"
      Must be a `np.ndarray` with shape `(n_samples, n_features)`.
 
 === "Code"
```

### Comparing `effector-0.0.269/docs/docs/references.md` & `effector-0.0.270/docs/docs/references.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/regional_effect_intro.md` & `effector-0.0.270/docs/docs/regional_effect_intro.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_global_pdp.png` & `effector-0.0.270/docs/docs/static/bike_sharing_global_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png` & `effector-0.0.270/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_global_rhale.png` & `effector-0.0.270/docs/docs/static/bike_sharing_global_rhale.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png` & `effector-0.0.270/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_weekends.png` & `effector-0.0.270/docs/docs/static/bike_sharing_regional_pdp_weekends.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_regional_pdp_workingdays.png` & `effector-0.0.270/docs/docs/static/bike_sharing_regional_pdp_workingdays.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_weekends.png` & `effector-0.0.270/docs/docs/static/bike_sharing_regional_rhale_weekends.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/bike_sharing_regional_rhale_workingdays.png` & `effector-0.0.270/docs/docs/static/bike_sharing_regional_rhale_workingdays.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/concept_example_black_box.png` & `effector-0.0.270/docs/docs/static/concept_example_black_box.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/concept_example_dataset.png` & `effector-0.0.270/docs/docs/static/concept_example_dataset.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/concept_example_global_effect_feat_1_pdp.png` & `effector-0.0.270/docs/docs/static/concept_example_global_effect_feat_1_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png` & `effector-0.0.270/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png` & `effector-0.0.270/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/effector_intro.gif` & `effector-0.0.270/docs/docs/static/effector_intro.gif`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/github-mark-white.png` & `effector-0.0.270/docs/docs/static/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/github-mark-white.svg` & `effector-0.0.270/docs/docs/static/github-mark-white.svg`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/github-mark.png` & `effector-0.0.270/docs/docs/static/github-mark.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/docs/static/github-mark.svg` & `effector-0.0.270/docs/docs/static/github-mark.svg`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/docs/mkdocs.yml` & `effector-0.0.270/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/bin_splitting.py` & `effector-0.0.270/effector/bin_splitting.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/binning_methods.py` & `effector-0.0.270/effector/binning_methods.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/global_effect.py` & `effector-0.0.270/effector/global_effect.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/global_effect_ale.py` & `effector-0.0.270/effector/global_effect_ale.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/global_effect_pdp.py` & `effector-0.0.270/effector/global_effect_pdp.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/global_effect_shap.py` & `effector-0.0.270/effector/global_effect_shap.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/helpers.py` & `effector-0.0.270/effector/helpers.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/interaction.py` & `effector-0.0.270/effector/interaction.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/partitioning.py` & `effector-0.0.270/effector/partitioning.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/regional_effect.py` & `effector-0.0.270/effector/regional_effect.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/regional_effect_ale.py` & `effector-0.0.270/effector/regional_effect_ale.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/regional_effect_pdp.py` & `effector-0.0.270/effector/regional_effect_pdp.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/regional_effect_shap.py` & `effector-0.0.270/effector/regional_effect_shap.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/utils.py` & `effector-0.0.270/effector/utils.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/utils_integrate.py` & `effector-0.0.270/effector/utils_integrate.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector/visualization.py` & `effector-0.0.270/effector/visualization.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/effector.egg-info/PKG-INFO` & `effector-0.0.270/effector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effector
-Version: 0.0.269
+Version: 0.0.270
 Summary: A Python library for global and regional effects
 Author-email: Vasilis Gkolemis <ntipakos@gmail.com>
 Maintainer-email: Julia Herbinger <julia.herbinger@gmail.com>, Christos Diou <cdiou@hua.gr>, Giuseppe Casalicchio <giuseppe.casalicchio@gmail.com>
 License: MIT License
 Project-URL: documentation, https://xai-effector.github.io
 Project-URL: source, https://github.com/givasile/effector
 Project-URL: tracker, https://github.com/givasile/effector/issues
```

### Comparing `effector-0.0.269/effector.egg-info/SOURCES.txt` & `effector-0.0.270/effector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/pyproject.toml` & `effector-0.0.270/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     {name = "Julia Herbinger", email = "julia.herbinger@gmail.com"},
     {name = "Christos Diou", email = "cdiou@hua.gr"},
     {name = "Giuseppe Casalicchio", email = "giuseppe.casalicchio@gmail.com"}
 ]
 license = {text = "MIT License"}
 requires-python = ">=3.7"
 keywords = ["explainability", "machine learning", "deep learning", "interpretability", "feature effect"]
-version = "0.0.269"
+version = "0.0.270"
 readme = "README.md"
 dependencies = [
     "matplotlib",
     "numpy",
     "scipy",
     "tqdm",
     "shap"
```

### Comparing `effector-0.0.269/real-examples/01_bike_sharing_dataset.ipynb` & `effector-0.0.270/real-examples/01_bike_sharing_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/synthetic-examples/01_linear_model.ipynb` & `effector-0.0.270/synthetic-examples/01_linear_model.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/synthetic-examples/02_global_effect_methods_comparison.ipynb` & `effector-0.0.270/synthetic-examples/02_global_effect_methods_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/synthetic-examples/03_regional_effects_synthetic_f.ipynb` & `effector-0.0.270/synthetic-examples/03_regional_effects_synthetic_f.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/synthetic-examples/04_regional_effects_real_f.ipynb` & `effector-0.0.270/synthetic-examples/04_regional_effects_real_f.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/tests/test_functional.py` & `effector-0.0.270/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/tests/test_functional_gam.py` & `effector-0.0.270/tests/test_functional_gam.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/tests/test_functional_linear.py` & `effector-0.0.270/tests/test_functional_linear.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/tests/test_regional_methods.py` & `effector-0.0.270/tests/test_regional_methods.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.269/tests/test_unit.py` & `effector-0.0.270/tests/test_unit.py`

 * *Files identical despite different names*

