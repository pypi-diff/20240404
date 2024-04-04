# Comparing `tmp/cumulus_library-1.4.1.tar.gz` & `tmp/cumulus_library-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-1.4.1.tar` & `cumulus_library-2.0.0.tar`

### file list

```diff
@@ -1,76 +1,98 @@
-lrwxr-xr-x   0        0        0        0 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      689 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/README.md
--rw-r--r--   0        0        0     1909 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       45 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/__init__.py
--rw-r--r--   0        0        0     3389 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/base_table_builder.py
--rwxr-xr-x   0        0        0    13354 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/cli.py
--rw-r--r--   0        0        0     5715 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      355 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     9487 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     6030 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     1542 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/builder_condition_codeableconcept.py
--rw-r--r--   0        0        0     4511 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/builder_core_medication.py
--rw-r--r--   0        0        0     4171 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/builder_core_medication.sql
--rw-r--r--   0        0        0     5875 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/builder_encounter_coding.py
--rw-r--r--   0        0        0     9739 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/builder_encounter_coding.sql
--rw-r--r--   0        0        0     1399 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/builder_patient_extension.py
--rw-r--r--   0        0        0     3138 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     3512 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/condition_codeable_concept.sql
--rw-r--r--   0        0        0     3370 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/count_core.py
--rw-r--r--   0        0        0     7562 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/count_core.sql
--rw-r--r--   0        0        0     2995 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     2302 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     1466 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/encounter_type.sql
--rw-r--r--   0        0        0      947 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/fhir_lookup_tables.sql
--rw-r--r--   0        0        0     4891 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/fhir_mapping_tables.sql
--rw-r--r--   0        0        0     1039 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1217 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1195 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2943 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1246 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1198 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     6443 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/patient_extensions.sql
--rw-r--r--   0        0        0     1440 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1961 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0       69 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/core/version.sql
--rw-r--r--   0        0        0     1638 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/discovery/code_definitions.py
--rw-r--r--   0        0        0     3227 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/discovery/code_detection.py
--rw-r--r--   0        0        0     2923 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/discovery/code_detection.sql
--rw-r--r--   0        0        0      160 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/discovery/manifest.toml
--rw-r--r--   0        0        0      836 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1835 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2023-10-26 14:22:29.017325 cumulus_library-1.4.1/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2023-10-26 14:22:29.061326 cumulus_library-1.4.1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2023-10-26 14:22:29.181329 cumulus_library-1.4.1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      410 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      145 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     3346 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    19609 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/study_parser.py
--rw-r--r--   0        0        0     1281 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/code_system_pairs.sql.jinja
--rw-r--r--   0        0        0     1998 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0      176 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/column_datatype.sql.jinja
--rw-r--r--   0        0        0     5879 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/core_medication.sql.jinja
--rw-r--r--   0        0        0     3175 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/count.sql.jinja
--rw-r--r--   0        0        0      601 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      634 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0      508 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/ctas_empty.sql.jinja
--rw-r--r--   0        0        0       61 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     2464 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      372 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0      439 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/is_table_not_empty.sql.jinja
--rw-r--r--   0        0        0       52 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       56 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0    13683 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     5669 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/template_sql/utils.py
--rw-r--r--   0        0        0     3311 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/cumulus_library/upload.py
--rw-r--r--   0        0        0     1304 2023-10-26 14:22:29.189329 cumulus_library-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1927 1970-01-01 00:00:00.000000 cumulus_library-1.4.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      689 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/README.md
+-rw-r--r--   0        0        0     6523 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       46 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/__init__.py
+-rw-r--r--   0        0        0     4837 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/base_table_builder.py
+-rw-r--r--   0        0        0     2898 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/base_utils.py
+-rwxr-xr-x   0        0        0    17396 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/cli.py
+-rw-r--r--   0        0        0     7633 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0    14588 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/databases.py
+-rw-r--r--   0        0        0      422 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/enums.py
+-rw-r--r--   0        0        0      523 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/errors.py
+-rw-r--r--   0        0        0      205 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2311 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0     1716 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/protected_table_builder.py
+-rw-r--r--   0        0        0        0 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4731 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3364 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6024 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0    10722 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/counts.py
+-rw-r--r--   0        0        0    14371 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/psm.py
+-rw-r--r--   0        0        0     5136 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/psm.sql
+-rw-r--r--   0        0        0     7541 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/count.sql.jinja
+-rw-r--r--   0        0        0     2311 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/counts_templates.py
+-rw-r--r--   0        0        0     1606 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
+-rw-r--r--   0        0        0      363 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
+-rw-r--r--   0        0        0     3272 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_templates.py
+-rw-r--r--   0        0        0     2943 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_condition.py
+-rw-r--r--   0        0        0     2710 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_documentreference.py
+-rw-r--r--   0        0        0     4562 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_encounter.py
+-rw-r--r--   0        0        0     4731 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_medication.py
+-rw-r--r--   0        0        0     2241 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_medicationrequest.py
+-rw-r--r--   0        0        0     2734 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_observation.py
+-rw-r--r--   0        0        0     2039 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_patient.py
+-rw-r--r--   0        0        0      867 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_prereq_tables.py
+-rw-r--r--   0        0        0     2548 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/condition.sql.jinja
+-rw-r--r--   0        0        0      854 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/core_templates.py
+-rw-r--r--   0        0        0     5042 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/core_utils.jinja
+-rw-r--r--   0        0        0     2765 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
+-rw-r--r--   0        0        0     4311 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja
+-rw-r--r--   0        0        0     5984 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medication.sql.jinja
+-rw-r--r--   0        0        0     2058 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
+-rw-r--r--   0        0        0     3331 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/observation.sql.jinja
+-rw-r--r--   0        0        0     1854 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/patient.sql.jinja
+-rw-r--r--   0        0        0     5350 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0      948 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/fhir_lookup_tables.sql
+-rw-r--r--   0        0        0     4879 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/fhir_mapping_tables.sql
+-rw-r--r--   0        0        0      971 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1163 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/observation_type.sql
+-rw-r--r--   0        0        0     7810 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_condition.sql
+-rw-r--r--   0        0        0     5116 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
+-rw-r--r--   0        0        0    16576 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql
+-rw-r--r--   0        0        0     1243 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_medication.sql
+-rw-r--r--   0        0        0     3286 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
+-rw-r--r--   0        0        0     6190 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_observation.sql
+-rw-r--r--   0        0        0     8484 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_patient.sql
+-rw-r--r--   0        0        0     8008 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
+-rw-r--r--   0        0        0    29145 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/count_core.sql
+-rw-r--r--   0        0        0     1440 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     2058 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0       69 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/version.sql
+-rw-r--r--   0        0        0     2580 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/code_definitions.py
+-rw-r--r--   0        0        0     2553 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/code_detection.py
+-rw-r--r--   0        0        0     1978 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
+-rw-r--r--   0        0        0     1618 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
+-rw-r--r--   0        0        0      160 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/manifest.toml
+-rw-r--r--   0        0        0     4377 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql
+-rw-r--r--   0        0        0      863 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     2312 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2024-04-04 12:54:43.434847 cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2024-04-04 12:54:43.514847 cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      410 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      145 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     3227 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    31623 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0       79 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/alias_table.sql.jinja
+-rw-r--r--   0        0        0    11473 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/base_templates.py
+-rw-r--r--   0        0        0     2532 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0     1893 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/coding_denormalize.sql.jinja
+-rw-r--r--   0        0        0      385 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/column_datatype.sql.jinja
+-rw-r--r--   0        0        0      563 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      586 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0      506 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/ctas_empty.sql.jinja
+-rw-r--r--   0        0        0       61 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     2534 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      535 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0      439 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/is_table_not_empty.sql.jinja
+-rw-r--r--   0        0        0       34 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/select_all.sql.jinja
+-rw-r--r--   0        0        0      370 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
+-rw-r--r--   0        0        0      169 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0      163 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0    10628 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/sql_utils.py
+-rw-r--r--   0        0        0     3308 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/upload.py
+-rw-r--r--   0        0        0     2316 2024-04-04 12:54:43.526847 cumulus_library-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 cumulus_library-2.0.0/PKG-INFO
```

### Comparing `cumulus_library-1.4.1/README.md` & `cumulus_library-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/base_table_builder.py` & `cumulus_library-2.0.0/cumulus_library/base_table_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """ abstract base for python-based study executors """
-import re
 
+import pathlib
+import re
+import sys
 from abc import ABC, abstractmethod
 from typing import final
 
-from cumulus_library.helper import get_progress_bar, query_console_output
+from cumulus_library import base_utils
+from cumulus_library.databases import DatabaseCursor
 
 
 class BaseTableBuilder(ABC):
     """Generic base class for python table builders.
 
     To use a table builder, extend this class exactly once in a new module.
     See ./studies/vocab or ./studies/core for example usage.
@@ -16,74 +19,115 @@
 
     display_text = "Building custom tables..."
 
     def __init__(self):
         self.queries = []
 
     @abstractmethod
-    def prepare_queries(self, cursor: object, schema: str):
+    def prepare_queries(self, cursor: object, schema: str, *args, **kwargs):
         """Main entrypoint for python table builders.
 
         When completed, prepare_queries should populate self.queries with sql
         statements to execute. This array will the be read by run queries.
 
         :param cursor: A PEP-249 compatible cursor
         :param schema: A schema name
