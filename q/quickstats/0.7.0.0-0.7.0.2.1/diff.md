# Comparing `tmp/quickstats-0.7.0.0.tar.gz` & `tmp/quickstats-0.7.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.0.tar", last modified: Sun Mar 24 13:24:55 2024, max compression
+gzip compressed data, was "quickstats-0.7.0.2.1.tar", last modified: Thu Apr  4 00:49:34 2024, max compression
```

## Comparing `quickstats-0.7.0.0.tar` & `quickstats-0.7.0.2.1.tar`

### file list

```diff
@@ -1,274 +1,280 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.0/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:53.000000 quickstats-0.7.0.0/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.0/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:53.000000 quickstats-0.7.0.0/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      693 2024-03-21 00:25:04.000000 quickstats-0.7.0.0/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2024-03-24 12:50:19.000000 quickstats-0.7.0.0/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:53.000000 quickstats-0.7.0.0/quickstats/algorithms/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.0/quickstats/algorithms/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:53.000000 quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/BaseMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/BisectionMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/NovelMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/SteppingMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10443 2024-03-20 10:40:19.000000 quickstats-0.7.0.0/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41666 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85699 2024-03-20 05:53:50.000000 quickstats-0.7.0.0/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9192 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32693 2024-03-24 12:06:38.000000 quickstats-0.7.0.0/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23980 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/clis/likelihood_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-03-20 05:54:19.000000 quickstats-0.7.0.0/quickstats/clis/nuisance_parameter_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.0/quickstats/clis/processor_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/clis/stat_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.0/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1003 2024-03-24 11:50:51.000000 quickstats-0.7.0.0/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15200 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/caching_nll_wrapper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/discrete_nuisance.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-03-21 22:06:32.000000 quickstats-0.7.0.0/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-03-22 06:53:00.000000 quickstats-0.7.0.0/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14303 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.0/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-03-20 05:53:32.000000 quickstats-0.7.0.0/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-03-20 05:53:33.000000 quickstats-0.7.0.0/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-03-24 11:56:22.000000 quickstats-0.7.0.0/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1417 2024-03-24 12:41:51.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-03-23 11:42:51.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      286 2024-03-24 07:41:44.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/formatter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1152 2024-03-23 11:29:11.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2202 2024-03-24 09:53:39.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_as_hdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1870 2024-03-24 09:53:36.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1479 2024-03-24 09:53:33.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_as_parquet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 21:34:35.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_awkward_array.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3684 2024-03-24 12:44:35.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-03-23 11:32:05.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      951 2024-03-23 11:31:01.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-03-24 12:37:44.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1245 2024-03-23 11:35:28.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-03-23 11:30:06.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-03-23 11:33:46.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-03-23 11:33:27.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-03-23 11:35:50.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-03-23 11:32:55.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:21.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-03-23 11:43:26.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:23.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2919 2024-03-24 09:15:48.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_output_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-03-24 11:10:08.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_progressbar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-03-23 11:36:26.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1751 2024-03-24 12:35:52.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1466 2024-03-23 11:30:31.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-03-23 11:36:37.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2208 2024-03-24 09:53:22.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-23 11:32:35.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:18.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-03-23 11:35:43.000000 quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-03-21 10:53:35.000000 quickstats-0.7.0.0/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9214 2024-03-24 12:10:07.000000 quickstats-0.7.0.0/quickstats/components/processors/roo_process_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7771 2024-03-24 11:55:10.000000 quickstats-0.7.0.0/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2985 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-03-22 11:17:26.000000 quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.0/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.0/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5291 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10858 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.0/quickstats/concurrent/parameterised_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7544 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/concurrent/parameterised_significance.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      438 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20586 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4838 2024-03-20 21:26:04.000000 quickstats-0.7.0.0/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7523 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7566 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6971 2024-03-22 08:43:44.000000 quickstats-0.7.0.0/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-03-23 10:27:07.000000 quickstats-0.7.0.0/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/extensions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/extensions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/extensions/extension_dataframe.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.7.0.0/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.7.0.0/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/interface/cppyy/basic_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.0/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.0/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/ModelConfig.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8814 2024-03-23 12:52:37.000000 quickstats-0.7.0.0/quickstats/interface/root/RDataFrame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/RooAbsArg.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.0/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.0/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.0/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-03-21 09:25:52.000000 quickstats-0.7.0.0/quickstats/interface/root/TChain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5213 2024-03-22 06:57:02.000000 quickstats-0.7.0.0/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5747 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/TH3.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-03-23 12:51:24.000000 quickstats-0.7.0.0/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      656 2024-03-22 00:45:22.000000 quickstats-0.7.0.0/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.0/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.0/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.0/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:53.000000 quickstats-0.7.0.0/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/QStringUtils.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-03-22 22:59:46.000000 quickstats-0.7.0.0/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.0/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.0/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6638 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    39416 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.0/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:54.000000 quickstats-0.7.0.0/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.0/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/parsers/param_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/parsers/roo_param_setup_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15670 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14143 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.0/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3311 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7671 2024-03-20 05:53:37.000000 quickstats-0.7.0.0/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4078 2024-03-23 07:31:01.000000 quickstats-0.7.0.0/quickstats/plots/general_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22373 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17020 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.7.0.0/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25852 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10391 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28865 2024-03-20 05:54:19.000000 quickstats-0.7.0.0/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.7.0.0/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/two_axis_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10197 2024-03-20 05:54:19.000000 quickstats-0.7.0.0/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19306 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/upper_limit_2D_plot_deprecated.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13196 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23332 2024-03-20 05:53:38.000000 quickstats-0.7.0.0/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31327 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/resources/default_workspace_extensions.json
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/quickstats/resources/mpl_stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/resources/mpl_stylesheets/hep.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/resources/mpl_stylesheets/science.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.0/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16849 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.0/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17876 2024-03-24 09:23:38.000000 quickstats-0.7.0.0/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.0/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      538 2024-03-20 21:44:44.000000 quickstats-0.7.0.0/quickstats/utils/path_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      421 2024-03-23 12:02:00.000000 quickstats-0.7.0.0/quickstats/utils/py_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27148 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14094 2024-03-24 08:17:19.000000 quickstats-0.7.0.0/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10233 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1440 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/utils/sys_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15006 2024-03-20 05:53:39.000000 quickstats-0.7.0.0/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-03-24 13:24:53.000000 quickstats-0.7.0.0/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-03-24 13:24:51.000000 quickstats-0.7.0.0/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10517 2024-03-24 13:24:52.000000 quickstats-0.7.0.0/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-03-24 13:24:51.000000 quickstats-0.7.0.0/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-03-24 13:24:51.000000 quickstats-0.7.0.0/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-03-24 13:24:51.000000 quickstats-0.7.0.0/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-03-24 13:24:55.000000 quickstats-0.7.0.0/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-03-22 21:08:00.000000 quickstats-0.7.0.0/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.1/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:11.000000 quickstats-0.7.0.2.1/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.1/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:11.000000 quickstats-0.7.0.2.1/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-02 17:25:02.000000 quickstats-0.7.0.2.1/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       26 2024-04-04 00:47:52.000000 quickstats-0.7.0.2.1/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:12.000000 quickstats-0.7.0.2.1/quickstats/algorithms/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.1/quickstats/algorithms/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:12.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/BaseMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/BisectionMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/NovelMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/SteppingMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:14.000000 quickstats-0.7.0.2.1/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-02 17:36:56.000000 quickstats-0.7.0.2.1/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9725 2024-04-02 18:33:01.000000 quickstats-0.7.0.2.1/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21556 2024-04-03 08:27:44.000000 quickstats-0.7.0.2.1/quickstats/analysis/config_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41208 2024-04-02 22:44:19.000000 quickstats-0.7.0.2.1/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85738 2024-04-02 23:14:17.000000 quickstats-0.7.0.2.1/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9238 2024-04-02 22:05:57.000000 quickstats-0.7.0.2.1/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31730 2024-04-02 17:50:16.000000 quickstats-0.7.0.2.1/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:14.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:15.000000 quickstats-0.7.0.2.1/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23980 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/likelihood_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/clis/nuisance_parameter_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/processor_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/clis/stat_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:18.000000 quickstats-0.7.0.2.1/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1003 2024-03-24 11:50:51.000000 quickstats-0.7.0.2.1/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15200 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/caching_nll_wrapper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/discrete_nuisance.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-03-22 06:53:00.000000 quickstats-0.7.0.2.1/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14303 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:20.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:20.000000 quickstats-0.7.0.2.1/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-03-24 11:56:22.000000 quickstats-0.7.0.2.1/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:24.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1417 2024-03-24 12:41:51.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-03-23 11:42:51.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      286 2024-03-24 07:41:44.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/formatter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1152 2024-03-23 11:29:11.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2202 2024-03-24 09:53:39.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_hdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1870 2024-03-24 09:53:36.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1479 2024-03-24 09:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_parquet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 21:34:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_awkward_array.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3684 2024-03-24 12:44:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-03-23 11:32:05.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      951 2024-03-23 11:31:01.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-03-24 12:37:44.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1245 2024-03-23 11:35:28.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-03-23 11:30:06.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-03-23 11:33:46.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-03-23 11:33:27.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-03-23 11:35:50.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-03-23 11:32:55.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:21.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-03-23 11:43:26.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:23.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2919 2024-03-24 09:15:48.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_output_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-03-24 11:10:08.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_progressbar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-03-23 11:36:26.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1751 2024-03-24 12:35:52.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1466 2024-03-23 11:30:31.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-03-23 11:36:37.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2208 2024-03-24 09:53:22.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-23 11:32:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:18.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-03-23 11:35:43.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-03-21 10:53:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9214 2024-03-24 12:10:07.000000 quickstats-0.7.0.2.1/quickstats/components/processors/roo_process_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10075 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:24.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-03-22 11:17:26.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:25.000000 quickstats-0.7.0.2.1/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.2.1/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5291 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10858 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7544 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_significance.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:27.000000 quickstats-0.7.0.2.1/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      412 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32263 2024-04-03 08:15:13.000000 quickstats-0.7.0.2.1/quickstats/core/configurations.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/constraints.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4325 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7523 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7707 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-02 20:40:30.000000 quickstats-0.7.0.2.1/quickstats/core/metaclasses.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7290 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/setup.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-03 08:23:27.000000 quickstats-0.7.0.2.1/quickstats/core/type_validation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-03-23 10:27:07.000000 quickstats-0.7.0.2.1/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:27.000000 quickstats-0.7.0.2.1/quickstats/extensions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/extensions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/extensions/extension_dataframe.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:27.000000 quickstats-0.7.0.2.1/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-25 07:40:31.000000 quickstats-0.7.0.2.1/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:28.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/basic_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/ModelConfig.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8814 2024-03-23 12:52:37.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RDataFrame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsArg.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-03-21 09:25:52.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TChain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8389 2024-03-26 09:52:30.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5747 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TH3.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-03-23 12:51:24.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      656 2024-03-22 00:45:22.000000 quickstats-0.7.0.2.1/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.2.1/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.2.1/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       61 2024-03-25 07:59:30.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      386 2024-03-26 07:09:55.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      421 2024-03-25 07:29:55.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/utils.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:11.000000 quickstats-0.7.0.2.1/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-03-22 22:59:46.000000 quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:30.000000 quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:30.000000 quickstats-0.7.0.2.1/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.2.1/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6638 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    39416 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.2.1/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:30.000000 quickstats-0.7.0.2.1/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.2.1/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/parsers/param_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/parsers/roo_param_setup_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:32.000000 quickstats-0.7.0.2.1/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15928 2024-03-26 14:28:15.000000 quickstats-0.7.0.2.1/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14143 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.2.1/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-03-26 13:58:38.000000 quickstats-0.7.0.2.1/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7671 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4078 2024-03-23 07:31:01.000000 quickstats-0.7.0.2.1/quickstats/plots/general_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22373 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17020 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.7.0.2.1/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25852 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10391 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28865 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.7.0.2.1/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/two_axis_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10197 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19306 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot_deprecated.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13196 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23332 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31327 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:32.000000 quickstats-0.7.0.2.1/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/default_workspace_extensions.json
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:33.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/hep.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/science.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.2.1/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17249 2024-04-03 00:26:22.000000 quickstats-0.7.0.2.1/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.2.1/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18636 2024-04-02 22:21:53.000000 quickstats-0.7.0.2.1/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.2.1/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2891 2024-03-26 09:43:05.000000 quickstats-0.7.0.2.1/quickstats/utils/path_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-03-27 12:33:54.000000 quickstats-0.7.0.2.1/quickstats/utils/py_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27148 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14094 2024-03-24 08:17:19.000000 quickstats-0.7.0.2.1/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13830 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1440 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/utils/sys_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-02 23:53:41.000000 quickstats-0.7.0.2.1/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:12.000000 quickstats-0.7.0.2.1/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-04-04 00:49:04.000000 quickstats-0.7.0.2.1/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10677 2024-04-04 00:49:07.000000 quickstats-0.7.0.2.1/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-04-04 00:49:04.000000 quickstats-0.7.0.2.1/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-04-04 00:49:05.000000 quickstats-0.7.0.2.1/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-04-04 00:49:05.000000 quickstats-0.7.0.2.1/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-03-22 21:08:00.000000 quickstats-0.7.0.2.1/setup.py
```

### Comparing `quickstats-0.7.0.0/PKG-INFO` & `quickstats-0.7.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.0
+Version: 0.7.0.2.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.0/README.md` & `quickstats-0.7.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/algorithms/nll_crossing/BaseMethod.py` & `quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/BaseMethod.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/analysis_base.py` & `quickstats-0.7.0.2.1/quickstats/analysis/analysis_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from typing import Dict, List, Optional, Union, Tuple
 import os
 import copy
 import json
 
