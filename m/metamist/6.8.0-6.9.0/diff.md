# Comparing `tmp/metamist-6.8.0.tar.gz` & `tmp/metamist-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.8.0.tar", last modified: Mon Feb 19 01:30:30 2024, max compression
+gzip compressed data, was "metamist-6.9.0.tar", last modified: Thu Apr  4 00:35:21 2024, max compression
```

## Comparing `metamist-6.8.0.tar` & `metamist-6.9.0.tar`

### file list

```diff
@@ -1,132 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.390390 metamist-6.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-19 01:27:02.000000 metamist-6.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-19 01:27:02.000000 metamist-6.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-02-19 01:30:30.390390 metamist-6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-19 01:27:02.000000 metamist-6.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.374390 metamist-6.8.0/metamist/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.374390 metamist-6.8.0/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56274 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23776 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82052 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/billing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    51702 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28817 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47701 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53117 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47305 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18090 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37702 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.378390 metamist-6.8.0/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.378390 metamist-6.8.0/metamist/audit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/audit/audit_upload_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/audit/audithelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/audit/delete_assay_files_from_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/audit/generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.378390 metamist-6.8.0/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-02-19 01:29:03.000000 metamist-6.8.0/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.386390 metamist-6.8.0/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_cost_budget_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_cost_details_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_hail_batch_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_time_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_total_cost_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/billing_total_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/body_get_proportionate_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/proportional_date_temporal_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14319 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/sequencing_group_meta_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/sequencing_group_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-02-19 01:28:57.000000 metamist-6.8.0/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.386390 metamist-6.8.0/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.386390 metamist-6.8.0/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    55252 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-02-19 01:27:02.000000 metamist-6.8.0/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-02-19 01:28:58.000000 metamist-6.8.0/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.374390 metamist-6.8.0/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 01:30:30.000000 metamist-6.8.0/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-19 01:27:02.000000 metamist-6.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 01:30:30.390390 metamist-6.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-02-19 01:27:02.000000 metamist-6.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:30:30.390390 metamist-6.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32146 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_project_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_update_participant_family.py
--rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-02-19 01:27:02.000000 metamist-6.8.0/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-02-19 01:27:02.000000 metamist-6.8.0/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.067308 metamist-6.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 00:31:39.000000 metamist-6.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 00:31:39.000000 metamist-6.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-04 00:35:21.067308 metamist-6.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-04 00:31:39.000000 metamist-6.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.043308 metamist-6.9.0/metamist/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.047308 metamist-6.9.0/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56280 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/analysis_runner_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23776 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82010 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/billing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51702 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28817 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47701 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53117 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47305 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.047308 metamist-6.9.0/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.047308 metamist-6.9.0/metamist/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/audit/delete_assay_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/audit/generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.051308 metamist-6.9.0/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-04 00:33:46.000000 metamist-6.9.0/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.059308 metamist-6.9.0/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13839 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_batch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_cromwell_subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_cromwell_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_seq_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_sku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_cost_record_wdl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_cost_budget_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_cost_details_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_time_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_total_cost_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/billing_total_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/body_get_assays_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/body_get_proportionate_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/proportional_date_temporal_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14319 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/seqr_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/sequencing_group_meta_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/sequencing_group_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-04 00:33:40.000000 metamist-6.9.0/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.059308 metamist-6.9.0/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.059308 metamist-6.9.0/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55508 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-04 00:31:39.000000 metamist-6.9.0/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-04-04 00:33:41.000000 metamist-6.9.0/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.047308 metamist-6.9.0/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-04 00:35:20.000000 metamist-6.9.0/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-04 00:35:21.000000 metamist-6.9.0/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:35:20.000000 metamist-6.9.0/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 00:35:20.000000 metamist-6.9.0/metamist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:35:20.000000 metamist-6.9.0/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 00:35:20.000000 metamist-6.9.0/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 00:35:20.000000 metamist-6.9.0/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-04 00:31:39.000000 metamist-6.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:35:21.067308 metamist-6.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-04 00:31:39.000000 metamist-6.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:35:21.063308 metamist-6.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_api_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_billing_ar_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_billing_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_billing_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_billing_daily_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_billing_gcp_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_billing_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_function_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_bq_generic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_layers_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32146 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_project_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19073 2024-04-04 00:31:39.000000 metamist-6.9.0/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-04 00:31:39.000000 metamist-6.9.0/test/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-04 00:31:39.000000 metamist-6.9.0/test/testbqbase.py
```

### Comparing `metamist-6.8.0/LICENSE` & `metamist-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/PKG-INFO` & `metamist-6.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.8.0
+Version: 6.9.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.8.0/README.md` & `metamist-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/__init__.py` & `metamist-6.9.0/metamist/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-6.8.0/metamist/api/analysis_api.py` & `metamist-6.9.0/metamist/api/analysis_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -225,16 +225,16 @@
                 'operation_id': 'get_analysis_runner_log',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'project_names',
-                    'author',
                     'output_dir',
+                    'ar_guid',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -244,28 +244,28 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project_names':
                         ([str],),
-                    'author':
-                        (str,),
                     'output_dir':
                         (str,),