-        :param verbose: toggle for verbose output mode
         """
         raise NotImplementedError
 
     @final
     def execute_queries(
-        self, cursor: object, schema: str, verbose: bool, drop_table: bool = False
+        self,
+        cursor: DatabaseCursor,
+        schema: str,
+        verbose: bool,
+        *args,
+        drop_table: bool = False,
+        **kwargs,
     ):
         """Executes queries set up by a prepare_queries call
 
         :param cursor: A PEP-249 compatible cursor
         :param schema: A schema name
         :param verbose: toggle for verbose output mode
         :param drop_table: drops any tables found in prepared_queries results
         """
-        self.prepare_queries(cursor, schema)
+        self.prepare_queries(cursor, schema, *args, **kwargs)
         if drop_table:
             table_names = []
             for query in self.queries:
                 # Get the first non-whitespace word after create table
                 table_name = re.search(
                     '(?i)(?<=create table )(([a-zA-Z0-9_".-]+))', query
-                )  # [0]
+                )
+
                 if table_name:
+                    if table_name[0] == "IF":
+                        # Edge case - if we're doing an empty conditional CTAS creation,
+                        # we need to run a slightly different regex
+                        table_name = re.search(
+                            '(?i)(?<=not exists )(([a-zA-Z0-9_".-]+))', query
+                        )
+
                     table_name = table_name[0]
-                    # if it contains a schema, remove it (usually it won't, but some CTAS
-                    # forms may)
+                    # if it contains a schema, remove it (usually it won't, but some
+                    # CTAS forms may)
                     if "." in table_name:
                         table_name = table_name.split(".")[1].replace('"', "")
                     table_names.append(table_name)
             for table_name in table_names:
                 cursor.execute(f"DROP TABLE IF EXISTS {table_name}")
-        with get_progress_bar(disable=verbose) as progress:
+        with base_utils.get_progress_bar(disable=verbose) as progress:
             task = progress.add_task(
                 self.display_text,
                 total=len(self.queries),
                 visible=not verbose,
             )
             for query in self.queries:
-                query_console_output(verbose, query, progress, task)
-                cursor.execute(query)
+                try:
+                    with base_utils.query_console_output(
+                        verbose, query, progress, task
+                    ):
+                        cursor.execute(query)
+                except Exception as e:  # pylint: disable=broad-exception-caught
+                    sys.exit(e)
+
+        self.post_execution(cursor, schema, verbose, drop_table, *args, **kwargs)
+
+    def post_execution(  # noqa: B027 - this looks like, but is not, an abstract method
+        self,
+        cursor: DatabaseCursor,
+        schema: str,
+        verbose: bool,
+        *args,
+        drop_table: bool = False,
+        **kwargs,
+    ):
+        """Hook for any additional actions to run after execute_queries"""
+        pass
 
-    def comment_queries(self):
+    def comment_queries(self, doc_str=None):
         """Convenience method for annotating outputs of template generators to disk"""
         commented_queries = ["-- noqa: disable=all"]
+        if doc_str:
+            commented_queries.append(doc_str)
+            commented_queries.append(
+                "\n-- ###########################################################\n"
+            )
         for query in self.queries:
             commented_queries.append(query)
             commented_queries.append(
-                "\n-- ###########################################################"
+                "\n-- ###########################################################\n"
             )
         commented_queries.pop()
         self.queries = commented_queries
 
-    def write_queries(self, filename: str = "output.sql"):
+    def write_queries(self, path: pathlib.Path | None = None):
         """writes all queries constructed by prepare_queries to disk"""
-        with open(filename, "w", encoding="utf-8") as file:
+        if path is None:
+            path = pathlib.Path.cwd() / "output.sql"
+
+        path.parents[0].mkdir(parents=True, exist_ok=True)
+        with open(path, "w", encoding="utf-8") as file:
             for query in self.queries:
                 file.write(query)
                 file.write("\n")
```

### Comparing `cumulus_library-1.4.1/cumulus_library/cli.py` & `cumulus_library-2.0.0/cumulus_library/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,357 +1,456 @@
 #!/usr/bin/env python3
 """Utility for building/retrieving data views in AWS Athena"""
 
 import json
 import os
+import pathlib
 import sys
 import sysconfig
 
-from pathlib import Path, PosixPath
-from typing import Dict, List, Optional
+import rich
 
-import pyathena
+from cumulus_library import (
+    __version__,
+    base_utils,
+    cli_parser,
+    databases,
+    enums,
+    errors,
+    protected_table_builder,
+    study_parser,
+    upload,
+)
+from cumulus_library.template_sql import base_templates
 
-from pyathena.pandas.cursor import PandasCursor
-from rich.console import Console
-from rich.table import Table
 
-from cumulus_library import __version__
-from cumulus_library.cli_parser import get_parser
-from cumulus_library.study_parser import StudyManifestParser
-from cumulus_library.upload import upload_files
-
-
-# ** Don't delete! **
-# This class isn't used in the rest of the code,
-# but it is used manually as a quick & dirty alternative to the CLI.
-class CumulusEnv:  # pylint: disable=too-few-public-methods
-    """
-    Wrapper for Cumulus Environment vars.
-    Simplifies connections to StudyBuilder without requiring CLI parsing.
-    """
-
-    def __init__(self):
-        self.region = os.environ.get("CUMULUS_LIBRARY_REGION", "us-east-1")
-        self.workgroup = os.environ.get("CUMULUS_LIBRARY_WORKGROUP", "cumulus")
-        self.profile = os.environ.get("CUMULUS_LIBRARY_PROFILE")
-        self.schema_name = os.environ.get("CUMULUS_LIBRARY_DATABASE")
-
-    def get_study_builder(self):
-        """Convenience method for getting athena args from environment"""
-        return StudyBuilder(self.region, self.workgroup, self.profile, self.schema_name)
-
-
-class StudyBuilder:
-    """Class for managing Athena cursors and executing Cumulus queries"""
+class StudyRunner:
+    """Class for managing cursors and executing Cumulus queries"""
 
     verbose = False
     schema_name = None
 
-    def __init__(  # pylint: disable=too-many-arguments
-        self, region: str, workgroup: str, profile: str, schema: str
-    ):
-        connect_kwargs = {}
-        for aws_env_name in [
-            "AWS_ACCESS_KEY_ID",
-            "AWS_SECRET_ACCESS_KEY",
-            "AWS_SESSION_TOKEN",
-        ]:
-            if aws_env_val := os.environ.get(aws_env_name):
-                connect_kwargs[aws_env_name.lower()] = aws_env_val
-        # the profile may not be required, provided the above three AWS env vars
-        # are set. If both are present, the env vars take precedence
-        if profile is not None:
-            connect_kwargs["profile_name"] = profile
-        self.cursor = pyathena.connect(
-            region_name=region,
-            work_group=workgroup,
-            schema_name=schema,
-            **connect_kwargs,
-        ).cursor()
-        self.pandas_cursor = pyathena.connect(
-            region_name=region,
-            work_group=workgroup,
-            schema_name=schema,
-            cursor_class=PandasCursor,
-            **connect_kwargs,
-        ).cursor()
-        self.schema_name = schema
-
-    def reset_data_path(self, study: PosixPath) -> None:
-        """
-        Removes existing exports from a study's local data dir
-        """
-        project_path = Path(__file__).resolve().parents[1]
-        path = Path(f"{str(project_path)}/data_export/{study}/")
-        if path.exists():
-            for file in path.glob("*"):
-                file.unlink()
+    def __init__(self, db: databases.DatabaseBackend, data_path: str):
+        self.db = db
+        self.data_path = data_path
+        self.cursor = db.cursor()
+        self.schema_name = db.schema_name
+
+    def update_transactions(self, prefix: str, status: str):
+        """Adds a record to a study's transactions table"""
+        self.cursor.execute(
+            base_templates.get_insert_into_query(
+                f"{prefix}__{enums.ProtectedTables.TRANSACTIONS.value}",
+                protected_table_builder.TRANSACTIONS_COLS,
+                [
+                    [
+                        prefix,
+                        __version__,
+                        status,
+                        base_utils.get_utc_datetime(),
+                    ]
+                ],
+                {"event_time": "TIMESTAMP"},
+            )
+        )
 
     ### Creating studies
 
-    def clean_study(self, targets: List[str], study_dict, prefix=False) -> None:
+    def clean_study(
+        self,
+        targets: list[str],
+        study_dict: dict,
+        *,
+        stats_clean: bool,
+        prefix: bool = False,
+    ) -> None:
         """Removes study table/views from Athena.
 
         While this is usually not required, since it it done as part of a build,
         this can be useful for cleaning up tables if a study prefix is changed
         for some reason.
 
-        :param target: The study prefix to use for IDing tables to remove"""
+        :param target: The study prefix to use for IDing tables to remove
+        :param study_dict: The dictionary of available study targets
+        :param stats_clean: If true, removes previous stats runs
+        :keyword prefix: If True, does a search by string prefix in place of study name
+        """
         if targets is None or targets == ["all"]:
             sys.exit(
                 "Explicit targets for cleaning not provided. "
                 "Provide one or more explicit study prefixes to remove."
             )
         for target in targets:
             if prefix:
-                parser = StudyManifestParser()
+                parser = study_parser.StudyManifestParser()
                 parser.clean_study(
-                    self.cursor, self.schema_name, self.verbose, prefix=target
+                    self.cursor,
+                    self.schema_name,
+                    verbose=self.verbose,
+                    stats_clean=stats_clean,
+                    prefix=target,
                 )
             else:
-                parser = StudyManifestParser(study_dict[target])
-                parser.clean_study(self.cursor, self.schema_name, self.verbose)
+                parser = study_parser.StudyManifestParser(study_dict[target])
+                parser.clean_study(
+                    self.cursor,
+                    self.schema_name,
+                    verbose=self.verbose,
+                    stats_clean=stats_clean,
+                )
 
     def clean_and_build_study(
-        self, target: PosixPath, continue_from: str = None
+        self,
+        target: pathlib.Path,
+        *,
+        stats_build: bool,
+        continue_from: str | None = None,
     ) -> None:
         """Recreates study views/tables
 
-        :param target: A PosixPath to the study directory
+        :param target: A path to the study directory
+        :param stats_build: if True, forces creation of new stats tables
+        :keyword continue_from: Restart a run from a specific sql file (for dev only)
         """
-        studyparser = StudyManifestParser(target)
-        if not continue_from:
-            studyparser.clean_study(self.cursor, self.schema_name, self.verbose)
-            studyparser.run_table_builder(self.cursor, self.schema_name, self.verbose)
-        studyparser.build_study(self.cursor, self.verbose, continue_from)
-        studyparser.run_counts_builder(self.cursor, self.schema_name, self.verbose)
+        studyparser = study_parser.StudyManifestParser(target, self.data_path)
+        try:
+            if not continue_from:
+                studyparser.run_protected_table_builder(
+                    self.cursor, self.schema_name, verbose=self.verbose
+                )
+                self.update_transactions(studyparser.get_study_prefix(), "started")
+                cleaned_tables = studyparser.clean_study(
+                    self.cursor,
+                    self.schema_name,
+                    verbose=self.verbose,
+                    stats_clean=False,
+                )
+                # If the study hasn't been created before, force stats table generation
+                if len(cleaned_tables) == 0:
+                    stats_build = True
+                studyparser.run_table_builder(
+                    self.cursor,
+                    self.schema_name,
+                    verbose=self.verbose,
+                    parser=self.db.parser(),
+                )
+            else:
+                self.update_transactions(studyparser.get_study_prefix(), "resumed")
+
+            studyparser.build_study(self.cursor, self.verbose, continue_from)
+            studyparser.run_counts_builders(
+                self.cursor, self.schema_name, verbose=self.verbose
+            )
+            studyparser.run_statistics_builders(
+                self.cursor,
+                self.schema_name,
+                verbose=self.verbose,
+                stats_build=stats_build,
+            )
+            self.update_transactions(studyparser.get_study_prefix(), "finished")
 
-    def run_single_table_builder(
-        self, target: PosixPath, table_builder_name: str
+        except errors.StudyManifestFilesystemError as e:
+            # This should be thrown prior to any database connections, so
+            # skipping logging
+            raise e
+        except Exception as e:
+            self.update_transactions(studyparser.get_study_prefix(), "error")
+            raise e
+
+    def run_matching_table_builder(
+        self, target: pathlib.Path, table_builder_name: str
     ) -> None:
         """Runs a single table builder
 
-        :param target: A PosixPath to the study directory
+        :param target: A path to the study directory
+        :param table_builder_name: a builder file referenced in the study's manifest
         """
-        studyparser = StudyManifestParser(target)
-        studyparser.run_single_table_builder(
-            self.cursor, self.schema_name, table_builder_name, self.verbose
+        studyparser = study_parser.StudyManifestParser(target)
+        studyparser.run_matching_table_builder(
+            self.cursor,
+            self.schema_name,
+            table_builder_name,
+            self.verbose,
+            parser=self.db.parser(),
         )
 
-    def clean_and_build_all(self, study_dict: Dict) -> None:
+    def clean_and_build_all(self, study_dict: dict, stats_build: bool) -> None:
         """Builds views for all studies.
 
         NOTE: By design, this method will always exclude the `template` study dir,
         since 99% of the time you don't need a live copy in the database.
 