-from quickstats import ConfigurableObject, ConfigComponent
+from quickstats import ConfigurableObject, ConfigComponent, ConfigUnit
 
 from .analysis_path_manager import AnalysisPathManager
-from .config_format_templates import DEFAULT_ANALYSIS_CONFIG_FORMAT
+from .config_templates import AnalysisConfig
 
 class AnalysisBase(ConfigurableObject):
     
-    CONFIG_FORMAT = DEFAULT_ANALYSIS_CONFIG_FORMAT
-    
-    REQUIRED_CONFIG_COMPONENTS = []
+    config : ConfigUnit(AnalysisConfig)
     
     @property
     def names(self) -> Dict[str, str]:
         try:
             names = self.config["names"]
         except Exception:
             names = {}
@@ -25,19 +23,17 @@
     def __init__(self, analysis_config:Optional[Union[Dict, str]]=None,
                  plot_config:Optional[Union[Dict, str]]=None,
                  outdir:Optional[str]=None,
                  ntuple_dir:Optional[str]=None,
                  array_dir:Optional[str]=None,
                  model_dir:Optional[str]=None,
                  path_manager:Optional[AnalysisPathManager]=None,
-                 disable_config_message:bool=False,
                  verbosity:Optional[Union[int, str]]="INFO"):
         
-        super().__init__(disable_config_message=disable_config_message,
-                         verbosity=verbosity)
+        super().__init__(verbosity=verbosity)
         
         if path_manager is None:
             self.path_manager = AnalysisPathManager()
         else:
             self.path_manager = path_manager
         
         self.load_analysis_config(analysis_config)
@@ -58,19 +54,15 @@
                 continue
             # already defined in path manager
             if (dirname == "outdir") and (self.path_manager.base_path is not None):
                 continue
             elif (dirname.replace("_dir", "") in self.path_manager.directories):
                 continue
             # use path defined in config file
-            try:
-                paths[dirname] = self.config["paths"][config_key]
-            # use path defined in the default config format
-            except Exception:
-                paths[dirname] = DEFAULT_ANALYSIS_CONFIG_FORMAT["paths"][config_key].default
+            paths[dirname] = self.config["paths"][config_key]
             
         # setup file paths used in the analysis pipeline
         self.update_paths(**paths)
                                         
     def update_paths(self, outdir:Optional[str]=None,
                      directories:Optional[Dict[str, str]]=None,
                      files:Optional[Dict[str, Union[str, Tuple[Optional[str], str]]]]=None,
@@ -125,18 +117,16 @@
         
     def load_analysis_config(self, config_source:Optional[Union[Dict, str]]=None):
         if isinstance(config_source, str):
             if not os.path.exists(config_source):
                 raise FileNotFoundError(f'config file "{config_source}" does not exist')
             config_path = os.path.abspath(config_source)
             self.path_manager.set_file("analysis_config", config_path)
-        if config_source is None:
-            self.load_config({})
-        else:
-            self.load_config(config_source)
+        if config_source is not None:
+            self.config.load(config_source)
         try:
             self.all_channels = list(self.config['channels'])
         except Exception:
             self.all_channels = []
         try:
             self.all_kinematic_regions = list(self.config['kinematic_regions'])
         except Exception:
@@ -149,18 +139,15 @@
             self.extra_samples = list(self.config['samples']['extra'])
         except Exception:
             self.extra_samples = []            
         try:
             self.all_variables = list(self.config['variables']['all'])
         except Exception:
             self.all_variables = []
-        try:
-            self.treename = self.config['names']['tree_name']
-        except Exception:
-            self.treename = self.DEFAULT_CONFIG_FORMAT["names"]["tree_name"].default
+        self.treename = self.config['names']['tree_name']
         
     def load_plot_config(self, config_source:Optional[Union[Dict, str]]=None):
         if isinstance(config_source, str):
             if not os.path.exists(config_source):
                 raise FileNotFoundError(f'config file "{config_source}" does not exist')
             config_path = os.path.abspath(config_source)
             self.path_manager.set_file("plot_config", config_path)
@@ -220,19 +207,15 @@
                 if sample not in resolved_class_labels:
                     resolved_class_labels[sample] = label
                 else:
                     raise RuntimeError(f"multiple class labels found for the sample \"{sample}\"")
         return resolved_class_labels
     
     def get_analysis_data_format(self):
-        try:
-            fmt = self.config["data_storage"]["analysis_data_arrays"]["storage_format"]
-        except Exception:
-            fmt = self.CONFIG_FORMAT["data_storage"]["analysis_data_arrays"]["storage_format"]
-        return fmt
+        return self.config["data_storage"]["analysis_data_arrays"]["storage_format"]
     
     def get_event_index_variable(self):
         if "event_number" not in self.names:
             raise RuntimeError('no event index variable defined')
         index_variable = self.names["event_number"]
         return index_variable
```

### Comparing `quickstats-0.7.0.0/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.7.0.2.1/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/data_loading.py` & `quickstats-0.7.0.2.1/quickstats/analysis/data_loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-from typing import List, Dict, Union, Optional
+from typing import List, Dict, Union, Optional, Any
 import os
 from itertools import chain
 from dataclasses import dataclass
 
 import pandas as pd
 import numpy as np
 
-from quickstats import (semistaticmethod, DescriptiveEnum, DataclassObject,
-                        ConfigComponent, ConfigurableObject)
+from quickstats import (semistaticmethod, DescriptiveEnum,
+                        ConfigComponent, ConfigurableObject,
+                        ConfigScheme, ConfigUnit)
 from quickstats.utils.common_utils import combine_dict
+from .config_templates import AnalysisConfig, AnalysisTrainingConfig
 from .analysis_base import AnalysisBase
 from .data_preprocessing import fix_negative_weights, shuffle_arrays, get_class_label_encodings
 
-@dataclass
-class SampleTransformation(DataclassObject):
-    normalize_weight: bool = False
-
-@dataclass
-class DatasetTransformation(DataclassObject):
-    scale_weight_by_mean: bool = False
-    negative_weight_mode: int = 0
-    random_state: int = None 
+class DataTransformer(ConfigurableObject):
 
-class DataTransformer(object):
+    config : ConfigUnit(AnalysisTrainingConfig,
+                        ["sample_transformation",
+                         "dataset_transformation"])
     
     def __init__(self, sample_weight_scales:Optional[Dict]=None,
-                 sample_transformation:Optional[Dict]=None,
-                 dataset_transformation:Optional[Dict]=None,
                  **kwargs):
+        super().__init__(**kwargs)
         self.set_sample_weight_scales(sample_weight_scales)
-        self.sample_transformation  = SampleTransformation.from_dict(sample_transformation)
-        self.dataset_transformation = DatasetTransformation.from_dict(dataset_transformation)
+        self.sample_transformation  = self.config.sample_transformation
+        self.dataset_transformation = self.config.dataset_transformation
         
     def set_random_state(self, random_state:Optional[int]=-1):
         self.dataset_transformation.random_state = random_state
         
     @semistaticmethod
     def make_copy(self, x:pd.DataFrame, y:pd.DataFrame,
                   weight:Optional[pd.DataFrame]=None):
@@ -95,14 +90,19 @@
     def set_sample_weight_scales(self, sample_weight_scales:Optional[Dict]=None):
         if sample_weight_scales is None:
             self.sample_weight_scales = {}
         else:
             self.sample_weight_scales = combine_dict(sample_weight_scales)
 
 class SplitAlgoBase(ConfigurableObject):
+
+    def __init__(self, source:Dict, **kwargs):
+        super().__init__(**kwargs)
+        self.config.load(source)
+    
     def get_analysis_dataset_names(self) -> List[str]:
         # use the full dataset by default
         return None
         
     def get_extra_variables(self):
         return []
     
@@ -143,35 +143,40 @@
             f"y_{dataset_type}"      : y,
             f"weight_{dataset_type}" : weight,
         }
         if sample_index is not None:
             dataset_split[f"index_{dataset_type}"] = sample_index
         return dataset_split
 
+class KFoldSplitConfig(ConfigScheme):
+    
+    datasets : ConfigComponent(Optional[List[str]], default=None,
+                               description="dataset(s) that should be used in kfold splitting; if none, the "
+                                           "full dataset will be used")
+    
+    index_variable : ConfigComponent(Optional[str], default=None,
+                                     description="the variable used for indexing (to keep track of "
+                                                 "train/val events in each fold); if none, "
+                                                 "no indices will be saved")
+    
+    n_splits : ConfigComponent(int, required=True,
+                               description="number of splits (= number of folds); one of the split "
+                                           "will be used for validation and the rest for training "
+                                           "with each fold rotating the splits")
+    
+    random_state : ConfigComponent(Optional[int], default=-1,
+                                   description="random state for shuffling data in each fold; "
+                                               "if negative, no shuffling will be made; "
+                                               "if None, the global random state instance from "
+                                               "numpy.random will be used (so every shuffle "
+                                               "will give a different result)")
+    
 class KFoldSplitAlgo(SplitAlgoBase):
     
-    CONFIG_FORMAT = {
-        "datasets": ConfigComponent(dtypes=["LIST[STR]", "NONE"], default=None,
-                                    description="dataset(s) that should be used in kfold splitting; if none, the "
-                                                "full dataset will be used"),
-        "index_variable": ConfigComponent(dtypes=["STR", "NONE"], default=None,
-                                          description="the variable used for indexing (to keep track of "
-                                                      "train/val events in each fold); if none, "
-                                                      "no indices will be saved"),
-        "n_splits": ConfigComponent(dtypes="INT", required=True,
-                                    description="number of splits (= number of folds); one of the split "
-                                                "will be used for validation and the rest for training "
-                                                "with each fold rotating the splits"),
-        "random_state": ConfigComponent(dtypes=["INT", "NONE"], default=-1,
-                                        description="random state for shuffling data in each fold; "
-                                                    "if negative, no shuffling will be made; "
-                                                    "if None, the global random state instance from "
-                                                    "numpy.random will be used (so every shuffle "
-                                                    "will give a different result)")
-    }
+    config : ConfigUnit(KFoldSplitConfig)
     
     def get_analysis_dataset_names(self) -> List[str]:
         dataset_config = self.config.get("datasets", None)
         if dataset_config is not None:
             dataset_names = list(dataset_config)
         else:
             dataset_names = None
@@ -231,30 +236,36 @@
                         var_index[sample] = dataset_i[sample]["x"][index_variable].values
             result_i = {}
             for dataset_type, dataset_i, var_index in [("train", train_dataset, train_var_index),
                                                        ("val", val_dataset, val_var_index)]:
                 
                 result_i.update(self.get_dataset_split(data_transformer, dataset_type, dataset_i, var_index))
             yield result_i
+
+class CustomSplitDatasetConfig(ConfigScheme):
+
+    train : ConfigComponent(List[str], required=True,
+                            description="dataset(s) that should be used as the train dataset")
     
-class CustomSplitAlgo(SplitAlgoBase):
+    validation : ConfigComponent(Optional[List[str]], default=None,
+                                 description="dataset(s) that should be used as the validation dataset; "
+                                             "if none, no validation dataset will be loaded")
+    
+    test : ConfigComponent(Optional[List[str]], default=None,
+                           description="dataset(s) that should be used as the test dataset; "
+                                       "if none, no test dataset will be loaded")
     