+                    'ar_guid':
+                        (str,),
                 },
                 'attribute_map': {
                     'project_names': 'project_names',
-                    'author': 'author',
                     'output_dir': 'output_dir',
+                    'ar_guid': 'ar_guid',
                 },
                 'location_map': {
                     'project_names': 'query',
-                    'author': 'query',
                     'output_dir': 'query',
+                    'ar_guid': 'query',
                 },
                 'collection_format_map': {
                     'project_names': 'multi',
                 }
             },
             headers_map={
                 'accept': [
@@ -930,16 +930,16 @@
 
         >>> thread = api.get_analysis_runner_log(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             project_names ([str]): [optional]
-            author (str): [optional]
             output_dir (str): [optional]
+            ar_guid (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `metamist-6.8.0/metamist/api/assay_api.py` & `metamist-6.9.0/metamist/api/assay_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/billing_api.py` & `metamist-6.9.0/metamist/api/billing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,17 +18,17 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
+from metamist.model.analysis_cost_record import AnalysisCostRecord
 from metamist.model.billing_column import BillingColumn
 from metamist.model.billing_cost_budget_record import BillingCostBudgetRecord
-from metamist.model.billing_hail_batch_cost_record import BillingHailBatchCostRecord
 from metamist.model.billing_source import BillingSource
 from metamist.model.billing_total_cost_query_model import BillingTotalCostQueryModel
 from metamist.model.billing_total_cost_record import BillingTotalCostRecord
 from metamist.model.http_validation_error import HTTPValidationError
 
 
 class BillingApi(object):
@@ -42,15 +42,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.cost_by_ar_guid_async = async_wrap(self.cost_by_ar_guid)
         self.cost_by_ar_guid_endpoint = _Endpoint(
             settings={
-                'response_type': (BillingHailBatchCostRecord,),
+                'response_type': ([AnalysisCostRecord],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/billing/cost-by-ar-guid/{ar_guid}',
                 'operation_id': 'cost_by_ar_guid',
                 'http_method': 'GET',
                 'servers': None,
@@ -95,15 +95,15 @@
             },
             api_client=api_client
         )
 
         self.cost_by_batch_id_async = async_wrap(self.cost_by_batch_id)
         self.cost_by_batch_id_endpoint = _Endpoint(
             settings={
-                'response_type': (BillingHailBatchCostRecord,),
+                'response_type': ([AnalysisCostRecord],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/billing/cost-by-batch-id/{batch_id}',
                 'operation_id': 'cost_by_batch_id',
                 'http_method': 'GET',
                 'servers': None,
@@ -956,15 +956,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            BillingHailBatchCostRecord
+            [AnalysisCostRecord]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1027,15 +1027,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            BillingHailBatchCostRecord
+            [AnalysisCostRecord]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.8.0/metamist/api/enums_api.py` & `metamist-6.9.0/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/family_api.py` & `metamist-6.9.0/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/import_api.py` & `metamist-6.9.0/metamist/api/import_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/participant_api.py` & `metamist-6.9.0/metamist/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/project_api.py` & `metamist-6.9.0/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/sample_api.py` & `metamist-6.9.0/metamist/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/seqr_api.py` & `metamist-6.9.0/metamist/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/sequencing_group_api.py` & `metamist-6.9.0/metamist/api/sequencing_group_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/api/web_api.py` & `metamist-6.9.0/metamist/api/web_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -22,14 +22,15 @@
     validate_and_convert_types,
     async_wrap
 )
 from metamist.model.http_validation_error import HTTPValidationError
 from metamist.model.project_summary import ProjectSummary
 from metamist.model.search_item import SearchItem
 from metamist.model.search_response_model import SearchResponseModel
+from metamist.model.seqr_dataset_type import SeqrDatasetType
 
 
 class WebApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -175,25 +176,27 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'sequencing_type',
                     'project',
+                    'seqr_dataset_type',
                     'sync_families',
                     'sync_individual_metadata',
                     'sync_individuals',
                     'sync_es_index',
                     'sync_saved_variants',
                     'sync_cram_map',
                     'post_slack_notification',
                 ],
                 'required': [
                     'sequencing_type',
                     'project',
+                    'seqr_dataset_type',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -204,14 +207,16 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'sequencing_type':
                         (str,),
                     'project':
                         (str,),
+                    'seqr_dataset_type':
+                        ([SeqrDatasetType],),
                     'sync_families':
                         (bool,),
                     'sync_individual_metadata':
                         (bool,),
                     'sync_individuals':
                         (bool,),
                     'sync_es_index':
@@ -233,14 +238,15 @@
                     'sync_saved_variants': 'sync_saved_variants',
                     'sync_cram_map': 'sync_cram_map',
                     'post_slack_notification': 'post_slack_notification',
                 },
                 'location_map': {
                     'sequencing_type': 'path',
                     'project': 'path',
+                    'seqr_dataset_type': 'body',
                     'sync_families': 'query',
                     'sync_individual_metadata': 'query',
                     'sync_individuals': 'query',
                     'sync_es_index': 'query',
                     'sync_saved_variants': 'query',
                     'sync_cram_map': 'query',
                     'post_slack_notification': 'query',
@@ -248,15 +254,17 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
 
     def get_project_summary(
         self,
         project,
@@ -405,28 +413,30 @@
             keyword
         return self.search_by_keyword_endpoint.call_with_http_info(**kwargs)
 
     def sync_seqr_project(
         self,
         sequencing_type,
         project,
+        seqr_dataset_type,
         **kwargs
     ):
         """Sync Seqr Project  # noqa: E501
 
-        Sync a metamist project with its seqr project (for a specific sequence type)  # noqa: E501
+        Sync a metamist project with its seqr project (for a specific sequence type) es_index_types: list of any of 'Haplotypecaller', 'SV_Caller', 'Mitochondria_Caller'  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sync_seqr_project(sequencing_type, project, async_req=True)
+        >>> thread = api.sync_seqr_project(sequencing_type, project, seqr_dataset_type, async_req=True)
         >>> result = thread.get()
 
         Args:
             sequencing_type (str):
             project (str):
+            seqr_dataset_type ([SeqrDatasetType]):
 
         Keyword Args:
             sync_families (bool): [optional] if omitted the server will use the default value of True
             sync_individual_metadata (bool): [optional] if omitted the server will use the default value of True
             sync_individuals (bool): [optional] if omitted the server will use the default value of True
             sync_es_index (bool): [optional] if omitted the server will use the default value of True
             sync_saved_variants (bool): [optional] if omitted the server will use the default value of True
@@ -481,9 +491,11 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['sequencing_type'] = \
             sequencing_type
         kwargs['project'] = \
             project
+        kwargs['seqr_dataset_type'] = \
+            seqr_dataset_type
         return self.sync_seqr_project_endpoint.call_with_http_info(**kwargs)
```

### Comparing `metamist-6.8.0/metamist/api_client.py` & `metamist-6.9.0/metamist/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -36,14 +36,29 @@
     deserialize_file,
     file_type,
     model_to_dict,
     none_type,
     validate_and_convert_types
 )
 
+def get_select_env_values():
+    env_values = {
+        'HAIL_ATTEMPT_ID': 'HAIL_ATTEMPT_ID',
+        'HAIL_BATCH_ID': 'HAIL_BATCH_ID',
+        'HAIL_JOB_ID': 'HAIL_JOB_ID',
+    }
+
+    as_map = {}
+    for env_key, dict_key in env_values.items():
+        value = os.getenv(env_key)
+        if value:
+            as_map[dict_key] = value
+
+    return as_map
+
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the OpenAPI
@@ -75,14 +90,18 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         ar_guid = try_get_ar_guid()
         if ar_guid:
             self.default_headers['sm-ar-guid'] = ar_guid
         if header_name is not None:
             self.default_headers[header_name] = header_value
+        extra_values = get_select_env_values()
+        if extra_values:
+            self.default_headers['sm-extra-values'] = json.dumps(extra_values)
+
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'OpenAPI-Generator/1.0.0/python'
 
     def __enter__(self):
         return self
```

### Comparing `metamist-6.8.0/metamist/apis/__init__.py` & `metamist-6.9.0/metamist/apis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from metamist.api.analysis_api import AnalysisApi
+from metamist.api.analysis_runner_api import AnalysisRunnerApi
 from metamist.api.assay_api import AssayApi
 from metamist.api.billing_api import BillingApi
 from metamist.api.enums_api import EnumsApi
 from metamist.api.family_api import FamilyApi
 from metamist.api.import_api import ImportApi
 from metamist.api.participant_api import ParticipantApi
 from metamist.api.project_api import ProjectApi
```

### Comparing `metamist-6.8.0/metamist/audit/audit_upload_bucket.py` & `metamist-6.9.0/metamist/audit/audit_upload_bucket.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/audit/audithelper.py` & `metamist-6.9.0/metamist/audit/audithelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/audit/delete_assay_files_from_audit.py` & `metamist-6.9.0/metamist/audit/delete_assay_files_from_audit.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/audit/generic_auditor.py` & `metamist-6.9.0/metamist/audit/generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/configuration.py` & `metamist-6.9.0/metamist/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -405,15 +405,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.8.0\n"\
+               "Version of the API: 6.9.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-6.8.0/metamist/exceptions.py` & `metamist-6.9.0/metamist/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-6.8.0/metamist/graphql/__init__.py` & `metamist-6.9.0/metamist/graphql/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # pylint: disable=global-statement,import-self
 """
 GraphQL utilities for Metamist, allows you to:
     - construct queries using the `gql` function (which validates graphql syntax)
     - validate queries with metamist schema (by fetching the schema)
 """
+
 import os
+from json.decoder import JSONDecodeError
 from typing import Any, Dict
 
+import backoff
 from gql import Client
 from gql import gql as gql_constructor
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.aiohttp import log as aiohttp_logger
+from gql.transport.exceptions import TransportServerError
 from gql.transport.requests import RequestsHTTPTransport
 from gql.transport.requests import log as requests_logger
 
 # this does not import itself, it imports the module
 from graphql import DocumentNode  # type: ignore
+from requests.exceptions import HTTPError
 
 from cpg_utils.cloud import get_google_identity_token
 
 import metamist.configuration
 
 _sync_client: Client | None = None
 _async_client: Client | None = None
@@ -133,16 +138,25 @@
         doc = gql(doc)
 
     (client or configure_sync_client(use_local_schema=use_local_schema)).validate(doc)
     return True
 
 
 # use older style typing to broaden supported Python versions
+@backoff.on_exception(
+    backoff.expo,
+    exception=(HTTPError, JSONDecodeError, TransportServerError),
+    max_time=10,
+    max_tries=3,
+)
 def query(
-    _query: str | DocumentNode, variables: Dict = None, client: Client = None, log_response: bool = False
+    _query: str | DocumentNode,
+    variables: Dict | None = None,
+    client: Client | None = None,
+    log_response: bool = False,
 ) -> Dict[str, Any]:
     """Query the metamist GraphQL API"""
     if variables is None:
         variables = {}
 
     # disable logging for gql
     current_level = aiohttp_logger.level
@@ -155,16 +169,25 @@
     )
 
     if not log_response:
         requests_logger.setLevel(current_level)
     return response
 
 
+@backoff.on_exception(
+    backoff.expo,
+    exception=(HTTPError, JSONDecodeError, TransportServerError),
+    max_time=10,
+    max_tries=3,
+)
 async def query_async(
-    _query: str | DocumentNode, variables: Dict = None, client: Client = None, log_response: bool = False
+    _query: str | DocumentNode,
+    variables: Dict | None = None,
+    client: Client | None = None,
+    log_response: bool = False,
 ) -> Dict[str, Any]:
     """Asynchronously query the Metamist GraphQL API"""
     if variables is None:
         variables = {}
 
     # disable logging for gql
     current_level = aiohttp_logger.level
```

### Comparing `metamist-6.8.0/metamist/graphql/schema.graphql` & `metamist-6.9.0/metamist/graphql/schema.graphql`

 * *Files 16% similar despite different names*

```diff
@@ -51,14 +51,34 @@
   active: Boolean!
   meta: JSON!
   sequencingGroups: [GraphQLSequencingGroup!]!
   project: GraphQLProject!
   auditLogs: [GraphQLAuditLog!]!
 }
 
+type GraphQLAnalysisRunner {
+  arGuid: String!
+  outputPath: String!
+  timestamp: DateTime!
+  accessLevel: String!
+  repository: String!
+  commit: String!
+  script: String!
+  description: String!
+  driverImage: String!
+  configPath: String!
+  cwd: String
+  environment: String!
+  hailVersion: String
+  batchUrl: String!
+  submittingUser: String!
+  meta: JSON!
+  project: GraphQLProject!
+}
+
 type GraphQLAssay {
   id: Int!
   type: String!
   meta: JSON!
   externalIds: JSON!
   sample: GraphQLSample!
 }
@@ -105,14 +125,15 @@
 }
 
 type GraphQLProject {
   id: Int!
   name: String!
   dataset: String!
   meta: JSON!
+  analysisRunner(arGuid: StrGraphQLFilter = null, author: StrGraphQLFilter = null, repository: StrGraphQLFilter = null, accessLevel: StrGraphQLFilter = null, environment: StrGraphQLFilter = null): [GraphQLAnalysisRunner!]!
   pedigree(internalFamilyIds: [Int!] = null, replaceWithParticipantExternalIds: Boolean! = true, replaceWithFamilyExternalIds: Boolean! = true, includeParticipantsNotInFamilies: Boolean! = false, emptyParticipantValue: String = null): [JSON!]!
   families: [GraphQLFamily!]!
   participants: [GraphQLParticipant!]!
   samples(type: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, id: StrGraphQLFilter = null, meta: JSON = null): [GraphQLSample!]!
   sequencingGroups(id: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
   analyses(type: StrGraphQLFilter = null, status: AnalysisStatusGraphQLFilter = null, active: BoolGraphQLFilter = null, meta: JSON = null, timestampCompleted: DatetimeGraphQLFilter = null): [GraphQLAnalysis!]!
 }
@@ -162,14 +183,15 @@
   project(name: String!): GraphQLProject!
   sample(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null, type: StrGraphQLFilter = null, meta: JSON = null, externalId: StrGraphQLFilter = null, participantId: IntGraphQLFilter = null, active: BoolGraphQLFilter = null): [GraphQLSample!]!
   sequencingGroups(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null, sampleId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
   assay(id: Int!): GraphQLAssay!
   participant(id: Int!): GraphQLParticipant!
   family(familyId: Int!): GraphQLFamily!
   myProjects: [GraphQLProject!]!
+  analysisRunner(arGuid: String!): GraphQLAnalysisRunner!
 }
 
 """Filter for GraphQL queries"""
 input StrGraphQLFilter {
   eq: String = null
   in_: [String!] = null
   nin: [String!] = null
```

### Comparing `metamist-6.8.0/metamist/model/analysis.py` & `metamist-6.9.0/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/analysis_query_model.py` & `metamist-6.9.0/metamist/model/analysis_query_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/analysis_status.py` & `metamist-6.9.0/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/analysis_update_model.py` & `metamist-6.9.0/metamist/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/assay.py` & `metamist-6.9.0/metamist/model/assay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/assay_upsert.py` & `metamist-6.9.0/metamist/model/assay_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_column.py` & `metamist-6.9.0/metamist/model/billing_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_cost_budget_record.py` & `metamist-6.9.0/metamist/model/billing_cost_budget_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_cost_details_record.py` & `metamist-6.9.0/metamist/model/billing_cost_details_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_hail_batch_cost_record.py` & `metamist-6.9.0/metamist/model/web_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class BillingHailBatchCostRecord(ModelNormal):
+class WebProject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,39 +77,47 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'ar_guid': (str,),  # noqa: E501
-            'batch_ids': ([str],),  # noqa: E501
-            'costs': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'dataset': (str,),  # noqa: E501
+            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'ar_guid': 'ar_guid',  # noqa: E501
-        'batch_ids': 'batch_ids',  # noqa: E501
-        'costs': 'costs',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'dataset': 'dataset',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingHailBatchCostRecord - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
+        """WebProject - a model defined in OpenAPI
+
+        Args:
+            id (int):
+            name (str):
+            dataset (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +142,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ar_guid (str): [optional]  # noqa: E501
-            batch_ids ([str]): [optional]  # noqa: E501
-            costs ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,14 +169,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
+        self.dataset = dataset
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,16 +193,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingHailBatchCostRecord - a model defined in OpenAPI
+    def __init__(self, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
+        """WebProject - a model defined in OpenAPI
+
+        Args:
+            id (int):
+            name (str):
+            dataset (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,17 +233,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ar_guid (str): [optional]  # noqa: E501
-            batch_ids ([str]): [optional]  # noqa: E501
-            costs ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -246,14 +258,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
+        self.dataset = dataset
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.8.0/metamist/model/billing_source.py` & `metamist-6.9.0/metamist/model/billing_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_time_column.py` & `metamist-6.9.0/metamist/model/billing_time_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_time_periods.py` & `metamist-6.9.0/metamist/model/billing_time_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_total_cost_query_model.py` & `metamist-6.9.0/metamist/model/billing_total_cost_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/billing_total_cost_record.py` & `metamist-6.9.0/metamist/model/billing_total_cost_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/body_get_assays_by_criteria.py` & `metamist-6.9.0/metamist/model/body_get_assays_by_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-6.9.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/body_get_participants.py` & `metamist-6.9.0/metamist/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/body_get_proportionate_map.py` & `metamist-6.9.0/metamist/model/body_get_proportionate_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/body_get_samples.py` & `metamist-6.9.0/metamist/model/body_get_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/error_response.py` & `metamist-6.9.0/metamist/model/error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/export_type.py` & `metamist-6.9.0/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/extra_participant_importer_handler.py` & `metamist-6.9.0/metamist/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/family_search_response_data.py` & `metamist-6.9.0/metamist/model/family_search_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/family_simple.py` & `metamist-6.9.0/metamist/model/family_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/family_update_model.py` & `metamist-6.9.0/metamist/model/family_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/http_validation_error.py` & `metamist-6.9.0/metamist/model/http_validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/meta_search_entity_prefix.py` & `metamist-6.9.0/metamist/model/meta_search_entity_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/nested_participant.py` & `metamist-6.9.0/metamist/model/nested_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/nested_sample.py` & `metamist-6.9.0/metamist/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/nested_sequencing_group.py` & `metamist-6.9.0/metamist/model/nested_sequencing_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/paging_links.py` & `metamist-6.9.0/metamist/model/paging_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/participant_search_response_data.py` & `metamist-6.9.0/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/participant_upsert.py` & `metamist-6.9.0/metamist/model/participant_upsert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/project.py` & `metamist-6.9.0/metamist/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/project_summary.py` & `metamist-6.9.0/metamist/model/project_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/proportional_date_temporal_method.py` & `metamist-6.9.0/metamist/model/proportional_date_temporal_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/sample_search_response_data.py` & `metamist-6.9.0/metamist/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/sample_upsert.py` & `metamist-6.9.0/metamist/model/sample_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/search_item.py` & `metamist-6.9.0/metamist/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/search_response.py` & `metamist-6.9.0/metamist/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/search_response_model.py` & `metamist-6.9.0/metamist/model/search_response_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/search_response_type.py` & `metamist-6.9.0/metamist/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/sequencing_group_meta_update_model.py` & `metamist-6.9.0/metamist/model/sequencing_group_meta_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/sequencing_group_search_response_data.py` & `metamist-6.9.0/metamist/model/sequencing_group_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/sequencing_group_upsert.py` & `metamist-6.9.0/metamist/model/sequencing_group_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/validation_error.py` & `metamist-6.9.0/metamist/model/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.8.0/metamist/model/web_project.py` & `metamist-6.9.0/metamist/model/analysis_cost_record_sku.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class WebProject(ModelNormal):
+class AnalysisCostRecordSku(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,47 +77,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'dataset': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'sku': (str,),  # noqa: E501
+            'cost': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'dataset': 'dataset',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
+        'sku': 'sku',  # noqa: E501
+        'cost': 'cost',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
-        """WebProject - a model defined in OpenAPI
+    def _from_openapi_data(cls, sku, cost, *args, **kwargs):  # noqa: E501
+        """AnalysisCostRecordSku - a model defined in OpenAPI
 
         Args:
-            id (int):
-            name (str):
-            dataset (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            sku (str):
+            cost (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -169,18 +163,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
-        self.dataset = dataset
-        self.meta = meta
+        self.sku = sku
+        self.cost = cost
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,22 +185,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
-        """WebProject - a model defined in OpenAPI
+    def __init__(self, sku, cost, *args, **kwargs):  # noqa: E501
+        """AnalysisCostRecordSku - a model defined in OpenAPI
 
         Args:
-            id (int):
-            name (str):
-            dataset (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            sku (str):
+            cost (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,18 +248,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
-        self.dataset = dataset
-        self.meta = meta
+        self.sku = sku
+        self.cost = cost
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.8.0/metamist/model_utils.py` & `metamist-6.9.0/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-6.8.0/metamist/parser/cloudhelper.py` & `metamist-6.9.0/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/parser/generic_metadata_parser.py` & `metamist-6.9.0/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/parser/generic_parser.py` & `metamist-6.9.0/metamist/parser/generic_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,15 @@
             output=self.output,
             sequencing_group_ids=[self.sequencing_group.internal_seqgroup_id],
         )
 
 
 class DefaultSequencing:
     """Groups default sequencing information"""
+
     def __init__(
         self,
         seq_type: str = 'genome',  # seq_type because `type` is a built-in
         technology: str = 'short-read',
         platform: str = 'illumina',
         facility: str = None,
         library: str = None,
@@ -530,14 +531,17 @@
         """
         Asynchronously parse rows of data, adding chunks of participants, samples, sequencing groups, assays, and analyses.
 
         Groups rows of participants by their IDs. For each participant, group samples by their IDs.
         If no participants are present, groups samples by their IDs.
         For each sample, gets its sequencing groups by their keys. For each sequencing group, groups assays and analyses.
         """
+        if not isinstance(rows, list):
+            rows = [rows]
+
         await self.validate_rows(rows)
 
         # one participant with no value
         participants = []
         if self.has_participants(rows):
             # start with participants
             participants = await self.group_participants(rows)
@@ -692,16 +696,20 @@
 
         return summary
 
     def prepare_detail(self, samples: list[ParsedSample]):
         """Uses tabulate to print a detailed summary of the samples being inserted / updated"""
         sample_participants = {}
         for sample in samples:
-            sample_participants[sample.external_sid] = sample.participant.external_pid if sample.participant else None
-        sample_sequencing_groups = {sample.external_sid: sample.sequencing_groups for sample in samples}
+            sample_participants[sample.external_sid] = (
+                sample.participant.external_pid if sample.participant else None
+            )
+        sample_sequencing_groups = {
+            sample.external_sid: sample.sequencing_groups for sample in samples
+        }
 
         details = []
         for sample, participant in sample_participants.items():
             for sg in sample_sequencing_groups[sample]:
                 sg_details = {
                     'Participant': participant if participant else '',
                     'Sample': sample,
@@ -739,15 +747,17 @@
         for a in assays:
             assays_count[str(a.meta.get('sequencing_type'))] += 1
             assays_types_count[str(a.assay_type)] += 1
         for sg in sequencing_groups:
             sequencing_group_counts[str(sg.sequencing_type)] += 1
 
         str_assay_count = ', '.join(f'{k}={v}' for k, v in assays_count.items())
-        str_assay_types_count = ', '.join(f'{k}={v}' for k, v in assays_types_count.items())
+        str_assay_types_count = ', '.join(
+            f'{k}={v}' for k, v in assays_types_count.items()
+        )
         str_seqg_count = ', '.join(
             f'{k}={v}' for k, v in sequencing_group_counts.items()
         )
 
         message = f"""\
 
 
@@ -1000,15 +1010,17 @@
 
         invalid_keys = [k for k, v in keys if v is None]
         if invalid_keys:
             raise ValueError(f'Invalid sequencing group key: {invalid_keys}')
 
         return tuple(v for _, v in keys)
 
-    async def get_sample_sequencing_groups(self, sample: ParsedSample) -> list[ParsedSequencingGroup]:
+    async def get_sample_sequencing_groups(
+        self, sample: ParsedSample
+    ) -> list[ParsedSequencingGroup]:
         """
         From a set of samples, group (by calling self.get_sequencing_group_key)
         and parse sequencing groups and their values.
         """
         sequencing_groups = []
         for seq_rows in group_by(sample.rows, self.get_sequencing_group_key).values():
             seq_type = self.get_sequencing_type(seq_rows[0])
@@ -1062,15 +1074,20 @@
         From a list of assays, get any relevant sequencing group meta
         """
         meta = {}
         for assay in assays:
             if assay.meta.get('sequencing_type') == 'exome':
                 keys = ('sequencing_facility', 'sequencing_library')
             elif assay.meta.get('sequencing_type') in RNA_SEQ_TYPES:
-                keys = ('sequencing_facility', 'sequencing_library', 'read_end_type', 'read_length')
+                keys = (
+                    'sequencing_facility',
+                    'sequencing_library',
+                    'read_end_type',
+                    'read_length',
+                )
             else:
                 continue
             for key in keys:
                 if assay.meta.get(key) is not None:
                     meta[key] = assay.meta[key]
         return meta
```

### Comparing `metamist-6.8.0/metamist/parser/sample_file_map_parser.py` & `metamist-6.9.0/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/metamist/rest.py` & `metamist-6.9.0/metamist/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.8.0
+    The version of the OpenAPI document: 6.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-6.8.0/metamist.egg-info/PKG-INFO` & `metamist-6.9.0/metamist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.8.0
+Version: 6.9.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.8.0/metamist.egg-info/SOURCES.txt` & `metamist-6.9.0/metamist.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 metamist.egg-info/dependency_links.txt
 metamist.egg-info/entry_points.txt
 metamist.egg-info/not-zip-safe
 metamist.egg-info/requires.txt
 metamist.egg-info/top_level.txt
 metamist/api/__init__.py
 metamist/api/analysis_api.py
+metamist/api/analysis_runner_api.py
 metamist/api/assay_api.py
 metamist/api/billing_api.py
 metamist/api/enums_api.py
 metamist/api/family_api.py
 metamist/api/import_api.py
 metamist/api/participant_api.py
 metamist/api/project_api.py
@@ -35,23 +36,33 @@
 metamist/audit/audithelper.py
 metamist/audit/delete_assay_files_from_audit.py
 metamist/audit/generic_auditor.py
 metamist/graphql/__init__.py
 metamist/graphql/schema.graphql
 metamist/model/__init__.py
 metamist/model/analysis.py
+metamist/model/analysis_cost_record.py
+metamist/model/analysis_cost_record_batch.py
+metamist/model/analysis_cost_record_batch_job.py
+metamist/model/analysis_cost_record_category.py
+metamist/model/analysis_cost_record_cromwell_subworkflow.py
+metamist/model/analysis_cost_record_cromwell_workflow.py
+metamist/model/analysis_cost_record_seq_group.py
+metamist/model/analysis_cost_record_sku.py
+metamist/model/analysis_cost_record_topic.py
+metamist/model/analysis_cost_record_total.py
+metamist/model/analysis_cost_record_wdl_task.py
 metamist/model/analysis_query_model.py
 metamist/model/analysis_status.py
 metamist/model/analysis_update_model.py
 metamist/model/assay.py
 metamist/model/assay_upsert.py
 metamist/model/billing_column.py
 metamist/model/billing_cost_budget_record.py
 metamist/model/billing_cost_details_record.py
-metamist/model/billing_hail_batch_cost_record.py
 metamist/model/billing_source.py
 metamist/model/billing_time_column.py
 metamist/model/billing_time_periods.py
 metamist/model/billing_total_cost_query_model.py
 metamist/model/billing_total_cost_record.py
 metamist/model/body_get_assays_by_criteria.py
 metamist/model/body_get_latest_complete_analysis_for_type_post.py
@@ -77,34 +88,47 @@
 metamist/model/proportional_date_temporal_method.py
 metamist/model/sample_search_response_data.py
 metamist/model/sample_upsert.py
 metamist/model/search_item.py
 metamist/model/search_response.py
 metamist/model/search_response_model.py
 metamist/model/search_response_type.py
+metamist/model/seqr_dataset_type.py
 metamist/model/sequencing_group_meta_update_model.py
 metamist/model/sequencing_group_search_response_data.py
 metamist/model/sequencing_group_upsert.py
 metamist/model/validation_error.py
 metamist/model/web_project.py
 metamist/models/__init__.py
 metamist/parser/__init__.py
 metamist/parser/cloudhelper.py
 metamist/parser/generic_metadata_parser.py
 metamist/parser/generic_parser.py
 metamist/parser/sample_file_map_parser.py
 test/test_analysis.py
+test/test_analysis_runner.py
+test/test_api_billing.py
+test/test_api_utils.py
 test/test_assay.py
 test/test_audit_log.py
+test/test_bq_billing_ar_batch.py
+test/test_bq_billing_base.py
+test/test_bq_billing_daily.py
+test/test_bq_billing_daily_extended.py
+test/test_bq_billing_gcp_daily.py
+test/test_bq_billing_raw.py
+test/test_bq_function_filter.py
+test/test_bq_generic_filter.py
 test/test_generate_data.py
 test/test_generic_auditor.py
 test/test_generic_filters.py
 test/test_get_participants.py
 test/test_graphql.py
 test/test_import_individual_metadata.py
+test/test_layers_billing.py
 test/test_metamist.py
 test/test_models.py
 test/test_parse_existing_cohort.py
 test/test_parse_file_map.py
 test/test_parse_generic_metadata.py
 test/test_parse_ont_processor.py
 test/test_parse_ont_sheet.py
@@ -112,8 +136,9 @@
 test/test_project_groups.py
 test/test_sample.py
 test/test_search.py
 test/test_sequencing_groups.py
 test/test_update_participant_family.py
 test/test_upsert.py
 test/test_web.py
-test/testbase.py
+test/testbase.py
+test/testbqbase.py
```

### Comparing `metamist-6.8.0/pyproject.toml` & `metamist-6.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/setup.py` & `metamist-6.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.8.0',
+    version='6.9.0',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/metamist',
     license='MIT',
     packages=all_packages,
     install_requires=[
+        'backoff>=2.2.1',
         'click',
         'google-auth',
         'google-api-core',  # dependency to google-auth that however is not
         # pulled automatically: https://github.com/googleapis/google-auth-library-python/blob/main/setup.py#L22-L27
         'urllib3 >= 1.25.3',
         'python-dateutil',
         'requests',
```

### Comparing `metamist-6.8.0/test/test_analysis.py` & `metamist-6.9.0/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_assay.py` & `metamist-6.9.0/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_audit_log.py` & `metamist-6.9.0/test/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_generate_data.py` & `metamist-6.9.0/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_generic_auditor.py` & `metamist-6.9.0/test/test_generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_generic_filters.py` & `metamist-6.9.0/test/test_generic_filters.py`

 * *Files 27% similar despite different names*

```diff
@@ -49,7 +49,58 @@
         """
         value = [1, 2]
         filter_ = GenericFilterTest(test_int=GenericFilter(in_=value))
         sql, values = filter_.to_sql()
 
         self.assertEqual('test_int IN :test_int_in', sql)
         self.assertDictEqual({'test_int_in': value}, values)
+
+    def test_gt_single(self):
+        """
+        Test that a single value filtered using the "gt" operator
+        """
+        filter_ = GenericFilterTest(test_int=GenericFilter(gt=123))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_int > :test_int_gt', sql)
+        self.assertDictEqual({'test_int_gt': 123}, values)
+
+    def test_gte_single(self):
+        """
+        Test that a single value filtered using the "gte" operator
+        """
+        filter_ = GenericFilterTest(test_int=GenericFilter(gte=123))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_int >= :test_int_gte', sql)
+        self.assertDictEqual({'test_int_gte': 123}, values)
+
+    def test_lt_single(self):
+        """
+        Test that a single value filtered using the "lt" operator
+        """
+        filter_ = GenericFilterTest(test_int=GenericFilter(lt=123))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_int < :test_int_lt', sql)
+        self.assertDictEqual({'test_int_lt': 123}, values)
+
+    def test_lte_single(self):
+        """
+        Test that a single value filtered using the "lte" operator
+        """
+        filter_ = GenericFilterTest(test_int=GenericFilter(lte=123))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_int <= :test_int_lte', sql)
+        self.assertDictEqual({'test_int_lte': 123}, values)
+
+    def test_not_in_multiple(self):
+        """
+        Test that values filtered using the "nin" operator convert as expected
+        """
+        value = [1, 2]
+        filter_ = GenericFilterTest(test_int=GenericFilter(nin=value))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_int NOT IN :test_int_nin', sql)
+        self.assertDictEqual({'test_int_nin': value}, values)
```

### Comparing `metamist-6.8.0/test/test_get_participants.py` & `metamist-6.9.0/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_graphql.py` & `metamist-6.9.0/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_import_individual_metadata.py` & `metamist-6.9.0/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_metamist.py` & `metamist-6.9.0/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_models.py` & `metamist-6.9.0/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_parse_existing_cohort.py` & `metamist-6.9.0/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_parse_file_map.py` & `metamist-6.9.0/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_parse_generic_metadata.py` & `metamist-6.9.0/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_parse_ont_processor.py` & `metamist-6.9.0/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_parse_ont_sheet.py` & `metamist-6.9.0/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_pedigree.py` & `metamist-6.9.0/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_project_groups.py` & `metamist-6.9.0/test/test_project_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_sample.py` & `metamist-6.9.0/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_search.py` & `metamist-6.9.0/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_sequencing_groups.py` & `metamist-6.9.0/test/test_sequencing_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,11 +131,11 @@
             sample.sequencing_groups[0].id
         )
         # now check the existing sequencing group was archived
         self.assertTrue(old_sg.archived)
 
         # check that the "active" sequencing group is the new one
         active_sgs = await self.sglayer.query(
-            SequencingGroupFilter(sample_id=GenericFilter(sample.id))
+            SequencingGroupFilter(sample_id=GenericFilter(eq=sample.id))
         )
         self.assertEqual(len(active_sgs), 1)
         self.assertEqual(updated_sample.sequencing_groups[0].id, active_sgs[0].id)
```

### Comparing `metamist-6.8.0/test/test_update_participant_family.py` & `metamist-6.9.0/test/test_update_participant_family.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_upsert.py` & `metamist-6.9.0/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.8.0/test/test_web.py` & `metamist-6.9.0/test/test_web.py`

 * *Files 10% similar despite different names*

```diff
@@ -217,26 +217,26 @@
             sample_keys=[],
             sequencing_group_keys=[],
             assay_keys=[],
             seqr_links={},
             seqr_sync_types=[],
         )
 
-        self.assertEqual(expected, result)
+        self.assertDataclassEqual(expected, result)
 
     @run_as_sync
     async def test_project_summary_single_entry(self):
         """Test project summary with a single participant with all fields"""
         # Now add a participant with a sample and sequence
         await self.partl.upsert_participants(participants=[get_test_participant()])
 
         result = await self.webl.get_project_summary(token=0, grid_filter=[])
 
         result.participants = []
-        self.assertEqual(SINGLE_PARTICIPANT_RESULT, result)
+        self.assertDataclassEqual(SINGLE_PARTICIPANT_RESULT, result)
 
     @run_as_sync
     async def test_project_summary_to_external(self):
         """Test project summary to_external function"""
         # Now add a participant with a sample and sequence
         await self.partl.upsert_participants(participants=[get_test_participant()])
 
@@ -285,15 +285,15 @@
                     query='M001',
                     field='batch',
                     is_meta=True,
                 )
             ],
         )
         filtered_result_success.participants = []
-        self.assertEqual(SINGLE_PARTICIPANT_RESULT, filtered_result_success)
+        self.assertDataclassEqual(SINGLE_PARTICIPANT_RESULT, filtered_result_success)
 
     @run_as_sync
     async def project_summary_with_filter_no_results(self):
         """Project grid but with test filter, that doesn't have results"""
         filtered_result_empty = await self.webl.get_project_summary(
             token=0,
             grid_filter=[
@@ -319,15 +319,15 @@
             sample_keys=[],
             sequencing_group_keys=[],
             assay_keys=[],
             seqr_links={},
             seqr_sync_types=[],
         )
 
-        self.assertEqual(empty_result, filtered_result_empty)
+        self.assertDataclassEqual(empty_result, filtered_result_empty)
 
     @run_as_sync
     async def test_project_summary_multiple_participants(self):
         """Try with multiple participants as some extra security"""
         await self.partl.upsert_participants(
             participants=[get_test_participant(), get_test_participant_2()]
         )
@@ -372,15 +372,15 @@
 
         two_samples_result = await self.webl.get_project_summary(
             token=0, grid_filter=[]
         )
 
         two_samples_result.participants = []
 
-        self.assertEqual(expected_data_two_samples, two_samples_result)
+        self.assertDataclassEqual(expected_data_two_samples, two_samples_result)
 
     @run_as_sync
     async def test_project_summary_multiple_participants_and_filter(self):
         """Try with multiple participants as some extra security"""
         await self.partl.upsert_participants(
             participants=[get_test_participant(), get_test_participant_2()]
         )
@@ -432,15 +432,15 @@
                     field='external_id',
                     is_meta=False,
                 )
             ],
         )
         two_samples_result_filtered.participants = []
 
-        self.assertEqual(
+        self.assertDataclassEqual(
             expected_data_two_samples_filtered, two_samples_result_filtered
         )
 
     @run_as_sync
     async def test_field_with_space(self):
         """Test filtering on a meta field with spaces"""
         await self.partl.upsert_participants(
@@ -495,15 +495,17 @@
                 ('meta.field with spaces', 'field with spaces'),
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
 
-        self.assertEqual(expected_data_two_samples_filtered, test_field_with_space)
+        self.assertDataclassEqual(
+            expected_data_two_samples_filtered, test_field_with_space
+        )
 
     @run_as_sync
     async def test_project_summary_inactive_sequencing_group(self):
         """
         Insert a sequencing-group, archive it, then check that the summary
         doesn't return that sequencing group
         """
```

### Comparing `metamist-6.8.0/test/testbase.py` & `metamist-6.9.0/test/testbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=invalid-overridden-method
 
 import asyncio
+import dataclasses
 import logging
 import os
 import socket
 import subprocess
 import unittest
 from functools import wraps
 from typing import Dict
@@ -92,40 +93,40 @@
             but that certainly has a host of its own problems.
 
             Then you can destroy the database within tearDownClass as all tests have been completed.
             """
             logger = logging.getLogger()
             try:
                 set_all_access(True)
-                db = MySqlContainer('mariadb:10.8.3')
+                db = MySqlContainer('mariadb:11.2.2')
                 port_to_expose = find_free_port()
                 # override the default port to map the container to
-                db.with_bind_ports(db.port_to_expose, port_to_expose)
+                db.with_bind_ports(db.port, port_to_expose)
                 logger.disabled = True
                 db.start()
                 logger.disabled = False
                 cls.dbs[cls.__name__] = db
 
                 db_prefix = 'db'
                 if am_i_in_test_environment:
                     db_prefix = '../db'
 
                 con_string = db.get_connection_url()
                 con_string = 'mysql://' + con_string.split('://', maxsplit=1)[1]
-                lcon_string = f'jdbc:mariadb://{db.get_container_host_ip()}:{port_to_expose}/{db.MYSQL_DATABASE}'
+                lcon_string = f'jdbc:mariadb://{db.get_container_host_ip()}:{port_to_expose}/{db.dbname}'
                 # apply the liquibase schema
                 command = [
                     'liquibase',
                     *('--changeLogFile', db_prefix + '/project.xml'),
                     *('--defaultsFile', db_prefix + '/liquibase.properties'),
                     *('--url', lcon_string),
                     *('--driver', 'org.mariadb.jdbc.Driver'),
                     *('--classpath', db_prefix + '/mariadb-java-client-3.0.3.jar'),
-                    *('--username', db.MYSQL_USER),
-                    *('--password', db.MYSQL_PASSWORD),
+                    *('--username', db.username),
+                    *('--password', db.password),
                     'update',
                 ]
                 subprocess.check_output(command, stderr=subprocess.STDOUT)
 
                 sm_db = SMConnections.make_connection(
                     ConnectionStringDatabaseConfiguration(con_string)
                 )
@@ -171,15 +172,15 @@
 
         return setup()
 
     @classmethod
     def tearDownClass(cls) -> None:
         db = cls.dbs.get(cls.__name__)
         if db:
-            db.exec(f'DROP DATABASE {db.MYSQL_DATABASE};')
+            db.exec(f'DROP DATABASE {db.dbname};')
             db.stop()
 
     def setUp(self) -> None:
         self._connection = self.connections[self.__class__.__name__]
         # create a connection on each test so we can generate a new
         # audit_log ID for each test
         self.connection = Connection(
@@ -220,14 +221,27 @@
             raise value.errors[0]
         return value.data
 
     async def audit_log_id(self):
         """Get audit_log_id for the test"""
         return await self.connection.audit_log_id()
 
+    def assertDataclassEqual(self, a, b):
+        """Assert two dataclasses are equal"""
+
+        def to_dict(obj):
+            d = dataclasses.asdict(obj)
+            for k, v in d.items():
+                if dataclasses.is_dataclass(v):
+                    d[k] = to_dict(v)
+            return d
+
+        self.maxDiff = None
+        self.assertDictEqual(to_dict(a), to_dict(b))
+
 
 class DbIsolatedTest(DbTest):
     """
     Database integration tests that performs clean-up at the start of each test
     """
 
     @run_as_sync
```