-        :param study_dict: A dict of PosixPaths
+        :param study_dict: A dict of paths
+        :param stats_build: if True, regen stats tables
         """
         study_dict = dict(study_dict)
         study_dict.pop("template")
         for precursor_study in ["vocab", "core"]:
-            self.clean_and_build_study(study_dict[precursor_study])
+            self.clean_and_build_study(
+                study_dict[precursor_study], stats_build=stats_build
+            )
             study_dict.pop(precursor_study)
         for key in study_dict:
-            self.clean_and_build_study(study_dict[key])
+            self.clean_and_build_study(study_dict[key], stats_build=stats_build)
 
     ### Data exporters
-    def export_study(self, target: PosixPath, data_path: PosixPath) -> None:
+    def export_study(
+        self, target: pathlib.Path, data_path: pathlib.Path, archive: bool
+    ) -> None:
         """Exports aggregates defined in a manifest
 
-        :param target: A PosixPath to the study directory
+        :param target: A path to the study directory
         """
         if data_path is None:
             sys.exit("Missing destination - please provide a path argument.")
-        studyparser = StudyManifestParser(target)
-        studyparser.export_study(self.pandas_cursor, data_path)
+        studyparser = study_parser.StudyManifestParser(target, data_path)
+        studyparser.export_study(self.db, self.schema_name, data_path, archive)
 
-    def export_all(self, study_dict: Dict, data_path: PosixPath):
+    def export_all(self, study_dict: dict, data_path: pathlib.Path, archive: bool):
         """Exports all defined count tables to disk"""
         for key in study_dict.keys():
-            self.export_study(study_dict[key], data_path)
+            self.export_study(study_dict[key], data_path, archive)
+
+    def generate_study_sql(
+        self, target: pathlib.Path, builder: str | None = None
+    ) -> None:
+        """Materializes study sql from templates
+
+        :param target: A path to the study directory
+        :param builder: Specify a single builder to generate sql from
+        """
+        studyparser = study_parser.StudyManifestParser(target)
+        studyparser.run_generate_sql(
+            cursor=self.cursor,
+            schema=self.schema_name,
+            builder=builder,
+            verbose=self.verbose,
+            parser=self.db.parser(),
+        )
+
+    def generate_study_markdown(
+        self,
+        target: pathlib.Path,
+    ) -> None:
+        """Materializes study sql from templates
 
+        :param target: A path to the study directory
+        """
+        studyparser = study_parser.StudyManifestParser(target)
+        studyparser.run_generate_markdown(
+            self.cursor,
+            self.schema_name,
+            verbose=self.verbose,
+            parser=self.db.parser(),
+        )
 
-def get_abs_posix_path(path: str) -> PosixPath:
+
+def get_abs_posix_path(path: str) -> pathlib.Path:
     """Convenience method for handling abs vs rel paths"""
     if path[0] == "/":
-        return Path(path)
+        return pathlib.Path(path)
     else:
-        return Path(Path.cwd(), path)
+        return pathlib.Path(pathlib.Path.cwd(), path)
 
 
 def create_template(path: str) -> None:
     """Creates a manifest in target dir if one doesn't exist"""
     abs_path = get_abs_posix_path(path)
-    manifest_path = Path(abs_path, "manifest.toml")
+    manifest_path = pathlib.Path(abs_path, "manifest.toml")
     if manifest_path.exists():
         sys.exit(f"A manifest.toml already exists at {abs_path}, skipping creation")
     abs_path.mkdir(parents=True, exist_ok=True)
 
     copy_lists = [
         ["studies/template/manifest.toml", "manifest.toml"],
         [".sqlfluff", ".sqlfluff"],
     ]
     for source, dest in copy_lists:
-        source_path = Path(Path(__file__).resolve().parents[0], source)
-        dest_path = Path(abs_path, dest)
+        source_path = pathlib.Path(pathlib.Path(__file__).resolve().parents[0], source)
+        dest_path = pathlib.Path(abs_path, dest)
         dest_path.write_bytes(source_path.read_bytes())
 
 
-def get_study_dict(alt_dir_paths: List) -> Optional[Dict[str, PosixPath]]:
+def get_study_dict(alt_dir_paths: list) -> dict[str, pathlib.Path] | None:
     """Gets valid study targets from ./studies/, and any pip installed studies
 
-    :returns: A list of pathlib.PosixPath objects
+    :returns: A list of Path objects
     """
     manifest_studies = {}
-    cli_path = Path(__file__).resolve().parents[0]
+    cli_path = pathlib.Path(__file__).resolve().parents[0]
 
     # first, we'll get any installed public studies
     with open(
-        Path(cli_path, "./module_allowlist.json"), "r", encoding="utf-8"
+        pathlib.Path(cli_path, "./module_allowlist.json"), encoding="utf-8"
     ) as study_allowlist_json:
         study_allowlist = json.load(study_allowlist_json)["allowlist"]
     site_packages_dir = sysconfig.get_path("purelib")
     for study, subdir in study_allowlist.items():
-        study_path = Path(site_packages_dir, subdir)
+        study_path = pathlib.Path(site_packages_dir, subdir)
         if study_path.exists():
             manifest_studies[study] = study_path
 
     # then we'll get all studies inside the project directory, followed by
     # any user supplied paths last. These take precedence.
-    paths = [Path(cli_path, "studies")]
+    paths = [pathlib.Path(cli_path, "studies")]
     if alt_dir_paths is not None:
         paths = paths + alt_dir_paths
     for path in paths:
         found_studies = get_studies_by_manifest_path(path)
         manifest_studies.update(found_studies)
     return manifest_studies
 
 
-def get_studies_by_manifest_path(path: PosixPath) -> dict:
+def get_studies_by_manifest_path(path: pathlib.Path) -> dict:
     """Recursively search for manifest.toml files from a given path"""
     manifest_paths = {}
     for child_path in path.iterdir():
         if child_path.is_dir():
             manifest_paths.update(get_studies_by_manifest_path(child_path))
         elif child_path.name == "manifest.toml":
             manifest_paths[path.name] = path
     return manifest_paths
 
 
-def run_cli(args: Dict):
+def run_cli(args: dict):
     """Controls which library tasks are run based on CLI arguments"""
+    console = rich.console.Console()
     if args["action"] == "create":
         create_template(args["create_dir"])
 
     elif args["action"] == "upload":
-        upload_files(args)
+        upload.upload_files(args)
 
-    # all other actions require connecting to AWS
+    # all other actions require connecting to the database
     else:
-        builder = StudyBuilder(
-            args["region"],
-            args["workgroup"],
-            args["profile"],
-            args["schema_name"],
-        )
-        if args["verbose"]:
-            builder.verbose = True
-        print("Testing connection to athena...")
-        builder.cursor.execute("SHOW DATABASES")
-
-        study_dict = get_study_dict(args["study_dir"])
-        if "prefix" not in args.keys():
-            if args["target"]:
-                for target in args["target"]:
-                    if target not in study_dict:
-                        sys.exit(
-                            f"{target} was not found in available studies: "
-                            f"{list(study_dict.keys())}.\n\n"
-                            "If you are trying to run a custom study, make sure "
-                            "you include `-s path/to/study/dir` as an arugment."
-                        )
-        if args["action"] == "clean":
-            builder.clean_study(
-                args["target"],
-                study_dict,
-                args["prefix"],
-            )
-        elif args["action"] == "build":
-            if "all" in args["target"]:
-                builder.clean_and_build_all(study_dict)
-            else:
-                for target in args["target"]:
-                    if args["builder"]:
-                        builder.run_single_table_builder(
-                            study_dict[target], args["builder"]
-                        )
-                    else:
-                        builder.clean_and_build_study(
-                            study_dict[target], continue_from=args["continue_from"]
+        db_backend = databases.create_db_backend(args)
+        try:
+            runner = StudyRunner(db_backend, data_path=args.get("data_path"))
+            if args.get("verbose"):
+                runner.verbose = True
+            console.print("[italic] Connecting to database...")
+            runner.cursor.execute("SHOW DATABASES")
+            study_dict = get_study_dict(args["study_dir"])
+            if "prefix" not in args.keys():
+                if args["target"]:
+                    for target in args["target"]:
+                        if target not in study_dict:
+                            sys.exit(
+                                f"{target} was not found in available studies: "
+                                f"{list(study_dict.keys())}.\n\n"
+                                "If you are trying to run a custom study, make sure "
+                                "you include `-s path/to/study/dir` as an arugment."
+                            )
+            if args["action"] == "clean":
+                runner.clean_study(
+                    args["target"],
+                    study_dict,
+                    stats_clean=args["stats_clean"],
+                    prefix=args["prefix"],
+                )
+            elif args["action"] == "build":
+                if "all" in args["target"]:
+                    runner.clean_and_build_all(study_dict, args["stats_build"])
+                else:
+                    for target in args["target"]:
+                        if args["builder"]:
+                            runner.run_matching_table_builder(
+                                study_dict[target], args["builder"]
+                            )
+                        else:
+                            runner.clean_and_build_study(
+                                study_dict[target],
+                                stats_build=args["stats_build"],
+                                continue_from=args["continue_from"],
+                            )
+
+            elif args["action"] == "export":
+                if args["archive"]:
+                    warning_text = (
+                        "🚨[bold red] This will export all study tables [/bold red]🚨"
+                        "\n\nDepending on your study definition, this data may contain "
+                        "data that would be characterized as a [italic]limited data "
+                        "set[/italic], primarily dates, on a per patient level.\n\n"
+                        "[bold]By doing this, you are assuming the responsibility for "
+                        "meeting your organization's security requirements for "
+                        "storing this data in a secure manager.[/bold]\n\n"
+                        "Type Y to proceed, or any other value to quit.\n"
+                    )
+                    console.print(warning_text)
+                    response = input()
+                    if response.lower() != "y":
+                        sys.exit()
+                if "all" in args["target"]:
+                    runner.export_all(study_dict, args["data_path"], args["archive"])
+                else:
+                    for target in args["target"]:
+                        runner.export_study(
+                            study_dict[target], args["data_path"], args["archive"]
                         )
 
-        elif args["action"] == "export":
-            if "all" in args["target"]:
-                builder.export_all(study_dict, args["data_path"])
-            else:
+            elif args["action"] == "generate-sql":
                 for target in args["target"]:
-                    builder.export_study(study_dict[target], args["data_path"])
+                    runner.generate_study_sql(study_dict[target], args["builder"])
 
-        # returning the builder for ease of unit testing
-        return builder
+            elif args["action"] == "generate-md":
+                for target in args["target"]:
+                    runner.generate_study_markdown(study_dict[target])
+        finally:
+            db_backend.close()
 
 
 def main(cli_args=None):
     """Reads CLI input/environment variables and invokes library calls"""
 
-    parser = get_parser()
+    parser = cli_parser.get_parser()
     args = vars(parser.parse_args(cli_args))
     if args["version"]:
         print(__version__)
         sys.exit(0)
     if args["action"] is None:
         parser.print_usage()
         sys.exit(1)
     if args.get("target"):
         for target in args["target"]:
             if target == "all":
                 args["target"] = ["all"]
                 break
 
     arg_env_pairs = (
+        ("db_type", "CUMULUS_LIBRARY_DB_TYPE"),
         ("profile", "CUMULUS_LIBRARY_PROFILE"),
         ("schema_name", "CUMULUS_LIBRARY_DATABASE"),
         ("workgroup", "CUMULUS_LIBRARY_WORKGROUP"),
         ("region", "CUMULUS_LIBRARY_REGION"),
         ("study_dir", "CUMULUS_LIBRARY_STUDY_DIR"),
         ("data_path", "CUMULUS_LIBRARY_DATA_PATH"),
+        ("load_ndjson_dir", "CUMULUS_LIBRARY_LOAD_NDJSON_DIR"),
         ("user", "CUMULUS_AGGREGATOR_USER"),
         ("id", "CUMULUS_AGGREGATOR_ID"),
         ("url", "CUMULUS_AGGREGATOR_URL"),
     )
     read_env_vars = []
     for pair in arg_env_pairs:
         if env_val := os.environ.get(pair[1]):
             if pair[0] == "study_dir":
                 args[pair[0]] = [env_val]
             else:
                 args[pair[0]] = env_val
             read_env_vars.append([pair[1], env_val])
 
     if len(read_env_vars) > 0:
-        table = Table(title="Values read from environment variables")
+        table = rich.table.Table(title="Values read from environment variables")
         table.add_column("Environment Variable", style="green")
         table.add_column("Value", style="cyan")
         for row in read_env_vars:
             if row[0] == "CUMULUS_AGGREGATOR_ID":
                 table.add_row(row[0], "#########")
             else:
                 table.add_row(row[0], row[1])
-        console = Console()
+        console = rich.console.Console()
         console.print(table)
 
     if args.get("study_dir"):
         posix_paths = []
         for path in args["study_dir"]:
             posix_paths.append(get_abs_posix_path(path))
         args["study_dir"] = posix_paths
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cumulus_library-1.4.1/cumulus_library/cli_parser.py` & `cumulus_library-2.0.0/cumulus_library/cli_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manages configuration for argparse"""
+
 import argparse
 
 
 def add_target_argument(parser: argparse.ArgumentParser) -> None:
     """Adds --target arg to a subparser"""
     parser.add_argument(
         "-t",
@@ -17,38 +18,38 @@
     parser.add_argument(
         "--builder",
         help=argparse.SUPPRESS,
     )
 
 
 def add_study_dir_argument(parser: argparse.ArgumentParser) -> None:
-    """Adds --study_dir arg to a subparser"""
+    """Adds --study-dir arg to a subparser"""
     parser.add_argument(
         "-s",
         "--study-dir",
         action="append",
         help=(
             "Optionally add one or more directories to look for study definitions in. "
-            "Default is in project directory and CUMULUS_LIBRARY_STUDY_DIR, if present, "
-            "followed by any supplied paths. Target, and all its subdirectories, "
-            "are checked for manifests. Overriding studies with the same namespace "
-            "supersede earlier ones."
+            "Default is in project directory and CUMULUS_LIBRARY_STUDY_DIR, "
+            "if present, followed by any supplied paths. Target, and all its "
+            "subdirectories, are checked for manifests. Overriding studies with the"
+            " same namespace supersede earlier ones."
         ),
     )
 
 
 def add_data_path_argument(parser: argparse.ArgumentParser) -> None:
     """Adds path arg to a subparser"""
     parser.add_argument(
         "data_path",
         default="./",
         nargs="?",
         help=(
             "The path to use for Athena counts data. "
-            "Can be povided via CUMULUS_LIBRARY_DATA_PATH environment variable."
+            "Can be provided via CUMULUS_LIBRARY_DATA_PATH environment variable."
         ),
     )
 
 
 def add_verbose_argument(parser: argparse.ArgumentParser) -> None:
     """Adds --verbose arg to a subparser"""
     parser.add_argument(
@@ -60,31 +61,52 @@
 
 
 def add_aws_config(parser: argparse.ArgumentParser) -> None:
     """Adds arguments related to aws credentials to a subparser"""
     aws = parser.add_argument_group("AWS config")
     aws.add_argument("--profile", help="AWS profile", default="default")
     aws.add_argument(
-        "--database",
-        # internally, we use PyAthena's terminology for this but the UX term is "database"
-        dest="schema_name",
-        help="Cumulus Athena database name",
-    )
-    aws.add_argument(
         "--workgroup",
         default="cumulus",
         help="Cumulus Athena workgroup (default: cumulus)",
     )
     aws.add_argument(
         "--region",
         help="AWS region data of Athena instance (default: us-east-1)",
         default="us-east-1",
     )
 
 
+def add_db_config(parser: argparse.ArgumentParser) -> None:
+    """Adds arguments related to database backends to a subparser"""
+    group = parser.add_argument_group("Database config")
+    group.add_argument(
+        "--db-type",
+        help="Which database backend to use (default athena)",
+        choices=["athena", "duckdb"],
+        default="athena",
+    )
+    group.add_argument(
+        "--database",
+        # In Athena, we use this as the schema_name (which is also called a Database
+        # in their UX).
+        #
+        # In DuckDB, we use this as the path to the filename to store tables.
+        #
+        # Since we started as an Athena-centric codebase, we mostly keep referring to
+        # this as name "schema_name". But to the user, both uses are still conceptually
+        # a "database".
+        dest="schema_name",
+        help="Database name (for Athena) or file (for DuckDB)",
+    )
+
+    # Backend-specific config:
+    add_aws_config(parser)
+
+
 def get_parser() -> argparse.ArgumentParser:
     """Provides parser for handling CLI arguments"""
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""Generates study tables and views from post-Cumulus ETL data.
 
 cumulus-library will attempt to create a connection to AWS Athena. The
@@ -101,65 +123,82 @@
 
     actions = parser.add_subparsers(
         title="actions",
         help="Available library actions",
         dest="action",
     )
 
-    create = actions.add_parser(
-        "create", help="Create a study instance from a template"
-    )
-    create.add_argument(
-        "create_dir",
-        default="./",
-        nargs="?",
-        help=(
-            "The the directory the study will be created in. Default is "
-            "the current directory."
-        ),
-    )
+    # Database cleaning
 
     clean = actions.add_parser(
         "clean", help="Removes tables & views beginning with '[target]__' from Athena"
     )
 
     add_target_argument(clean)
     add_study_dir_argument(clean)
     add_verbose_argument(clean)
-    add_aws_config(clean)
+    add_db_config(clean)
+    clean.add_argument(
+        "--statistics",
+        action="store_true",
+        help="Remove artifacts of previous statistics runs",
+        dest="stats_clean",
+    )
     clean.add_argument(
         "--prefix",
         action="store_true",
         help=argparse.SUPPRESS,
     )
 
+    # Database building
+
     build = actions.add_parser(
         "build",
         help="Removes and recreates Athena tables & views for specified studies",
     )
     add_target_argument(build)
     add_table_builder_argument(build)
     add_study_dir_argument(build)
     add_verbose_argument(build)
-    add_aws_config(build)
-
+    add_db_config(build)
+    add_data_path_argument(build)
+    build.add_argument(
+        "--statistics",
+        action="store_true",
+        help=(
+            "Force regenerating statistics data from latest dataset. "
+            "Stats are created by default when study is initially run"
+        ),
+        dest="stats_build",
+    )
+    build.add_argument(
+        "--load-ndjson-dir", help="Load ndjson files from this folder", metavar="DIR"
+    )
     build.add_argument(
         "--continue",
         dest="continue_from",
         help=argparse.SUPPRESS,
     )
 
+    # Database export
+
     export = actions.add_parser(
         "export", help="Generates files on disk from Athena views"
     )
     add_target_argument(export)
     add_study_dir_argument(export)
     add_data_path_argument(export)
     add_verbose_argument(export)
-    add_aws_config(export)
+    add_db_config(export)
+    export.add_argument(
+        "--archive",
+        action="store_true",
+        help="Generates archive of :all: study tables, ignoring manifest export list.",
+    )
+    # Aggregator upload
 
     upload = actions.add_parser(
         "upload", help="Bulk uploads data to Cumulus aggregator"
     )
     add_target_argument(upload)
     add_data_path_argument(upload)
     upload.add_argument(
@@ -179,8 +218,27 @@
     upload.add_argument(
         "--preview",
         default=False,
         action="store_true",
         help="Run pre-fetch and prepare upload, but log output instead of sending.",
     )
 
+    # Generate a study's template-driven sql
+    sql = actions.add_parser(
+        "generate-sql", help="Generates a study's template-driven sql for reference"
+    )
+    add_target_argument(sql)
+    add_study_dir_argument(sql)
+    add_db_config(sql)
+    add_table_builder_argument(sql)
+
+    # Generate markdown tables for documentation
+    markdown = actions.add_parser(
+        "generate-md", help="Generates markdown tables for study documentation"
+    )
+    add_target_argument(markdown)
+    add_study_dir_argument(markdown)
+    add_data_path_argument(markdown)
+    add_db_config(markdown)
+    add_verbose_argument(markdown)
+
     return parser
```

### Comparing `cumulus_library-1.4.1/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-2.0.0/cumulus_library/parsers/fhir_valueset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-import os
-from typing import List
-
 from fhirclient.models.coding import Coding
 
-from cumulus_library.helper import load_json
-from cumulus_library.template_sql.templates import get_create_view_query
+from cumulus_library import base_utils
+from cumulus_library.template_sql import base_templates
 
 
-def get_include_coding(valueset_json) -> List[Coding]:
-    """
-    Obtain a list of Coding "concepts" from a ValueSet.
+def get_include_coding(valueset_json) -> list[Coding]:
+    """Obtain a list of Coding "concepts" from a ValueSet.
+
     This method currently supports only "include" of "concept" defined fields.
-    Not supported: recursive fetching of contained ValueSets, which requires UMLS API Key and Wget, etc.
+    Not supported: recursive fetching of contained ValueSets, which requires UMLS
+    API Key and Wget, etc.
 
     examples
     https://vsac.nlm.nih.gov/valueset/2.16.840.1.113762.1.4.1146.1629/expansion/Latest
     https://cts.nlm.nih.gov/fhir/res/ValueSet/2.16.840.1.113762.1.4.1146.1629?_format=json
 
     :param valueset_json: ValueSet file, expecially those provided by NLM/ONC/VSAC
     :return: list of codeable concepts (system, code, display) to include
     """
-    valueset = load_json(valueset_json)
+    valueset = base_utils.load_json(valueset_json)
     parsed = []
 
     for include in valueset["compose"]["include"]:
         if "concept" in include.keys():
             for concept in include["concept"]:
                 concept["system"] = include["system"]
                 parsed.append(Coding(concept))
     return parsed
 
 
-def create_view_sql(view_name: str, concept_list: List[Coding]) -> str:
+def create_view_sql(view_name: str, concept_list: list[Coding]) -> str:
     """
     :param view_name: like study__define_type
     :param concept_list: list of concepts to include in definition
     :return: sql statement to execute
     """
     if view_name is None:
         raise TypeError("No view name provided")
     content = []
     for concept in concept_list:
         content.append([concept.system, concept.code, concept.display])
-    return get_create_view_query(
+    return base_templates.get_create_view_query(
         view_name=view_name, dataset=content, view_cols=["system", "code", "display"]
     )
 
 
 """    header = f"create or replace view {view_name} as select * from (values"
     footer = ") AS t (system, code, display) ;"
     content = list()
     for concept in concept_list:
         content.append(f"('{concept.system}', '{concept.code}', '{concept.display}')")
     content = "\n,".join(content)
     return header + "\n" + content + "\n" + footer
 """
 
 
-def write_view_sql(view_name: str, concept_list: List[Coding]) -> None:
+def write_view_sql(view_name: str, concept_list: list[Coding]) -> None:
     """Convenience wrapper for writing create_view_sql to disk"""
     with open(f"{view_name}.sql", "w") as fp:
         fp.write(create_view_sql(view_name, concept_list))
```

### Comparing `cumulus_library-1.4.1/cumulus_library/schema/columns.py` & `cumulus_library-2.0.0/cumulus_library/schema/columns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # pylint: disable=W,C,R
-from enum import Enum, EnumMeta
-from cumulus_library.schema.typesystem import Datatypes, Coding, Vocab
-from cumulus_library.schema.valueset import Gender, Race, Ethnicity
-from cumulus_library.schema.valueset import DurationUnits
-from cumulus_library.schema.valueset import EncounterCode
-from cumulus_library.schema.valueset import ObservationInterpretationDetection
+from enum import Enum
+
+from cumulus_library.schema.typesystem import Datatypes, Vocab
+from cumulus_library.schema.valueset import (
+    DurationUnits,
+    EncounterCode,
+    Ethnicity,
+    Gender,
+    ObservationInterpretationDetection,
+    Race,
+)
 
 
 class ColumnEnum(Enum):
     # Counts
     cnt = Datatypes.Int, "Count"
     cnt_subject = Datatypes.Int, "Count Patients"
     cnt_encounter = Datatypes.Int, "Count Encounters"
```

### Comparing `cumulus_library-1.4.1/cumulus_library/schema/counts.py` & `cumulus_library-2.0.0/cumulus_library/statistics/counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Class for generating counts tables from templates"""
-import sys
 
+import sys
 from pathlib import Path
-from typing import Union
 
 from cumulus_library.base_table_builder import BaseTableBuilder
-from cumulus_library.study_parser import StudyManifestParser
-from cumulus_library.template_sql import templates
 from cumulus_library.errors import CountsBuilderError
+from cumulus_library.statistics.statistics_templates import counts_templates
+from cumulus_library.study_parser import StudyManifestParser
 
 
 class CountsBuilder(BaseTableBuilder):
     """Extends BaseTableBuilder for counts-related use cases"""
 
-    def __init__(self, study_prefix: str = None):
+    def __init__(self, study_prefix: str | None = None):
         if study_prefix is None:
             # This slightly wonky approach will give us the path of the
             # directory of a class extending the CountsBuilder
             study_path = Path(sys.modules[self.__module__].__file__).parent
 
             try:
                 parser = StudyManifestParser(study_path)
@@ -39,15 +38,15 @@
         """
         if duration:
             return f"{self.study_prefix}__{table_name}_{duration}"
         else:
             return f"{self.study_prefix}__{table_name}"
 
     def get_where_clauses(
-        self, clause: Union[list, str, None] = None, min_subject: int = 10
+        self, clause: list | str | None = None, min_subject: int = 10
     ) -> str:
         """Convenience method for constructing arbitrary where clauses.
 
         :param clause: either a string or a list of sql where statements
         :param min_subject: if clause is none, the bin size for a cnt_subject filter
             (deprecated, use count_[fhir_resource](min_subject) instead)
         """
@@ -68,36 +67,43 @@
         :param table_name: The name of the table to create. Must start with study prefix
         :param source_table: The table to create counts data from
         :param table_cols: The columns from the source table to add to the count table
         :keyword where_clauses: An array of where clauses to use for filtering the data
         :keyword min_subject: An integer setting the minimum bin size for inclusion
             (default: 10)
         :keyword fhir_resource: The type of FHIR resource to count (see
-            template_sql/templates.CountableFhirResource)
+            statistics/statistics_templates/count_templates.CountableFhirResource)
         """
         if not table_name or not source_table or not table_cols:
             raise CountsBuilderError(
                 "count_query missing required arguments. " f"output table: {table_name}"
             )
         for key in kwargs:
-            if key not in ["min_subject", "where_clauses", "fhir_resource"]:
+            if key not in [
+                "min_subject",
+                "where_clauses",
+                "fhir_resource",
+                "filter_resource",
+            ]:
                 raise CountsBuilderError(f"count_query received unexpected key: {key}")
-        return templates.get_count_query(table_name, source_table, table_cols, **kwargs)
+        return counts_templates.get_count_query(
+            table_name, source_table, table_cols, **kwargs
+        )
 
     # ----------------------------------------------------------------------
     # The following function all wrap get_count_query as convenience methods.
     # We're not trying to be overly clever about this to persist the docstrings as the
     # primary interface that study authors would see when using these functions.
 
     def count_condition(
         self,
         table_name: str,
         source_table: str,
         table_cols: list,
-        where_clauses: Union[list, None] = None,
+        where_clauses: list | None = None,
         min_subject: int = 10,
     ) -> str:
         """wrapper method for constructing condition counts tables
 
         :param table_name: The name of the table to create. Must start with study prefix
         :param source_table: The table to create counts data from
         :param table_cols: The columns from the source table to add to the count table
@@ -108,48 +114,50 @@
         return self.get_count_query(
             table_name,
             source_table,
             table_cols,
             where_clauses=where_clauses,
             min_subject=min_subject,
             fhir_resource="condition",
+            filter_resource="encounter",
         )
 
-    def count_document(
+    def count_documentreference(
         self,
         table_name: str,
         source_table: str,
         table_cols: list,
-        where_clauses: Union[list, None] = None,
+        where_clauses: list | None = None,
         min_subject: int = 10,
     ) -> str:
-        """wrapper method for constructing document counts tables
+        """wrapper method for constructing documentreference counts tables
 
         :param table_name: The name of the table to create. Must start with study prefix
         :param source_table: The table to create counts data from
         :param table_cols: The columns from the source table to add to the count table
         :param where_clauses: An array of where clauses to use for filtering the data
         :param min_subject: An integer setting the minimum bin size for inclusion
             (default: 10)
         """
         return self.get_count_query(
             table_name,
             source_table,
             table_cols,
             where_clauses=where_clauses,
             min_subject=min_subject,
-            fhir_resource="document",
+            fhir_resource="documentreference",
+            filter_resource="encounter",
         )
 
     def count_encounter(
         self,
         table_name: str,
         source_table: str,
         table_cols: list,
-        where_clauses: Union[list, None] = None,
+        where_clauses: list | None = None,
         min_subject: int = 10,
     ) -> str:
         """wrapper method for constructing encounter counts tables
 
         :param table_name: The name of the table to create. Must start with study prefix
         :param source_table: The table to create counts data from
         :param table_cols: The columns from the source table to add to the count table
@@ -162,20 +170,46 @@
             source_table,
             table_cols,
             where_clauses=where_clauses,
             min_subject=min_subject,
             fhir_resource="encounter",
         )
 
+    def count_medicationrequest(
+        self,
+        table_name: str,
+        source_table: str,
+        table_cols: list,
+        where_clauses: list | None = None,
+        min_subject: int = 10,
+    ) -> str:
+        """wrapper method for constructing medicationrequests counts tables
+
+        :param table_name: The name of the table to create. Must start with study prefix
+        :param source_table: The table to create counts data from
+        :param table_cols: The columns from the source table to add to the count table
+        :param where_clauses: An array of where clauses to use for filtering the data
+        :param min_subject: An integer setting the minimum bin size for inclusion
+            (default: 10)
+        """
+        return self.get_count_query(
+            table_name,
+            source_table,
+            table_cols,
+            where_clauses=where_clauses,
+            min_subject=min_subject,
+            fhir_resource="medicationrequest",
+        )
+
     def count_observation(
         self,
         table_name: str,
         source_table: str,
         table_cols: list,
-        where_clauses: Union[list, None] = None,
+        where_clauses: list | None = None,
         min_subject: int = 10,
     ) -> str:
         """wrapper method for constructing observation counts tables
 
         :param table_name: The name of the table to create. Must start with study prefix
         :param source_table: The table to create counts data from
         :param table_cols: The columns from the source table to add to the count table
@@ -193,15 +227,15 @@
         )
 
     def count_patient(
         self,
         table_name: str,
         source_table: str,
         table_cols: list,
-        where_clauses: Union[list, None] = None,
+        where_clauses: list | None = None,
         min_subject: int = 10,
     ) -> str:
         """wrapper method for constructing patient counts tables
 
         :param table_name: The name of the table to create. Must start with study prefix
         :param source_table: The table to create counts data from
         :param table_cols: The columns from the source table to add to the count table
@@ -226,14 +260,14 @@
 
         :param filepath: path to file to write queries out to.
         """
         self.prepare_queries(cursor=None, schema=None)
         self.comment_queries()
         self.write_queries(filename=filepath)
 
-    def prepare_queries(self, cursor: object = None, schema: str = None):
+    def prepare_queries(self, cursor: object | None = None, schema: str | None = None):
         """Stub implementing abstract base class
 
-        This should be overridden in any count generator. See core study count_core.py
+        This should be overridden in any count generator. See studies/core/count_core.py
         for an example
         """
         pass
```

### Comparing `cumulus_library-1.4.1/cumulus_library/schema/typesystem.py` & `cumulus_library-2.0.0/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/schema/valueset.py` & `cumulus_library-2.0.0/cumulus_library/schema/valueset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=W,C,R
 from enum import Enum
-from cumulus_library.schema.typesystem import Coding, Vocab
+
+from cumulus_library.schema.typesystem import Coding
 
 ################################################################################
 # FHIR ValueSets
 ################################################################################
 
 
 class ValueSet(Enum):
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/core/builder_core_medication.py` & `cumulus_library-2.0.0/cumulus_library/studies/core/builder_medication.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,93 @@
 """ Module for generating core medication table"""
 
-from cumulus_library.base_table_builder import BaseTableBuilder
-from cumulus_library.helper import get_progress_bar, query_console_output
-from cumulus_library.template_sql.templates import (
-    get_core_medication_query,
-    get_is_table_not_empty_query,
-    get_column_datatype_query,
-    get_ctas_empty_query,
-)
-from cumulus_library.template_sql.utils import is_codeable_concept_populated
+from cumulus_library import base_table_builder, base_utils
+from cumulus_library.studies.core.core_templates import core_templates
+from cumulus_library.template_sql import base_templates, sql_utils
 
 
-class MedicationBuilder(BaseTableBuilder):
-    display_text = "Creating core medication table..."
+class MedicationBuilder(base_table_builder.BaseTableBuilder):
+    display_text = "Creating Medication table..."
 
     def _check_data_in_fields(self, cursor, schema: str):
-        """Validates whether either observed medication source is present"""
+        """Validates whether either observed medication source is present
+
+        We opt to not use the core_templates.utils based version of
+        checking for data fields, since Medication can come in from
+        a few different sources - the format is unique to this FHIR
+        resource.
+        """
 
         data_types = {
             "inline": False,
             "by_contained_ref": False,
             "by_external_ref": False,
         }
 
         table = "medicationrequest"
-        base_col = "medicationcodeableconcept"
-
-        with get_progress_bar(transient=True) as progress:
+        inline_col = "medicationcodeableconcept"
+        with base_utils.get_progress_bar(transient=True) as progress:
             task = progress.add_task(
                 "Detecting available medication sources...",
-                total=7,
+                total=3,
             )
 
             # inline medications from FHIR medication
-            data_types["inline"] = is_codeable_concept_populated(
-                schema, table, base_col, cursor
+            data_types["inline"] = sql_utils.is_field_populated(
+                schema=schema,
+                source_table=table,
+                hierarchy=[(inline_col, dict), ("coding", list)],
+                cursor=cursor,
             )
             if data_types["inline"]:
-                query = get_column_datatype_query(schema, table, base_col)
+                query = base_templates.get_column_datatype_query(
+                    schema, table, [inline_col]
+                )
                 cursor.execute(query)
                 progress.advance(task)
                 if "userselected" not in str(cursor.fetchone()[0]):
                     has_userselected = False
                 else:
                     has_userselected = True
             else:
                 has_userselected = False
-            # Validating presence of FHIR medication requests
-            query = get_is_table_not_empty_query(
-                "medicationrequest", "medicationreference"
-            )
-            cursor.execute(query)
             progress.advance(task)
-            if cursor.fetchone() is None:
-                return data_types, has_userselected
-            query = get_column_datatype_query(
-                schema, "medicationrequest", "medicationreference"
-            )
-            cursor.execute(query)
-            progress.advance(task)
-            if "reference" not in cursor.fetchone()[0]:
-                return data_types, has_userselected
-            query = get_is_table_not_empty_query(
-                "medicationrequest", "medicationreference.reference"
-            )
-            cursor.execute(query)
-            progress.advance(task)
-            if cursor.fetchone() is None:
+            # Validating presence of FHIR medication requests
+            if not sql_utils.is_field_populated(
+                schema=schema,
+                source_table=table,
+                hierarchy=[("medicationreference", dict), ("reference", dict)],
+                expected=["reference"],
+                cursor=cursor,
+            ):
                 return data_types, has_userselected
 
             # checking med ref contents for our two linkage cases
-            query = get_is_table_not_empty_query(
+            query = base_templates.get_is_table_not_empty_query(
                 "medicationrequest",
                 "medicationreference.reference",
                 conditions=["medicationreference.reference LIKE '#%'"],
             )
             cursor.execute(query)
             progress.advance(task)
             if cursor.fetchone() is not None:
                 data_types["by_contained_ref"] = True
-            query = get_is_table_not_empty_query(
+            query = base_templates.get_is_table_not_empty_query(
                 "medicationrequest",
                 "medicationreference.reference",
                 conditions=["medicationreference.reference LIKE 'Medication/%'"],
             )
             cursor.execute(query)
             progress.advance(task)
             if cursor.fetchone() is not None:
                 data_types["by_external_ref"] = True
 
             return data_types, has_userselected
 
-    def prepare_queries(self, cursor: object, schema: str) -> dict:
+    def prepare_queries(self, cursor: object, schema: str, *args, **kwargs) -> dict:
         """Constructs queries related to condition codeableConcept
 
         :param cursor: A database cursor object
         :param schema: the schema/db name, matching the cursor
 
         """
         medication_datasources, has_userselected = self._check_data_in_fields(
@@ -103,17 +95,31 @@
         )
         if (
             medication_datasources["inline"]
             or medication_datasources["by_contained_ref"]
             or medication_datasources["by_external_ref"]
         ):
             self.queries.append(
-                get_core_medication_query(medication_datasources, has_userselected)
+                core_templates.get_core_template(
+                    "medication",
+                    config={
+                        "medication_datasources": medication_datasources,
+                        "has_userselected": has_userselected,
+                    },
+                )
             )
         else:
             self.queries.append(
-                get_ctas_empty_query(
+                base_templates.get_ctas_empty_query(
                     schema,
                     "core__medication",
-                    ["id", "resourcetype", "code", "ingredient"],
+                    [
+                        "id",
+                        "encounter_ref",
+                        "patient_ref",
+                        "code",
+                        "display",
+                        "code_system",
+                        "userselected",
+                    ],
                 )
             )
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-2.0.0/cumulus_library/studies/core/study_period.sql`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,68 @@
--- #############################################################
--- DocumentReference
--- https://hl7.org/fhir/us/core/StructureDefinition-us-core-documentreference.html
-
---Each DocumentReference must have:
---    a status
---    a code describing the type of document
---    a document category
---    a patient
---    document referenced (content)
---    the MIME type (i.e. contentType) of the document
-
---Each DocumentReference must support:
---    a business identifier for the DocumentReference (possibly generated by the transcription system or EHR)
---    date and time the reference was created
---    an author
---    a code identifying the specific details about the format of the document — over and above the content’s MIME type
---    the patient encounter that is being referenced
---    clinically relevant date
-
-CREATE TABLE core__documentreference AS
-WITH temp_documentreference AS (
+CREATE TABLE core__study_period AS
+WITH documented_encounter AS (
     SELECT DISTINCT
-        dr.type,
-        dr.status,
-        dr.docstatus,
-        dr.context,
-        dr.subject.reference AS subject_ref,
-        dr.id AS doc_id,
-        date(
-            from_iso8601_timestamp(dr.context.period."start")
-        ) AS author_date,
-        concat('DocumentReference/', dr.id) AS doc_ref
-    FROM documentreference AS dr
-)
-
-SELECT DISTINCT
-    type_coding.type_row AS doc_type,
-    coalesce(type_coding.type_row.code, 'None') AS doc_type_code,
-    CASE
-        WHEN
-            type_coding.type_row.display IS NOT NULL
-            THEN replace(type_coding.type_row.display, ',')
-        ELSE type_row.code
-    END AS doc_type_display,
-    tdr.status,
-    tdr.docstatus,
-    context_encounter.encounter.reference AS encounter_ref,
-    date_trunc('day', tdr.author_date) AS author_date,
-    date_trunc('week', tdr.author_date) AS author_week,
-    date_trunc('month', tdr.author_date) AS author_month,
-    date_trunc('year', tdr.author_date) AS author_year,
-    tdr.subject_ref,
-    tdr.doc_id,
-    tdr.doc_ref
-FROM temp_documentreference AS tdr,
-    unnest(context.encounter) AS context_encounter (encounter), --noqa
-    unnest(type.coding) AS type_coding (type_row)
-WHERE author_date BETWEEN date('2016-06-01') AND current_date;
-
--- count *group by* DocumentReference.type
-CREATE TABLE core__count_documentreference_month AS
-WITH powerset AS (
-    SELECT
-        count(DISTINCT d.subject_ref) AS cnt_subject,
-        count(DISTINCT d.encounter_ref) AS cnt_encounter,
-        count(DISTINCT d.doc_id) AS cnt_document,
-        d.doc_type_display,
-        d.author_month,
-        e.enc_class_display
-    FROM core__documentreference AS d, core__encounter AS e
+        ce.period_start_day,
+        ce.period_start_week,
+        ce.period_start_month,
+        ce.period_end_day,
+        ce.age_at_visit,
+        cdr.author_day,
+        cdr.author_week,
+        cdr.author_month,
+        cdr.author_year,
+        cp.gender,
+        cp.race_display,
+        cp.ethnicity_display,
+        cp.subject_ref,
+        ce.encounter_ref,
+        ce.status,
+        cdr.documentreference_ref,
+        date_diff('day', ce.period_start_day, date(cdr.author_day)) AS diff_enc_note_days,
+        coalesce(ce.class_code, 'None') AS enc_class_code,
+        coalesce(ce.class_display, 'None') AS enc_class_display,
+        coalesce(cdr.type_code, 'None') AS doc_type_code,
+        coalesce(cdr.type_display, 'None') AS doc_type_display
+    FROM
+        core__patient AS cp,
+        core__encounter AS ce,
+        core__documentreference AS cdr
     WHERE
-        d.encounter_ref = e.encounter_ref
-        AND d.status = 'current'
-        AND d.docstatus IN (NULL, 'final', 'amended')
-    GROUP BY cube(d.doc_type_display, d.author_month, e.enc_class_display)
+        (cp.subject_ref = ce.subject_ref)
+        AND (ce.encounter_ref = cdr.encounter_ref)
+        AND (cdr.author_day BETWEEN date('2016-06-01') AND current_date)
+        AND (ce.period_start_day BETWEEN date('2016-06-01') AND current_date)
+        AND (ce.period_end_day BETWEEN date('2016-06-01') AND current_date)
 )
 
-SELECT DISTINCT
-    cnt_document AS cnt,
-    author_month,
-    enc_class_display,
-    doc_type_display
-FROM powerset
-WHERE cnt_subject >= 10
-ORDER BY cnt_document DESC, enc_class_display ASC;
+SELECT
+    de.period_start_day,
+    de.period_start_week,
+    de.period_start_month,
+    de.period_end_day,
+    de.age_at_visit,
+    de.author_day,
+    de.author_week,
+    de.author_month,
+    de.author_year,
+    de.gender,
+    de.race_display,
+    de.ethnicity_display,
+    de.subject_ref,
+    de.encounter_ref,
+    de.status,
+    de.documentreference_ref,
+    de.diff_enc_note_days,
+    de.enc_class_code,
+    de.enc_class_display,
+    de.doc_type_code,
+    de.doc_type_display,
+    coalesce(ed.code IS NOT NULL, FALSE) AS ed_note
+FROM documented_encounter AS de
+LEFT JOIN core__ed_note AS ed
+    ON de.doc_type_code = ed.from_code;
+
+CREATE TABLE core__meta_date AS
+SELECT
+    min(period_start_day) AS min_date,
+    max(period_end_day) AS max_date
+FROM core__study_period;
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/core/fhir_lookup_tables.sql` & `cumulus_library-2.0.0/cumulus_library/studies/core/fhir_lookup_tables.sql`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
             'short stay'
         ),
         (
             'VR',
             'virtual'
         )
     )
-        AS t (code, display)
+        AS t (code, display);
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/core/fhir_mapping_tables.sql` & `cumulus_library-2.0.0/cumulus_library/studies/core/fhir_mapping_tables.sql`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         ('RXNORM', 'RXNORM'),
 
         ('UMLS', 'http://www.nlm.nih.gov/research/umls/'),
         ('UMLS', 'UMLS'),
 
         ('CPT', 'http://www.ama-assn.org/go/cpt'),
         ('CPT', 'CPT')
-    ) AS t (code_system, uri); --noqa: AL05
+    ) AS t (code_system, uri);
 
 -- ############################################################
 -- FHIR mapping of Resource names to expected URIs
 
 CREATE TABLE core__fhir_mapping_resource_uri AS
 SELECT * FROM
     (
@@ -133,8 +133,8 @@
         ('HH', 'HH'),
         ('IMP', 'IMP'),
         ('ACUTE', 'ACUTE'),
         ('NONAC', 'NONAC'),
         ('PRENC', 'PRENC'),
         ('SS', 'SS'),
         ('VR', 'VR')
-    ) AS t (expected, found)
+    ) AS t (expected, found);
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/core/patient_extensions.sql` & `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_patient.sql`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 -- noqa: disable=all
-/*
-This is a reference output of the SQL generated by denormalizer.py that is
-used by the core__patient table. It is not invoked directly. We may
-in the future add additional extensions.
-*/
+-- This sql was autogenerated as a reference example using the library
+-- CLI. Its format is tied to the specific database it was run against,
+-- and it may not be correct for all databases. Use the CLI's build 
+-- option to derive the best SQL for your dataset.
+
+-- ###########################################################
 
 CREATE TABLE core__patient_ext_race AS (
     WITH
 
     system_ombCategory AS (
         SELECT DISTINCT
-            s.id,
+            s.id AS id,
             '0' AS priority,
             'ombCategory' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS race_code,
             ext_child.ext.valuecoding.display AS race_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-race'
             AND ext_child.ext.url = 'ombCategory'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
     system_detailed AS (
         SELECT DISTINCT
-            s.id,
+            s.id AS id,
             '1' AS priority,
             'detailed' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS race_code,
             ext_child.ext.valuecoding.display AS race_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-race'
             AND ext_child.ext.url = 'detailed'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
     system_text AS (
         SELECT DISTINCT
-            s.id,
+            s.id AS id,
             '2' AS priority,
             'text' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS race_code,
             ext_child.ext.valuecoding.display AS race_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-race'
             AND ext_child.ext.url = 'text'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
     union_table AS (
@@ -79,87 +80,107 @@
         SELECT
             id,
             priority,
             system,
             race_code,
             race_display
         FROM system_text
+        
         ORDER BY id, priority
     )
 
     SELECT
         id,
         system,
         race_code,
         race_display
     FROM (
         SELECT
             id,
             system,
-            ARRAY_AGG(race_code) AS race_code,
-            ARRAY_AGG(
-                race_display
+            LOWER(
+                ARRAY_JOIN(
+                    ARRAY_SORT(
+                        ARRAY_AGG(
+                            race_code
+                        )
+                    ), '; '
+                )
+            )
+                AS race_code,
+            LOWER(
+                ARRAY_JOIN(
+                    ARRAY_SORT(
+                        ARRAY_AGG(
+                            race_display
+                        )
+                    ), '; '
+                )
             ) AS race_display,
             ROW_NUMBER()
-            OVER (
-                PARTITION BY id, system
-            ) AS available_priority
+                OVER (
+                    PARTITION BY id, system
+                    ORDER BY priority ASC
+                ) AS available_priority
         FROM union_table
-        GROUP BY id, system
+        GROUP BY id, system, priority
     )
     WHERE available_priority = 1
 );
+
+-- ###########################################################
+
 CREATE TABLE core__patient_ext_ethnicity AS (
     WITH
 
     system_ombCategory AS (
         SELECT DISTINCT
-            s.id,
+            s.id AS id,
             '0' AS priority,
             'ombCategory' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS ethnicity_code,
             ext_child.ext.valuecoding.display AS ethnicity_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
             AND ext_child.ext.url = 'ombCategory'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
     system_detailed AS (
         SELECT DISTINCT
-            s.id,
+            s.id AS id,
             '1' AS priority,
             'detailed' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS ethnicity_code,
             ext_child.ext.valuecoding.display AS ethnicity_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
             AND ext_child.ext.url = 'detailed'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
     system_text AS (
         SELECT DISTINCT
-            s.id,
+            s.id AS id,
             '2' AS priority,
             'text' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS ethnicity_code,
             ext_child.ext.valuecoding.display AS ethnicity_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
             AND ext_child.ext.url = 'text'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
     union_table AS (
@@ -182,32 +203,88 @@
         SELECT
             id,
             priority,
             system,
             ethnicity_code,
             ethnicity_display
         FROM system_text
+        
         ORDER BY id, priority
     )
 
     SELECT
         id,
         system,
         ethnicity_code,
         ethnicity_display
     FROM (
         SELECT
             id,
             system,
-            ARRAY_AGG(ethnicity_code) AS ethnicity_code,
-            ARRAY_AGG(
-                ethnicity_display
+            LOWER(
+                ARRAY_JOIN(
+                    ARRAY_SORT(
+                        ARRAY_AGG(
+                            ethnicity_code
+                        )
+                    ), '; '
+                )
+            )
+                AS ethnicity_code,
+            LOWER(
+                ARRAY_JOIN(
+                    ARRAY_SORT(
+                        ARRAY_AGG(
+                            ethnicity_display
+                        )
+                    ), '; '
+                )
             ) AS ethnicity_display,
             ROW_NUMBER()
-            OVER (
-                PARTITION BY id, system
-            ) AS available_priority
+                OVER (
+                    PARTITION BY id, system
+                    ORDER BY priority ASC
+                ) AS available_priority
         FROM union_table
-        GROUP BY id, system
+        GROUP BY id, system, priority
     )
     WHERE available_priority = 1
-);
+);
+
+-- ###########################################################
+
+
+CREATE TABLE core__patient AS
+WITH temp_patient AS (
+    SELECT DISTINCT
+        p.id,
+        p.gender,
+        p.address,
+        date(from_iso8601_timestamp(p.birthDate)) AS birthDate,
+        er.race_display,
+        ee.ethnicity_display
+    FROM
+        patient AS p
+    LEFT JOIN core__patient_ext_race AS er ON p.id = er.id
+    LEFT JOIN core__patient_ext_ethnicity AS ee ON p.id = ee.id
+)
+
+SELECT DISTINCT
+    tp.id,
+    tp.gender,
+    tp.birthDate,
+    CASE
+        WHEN
+            t_address.addr_row.postalcode IS NOT NULL
+            THEN substr(t_address.addr_row.postalcode, 1, 3)
+        ELSE 'None'
+    END AS postalCode_3,
+    concat('Patient/', tp.id) AS subject_ref,
+    coalesce(tp.race_display, 'unknown') AS race_display,
+    coalesce(tp.ethnicity_display, 'unknown') AS ethnicity_display
+FROM
+    temp_patient AS tp,
+    unnest(tp.address) AS t_address (addr_row)
+
+WHERE
+    tp.birthDate IS NOT NULL
+    AND tp.gender IS NOT NULL;
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/core/setup.sql` & `cumulus_library-2.0.0/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/template/counts.sql` & `cumulus_library-2.0.0/cumulus_library/studies/template/counts.sql`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
         count(DISTINCT tflo.encounter_ref) AS cnt_encounter,
         tflo.influenza_test_code AS influenza_lab_code,
         upper(tflo.influenza_test_result.display) AS influenza_result_display,
         tflo.influenza_test_month
     FROM template__influenza_lab_observations AS tflo
     GROUP BY
         cube(
-                tflo.influenza_test_code,
-                tflo.influenza_test_result,
-                tflo.influenza_test_month
+            tflo.influenza_test_code, --noqa: LT02
+            tflo.influenza_test_result, --noqa: LT02
+            tflo.influenza_test_month --noqa: LT02
         )
 )
 
 SELECT DISTINCT
     cnt_encounter AS cnt,
     influenza_lab_code,
     influenza_result_display,
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-2.0.0/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/template/manifest.toml` & `cumulus_library-2.0.0/cumulus_library/studies/template/manifest.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # 'study_prefix' should be a string at the start of each table. We'll use this
 # to clean up queries, so it should be unique. Name your tables in the following
 # format: [study_prefix]__[table_name]. It should probably, but not necessarily,
 # be the same name as the folder the study definition is in.
 study_prefix = "template"
 
+# For most use cases, this should not be required, but if you need to programmatically
+# build tables, you can provide a list of files implementing BaseTableBuilder.
+# See vocab and core studies for examples of this pattern. These run before
+# any SQL execution
+# [table_builder_config]
+# file_names = [
+#     "my_table_builder.py",
+# ]
+
 # The following section describes all tables that should be generated directly
 # from SQL files.
 [sql_config]
 # 'file_names' defines a list of sql files to execute, in order, in this folder.
 # Recommended order: Any ancillary config (like a list of condition codes),
 # tables/view selecting subsets of data from FHIR data, tables/views creating 
 # summary statistics.
@@ -34,14 +43,18 @@
 # other studies authored inside BCH. These will always be run after any other
 # SQL queries have been generated
 # [counts_builder_config]
 # file_names = [
 #    "count.py"
 # ]
 
-# For most use cases, this should not be required, but if you need to programmatically
-# build tables, you can provide a list of files implementing BaseTableBuilder.
-# See vocab and core studies for examples of this pattern
-# [table_builder_config]
-# file_names = [
-#     "my_table_builder.py",
+# For more specialized statistics, we provide a toml-based config entrypoint. The
+# details of these configs will vary, depending on which statistical method you're
+# invoking. For more details, see the statistics section of the docs for a list of
+# supported approaches.
+# These will run last, so all the data in your study will exist by the time these
+# are invoked.
+# [statistics_config]
+# file_names = 
+# [
+#    "psm_config.toml"
 # ]
```

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/template/setup.sql` & `cumulus_library-2.0.0/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-1.4.1/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-2.0.0/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 """ Module for directly loading ICD bsvs into athena tables """
-import csv
 
-from pathlib import Path
+import csv
+import pathlib
 
-from cumulus_library.base_table_builder import BaseTableBuilder
-from cumulus_library.helper import query_console_output, get_progress_bar
-from cumulus_library.template_sql.templates import (
-    get_ctas_query,
-    get_insert_into_query,
-)
+from cumulus_library import base_table_builder
+from cumulus_library.template_sql import base_templates
 
 
-class VocabIcdRunner(BaseTableBuilder):
+class VocabIcdRunner(base_table_builder.BaseTableBuilder):
     display_text = "Creating ICD vocab..."
     partition_size = 1200
 
     @staticmethod
     def clean_row(row, filename):
         """Removes non-SQL safe charatcers from the input row."""
         for i in range(len(row)):
             cell = str(row[i]).replace("'", "").replace(";", ",")
             row[i] = cell
         return row
 
-    def prepare_queries(self, cursor: object, schema: str):
+    def prepare_queries(self, cursor: object, schema: str, *args, **kwargs):
         """Creates queries for populating ICD vocab
 
         TODO: this would be a lot faster if we converted the bsv to parquet,
         uploaded that, and then created the table from an external datasource
 
         :param cursor: A database cursor object
         :param schema: the schema/db name, matching the cursor
         """
 
         table_name = "vocab__icd"
         icd_files = ["ICD10CM_2023AA", "ICD10PCS_2023AA", "ICD9CM_2023AA"]
-        path = Path(__file__).parent
+        path = pathlib.Path(__file__).parent
 
         headers = ["CUI", "TTY", "CODE", "SAB", "STR"]
-        header_types = [f"{x} string" for x in headers]
         rows_processed = 0
         dataset = []
         created = False
         for filename in icd_files:
-            with open(f"{path}/{filename}.bsv", "r") as file:
+            with open(f"{path}/{filename}.bsv") as file:
                 # For the first row in the dataset, we want to coerce types from
                 # varchar(len(item)) athena default to to an unrestricted varchar, so
                 # we'll create a table with one row - this make the recast faster, and
                 # lets us set the partition_size a little higher by limiting the
                 # character bloat to keep queries under athena's limit of 262144.
                 reader = csv.reader(file, delimiter="|")
                 if not created:
                     row = self.clean_row(next(reader), filename)
                     self.queries.append(
-                        get_ctas_query(
+                        base_templates.get_ctas_query(
                             schema_name=schema,
                             table_name=table_name,
                             dataset=[row],
                             table_cols=headers,
                         )
                     )
                     created = True
                 for row in reader:
                     row = self.clean_row(row, filename)
                     dataset.append(row)
                     rows_processed += 1
                     if rows_processed == self.partition_size:
                         self.queries.append(
-                            get_insert_into_query(
+                            base_templates.get_insert_into_query(
                                 table_name=table_name,
                                 table_cols=headers,
                                 dataset=dataset,
                             )
                         )
                         dataset = []
                         rows_processed = 0
                 if rows_processed > 0:
                     self.queries.append(
-                        get_insert_into_query(
+                        base_templates.get_insert_into_query(
                             table_name=table_name, table_cols=headers, dataset=dataset
                         )
                     )
```

### Comparing `cumulus_library-1.4.1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-2.0.0/cumulus_library/template_sql/coding_denormalize.sql.jinja`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,27 @@
+{%- import 'syntax.sql.jinja' as syntax -%}
 CREATE TABLE {{ target_table }} AS (
     WITH
     {%- for system in code_systems %}
 
     system_{{ column_name }}_{{ loop.index0 }} AS (
         SELECT DISTINCT
             s.{{ source_id }} AS id,
             {%- if filter_priority %}
             '{{ loop.index0 }}' AS priority,
             {%- endif %}
-            u.codeable_concept.code AS code,
-            u.codeable_concept.display AS display,
-            u.codeable_concept.system AS code_system
+            u.parent_col.{{ column_name }}.code,
+            u.parent_col.{{ column_name }}.display,
+            u.parent_col.{{ column_name }}.system AS code_system
         FROM
             {{ source_table }} AS s,
-        {%- if is_array %}
-            UNNEST(s.{{ column_name }}) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
-        {%- else %}
-            UNNEST(s.{{ column_name }}.coding) AS u (codeable_concept)
-        {%- endif %}
+            UNNEST(s.{{ parent_field }}) AS u (parent_col)
         {%- if filter_priority %}
         WHERE
-            u.codeable_concept.system = '{{ system }}'
+            u.parent_col.{{ column_name }}.system LIKE '{{ system }}'
         {%- endif %}
     ), --noqa: LT07
     {%- endfor %}
 
     union_table AS (
         {%- for system in code_systems %}
         SELECT
@@ -33,31 +29,30 @@
             {%- if filter_priority %}
             priority,
             {%- endif %}
             code_system,
             code,
             display
         FROM system_{{ column_name }}_{{ loop.index0 }}
-        {%- if not loop.last %}
-        UNION 
-        {%- endif -%}
+        {{ syntax.union_delineate(loop) }}
         {%- endfor %}
     )
     {%- if filter_priority -%},
 
     partitioned_table AS (
         SELECT
             id,
             code,
             code_system,
             display,
             priority,
             ROW_NUMBER()
                 OVER (
                     PARTITION BY id
+                    ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
         GROUP BY id, priority, code_system, code, display
         ORDER BY priority ASC
     )
 
     SELECT
```

### Comparing `cumulus_library-1.4.1/cumulus_library/template_sql/core_medication.sql.jinja` & `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medication.sql.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CREATE TABLE core__medication AS (
     WITH
     {# Gets medication data from inline ETL extraction.
 
     95% of the time, this dataset is the 'correct' dataset for Cerner.
     It may not be present in EPIC datasets. #}
-    {%- if medication_datasources.inline %}
+    {%- if config.medication_datasources.inline %}
     mcc_nonnull AS (
         SELECT 
             id,
             encounter, 
             subject, 
             medicationcodeableconcept 
         FROM medicationrequest 
@@ -19,41 +19,41 @@
         SELECT
             id,
             subject.reference as patient_ref,
             encounter.reference AS encounter_ref,
             t.r.code,
             t.r.display,
             t.r.system AS code_system,
-            {% if has_userselected %}
+            {% if config.has_userselected %}
             t.r.userselected
             {% else %}
             false AS userselected
             {% endif %}
         FROM mcc_nonnull,
         unnest(medicationcodeableconcept.coding) AS t(r)
     )
     {%- endif -%}
 
     {# comma handling for ctas chaining #}
-    {%- if medication_datasources.inline  and
-        (medication_datasources.by_contained_ref or 
-        medication_datasources.by_external_ref)
+    {%- if config.medication_datasources.inline  and
+        (config.medication_datasources.by_contained_ref or 
+        config.medication_datasources.by_external_ref)
     -%}
     ,
     {%- endif %}
     {# This section is also Cerner specific. Sometimes medication codes are blank
     and we can get :some: info from the contains field.
 
     As of this writing, the code coming back via contained when code is not
     present contains text only. In these cases, we'll cast the text
     as a display element.
 
     TODO: If we ever find a case where there is a valid code, we'll
     need to add a new case detection. #}
-    {%- if medication_datasources.by_contained_ref %}
+    {%- if config.medication_datasources.by_contained_ref %}
     mrc_med_ref AS (
         SELECT medicationreference
         FROM medicationrequest
         WHERE
             medicationreference IS NOT NULL
             AND medicationcodeableconcept IS NULL
     ),
@@ -97,35 +97,35 @@
             'None' AS code_system,
             FALSE AS userselected
         FROM mrc_contained_unnest AS cu
         INNER JOIN mrc_ref_id AS ri ON cu.id = ri.id
     )
     {%- endif -%}
     {# comma handling for ctas chaining #}
-    {%- if medication_datasources.by_contained_ref 
-        and medication_datasources.by_external_ref -%}
+    {%- if config.medication_datasources.by_contained_ref 
+        and config.medication_datasources.by_external_ref -%}
     ,
     {%- endif %}
     {# Gets medication by reference from external medications table.
 
     This is generally how we expect EPIC to provide medication data. #}
-    {%- if medication_datasources.by_external_ref %}
+    {%- if config.medication_datasources.by_external_ref %}
     mre_med_ref AS (
         SELECT
             mr.id,
             mr.encounter,
             mr.subject,
             mr.medicationreference
         FROM medicationrequest AS mr
         WHERE mr.medicationreference IS NOT NULL
     ),
 
     mre_ref_id AS (
         SELECT DISTINCT
-            mr.id AS id,
+            mr.id,
             mr.encounter,
             mr.subject,
             substring(mr.medicationreference.reference, 12) AS medication_id
         FROM mre_med_ref AS mr
         WHERE
             mr.medicationreference.reference IS NOT NULL
             AND mr.medicationreference.reference LIKE 'Medication/%'
@@ -144,59 +144,59 @@
     ),
 
     external_medication AS (
         SELECT
             mmn.id,
             mmn.encounter.reference AS encounter_ref,
             mmn.subject.reference AS patient_ref,
-            t.r.code AS code,
+            t.r.code,
             mmn.code.text AS display,
             t.r.system AS code_system,
             FALSE AS userselected
         FROM mre_med_nonnull AS mmn,
             unnest(mmn.code.coding) AS t (r)
     )
     {%- endif %}
     {# Selective unioning of the above tables #}
-    {%- if medication_datasources.inline %}
+    {%- if config.medication_datasources.inline %}
     SELECT
         id,
         encounter_ref,
         patient_ref,
         code,
         display,
         code_system,
         userselected
     FROM
         inline_medication
-        {%- if medication_datasources.inline  and
-            (medication_datasources.by_contained_ref or 
-            medication_datasources.by_external_ref)
+        {%- if config.medication_datasources.inline  and
+            (config.medication_datasources.by_contained_ref or 
+            config.medication_datasources.by_external_ref)
         %}
     UNION
     {% endif %}
     {%- endif %}
-    {%- if medication_datasources.by_contained_ref %}
+    {%- if config.medication_datasources.by_contained_ref %}
     SELECT
         id,
         encounter_ref,
         patient_ref,
         code,
         display,
         code_system,
         userselected
     FROM
         contained_medication
-        {%- if medication_datasources.by_contained_ref 
-            and medication_datasources.by_external_ref 
+        {%- if config.medication_datasources.by_contained_ref 
+            and config.medication_datasources.by_external_ref 
         %}
     UNION
     {% endif %}
     {%- endif %}
-    {%- if medication_datasources.by_external_ref %}
+    {%- if config.medication_datasources.by_external_ref %}
     SELECT
         id,
         encounter_ref,
         patient_ref,
         code,
         display,
         code_system,
```

### Comparing `cumulus_library-1.4.1/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-2.0.0/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{%- import 'syntax.sql.jinja' as syntax -%}
 CREATE TABLE {{ target_table }} AS (
     WITH
     {%- for system in ext_systems %}
 
     system_{{ system }} AS (
         SELECT DISTINCT
             s.{{ source_id }} AS id,
@@ -25,17 +26,15 @@
         SELECT
             id,
             priority,
             system,
             {{ target_col_prefix }}_code,
             {{ target_col_prefix }}_display
         FROM system_{{ system }}
-        {%- if not loop.last %}
-        UNION 
-        {%- endif -%}
+        {{ syntax.union_delineate(loop) }}
         {%- endfor %}
         ORDER BY id, priority
     )
 
     SELECT
         id,
         system,
@@ -70,13 +69,14 @@
             LOWER(
                 {{ target_col_prefix }}_display
             ) AS {{ target_col_prefix }}_display,
             {%- endif %}
             ROW_NUMBER()
                 OVER (
                     PARTITION BY id, system
+                    ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
-        GROUP BY id, system
+        GROUP BY id, system, priority
     )
     WHERE available_priority = 1
 );
```

### Comparing `cumulus_library-1.4.1/cumulus_library/upload.py` & `cumulus_library-2.0.0/cumulus_library/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """ Handles pushing data to the aggregator"""
-import sys
 
+import sys
 from pathlib import Path
 
 import requests
-
 from pandas import read_parquet
 from rich.progress import Progress, TaskID
 
-from cumulus_library.helper import get_progress_bar
+from cumulus_library import base_utils
 
 
 def upload_data(
     progress: Progress,
     file_upload_progress: TaskID,
     file_path: Path,
     version: int,
@@ -86,11 +85,11 @@
             filter(lambda x: str(x).endswith("__meta_version.parquet"), file_paths)
         )
         version = str(read_parquet(meta_version)["data_package_version"][0])
         file_paths.remove(meta_version)
     except StopIteration:
         version = "0"
     num_uploads = len(file_paths)
-    with get_progress_bar() as progress:
+    with base_utils.get_progress_bar() as progress:
         file_upload_progress = progress.add_task("Uploading", total=num_uploads)
         for file_path in file_paths:
             upload_data(progress, file_upload_progress, file_path, version, args)
```

### Comparing `cumulus_library-1.4.1/PKG-INFO` & `cumulus_library-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 1.4.1
+Version: 2.0.0
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
-Requires-Python: >= 3.9
+Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ctakesclient >= 1.3
+Requires-Dist: cumulus-fhir-support >= 1
+Requires-Dist: duckdb >= 0.9
 Requires-Dist: fhirclient >= 4.1
 Requires-Dist: Jinja2 > 3
-Requires-Dist: pandas <3, >=2.1.1
+Requires-Dist: pandas <3, >=2.1.3
+Requires-Dist: psmpy <1, >=0.3.13
 Requires-Dist: pyarrow >= 11.0
 Requires-Dist: pyathena >= 2.23
+Requires-Dist: pytablewriter >= 1.2
 Requires-Dist: requests >= 2.28
 Requires-Dist: rich >= 13.2
-Requires-Dist: sqlfluff >= 2.3.4
+Requires-Dist: sqlfluff  >= 3
+Requires-Dist: sqlparse >0.4
 Requires-Dist: toml >= 0.10
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: pylint ; extra == "dev"
+Requires-Dist: ruff == 0.2.1 ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
+Requires-Dist: freezegun ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: requests-mock ; extra == "test"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
 Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
-Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library-core
+Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library
 Provides-Extra: dev
 Provides-Extra: test
 
 # Cumulus Library - Core
 
 A framework for designing, executing, and distributing SQL queries packaged as "studies", e.g., for quality monitoring, clinical research, or public health. Part of the [SMART on FHIR Cumulus Project](https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/)
```