-    CONFIG_FORMAT = {
-        "datasets": {
-            "train": ConfigComponent(dtypes="LIST[STR]", required=True,
-                                     description="dataset(s) that should be used as the train dataset"),
-            "validation": ConfigComponent(dtypes=["LIST[STR]", "NONE"], default=None,
-                                          description="dataset(s) that should be used as the validation dataset; "
-                                                      "if none, no validation dataset will be loaded"),
-            "test": ConfigComponent(dtypes=["LIST[STR]", "NONE"], default=None,
-                                    description="dataset(s) that should be used as the test dataset; "
-                                                "if none, no test dataset will be loaded")
-        }
-    }
+class CustomSplitConfig(ConfigScheme):
+
+    datasets : ConfigComponent(CustomSplitDatasetConfig)
     
+class CustomSplitAlgo(SplitAlgoBase):
+
+    config : ConfigUnit(CustomSplitConfig)
+
     def get_train_val_test_map(self):
         datasets_config = self.config["datasets"]
         dataset_map = {}
         dataset_map["train"] = list(datasets_config["train"])
         if "validation" in datasets_config:
             dataset_map["val"] = list(datasets_config["validation"])
         if "test" in datasets_config:
@@ -274,38 +285,45 @@
         self.stdout.info(f'         Test dataset: {dataset_map.get("test", None)}', bare=True)
         result = {}
         for dataset_type, dataset_names in dataset_map.items():
             selected_datasets = [analysis_datasets[dataset_name] for dataset_name in dataset_names]
             combined_dataset = self.combine_analysis_datasets(selected_datasets)
             result.update(self.get_dataset_split(data_transformer, dataset_type, combined_dataset))
         return result
+
+class IndexSplitSubConfig(ConfigScheme):
+
+    train : ConfigComponent(Dict, required=True, default_factory=dict,
+                            description="a dictionary containing that maps the sample to the corresponding "
+                                        "selection indices for the train dataset in the form "
+                                        "{<sample_name>: <array of index values>}")
+    
+    validation : ConfigComponent(Optional[Dict], default=None,
+                                 description="a dictionary containing that maps the sample to the corresponding "
+                                             "selection indices for the validation dataset in the form "
+                                             "{<sample_name>: <array of index values>}; if none, no validation "
+                                             "dataset will be loaded")
+    
+    test : ConfigComponent(Optional[Dict], default=None,
+                           description="a dictionary containing that maps the sample to the corresponding "
+                                       "selection indices for the test dataset in the form "
+                                       "{<sample_name>: <array of index values>}; if none, no test "
+                                       "dataset will be loaded")    
     
+class IndexSplitConfig(ConfigScheme):
+
+    indices : ConfigComponent(IndexSplitSubConfig)
+
+    index_variable : ConfigComponent(str, required=True,
+                                     description="the variable used for indexing")
+
 class IndexSplitAlgo(SplitAlgoBase):
     
-    CONFIG_FORMAT = {
-        "indices":{
-            "train": ConfigComponent(dtypes="DICT", required=True,
-                                     description="a dictionary containing that maps the sample to the corresponding "
-                                                 "selection indices for the train dataset in the form "
-                                                 "{<sample_name>: <array of index values>}"),
-            "validation": ConfigComponent(dtypes=["DICT", "NONE"], default=None,
-                                          description="a dictionary containing that maps the sample to the corresponding "
-                                                      "selection indices for the validation dataset in the form "
-                                                      "{<sample_name>: <array of index values>}; if none, no validation "
-                                                      "dataset will be loaded"),
-            "test": ConfigComponent(dtypes=["DICT", "NONE"], default=None,
-                                    description="a dictionary containing that maps the sample to the corresponding "
-                                                "selection indices for the test dataset in the form "
-                                                "{<sample_name>: <array of index values>}; if none, no test "
-                                                "dataset will be loaded"),
-        },
-        "index_variable": ConfigComponent(dtypes="STR", required=True,
-                                          description="the variable used for indexing")
-    }
-
+    config : ConfigUnit(IndexSplitConfig)
+    
     def get_extra_variables(self):
         index_variable = self.config["index_variable"]
         return [index_variable]
     
     def get_split_indices(self):
         split_indices = {}
         split_indices["train"] = self.config["indices"]["train"]
@@ -361,27 +379,31 @@
                     "x": df_selected[train_variables],
                     "y": df_selected[["true_label"]]
                 }
                 if "weight" in df_selected.columns:
                     dataset_i[sample]["weight"] = df_selected[["weight"]]
             result.update(self.get_dataset_split(data_transformer, dataset_type, dataset_i, unique_indices))
         return result
+
+class ManualSplitConfig(ConfigScheme):
+    
+    datasets : ConfigComponent(Optional[List[str]], default=None,
+                               description="dataset(s) that should be used in the manual splitting; if none, the "
+                                           "full dataset will be used")
+    
+    split_func : ConfigComponent(Any, required=True,
+                                 description="A callable with signature (x, y, weight, **kwargs) -> "
+                                             "{<dataset_name>: (x, y, weight)}")
+    
+    extra_variables : ConfigComponent(List[str], default_factory=list,
+                                      description="extra variables needed for the manual split method")
     
 class ManualSplitAlgo(SplitAlgoBase):
     
-    CONFIG_FORMAT = {
-        "datasets": ConfigComponent(dtypes=["LIST[STR]", "NONE"], default=None,
-                                    description="dataset(s) that should be used in the manual splitting; if none, the "
-                                                "full dataset will be used"),
-        "split_func": ConfigComponent(dtypes="ANY", required=True,
-                                      description="A callable with signature (x, y, weight, **kwargs) -> "
-                                                  "{<dataset_name>: (x, y, weight)}"),
-        "extra_variables": ConfigComponent(dtypes="LIST[STR]", default=[],
-                                           description="extra variables needed for the manual split method")     
-    }
+    config = ConfigUnit(ManualSplitConfig)
     
     def get_analysis_dataset_names(self) -> List[str]:
         dataset_config = self.config.get("datasets", None)
         if dataset_config is not None:
             dataset_names = list(dataset_config)
         else:
             dataset_names = None
@@ -421,18 +443,21 @@
         obj = object.__new__(cls)
         obj._value_ = value
         obj.description = description
         obj.split_algo = split_algo
         return obj
     
 class DataLoader(AnalysisBase):
-    
-    REQUIRED_CONFIG_COMPONENTS = ["paths:arrays", "samples:*", "kinematic_regions:*",
-                                  "variables:*", "training:*", "channels:*",
-                                  "names:weight", "names:event_number"]
+
+    config : ConfigUnit(AnalysisConfig,
+                        ["paths", "samples",
+                         "kinematic_regions",
+                         "variables", "training",
+                         "channels", "names",
+                         "data_storage"])
     
     DEFAULT_DATASET_SPLIT_SETUP = {
         "method": "kfold",
         "options": {
             "datasets": None,
             "index_variable": None,
             "n_splits": 5,
@@ -441,19 +466,21 @@
     }
     
     def __init__(self, analysis_config:Union[Dict, str],
                  array_dir:Optional[str]=None,
                  model_dir:Optional[str]=None,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
+        
         super().__init__(analysis_config=analysis_config,
                          array_dir=array_dir,
                          model_dir=model_dir,
                          verbosity=verbosity,
                          **kwargs)
+        
         self.set_data_transformer()
         self.set_split_algo()
         self.data_format = self.get_analysis_data_format()
         self.weight_variable = self.config['names'].get("weight", None)
         sample_weight_scales = self.config.get("rescale_weights", {}).get("data_loading", None)
         self.set_weight_scales(sample_scales=sample_weight_scales)
         
@@ -468,29 +495,22 @@
             self.stdout.info(f'Set luminosity weight scale to {self.lumi_weight_scale}')
         if self.sample_weight_scales is not None:
             for sample, scale_factor in self.sample_weight_scales.items():
                 self.stdout.info(f'Set event weight scale for the sample "{sample}" to {scale_factor}')
 
     def set_data_transformer(self, data_transformer:Optional[DataTransformer]=None):
         if data_transformer is None:
-            train_config = self.config["training"]
-            sample_transformation  = train_config.get("sample_transformation", {})
-            dataset_transformation = train_config.get("dataset_transformation", {})
-            data_transformer = DataTransformer(sample_transformation=sample_transformation,
-                                               dataset_transformation=dataset_transformation)
+            data_transformer = DataTransformer()
+            data_transformer.config.merge(self.config["training"])
         self.data_transformer = data_transformer
         
     def set_split_algo(self, split_algo:Optional[SplitAlgoBase]=None):
         if split_algo is None:
-            try:
-                split_method = self.config["training"]["datasets"]["split_method"]
-                split_options = self.config["training"]["datasets"]["split_options"]
-            except Exception:
-                split_method = self.DEFAULT_DATASET_SPLIT_SETUP["method"]
-                split_options = self.DEFAULT_DATASET_SPLIT_SETUP["options"]
+            split_method = self.config["training"]["datasets"]["split_method"]
+            split_options = self.config["training"]["datasets"]["split_options"]
             split_method = DatasetSplitMethod.parse(split_method)
             split_algo = split_method.split_algo(split_options,
                                                  verbosity=self.stdout.verbosity)
         self.split_algo = split_algo
         
     def set_random_state(self, random_state:Optional[int]=-1):
         self.data_transformer.set_random_state(random_state)
```

### Comparing `quickstats-0.7.0.0/quickstats/analysis/data_preprocessing.py` & `quickstats-0.7.0.2.1/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/event_categorization.py` & `quickstats-0.7.0.2.1/quickstats/analysis/event_categorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Union, List, Dict, Tuple
 import os
 import json
 
 import numpy as np
 import pandas as pd
 
-from quickstats import DescriptiveEnum, Timer
+from quickstats import DescriptiveEnum, ConfigUnit
 from quickstats.maths.statistics import (get_poisson_interval, get_counting_significance,
                                          get_combined_counting_significance)
 from quickstats.utils.common_utils import is_valid_file, combine_dict
 from .data_loading import DataLoader
 from .multi_class_boundary_tree import MultiClassBoundaryTree
 from .data_preprocessing import get_class_label_encodings
+from .config_templates import AnalysisConfig
 
 class CategorizationOutputMode(DescriptiveEnum):
     MINIMAL  = (0, "Save only outputs needed for statistical evaluation")
     MINITREE = (1, "Save minitrees for all test samples")
     ARRAY    = (2, "Save arrays(csv/h5) for all test samples")
     STANDARD = (3, "Save arrays(csv/h5) and minitrees for all test samples")
     FULL     = (4, "Save arrays(csv/h5), histograms and minitrees for all test samples")
@@ -31,20 +32,23 @@
         obj.description = description
         obj.dirname = dirname
         obj.filename = filename
         obj.short_name = short_name
         return obj
 
 class EventCategorization(DataLoader):
-    
-    REQUIRED_CONFIG_COMPONENTS = ["paths:arrays", "paths:model", "paths:output",
-                                  "samples:*", "kinematic_regions:*",
-                                  "variables:*", "training:*", "channels:*",
-                                  "observables:*", "categorization:*",
-                                  "benchmark:*", "names:weight", "names:event_number"]
+
+    config : ConfigUnit(AnalysisConfig,
+                        ["paths", "samples",
+                         "kinematic_regions",
+                         "variables", "training",
+                         "channels", "names",
+                         "observables", "categorization",
+                         "benchmark", "observable",
+                         "data_storage"])
     
     def __init__(self, study_name:str, target_channels:List[str],
                  analysis_config:Optional[Union[Dict, str]]=None,
                  array_dir:Optional[str]=None, outdir:Optional[str]=None,
                  data_preprocessor=None, do_blind:bool=True,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
```

### Comparing `quickstats-0.7.0.0/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.7.0.2.1/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.7.0.2.1/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from typing import Union, List, Optional, Dict
 from itertools import repeat
 import os
 import sys
 import copy
 
-from quickstats import semistaticmethod
+from quickstats import semistaticmethod, ConfigUnit
 from quickstats.utils.common_utils import execute_multi_tasks
 from quickstats.utils.data_conversion import downcast_dataframe
 from quickstats.analysis import AnalysisBase
+from .config_templates import AnalysisConfig
 
 class NTupleConversionTool(AnalysisBase):
-    
-    REQUIRED_CONFIG_COMPONENTS = ["paths:*"]
+
+    config : ConfigUnit(AnalysisConfig,
+                        ["paths",
+                         "names",
+                         "data_storage"])
     
     DEFAULT_COLUMNS = {}
     
     DEFAULT_NTUPLE_SAMPLE_BASENAME = "{sample_name}.root"
     DEFAULT_ARRAY_SAMPLE_BASENAME  = "{sample_name}.{fmt}"
     
     DEFAULT_NTUPLE_SYST_SAMPLE_BASENAME = "{sample_name}_{syst_name}.root"
@@ -27,15 +31,14 @@
                  ntuple_dir:Optional[str]=None,
                  array_dir:Optional[str]=None,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
         super().__init__(analysis_config=analysis_config,
                          ntuple_dir=ntuple_dir,
                          array_dir=array_dir,
-                         disable_config_message=True,
                          verbosity=verbosity,
                          **kwargs)
         self.stdout.info(f'Initialized ntuple directory as "{self.get_directory("ntuple")}".')
         self.stdout.info(f'Initialized array directory as "{self.get_directory("array")}".')
         self.stdout.info(f'Initialized ntuple treename as "{self.treename}".')
         
     @semistaticmethod
@@ -77,15 +80,14 @@
         
         if columns is None:
             columns = copy.deepcopy(self.DEFAULT_COLUMNS)
 
         self.stdout.info(f'Processing file "{filename}"')
 
         #NTupleProcessTool.remove_csv(sample, outdir)
-        
         if library == "quickstats":
             # does not support chunksize
             from quickstats.utils.data_conversion import root2dataframe
             df = root2dataframe(filename, treename, columns=columns,
                                 mode=2, downcast=downcast, library="root",
                                 multithread=False)
             df_iter = [df]
@@ -94,15 +96,14 @@
             _columns = ["noexpand:" + k for k in columns.values()]
             df_iter = root_pandas.read_root(filename, 
                                             key=treename,
                                             columns=_columns,
                                             chunksize=chunksize)
         else:
             raise RuntimeError(f"invalid library: {library}")
-                               
         for i, df in enumerate(df_iter):
             
             if len(df) == 0: 
                 continue            
             
             if library == "root_pandas":
                 df.columns = list(columns)
@@ -129,15 +130,14 @@
             if i == 0:
                 self.stdout.info(f'Saving data array as "{outpath}"')
                 self._save(df, outpath=outpath, fmt=fmt, 
                            mode='w', complevel=complevel)
             else:
                 self._save(df, outpath=outpath, fmt=fmt, 
                            mode='a', complevel=complevel)
-                
             self._finalize(df, **kwargs, sample_name=sample_name, outdir=outdir,
                            fmt=fmt, complevel=complevel, iteration=i)
             
     @semistaticmethod
     def get_ntuple_sample_path(self, sample_name:Dict, dirname:str):
         basename = self.DEFAULT_NTUPLE_SAMPLE_BASENAME.format(sample_name=sample_name)
         return os.path.join(dirname, basename)
```

### Comparing `quickstats-0.7.0.0/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.7.0.2.1/quickstats/analysis/ntuple_process_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 import os
 import glob
 import json
 import math
 
 import numpy as np
 
-from quickstats import ConfigurableObject, semistaticmethod
+from quickstats import semistaticmethod, ConfigurableObject, ConfigUnit
 from quickstats.utils.common_utils import (combine_dict, reindex_dataframe,
                                            filter_dataframe_by_index_values)
 from .analysis_path_manager import AnalysisPathManager
-from .config_format_templates import DEFAULT_SAMPLE_CONFIG_FORMAT
+from .config_templates import SampleConfig
 
 class NTupleProcessTool(ConfigurableObject):
     """ Tool for processing root ntuples
     """
-    
-    CONFIG_FORMAT = DEFAULT_SAMPLE_CONFIG_FORMAT
-    
-    REQUIRED_CONFIG_COMPONENTS = ["sample_dir", "sample_subdir", "samples", "merge_samples"]
+
+    config : ConfigUnit(SampleConfig)
     
     DEFAULT_SAMPLE_OUTNAME             = "{sample_name}_{sample_type}.root"
     DEFAULT_SYST_SAMPLE_OUTNAME        = "{sample_name}_{syst_name}_{syst_var}_{sample_type}.root"
     DEFAULT_MERGED_SAMPLE_OUTNAME      = "{sample_name}.root"
     DEFAULT_MERGED_SYST_SAMPLE_OUTNAME = "{sample_name}_{syst_name}_{syst_var}.root"
     DEFAULT_CUTFLOW_OUTNAME            = "cutflow_{sample_name}_{sample_type}.csv"
     DEFAULT_WEIGHT_OUTNAME             = "yield_{sample_name}_{sample_type}.json"
@@ -65,20 +63,19 @@
                  process_config:Optional[Union["RooProcessConfig", str]]=None,
                  process_flags:Optional[List[str]]=None,
                  cache:bool=True,
                  use_template:bool=False,
                  multithread:bool=True,
                  backend:Optional[str]=None,
                  backend_options:Optional[Dict]=None,
-                 disable_config_message:bool=False,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
         
-        super().__init__(disable_config_message=disable_config_message,
-                         verbosity=verbosity)
+        super().__init__(verbosity=verbosity)
+        
         self.outdir = outdir
         self.path_manager = AnalysisPathManager(base_path=outdir)
         self.path_manager.set_directory("ntuple", "ntuples")
         self.path_manager.set_directory("cutflow", "cutflow")
         
         self.load_sample_config(sample_config)
         
@@ -98,20 +95,15 @@
         
     def load_sample_config(self, config_source:Union[Dict, str]):
         if isinstance(config_source, str):
             if not os.path.exists(config_source):
                 raise FileNotFoundError(f'config file "{config_source}" does not exist')
             config_path = os.path.abspath(config_source)
             self.path_manager.set_file("sample_config", config_path)
-        self.load_config(config_source)
-        
-        if 'systematic_samples' not in self.config:
-            self.config['systematic_samples'] = {}
-        if 'systematics' not in self.config:
-            self.config['systematics'] = {}
+        self.config.load(config_source)
             
         if 'Nominal' in self.sample_config['systematic_samples']:
             raise ValueError('Nominal samples should be placed in the "samples" key '
                              '(instead of "systematic_samples")')
         sample_list = list(self.sample_config['samples'])
         self._syst_theme_list = list(self.sample_config['systematic_samples'])
         for syst_theme in self.syst_theme_list:
@@ -334,29 +326,14 @@
         return [os.path.join(outdir, basename_cutflow), os.path.join(outdir, basename_weight)]  
     
     @semistaticmethod
     def get_merged_cutflow_outpath(self, sample_config:Dict, outdir:str):
         sample_name = sample_config["sample"]
         basename = self.DEFAULT_MERGED_CUTFLOW_OUTNAME.format(sample_name=sample_name)
         return os.path.join(outdir, basename)    
-    
-    @semistaticmethod
-    def get_expanded_paths(self, paths:Union[str, List[str]]):
-        all_paths = []
-        if isinstance(paths, str):
-            paths = [paths]
-        for path in paths:
-            if os.path.isdir(path):
-                subpaths = glob.glob(os.path.join(path, "*.root"))
-            else:
-                subpaths = glob.glob(path)
-            if len(subpaths) == 0:
-                raise RuntimeError(f"no matching samples found for {path}")
-            all_paths.extend(subpaths)
-        return all_paths
                     
     def prerun_process(self, sample_config:Dict):
         pass
     
     def process_syst_samples(self, syst_names:Optional[List[str]]=None,
                              syst_themes:Optional[List[str]]=None,
                              samples:Optional[List[str]]=None,
@@ -374,25 +351,24 @@
                 for sample_type in paths[syst_theme][sample]:
                     sample_paths = paths[syst_theme][sample][sample_type]
                     sample_config = {
                         "name": sample,
                         "path": sample_paths,
                         "type": sample_type
                     }
-                    expended_paths = self.get_expanded_paths(sample_paths)
                     syst_names_by_theme = self.get_syst_names_from_theme(syst_theme)
                     syst_names_by_theme = np.intersect1d(syst_names_by_theme, syst_names)
                     for syst_name in syst_names_by_theme:
                         self.processor.global_variables['sample'] = sample
                         self.processor.global_variables['sample_type'] = sample_type
                         self.processor.global_variables['syst_theme'] = syst_theme
                         self.processor.global_variables['syst_name'] = syst_name
                         self.processor.global_variables['outdir'] = outdir
                         self.prerun_process(sample_config)
-                        self.processor.run(expended_paths)
+                        self.processor.run(sample_paths)
                         self.processor.clear_global_variables()
 
     def process_samples(self, samples:Optional[Union[List[str], str]]=None,
                         sample_types:Optional[Union[List[str], str]]=None):
         if isinstance(samples, str):
             samples = [samples]
         if isinstance(sample_types, str):
@@ -411,20 +387,19 @@
             for sample_type in paths[sample]:
                 sample_paths = paths[sample][sample_type]
                 sample_config = {
                     "name": sample,
                     "path": sample_paths,
                     "type": sample_type
                 }
-                expended_paths = self.get_expanded_paths(sample_paths)
                 self.processor.global_variables['sample'] = sample
                 self.processor.global_variables['sample_type'] = sample_type
                 self.processor.global_variables['outdir'] = outdir
                 self.prerun_process(sample_config)
-                self.processor.run(expended_paths)
+                self.processor.run(sample_paths)
                 self.processor.clear_global_variables()
                 
     def merge_outputs(self, source_path_func:Callable,
                       target_path_func:Callable,
                       merge_func:Callable,
                       outdir:str,
                       samples:Optional[List[str]]=None,
@@ -510,14 +485,16 @@
         import pandas as pd
         if (filename is None) or (not os.path.exists(filename)):
             return df, None
         with open(filename, 'r') as file:
             data = json.load(file)
         cutflow_names = df['name'].values
         yield_values = [data.pop(name, None) for name in cutflow_names]
+        if (None in yield_values) and not (len(set(yield_values)) == 1):
+            self.stdout.warning(f"Missing some cutflow entries from the yield file {filename}")
         if not data:
             return df, yield_values
         extra_cutflow = {}
         extra_yields = {}
         for key, value in data.items():
             if key.startswith("CUTFLOW"):
                 key = key.strip("CUTFLOW").strip()
@@ -596,19 +573,19 @@
     def load_cutflow_report(self, samples:Optional[List[str]]=None):
         import pandas as pd
         samples = self.get_validated_samples(samples, merged=True)
         
         cutflow_dir   = self.path_manager.get_directory("cutflow")
         
         cutflow_report = {}
-        for sample in self.merged_sample_list:
+        for sample in self.merge_sample_map:
             if sample not in samples:
                 continue
             sample_config = {
-                "name": sample
+                "sample": sample
             }
             cutflow_file = self.get_merged_cutflow_outpath(sample_config, cutflow_dir)
             if not os.path.exists(cutflow_file):
                 self.stdout.warning(f'Missing cutflow file for the sample "{sample}".')
                 continue
             df = pd.read_csv(cutflow_file)
             cutflow_report[sample] = df
```

### Comparing `quickstats-0.7.0.0/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.7.0.2.1/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.7.0.2.1/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.7.0.2.1/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.7.0.2.1/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.7.0.2.1/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/core.py` & `quickstats-0.7.0.2.1/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/inspect_rfile.py` & `quickstats-0.7.0.2.1/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/likelihood_tools.py` & `quickstats-0.7.0.2.1/quickstats/clis/likelihood_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/limit_setting.py` & `quickstats-0.7.0.2.1/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/nuisance_parameter_tools.py` & `quickstats-0.7.0.2.1/quickstats/clis/nuisance_parameter_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/processor_tools.py` & `quickstats-0.7.0.2.1/quickstats/clis/processor_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/stat_tools.py` & `quickstats-0.7.0.2.1/quickstats/clis/stat_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/clis/workspace_tools.py` & `quickstats-0.7.0.2.1/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/__init__.py` & `quickstats-0.7.0.2.1/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/analysis_base.py` & `quickstats-0.7.0.2.1/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/analysis_object.py` & `quickstats-0.7.0.2.1/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/asimov_generator.py` & `quickstats-0.7.0.2.1/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/asymptotic_cls.py` & `quickstats-0.7.0.2.1/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/basics.py` & `quickstats-0.7.0.2.1/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/caching_nll_wrapper.py` & `quickstats-0.7.0.2.1/quickstats/components/caching_nll_wrapper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/discrete_nuisance.py` & `quickstats-0.7.0.2.1/quickstats/components/discrete_nuisance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/extended_minimizer.py` & `quickstats-0.7.0.2.1/quickstats/components/extended_minimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 import ROOT
 
 import cppyy
 
 import quickstats
-from quickstats import AbstractObject, Timer
+from quickstats import AbstractObject, timer
 from quickstats.utils.string_utils import split_str
 from quickstats.utils.common_utils import combine_dict
 from quickstats.interface.root import RooArgSet
 from .discrete_nuisance import DiscreteNuisance
 from .caching_nll_wrapper import CachingNLLWrapper
 
 class ExtendedMinimizer(AbstractObject):
@@ -676,20 +676,20 @@
         """Minimization involving discrete nuisances
         """
         status = 0
         
         do_short_combination = self.config['do_short_combination']
         if do_short_combination:
             self.stdout.info('Begin discrete minimization with short combinations.')
-            with Timer() as t:
+            with timer() as t:
                 status = self.robust_minimize(cascade=cascade)
                 self.min_nll = self.get_nll_val()
                 prev_nll = self.min_nll
             self.stdout.info(f'First overall minimization finished in {t.interval:.3f} s.')
-            with Timer() as t:
+            with timer() as t:
                 max_iteration = self.config['max_short_combination_iteration']
                 min_tol = self.config['discrete_min_tol']
                 for i in range(max_iteration):
                     self.stdout.info(f'Current iteration: {i + 1}')
                     status = self.iterative_minimize(cascade=cascade)
                     delta_nll = abs(prev_nll - self.min_nll)
                     self.stdout.info(f'Previous NLL = {prev_nll}, Minimum NLL = {self.min_nll}, Delta NLL = {delta_nll}')
@@ -697,15 +697,15 @@
                         self.stdout.info(f'Delta NLL is within the required tolerence of {min_tol}.')
                         break
                     prev_nll = self.min_nll
                 num_iteration = i + 1
             self.stdout.info(f'Discrete minimization finished in {num_iteration} iterations. Iterations time taken: {t.interval:.3f} s')
         else:
             self.stdout.info('Begin discrete minimization with full combinations.')
-            with Timer() as t:
+            with timer() as t:
                 clean_snapshot = ROOT.RooArgSet()
                 nll_params = self.nll.getParameters(0)
                 nll_params.remove(self.discrete_nuisance.multipdf_cats)
                 nll_params.snapshot(clean_snapshot)
                 #??
                 #min_nll = 10 + nll.getVal()
                 self.multiple_minimize(mode=0, clean_snapshot=clean_snapshot, cascade=cascade)
@@ -719,15 +719,15 @@
             self.stdout.info(f'Discrete minimization finished. Total time taken: {t.interval:.3f} s')
         final_combination = self.discrete_nuisance.get_current_pdf_indices()
         self.stdout.info(f'Final index combination: {list(final_combination)}')
         return status
         
     # taken from https://github.com/cms-analysis/HiggsAnalysis-CombinedLimit/blob/main/src/CascadeMinimizer.cc
     def iterative_minimize(self, cascade:bool=True):
-        with Timer() as t:
+        with timer() as t:
             min_tol = self.config['discrete_min_tol']
             if self.min_nll is None:
                 self.min_nll = self.get_nll_val()
             if abs(self.min_nll - self.get_nll_val()) > min_tol:
                 self.robust_minimize(cascade=cascade)
             nll_params_all = self.nll.getParameters(0)
             all_snapshot = nll_params_all.snapshot()
@@ -815,15 +815,15 @@
 
         self.stdout.info(f'Total number of combinations after filtering contributing indices: {len(combinations)}')
 
         new_discrete_minimum = False
         # skip the best fit case if already done
         i_start = 1 if (mode != 0) else 0
         self.stdout.info(f'Begin fast loop minimization of {len(combinations)} index combinations.')
-        with Timer() as t:
+        with timer() as t:
             fit_counter = 0
             max_deviation = 5
             multipdf_cats = self.discrete_nuisance.multipdf_cats
             # the overhead in this for loop should be way less than the fit time
             for combination in combinations[i_start:]:
                 changed_index = self.discrete_nuisance.set_category_indices(combination)
                 if fit_counter > 0:
```

### Comparing `quickstats-0.7.0.0/quickstats/components/extended_model.py` & `quickstats-0.7.0.2.1/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/extended_rfile.py` & `quickstats-0.7.0.2.1/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/likelihood.py` & `quickstats-0.7.0.2.1/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/modelling/component_source.py` & `quickstats-0.7.0.2.1/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/modelling/data_modelling.py` & `quickstats-0.7.0.2.1/quickstats/components/modelling/data_modelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import uuid
 
 import numpy as np
 
 import ROOT
 
-from quickstats import semistaticmethod, Timer
+from quickstats import semistaticmethod, timer
 from quickstats.components import ROOTObject
 from quickstats.components.modelling import TreeDataSource, PdfFitTool
 from quickstats.utils.common_utils import combine_dict, execute_multi_tasks, in_notebook
 
 class DataModelling(ROOTObject):
     
     _DEFAULT_FIT_OPTION_ = {
@@ -194,15 +194,15 @@
 
     @semistaticmethod
     def _run(self, filename:str, tree_name:str, model_class:Callable, param_templates:Callable,
              fit_options:Dict, plot_options:Optional[Dict]=None, save_summary_as:Optional[str]=None, 
              save_param_as:Optional[str]=None, save_plot_as:Optional[str]=None,
              save_data_as:Optional[str]=None):
         
-        with Timer() as t:
+        with timer() as t:
             canvas = ROOT.TCanvas(uuid.uuid4().hex)
             observable_config = {
                 'name'        : fit_options['observable'],
                 'range'       : fit_options['range'],
                 'n_bins'      : fit_options['n_bins']
             }
             data_source = TreeDataSource(tree_name, filename,
```

### Comparing `quickstats-0.7.0.0/quickstats/components/modelling/model_source.py` & `quickstats-0.7.0.2.1/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.7.0.2.1/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.7.0.2.1/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.7.0.2.1/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import json
 from typing import List, Optional, Union, Dict
 
 import numpy as np
 
 import quickstats
-from quickstats import semistaticmethod, Timer
+from quickstats import semistaticmethod, timer
 from . import AnalysisBase
 from quickstats.utils import root_utils, common_utils, string_utils
 from quickstats.utils.common_utils import combine_dict
 
 import ROOT
 
 class NuisanceParameterRanking(AnalysisBase):
@@ -60,29 +60,29 @@
         nuis_init = nuis.getVal()
         scan_set = ROOT.RooArgSet(nuis)
         
         self.stdout.info(f'Computing error for the NP "{nuis_name}" at {nuis_init}')
         self.stdout.info("Begin minimization")
 
         # evaluate postfit variation
-        with Timer() as t:
+        with timer() as t:
             status = self.minimizer.minimize(scan=1, scan_set=scan_set)
         time_uncond_fit = t.interval
         self.stdout.info(f'Minimization finished. Total time taken: {time_uncond_fit:.3f}s.')
            
         nuis_hat     = nuis.getVal()
         nuis_errhi   = nuis.getErrorHi()
         nuis_errlo   = nuis.getErrorLo()
         if has_poi:
             poi_hat  = self.poi.getVal()
         else:
             poi_hat  = None
         
         # evaluate prefit variation
-        with Timer() as t:
+        with timer() as t:
             all_constraints = self.model.get_all_constraints()
             prefit_variation, _, nuis_nom = self.model.inspect_constrained_nuisance_parameter(nuis, all_constraints)
         time_prefit_variation = t.interval
         self.stdout.info(f'Prefit variation extracted. Total time taken: {time_prefit_variation:.3f}s.')
             
         self.save_snapshot(self.kBestFitSnapshotName)
         
@@ -129,15 +129,15 @@
         return result
     
     def _evaluate_poi_bestfit_with_cond_nuis(self, nuis:"ROOT.RooRealVar", nuis_val:float,
                                              snapshot_names:Optional[List[str]]=None):
         if not isinstance(snapshot_names, list):
             snapshot_names = list(snapshot_names)
         status = -1
-        with Timer() as t:
+        with timer() as t:
             for snapshot_name in snapshot_names:
                 if snapshot_name is not None:
                     self.load_snapshot(snapshot_name)
                 self.poi.setConstant(0)
                 nuis.setVal(nuis_val)
                 nuis.setConstant(1)
                 status = self.minimizer.minimize()
```

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/__init__.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_as_hdf.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_hdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_as_parquet.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_parquet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_output_action.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_output_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_progressbar.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_progressbar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_safe_define.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/builtin_methods.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/roo_process_config.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/roo_process_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/processors/roo_processor.py` & `quickstats-0.7.0.2.1/quickstats/components/processors/roo_processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 import time
 import ROOT
 
 from .builtin_methods import BUILTIN_METHODS
 from .actions import *
 from .roo_process_config import RooProcessConfig
 
-from quickstats import Timer, AbstractObject, PathManager
+from quickstats import timer, AbstractObject, PathManager
 from quickstats.interface.root import TFile, RDataFrame, RDataFrameBackend
-from quickstats.utils.root_utils import declare_expression, close_all_root_files, set_cachedir
+from quickstats.interface.xrootd import get_cachedir, set_cachedir, switch_cachedir
+from quickstats.utils.root_utils import declare_expression, close_all_root_files
+from quickstats.utils.path_utils import is_remote_path
+from quickstats.utils.common_utils import get_cpu_count
 
 class RooProcessor(AbstractObject):
 
     @property
     def distributed(self):
         return self.backend != RDataFrameBackend.DEFAULT
         
     def __init__(self, config_source:Optional[Union[RooProcessConfig, str]]=None,
                  config_text:Optional[str]=None,
                  flags:Optional[List[str]]=None,
                  backend:Optional[str]=None,
                  backend_options:Optional[Dict]=None,
-                 multithread:bool=True,
+                 multithread:int=True,
                  cache:bool=False,
                  use_template:bool=False,
                  verbosity:Optional[Union[int, str]]="INFO"):
         super().__init__(verbosity=verbosity)
         self.cache = cache
         self.action_tree = None
         if flags is not None:
@@ -43,28 +46,46 @@
         self.use_template = use_template
         self.multithread = multithread
         if backend is None:
             self.backend = RDataFrameBackend.DEFAULT
         else:
             self.backend = RDataFrameBackend.parse(backend)
         self.backend_options = backend_options
+        self.set_remote_file_options(localize=False,
+                                     cachedir=get_cachedir())
         
         self.load_buildin_functions()
         
-        if multithread:
-            ROOT.EnableImplicitMT()
+        if multithread:            
+            if multithread > 1:
+                ROOT.EnableImplicitMT(multithread)
+                num_thread = multithread
+            else:
+                ROOT.EnableImplicitMT()
+                num_thread = get_cpu_count()
+            self.stdout.info(f'Enabled multithreading with {num_thread} threads.')
+        elif ROOT.IsImplicitMTEnabled():
+            ROOT.DisableImplicitMT()
         
         if config_source is not None:
             self.load_config(config_source)
             
     def set_cache(self, cache:bool=True):
         self.cache = cache
         
-    def set_remote_cachedir(self, cachedir:Optional[str]=None):
-        self.set_cachedir(cachedir, forcecache=True)
+    def set_remote_file_options(self, localize:bool=False,
+                                cache:bool=True, cachedir:Optional[str]="/tmp",
+                                copy_options:Optional[Dict]=None):
+        remote_file_options = {
+            'localize': localize,
+            'cache': cache,
+            'cachedir': cachedir,
+            'copy_options': copy_options
+        }
+        self.remote_file_options = remote_file_options
             
     def load_buildin_functions(self):
         # bug of redefining module from ROOT
         try:
             import ROOT
             Internal = ROOT.Internal
         except:
@@ -150,41 +171,74 @@
     def sanity_check(self):
         if not self.action_tree:
             raise RuntimeError("action tree not initialized")        
         if not self.action_tree.root_node.has_child:
             self.stdout.warning("No actions to be performed.")
             return None
 
+    @staticmethod
+    def _has_remote_files(filenames:List[str]):
+        return any(is_remote_path(filename) for filename in filenames)
+
+    def list_files(self, filenames:List[str], resolve_cache:bool=True):
+        cachedir = self.remote_file_options['cachedir']
+        with switch_cachedir(cachedir):
+            files = TFile.list_files(filenames, resolve_cache=resolve_cache,
+                                     raise_on_error=False)
+        return files
+
+    def _fetch_remote_files(self, filenames:List[str]):
+        opts = self.remote_file_options
+        copy_options = opts.get('copy_options', None)
+        if copy_options is None:
+            copy_options = {}
+        TFile.fetch_remote_files(filenames, cache=opts['cache'],
+                                 cachedir=opts['cachedir'],
+                                 **copy_options)
+        
     def load_rdataframe(self,
                         filenames:Union[List[str], str],
                         treename:Optional[str]=None):
+        
         if treename is None:
             treename = self.default_treename
+            
         if treename is None:
             raise RuntimeError("treename is undefined")
-        filenames = TFile.list_files(filenames, resolve_cache=True)
+            
+        filenames = self.list_files(filenames, resolve_cache=True)
+        
         if not filenames:
             self.stdout.info('No files to be processed. Skipped.')
             return None
+            
+        has_remote_file = self._has_remote_files(filenames)
+        # copy remote files to local storage
+        if has_remote_file and self.remote_file_options['localize']:
+            remote_files = [filename for filename in filenames if is_remote_path(filename)]
+            self._fetch_remote_files(remote_files)
+            filenames = self.list_files(filenames, resolve_cache=True)
+
         if len(filenames) == 1:
             self.stdout.info(f'Processing file "{filenames[0]}".')
         else:
             self.stdout.info("Professing files")
             for filename in filenames:
                 self.stdout.info(f'  "{filename}"', bare=True)
+                
         rdf = RDataFrame.from_files(filenames, treename=treename,
                                     backend=self.backend,
                                     backend_options=self.backend_options,
                                     multithread_safe=self.multithread)
         self.rdf = rdf
         return self
     
     def run(self, filenames:Optional[Union[List[str], str]]=None):
         self.sanity_check()
-        with Timer() as t:
+        with timer() as t:
             if filenames is not None:
                 self.load_rdataframe(filenames)
             self.action_tree.reset()
             self.run_all_actions()
             self.shallow_cleanup()
         self.stdout.info(f"Task finished. Total time taken: {t.interval:.3f} s.")
         return self
```

### Comparing `quickstats-0.7.0.0/quickstats/components/pvalue_toys.py` & `quickstats-0.7.0.2.1/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/roo_inspector.py` & `quickstats-0.7.0.2.1/quickstats/components/roo_inspector.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import glob
 import json
 import fnmatch
 
 import ROOT
 
-from quickstats import AbstractObject, Timer
+from quickstats import AbstractObject
 from quickstats.interface.root import TChain
 from quickstats.utils.common_utils import str_list_filter
 
 class RooInspector(AbstractObject):
     def __init__(self, treename:str,
                  file_expr:Union[str, List[str]], 
                  filter_expr:Optional[str]=None,
```

### Comparing `quickstats-0.7.0.0/quickstats/components/root_object.py` & `quickstats-0.7.0.2.1/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/toy_limit_calculator.py` & `quickstats-0.7.0.2.1/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/__init__.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/sample.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/settings.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/systematic.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_comparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 import ROOT
 from ROOT.RooPrintable import (kName, kClassName, kValue, kArgs, kExtras, kAddress,
                                kTitle, kCollectionHeader, kSingleLine)
 
 import quickstats
-from quickstats import semistaticmethod, Timer, AbstractObject, GeneralEnum
+from quickstats import semistaticmethod, timer, AbstractObject, GeneralEnum
 from quickstats.components import ExtendedModel
 from quickstats.core.io import get_colored_text, format_comparison_text
 from quickstats.utils.root_utils import load_macro, get_macro_dir
 from quickstats.maths.numerics import is_float, pretty_value
 from quickstats.components.basics import WSArgument
 from quickstats.interface.root.roofit_extension import get_str_data
 
@@ -703,18 +703,18 @@
         
         self.target_items = items
         self.visibility_map = visibility_map
         self.data = {}
 
     def set_targets(self, ws_path_1:str, ws_path_2:str):
         self.stdout.info("Initializing targets...")
-        with Timer() as t:
+        with timer() as t:
             self.model_1 = ExtendedModel(ws_path_1, data_name=None, verbosity="WARNING")
         self.stdout.info(f'Loaded workspace (left) from "{ws_path_1}". Time taken: {t.interval:.3f}s.')
-        with Timer() as t:
+        with timer() as t:
             self.model_2 = ExtendedModel(ws_path_2, data_name=None, verbosity="WARNING")
         self.stdout.info(f'Loaded workspace (right) from "{ws_path_2}". Time taken: {t.interval:.3f}s.')
         
     def _parse_items(self, items:Optional[Union[List[str], List[WSItem], WSItem, str]]=None) -> List[WSItem]:
         if items is None:
             parsed_items = list(self.kDefaultItems)
         elif isinstance(items, str):
@@ -752,15 +752,15 @@
                 if _item not in items:
                     self.stdout.info(f'Added "{_item.title}" to the requested data pool needed for '
                                      'inferring renamed and redefined variables.')
                     items.append(_item)
         
         self.clear_data()
         self.stdout.info("Loading workspace information...")
-        with Timer() as t:
+        with timer() as t:
             for item in items:
                 item_name = item.name.lower()
                 self.data[item_name] = self.get_item_data(item)
         self.stdout.info(f"All requested data have been successfully loaded. Time taken: {t.interval:.3f}s.")        
 
     def _get_workspace_data(self):
         item = WSItem.WORKSPACE
@@ -920,15 +920,15 @@
     def _process_dataset_data(self):
         item = WSItem.DATASET
         item_name = item.name.lower()
         self.stdout.info('Processing dataset definitions...')
         if item_name not in self.data:
             self.stdout.warning("Dataset data not loaded. Skipping.")
             return None
-        with Timer() as t:
+        with timer() as t:
             data = self.data[item_name]
             common_dataset_names = data.get_df("common")['name'].values
             dataset_names_1 = data.get_df("left_only")['name'].values
             dataset_names_2 = data.get_df("right_only")['name'].values
             df = data.df_merge
             df.set_index("name", inplace=True)
             for ds_name in common_dataset_names:
@@ -960,15 +960,15 @@
         items_to_request = []
         if pdf_item_name not in self.data:
             items_to_request.append(WSItem.PDF)
         if function_item_name not in self.data:
             items_to_request.append(WSItem.FUNCTION)
         
         if len(items_to_request) > 0:
-            with Timer() as t:
+            with timer() as t:
                 for item in items_to_request:
                     self.stdout.info(f'Added "{item.title}" to the requested data pool needed for '
                                      'inferring renamed and redefined variables.')
                     item_name = item.name.lower()
                     self.data[item_name] = self.get_item_data(item)
             self.stdout.info(f"All requested data have been successfully loaded. Time taken: {t.interval:.3f}s.")
             return self._get_combined_mapping_statistics()
@@ -1019,15 +1019,15 @@
 
     def _process_renamed_and_remapped_variables(self):
         
         relevant_items = self._get_items_with_definition()
                 
         if len(relevant_items) > 0:
             self.stdout.info("Processing renamed and remapped variables...")
-            with Timer() as t:
+            with timer() as t:
                 map_stat_left, map_stat_right = self._get_combined_mapping_statistics()
                 mappings = self._get_mappings(map_stat_left, map_stat_right)
                 for item_str in relevant_items:
                     data = self.data[item_str]
                     data.process_mappings(mappings)
             self.stdout.info(f"Processing finished. Time taken: {t.interval:.3f}s")
```

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_decomposer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Optional, Union, List, Dict, Sequence
     
 import numpy as np
 
 import ROOT
 
 import quickstats
-from quickstats import semistaticmethod, AbstractObject, Timer
+from quickstats import AbstractObject, semistaticmethod, timer
 from quickstats.maths.numerics import is_integer
 from quickstats.utils.string_utils import split_str
 from quickstats.utils.common_utils import remove_list_duplicates
 from quickstats.components import ExtendedModel
 from quickstats.components.workspaces import XMLWSBase
 from quickstats.interface.root import RooAbsPdf, RooDataSet
 
@@ -93,15 +93,15 @@
     
     def create_decomposed_workspace(self, infile:str, outfile:str,
                                     category_expr:Union[List[Union[str, int]], str, int]="*",
                                     snapshots_to_save:Optional[List[str]]=None,
                                     rebuild_nuis:bool=False,
                                     rebuild_pdf:bool=False,
                                     import_class_code:bool=True):
-        with Timer() as t:
+        with timer() as t:
             model = ExtendedModel(infile, data_name=None, verbosity="WARNING")
             orig_cat = model.pdf.indexCat()
             categories = self.parse_categories(category_expr, orig_cat)
             snapshots = self.parse_snapshots(model.workspace, snapshots_to_save)
             if not categories:
                 raise RuntimeError('no categories selected')
             new_ws  = ROOT.RooWorkspace(model.workspace.GetName(), model.workspace.GetTitle())
```

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     tabulate = None
     
 import numpy as np
 
 import ROOT
 
 import quickstats
-from quickstats import semistaticmethod, AbstractObject, GeneralEnum, Timer
+from quickstats import semistaticmethod, AbstractObject, GeneralEnum, timer
 from quickstats.components import ExtendedModel
 from quickstats.utils.xml_tools import TXMLTree
 from quickstats.utils.root_utils import load_macro, get_macro_dir, is_corrupt
 from quickstats.utils.common_utils import format_delimiter_enclosed_text
 from quickstats.maths.numerics import is_float, pretty_value
 from quickstats.components.workspaces import XMLWSBase, WSObjectType, BracketType
 from quickstats.interface.root import RooDataSet
@@ -53,15 +53,15 @@
                  use_cms_opt_pdf=True) -> None:
         super().__init__(source=source, basedir=basedir,
                          unlimited_stack=unlimited_stack,
                          verbosity=verbosity)
         self.minimizer_config = minimizer_config
         self.load_extension()
         self.use_cms_opt_pdf = False
-        with Timer() as t:
+        with timer() as t:
             self.initialize(source=source)
         self.use_cms_opt_pdf = use_cms_opt_pdf and hasattr(ROOT, "RooSimultaneousOpt")
         self.init_time = t.interval
         
     def initialize(self, source:Union[str, Dict]) -> None:
         self.combination_config = {}
         self.channel_config     = {}
@@ -1007,15 +1007,15 @@
     
     def create_combined_workspace(self, infiles:Optional[Dict[str, str]]=None,
                                   outfile:Optional[str]=None,
                                   save_rename_ws:bool=False,
                                   save_combine_ws:bool=False,
                                   save_final_ws:bool=True,
                                   import_class_code:bool=True) -> None:
-        with Timer() as t:
+        with timer() as t:
             # override path to the input channel workspaces
             if infiles is not None:
                 for channel in self.channel_config:
                     if channel not in infiles:
                         raise ValueError(f'missing input workspace path for the channel "{channel}"')
                     self.channel_config[channel]['input_file'] = infiles[channel]
             self.reset_combination()
```

### Comparing `quickstats-0.7.0.0/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Optional, Union, List, Dict
 
 import numpy as np
 
 import ROOT
 
 import quickstats
-from quickstats import semistaticmethod, Timer, AbstractObject, GeneralEnum
+from quickstats import semistaticmethod, timer, AbstractObject, GeneralEnum
 from quickstats.components import ExtendedModel
 from quickstats.utils.xml_tools import TXMLTree
 from quickstats.utils.common_utils import format_delimiter_enclosed_text, remove_list_duplicates
 from quickstats.maths.numerics import is_float, pretty_value
 from quickstats.components.basics import WSArgument
 from quickstats.components.workspaces import XMLWSBase, WSObjectType, AsimovHandler
 from quickstats.interface.root import RooAbsPdf
@@ -365,15 +365,15 @@
                 if update_formula:
                     new_formula_var = ROOT.RooFormulaVar(obj.GetName(), obj.GetTitle(), formula, actual_vars)
                     getattr(ws_tmp, "import")(new_formula_var, ROOT.RooFit.RenameVariable(old_var_expr, new_var_expr), ROOT.RooFit.RecycleConflictNodes())
             obj = iter.Next()
     
     def create_modified_workspace(self, infile:Optional[str]=None, outfile:Optional[str]=None,
                                   import_class_code:bool=True, recreate:bool=True):
-        with Timer() as t:
+        with timer() as t:
             self.sanity_check()
             # override path to the input workspace
             if infile is None:
                 infile = self.config['input_file']
             # override path to the output workspace
             if outfile is None:
                 outfile = self.config['output_file']
```

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/abstract_runner.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/abstract_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from typing import Optional, Union, Dict, List, Any
-from quickstats import semistaticmethod, AbstractObject, Timer
+from quickstats import semistaticmethod, AbstractObject, timer
 from quickstats.concurrent.logging import standard_log
 from quickstats.utils.common_utils import execute_multi_tasks, is_valid_file
 
 class AbstractRunner(AbstractObject):
     
     @property
     def config(self):
@@ -90,15 +90,15 @@
                     return cached_result
             except Exception:
                 self.stdout.info(f'Broken output: {outpath}. Ignored.')
         return None
     
     def run_batch(self, argument_list, auxiliary_args:Optional[Dict]=None, cache_only:bool=False):
         parallel = self.config['parallel']
-        with Timer() as t:
+        with timer() as t:
             self._prerun_batch()
             if cache_only:
                 raw_result = execute_multi_tasks(self.get_cached_output, argument_list, parallel=parallel)
                 raw_result = [result for result in raw_result if result is not None]
             else:
                 raw_result = execute_multi_tasks(self.run_instance, argument_list, parallel=parallel)
             results = self.postprocess(raw_result, auxiliary_args)
```

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/logging.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/concurrent/parameterised_significance.py` & `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_significance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/core/abstract_object.py` & `quickstats-0.7.0.2.1/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/core/decorators.py` & `quickstats-0.7.0.2.1/quickstats/core/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,14 @@
         if (obj is not None):
             return partial(self.f, obj)
         return self.f
 
     @property
     def __func__(self):
         return self.f
-
-def require_package(pkg_names:str):
-    def check_package(func):
-        def wrapper(*args, **kwargs):
-            missing_pkgs = [name for name in pkg_names if importlib.util.find_spec(name) is None]
-            if missing_pkgs:
-                func_name = func.__name__
-                raise RuntimeError(f'missing modules required by the function {func_name}: {", ".join(missing_pkgs)}')
-            result = function(*args, **kwargs)
-            return result
-        return wrapper
-    return check_package
         
 def cls_method_timer(func):
     """
     Decorator function to measure the execution time of a class method.
 
     The `cls_method_timer` decorator function can be applied to any class method to automatically measure 
     the execution time of the method. When the decorated method is called, it records the start and end 
@@ -99,32 +87,32 @@
         t2 = time.time()
         method_name = f"{type(self).__name__}::{func.__name__}"
         self.stdout.info(f'Task {method_name!r} executed in {(t2 - t1):.3f} s')
         return result
 
     return wrapper
 
-class Timer:    
+class timer:    
     """
     Context manager class for measuring the execution time of a code block.
 
     Example:
-        with Timer() as t:
+        with timer() as t:
             # Perform some time-consuming task here
             time.sleep(2)
 
         print("Elapsed time:", t.interval)  # outputs: "Elapsed time: 2.0 seconds"
 
     """
     def __enter__(self):
         """
         Records the start time when entering the context.
 
         Returns:
-            Timer: The Timer instance itself.
+            timer: The timer instance itself.
         """
         self.start = time.time()
         return self
 
     def __exit__(self, *args):
         """
         Calculates the time interval when exiting the context.
```

### Comparing `quickstats-0.7.0.0/quickstats/core/enums.py` & `quickstats-0.7.0.2.1/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/core/io.py` & `quickstats-0.7.0.2.1/quickstats/core/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 getThreads = True
 getMultiprocessing = True
 getProcesses = True
 
 @total_ordering
 class Verbosity(Enum):
-    
+    IGNORE = (100, 'IGNORE')
     CRITICAL = (50, 'CRITICAL')
     ERROR = (40, 'ERROR')
     TIPS = (35, 'TIPS')
     WARNING = (30, 'WARNING')
     INFO = (20, 'INFO')
     DEBUG = (10, 'DEBUG')
     NOTSET = (0, 'NOTSET')
@@ -153,14 +153,17 @@
         self.__call__(text, Verbosity.ERROR, color=color, bare=bare)
         
     def critical(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.CRITICAL, color=color, bare=bare)
 
     def debug(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.DEBUG, color=color, bare=bare)
+
+    def write(self, text:str='', color=None):
+        self.__call__(text, verbosity.IGNORE, color=color, bare=True)
         
     def set_format(self, fmt:Optional[str]=None):
         if fmt is None:
             fmt = self.DEFAULT_FORMAT
         self._formatter = logging.Formatter(fmt)
         
     def set_timefmt(self, datefmt:Optional[str]=None, msecfmt:Optional[str]=None):
```

### Comparing `quickstats-0.7.0.0/quickstats/core/methods.py` & `quickstats-0.7.0.2.1/quickstats/core/methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 import glob
 import json
 import shutil
 import importlib
 
 import quickstats
 
+__all__ = ["compile_macros", "get_all_macros",
+           "set_verbosity", "get_root_version",
+           "get_workspace_extensions",
+           "get_workspace_extension_config",
+           "add_macro", "remove_macro",
+           "load_corelib", "load_extensions",
+           "load_processor_methods", "module_exist"]
+
 def compile_macros(macros:Optional[Union[str, List[str]]]=None):
     """
     Compile ROOT macros
     
     Arguments:
         macros: (Optional) str or list of str
             If str, it is a string containing comma delimited list of macro names to be compiled.
```

### Comparing `quickstats-0.7.0.0/quickstats/core/path_manager.py` & `quickstats-0.7.0.2.1/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/core/virtual_trees.py` & `quickstats-0.7.0.2.1/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/extensions/extension_dataframe.py` & `quickstats-0.7.0.2.1/quickstats/extensions/extension_dataframe.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/cppyy/core.py` & `quickstats-0.7.0.2.1/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/cppyy/macros.py` & `quickstats-0.7.0.2.1/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.7.0.2.1/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/ModelConfig.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/ModelConfig.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RDataFrame.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RDataFrame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooAbsArg.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsArg.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooAbsData.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooArgSet.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooArgSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooCategory.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooDataSet.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooMsgService.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/RooRealVar.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/TChain.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/TChain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/TF1.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/TH1.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/TH2.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/TH3.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/TH3.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/__init__.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/helper.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/macros.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/interface/root/roofit_extension.py` & `quickstats-0.7.0.2.1/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/QStringUtils.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/maths/interpolation.py` & `quickstats-0.7.0.2.1/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/maths/numerics.py` & `quickstats-0.7.0.2.1/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/maths/statistics.py` & `quickstats-0.7.0.2.1/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/maths/statistics_jitted.py` & `quickstats-0.7.0.2.1/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/maths/symbolics.py` & `quickstats-0.7.0.2.1/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/parsers/param_parser.py` & `quickstats-0.7.0.2.1/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/parsers/roo_param_setup_parser.py` & `quickstats-0.7.0.2.1/quickstats/parsers/roo_param_setup_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/__init__.py` & `quickstats-0.7.0.2.1/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/abstract_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/abstract_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,20 @@
         if xmin is not None:
             xlim[0] = xmin
         if xmax is not None:
             xlim[1] = xmax
         if ypad is not None:
             if ypad < 0 or ypad > 1:
                 raise ValueError('"ypad" must be between 0 and 1')
-            ylim[1] = ylim[0] + (ylim[1] - ylim[0]) / (1 - ypad)
+            if ax.get_yaxis().get_scale() == "log":
+                if ylim[0] <= 0:
+                    raise ValueError("ymin must be positive in a logscale plot")
+                ylim[1] = (ylim[1] ** (1 + ypad)) / (ylim[0] ** ypad)
+            else:
+                ylim[1] = ylim[0] + (ylim[1] - ylim[0]) / (1 - ypad)
         if ymin is not None:
             ylim[0] = ymin
         if ymax is not None:
             ylim[1] = ymax
         ax.set_xlim(*xlim)
         ax.set_ylim(*ylim)
```

### Comparing `quickstats-0.7.0.0/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.7.0.2.1/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/collective_data_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/color_schemes.py` & `quickstats-0.7.0.2.1/quickstats/plots/color_schemes.py`

 * *Files 13% similar despite different names*

```diff
@@ -84,16 +84,18 @@
     hist_series=['#99CCFF', '#EFCF6E', '#64CB34'],
     shading_light=["#FBF0D9", "#C0E7DC", "#E4C0F4", "#B3D4E8"],
     shading_medium=["#E0DCC5", "#C5E00C", "#E0C5D4", "#C5C5E0"],
     shading_dark=["#C1B98A", "#8AC199", "#C18AA9", "#8B8AC1"],
     ibm=["#648fff", "#785ef0", "#dc267f", "#fe6100", "#ffb000"],
     butterflycore=["#f4cccc", "#ffe599", "#b6d7a8", "#9fc5e8", "#9C98DB", "#D6BFAB", "#876659"],
     simple_contrast=["#ED553B", "#20639B", "#3CAEA3", "#F6D55C", "#BF51A0", "#735245"],
+    vibrant_contrast=["#dc493a", "#06b8a6", "#4392f0", "#451ea6", "#f57600", "#34a853",
+                      "#e6308a", "#686f6c", "#d08b02", "#d1d600"],
     checker=["#068EAC", "#DE5B7D", "#4A9451", "#F97623", "#FAE215", "#BF51A0",
              "#84E4D0", "#B32A32", "#ADE85B", "#FFA41A", "#505BB6", "#596D3D",
              "#2C388E", "#5B3F7B", "#8D89C2", "#6586B3", "#CCA18D", "#735245"],
     atlas_hdbs=["hdbs:spacecadet", "hdbs:starcommandblue", "hdbs:pictorialcarmine",
                 "hdbs:outrageousorange", "hdbs:maroonX11", "hdbs:mintcream"],
     atlas_hh=["hh:darkpink", "hh:medturquoise", "hh:darkyellow",
               "hh:darkgreen", "hh:darkblue", "hh:lightturquoise", "hh:offwhite"],
-    qualitative=["#FF1F5B", "#00CD6C", "#009ADE", "#AF58BA", "#FF6C1E", "F28522"]
+    qualitative=["#FF1F5B", "#00CD6C", "#009ADE", "#AF58BA", "#FF6C1E", "#F28522"]
 )
```

### Comparing `quickstats-0.7.0.0/quickstats/plots/core.py` & `quickstats-0.7.0.2.1/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/correlation_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/general_1D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/general_2D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/general_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/general_distribution_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/np_ranking_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/sample_purity_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/score_distribution_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/stat_plot_config.py` & `quickstats-0.7.0.2.1/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/template.py` & `quickstats-0.7.0.2.1/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/two_axis_1D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/two_axis_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/upper_limit_2D_plot_deprecated.py` & `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.7.0.2.1/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/root_checker.py` & `quickstats-0.7.0.2.1/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/utils/common_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/common_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Union, Dict, List, Tuple, Callable
 import os
 import sys
 import copy
 import fnmatch
 import time
 import json
+import yaml
 import inspect
 import datetime
 import functools
 import collections.abc
 
 import numpy as np
 
@@ -471,8 +472,18 @@
         elif isinstance(value, str):
             df = df[df[attribute].str.fullmatch(value)]
         elif isinstance(value, Callable):
             df = df[df[attribute].apply(value)]
         else:
             df = df[df[attribute] == value]
     df = df.reset_index(drop=True)
-    return df        
+    return df      
+
+class IndentDumper(yaml.Dumper):
+    def increase_indent(self, flow=False, indentless=False):
+        return super(IndentDumper, self).increase_indent(flow, False)
+
+def save_yaml(obj, filename:str, indent:int=2):
+    with open(filename, 'w') as f:
+        yaml.dump(obj, f, Dumper=IndentDumper,
+                  default_flow_style=False,
+                  sort_keys=False, indent=indent)
```

### Comparing `quickstats-0.7.0.0/quickstats/utils/data_conversion.py` & `quickstats-0.7.0.2.1/quickstats/utils/data_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 import glob
 import uuid
 
 import numpy as np
 
-from quickstats import DescriptiveEnum
+from quickstats import DescriptiveEnum, module_exist
 
 root_datatypes = ["bool", "Bool_t", "Byte_t", "char", "char*", "Char_t", 
                   "double", "Double32_t", "Double_t", "float",
                   "Float16_t", "Float_t", "int", "Int_t", 
                   "long", "long long", "Long_t", "Long64_t",
                   "short", "Short_t", "Size_t", "UChar_t",
                   "UInt_t", "ULong64_t", "ULong_t",
@@ -206,23 +206,35 @@
                 else:
                     result = pd.concat([result, batch])
             return result
     else:
         if (library == 'pandas') and (downcast):
             return make_iter_result(results, downcast=True)
         return make_iter_result(results, downcast=False)
+
+def get_columns(filename:str, treename:str):
+    if module_exist('uproot'):
+        try:
+            import uproot
+            return list(uproot.open(filename)[treename].keys())
+        except:
+            pass
+    return None
     
 def rdf2numpy(rdf, columns:Union[Dict[str, str], List[str]]=None,
               cut:Optional[str]=None, convert_vectors:bool=True,
-              mode:Union[str, int, ConversionMode]=1):
+              mode:Union[str, int, ConversionMode]=1,
+              all_columns:Optional[List[str]]=None):
+    if all_columns is None:
+        all_columns = [str(name) for name in rdf.GetColumnNames()]
     if cut is not None:
         rdf = rdf.Filter(cut)     
     rename_columns = {}
     if columns is None:
-        column_names = [str(name) for name in rdf.GetColumnNames()]
+        column_names = list(all_columns)
         columns = {}
         for name in column_names:
             if "." in name:
                 name_fix = name.replace(".", "_")
                 if name_fix not in column_names:
                     columns[name_fix] = name
                 else:
@@ -232,22 +244,23 @@
                 columns[name] = name
     if isinstance(columns, dict):
         save_columns = []
         for column_name, definition in columns.items():
             if column_name == definition:
                 save_columns.append(column_name)
                 continue
-            if rdf.HasColumn(column_name):
+            if column_name in all_columns:
                 new_column_name = f"var_{uuid.uuid4().hex}"
                 rename_columns[new_column_name] = column_name
                 column_name = new_column_name
-            if rdf.HasColumn(definition):
+            if definition in all_columns:
                 rdf = rdf.Alias(column_name, definition)
             else:
                 rdf = rdf.Define(column_name, definition)
+            all_columns.append(column_name)
             save_columns.append(column_name)
     else:
         save_columns = list(columns)
     conversion_mode = ConversionMode.parse(mode)
 
     if conversion_mode in [ConversionMode.REMOVE_NON_STANDARD_TYPE,
                            ConversionMode.REMOVE_NON_ARRAY_TYPE]:
@@ -278,20 +291,25 @@
                 try:
                     rdf = rdf.Define(new_column_name, f"RVec2Vec({column_name})")
                 except Exception:
                     tmp_column_name = f"var_{uuid.uuid4().hex}"
                     rdf = rdf.Alias(tmp_column_name, column_name)
                     rdf = rdf.Define(new_column_name, f"RVec2Vec({tmp_column_name})")
                 vector_columns.append(new_column_name)
-
     available_columns = [str(name) for name in rdf.GetColumnNames()]
     missing_columns = np.setdiff1d(save_columns, available_columns)
     if len(missing_columns) > 0:
         raise RuntimeError(f'missing column(s): {", ".join(missing_columns)}')
-    result = rdf.AsNumpy(save_columns)
+    result = None
+    #if module_exist('awkward'):
+    #    import awkward as ak
+    #    if hasattr(ak, 'from_rdataframe'):
+    #        result = ak.to_numpy(ak.from_rdataframe(rdf, columns=save_columns))
+    if result is None:
+        result = rdf.AsNumpy(save_columns)
     for vector_column in vector_columns:
         # not the most efficient way, but easiest
         numpy_array = np.array([np.array(v.data()) for v in result[vector_column]], dtype=object)
         # in case it't array of regular size
         if len(numpy_array) and (numpy_array[0].dtype == object):
             result[vector_column] = np.array([np.array(v.data()) for v in result[vector_column]])
         else:
@@ -317,17 +335,19 @@
     if library.lower() == "auto":
         library = get_default_library(custom_columns=isinstance(columns,dict))
     if library.lower() == "root":
         from quickstats.interface.root.helper import RMultithreadEnv
         with RMultithreadEnv(multithread):
             import ROOT
             rdf = ROOT.RDataFrame(treename, filename)
+            all_columns = get_columns(filename, treename=treename)
             return rdf2numpy(rdf, columns=columns, cut=cut,
                              convert_vectors=convert_vectors,
-                             mode=mode)
+                             mode=mode,
+                             all_columns=all_columns)
     elif library.lower() == "uproot":
         import uproot
         if not isinstance(filename, list):
             filename = [filename]
         # iterate over multiple files
         files = {f:treename for f in filename}
         if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
```

### Comparing `quickstats-0.7.0.0/quickstats/utils/hep_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/utils/roofit_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/utils/roostats_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/utils/root_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/utils/string_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/string_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Callable, List
+from typing import Optional, Callable, List, Dict
 import re
 import ast
 import uuid
 import string
 
 import numpy as np
 
@@ -262,8 +262,89 @@
                 break
             for altkey in altkeys:
                 groupdict.pop(altkey)
         if not valid_match:
             continue
         result = (str_, groupdict)
         results.append(result)
-    return results
+    return results
+
+
+def insert_breaks_preserving_words(text: str, max_width: int, indent: str) -> str:
+    """
+    Inserts line breaks into a string to ensure it fits within a specified width without breaking words.
+    Subsequent lines are indented with the given indent string.
+
+    Args:
+        text: The original string to process.
+        max_width: The maximum width of each line, in characters.
+        indent: The string used to indent lines after the first line.
+
+    Returns:
+        The modified string with line breaks and indentation inserted.
+    """
+    words = text.split()
+    if not words:
+        return ""
+
+    current_line = words[0]
+    formatted_lines = []
+
+    for word in words[1:]:
+        # Check if adding the next word would exceed the max width
+        if len(current_line) + len(word) + 1 <= max_width:
+            current_line += " " + word
+        else:
+            formatted_lines.append(current_line)
+            current_line = indent + word
+            max_width = len(indent) + max_width  # Adjust max_width for indentation
+    formatted_lines.append(current_line)  # Add the last line
+
+    return "\n".join(formatted_lines)
+
+def format_dict_to_string(dictionary: Dict[str, str], separator: str = " : ",
+                          left_margin: int = 0, line_break: int = 100) -> str:
+    """
+    Formats a dictionary into a neatly aligned string representation, with each key-value pair on a new line. 
+
+    Args:
+        dictionary: The dictionary to format. Keys should be strings, and values are expected to be strings that 
+                    can contain multiple words.
+        separator: The string used to separate keys from their values. Defaults to ": ".
+        left_margin: The number of spaces to prepend to each line for indentation. Defaults to 0.
+        line_break: The maximum allowed width of each line, in characters, before wrapping the text to a new line. 
+                    Defaults to 100.
+
+    Returns:
+        A string representation of the dictionary. Each key-value pair is on its own line, with lines broken such 
+        that words are not split across lines, respecting the specified `line_break` width.
+
+    Example:
+        >>> example_dict = {"Key1": "This is a short value.", "Key2": "This is a much longer value that will be wrapped according to the specified line break width."}
+        >>> print(format_dict_to_string(example_dict, left_margin=4, line_break=80))
+         Key1: This is a short value.
+         Key2: This is a much longer value that will be wrapped according to the
+               specified line break width.
+
+    Note:
+        The function removes existing newlines in values to prevent unexpected line breaks and treats the entire 
+        value as a single paragraph that needs to be wrapped according to `line_break`.
+    """
+    if not dictionary:
+        return ""
+
+    max_key_length = max(len(key) for key in dictionary)
+    indent_size = left_margin + max_key_length + len(separator)
+    effective_text_width = line_break - indent_size
+
+    if effective_text_width <= 0:
+        raise ValueError("Line break width must be greater than the size of indentation and separator.")
+
+    formatted_lines = []
+    indent_string = " " * indent_size
+    for key, value in dictionary.items():
+        cleaned_value = value.replace("\n", " ")
+        wrapped_value = insert_breaks_preserving_words(cleaned_value, effective_text_width, indent_string)
+        line = f"{' ' * left_margin}{key:{max_key_length}}{separator}{wrapped_value}"
+        formatted_lines.append(line)
+
+    return "\n".join(formatted_lines) + "\n"
```

### Comparing `quickstats-0.7.0.0/quickstats/utils/sys_utils.py` & `quickstats-0.7.0.2.1/quickstats/utils/sys_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.0/quickstats/utils/xml_tools.py` & `quickstats-0.7.0.2.1/quickstats/utils/xml_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,24 +261,27 @@
                                     tag, otherwise they are emitted as a pair
                                     of start/end tags
         """
         if not encoding:
             encoding = "us-ascii"
         enc_lower = encoding.lower()
         with ET._get_writer(file_or_filename, enc_lower) as write:
+            # python updates changed behavior
+            if isinstance(write, tuple):
+                write = write[0]
             if (xml_declaration or
                     (xml_declaration is None and
                      enc_lower not in ("utf-8", "us-ascii", "unicode"))):
                 declared_encoding = encoding
                 if enc_lower == "unicode":
                     # Retrieve the default encoding for the xml declaration
                     import locale
                     declared_encoding = locale.getpreferredencoding()
                 write("<?xml version='1.0' encoding='%s'?>\n" % (
-                    declared_encoding,))
+                      declared_encoding,))
             else:
                 qnames, namespaces = ET._namespaces(self._root, default_namespace)
                 _serialize_xml(write, self._root, qnames, namespaces,
                           short_empty_elements=short_empty_elements)
                 
     def save(self, filename, **kwargs):
         if not self._root:
```

### Comparing `quickstats-0.7.0.0/quickstats.egg-info/PKG-INFO` & `quickstats-0.7.0.2.1/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.0
+Version: 0.7.0.2.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.0/quickstats.egg-info/SOURCES.txt` & `quickstats-0.7.0.2.1/quickstats.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 quickstats/algorithms/nll_crossing/BisectionMethod.py
 quickstats/algorithms/nll_crossing/NovelMethod.py
 quickstats/algorithms/nll_crossing/SteppingMethod.py
 quickstats/algorithms/nll_crossing/__init__.py
 quickstats/analysis/__init__.py
 quickstats/analysis/analysis_base.py
 quickstats/analysis/analysis_path_manager.py
-quickstats/analysis/config_format_templates.py
+quickstats/analysis/config_templates.py
 quickstats/analysis/data_loading.py
 quickstats/analysis/data_preprocessing.py
 quickstats/analysis/event_categorization.py
 quickstats/analysis/multi_class_boundary_tree.py
 quickstats/analysis/ntuple_conversion_tool.py
 quickstats/analysis/ntuple_process_tool.py
 quickstats/analysis/sample_poly_param_tool.py
@@ -127,22 +127,24 @@
 quickstats/concurrent/nuisance_parameter_ranking_runner.py
 quickstats/concurrent/parameterised_asymptotic_cls.py
 quickstats/concurrent/parameterised_likelihood.py
 quickstats/concurrent/parameterised_runner.py
 quickstats/concurrent/parameterised_significance.py
 quickstats/core/__init__.py
 quickstats/core/abstract_object.py
-quickstats/core/configs.py
-quickstats/core/configurable_object.py
-quickstats/core/dataclass_object.py
+quickstats/core/configurations.py
+quickstats/core/constraints.py
 quickstats/core/decorators.py
 quickstats/core/enums.py
 quickstats/core/io.py
+quickstats/core/metaclasses.py
 quickstats/core/methods.py
 quickstats/core/path_manager.py
+quickstats/core/setup.py
+quickstats/core/type_validation.py
 quickstats/core/virtual_trees.py
 quickstats/extensions/__init__.py
 quickstats/extensions/extension_dataframe.py
 quickstats/interface/__init__.py
 quickstats/interface/cppyy/__init__.py
 quickstats/interface/cppyy/basic_methods.py
 quickstats/interface/cppyy/core.py
@@ -167,14 +169,17 @@
 quickstats/interface/root/TH3.py
 quickstats/interface/root/TObject.py
 quickstats/interface/root/__init__.py
 quickstats/interface/root/helper.py
 quickstats/interface/root/io.py
 quickstats/interface/root/macros.py
 quickstats/interface/root/roofit_extension.py
+quickstats/interface/xrootd/__init__.py
+quickstats/interface/xrootd/core.py
+quickstats/interface/xrootd/utils.py
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
 quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
 quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
 quickstats/macros/QuickStatsCore/QStringUtils.cxx
 quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
 quickstats/macros/QuickStatsCore/RooFitExt.cxx
```

### Comparing `quickstats-0.7.0.0/setup.py` & `quickstats-0.7.0.2.1/setup.py`

 * *Files identical despite different names*

