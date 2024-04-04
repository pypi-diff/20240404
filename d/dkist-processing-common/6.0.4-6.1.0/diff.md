# Comparing `tmp/dkist-processing-common-6.0.4.tar.gz` & `tmp/dkist-processing-common-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-6.0.4.tar", last modified: Tue Mar 26 20:45:40 2024, max compression
+gzip compressed data, was "dkist-processing-common-6.1.0.tar", last modified: Thu Apr  4 13:57:41 2024, max compression
```

## Comparing `dkist-processing-common-6.0.4.tar` & `dkist-processing-common-6.1.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.510596 dkist-processing-common-6.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    22813 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4367 2024-03-26 20:45:40.514596 dkist-processing-common-6.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.502596 dkist-processing-common-6.0.4/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.502596 dkist-processing-common-6.0.4/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.502596 dkist-processing-common-6.0.4/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2439 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8719 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5818 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.502596 dkist-processing-common-6.0.4/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/asdf.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.502596 dkist-processing-common-6.0.4/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.506596 dkist-processing-common-6.0.4/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5350 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5176 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3333 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)    11331 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/task_name.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.506596 dkist-processing-common-6.0.4/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6461 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/unique_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.506596 dkist-processing-common-6.0.4/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12488 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    12130 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8504 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.506596 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13806 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.510596 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47891 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3349 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8852 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5833 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19073 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.510596 dkist-processing-common-6.0.4/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26025 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4083 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)    10946 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8346 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10629 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9356 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36297 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    12486 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)    24306 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_stems.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_task_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4027 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6658 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)    15911 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    15170 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.502596 dkist-processing-common-6.0.4/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4367 2024-03-26 20:45:40.000000 dkist-processing-common-6.0.4/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4991 2024-03-26 20:45:40.000000 dkist-processing-common-6.0.4/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-26 20:45:40.000000 dkist-processing-common-6.0.4/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-03-26 20:45:40.000000 dkist-processing-common-6.0.4/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-26 20:45:40.000000 dkist-processing-common-6.0.4/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.510596 dkist-processing-common-6.0.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 20:45:40.510596 dkist-processing-common-6.0.4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-03-26 20:45:40.514596 dkist-processing-common-6.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-03-26 20:45:34.000000 dkist-processing-common-6.0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.966590 dkist-processing-common-6.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    23402 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2024-04-04 13:57:41.966590 dkist-processing-common-6.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.954590 dkist-processing-common-6.1.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.954590 dkist-processing-common-6.1.0/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.954590 dkist-processing-common-6.1.0/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)    10111 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.958590 dkist-processing-common-6.1.0/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/asdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.958590 dkist-processing-common-6.1.0/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.958590 dkist-processing-common-6.1.0/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)    11331 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.962590 dkist-processing-common-6.1.0/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/unique_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.962590 dkist-processing-common-6.1.0/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12488 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    12852 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.962590 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13806 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.962590 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47891 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7986 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8852 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19073 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.966590 dkist-processing-common-6.1.0/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26212 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    10946 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10629 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36297 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16481 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_stems.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4253 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    15911 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15170 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.954590 dkist-processing-common-6.1.0/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2024-04-04 13:57:41.000000 dkist-processing-common-6.1.0/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2024-04-04 13:57:41.000000 dkist-processing-common-6.1.0/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-04 13:57:41.000000 dkist-processing-common-6.1.0/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-04 13:57:41.000000 dkist-processing-common-6.1.0/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-04 13:57:41.000000 dkist-processing-common-6.1.0/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.966590 dkist-processing-common-6.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:57:41.966590 dkist-processing-common-6.1.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-04 13:57:41.966590 dkist-processing-common-6.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-04 13:57:35.000000 dkist-processing-common-6.1.0/setup.py
```

### Comparing `dkist-processing-common-6.0.4/.gitignore` & `dkist-processing-common-6.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/.pre-commit-config.yaml` & `dkist-processing-common-6.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/CHANGELOG.rst` & `dkist-processing-common-6.1.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v6.1.0 (2024-04-04)
+===================
+
+Features
+--------
+
+- Implement a common 'rollback' method on all Tasks, and Task specific rollback steps where applicable, to facilitate manual processing and operational fault remediation/recovery. (`#177 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/177>`__)
+
+
+Misc
+----
+
+- Make the scratch inventory (Redis) db count configurable through an environment variable with a default which remains the same as the previously hardcoded value. (`#177 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/177>`__)
+
+
 v6.0.4 (2024-03-26)
 ===================
 
 Bugfixes
 --------
 
 - `FitsAccessBase.from_header` no longer clobbers "NAXISn" (and likely other FITS controlled keys) values from input header. (`#179 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/179>`__)
```

### Comparing `dkist-processing-common-6.0.4/PKG-INFO` & `dkist-processing-common-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.0.4
+Version: 6.1.0
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.0.4/README.rst` & `dkist-processing-common-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/bitbucket-pipelines.yml` & `dkist-processing-common-6.1.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/check_changelog_updated.sh` & `dkist-processing-common-6.1.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/_util/config.py` & `dkist-processing-common-6.1.0/dkist_processing_common/_util/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     globus_transport_params: dict = Field(default_factory=dict)
     globus_client_id: str | None = None
     globus_client_secret: str | None = None
     object_store_endpoint: str | None = None
     scratch_endpoint: str | None = None
     # scratch
     scratch_base_path: str = Field(default="scratch/")
+    scratch_inventory_db_count: int = 16
     # docs
     docs_base_url: str = Field(default="my_test_url")
 
     @property
     def metadata_store_api_base(self) -> str:
         """Metadata store api url."""
         gateway = self.service_mesh_detail(service_name="internal-api-gateway")
@@ -67,10 +68,15 @@
     def scratch_inventory_mesh_service(self) -> MeshService:
         """Scratch inventory host and port."""
         mesh = self.service_mesh_detail(service_name="automated-processing-scratch-inventory")
         if mesh == DEFAULT_MESH_SERVICE:
             return MeshService(mesh_address="localhost", mesh_port=6379)  # testing default
         return mesh
 
+    @property
+    def scratch_inventory_max_db_index(self) -> int:
+        """Scratch inventory's largest db index."""
+        return self.scratch_inventory_db_count - 1
+
 
 service_configuration = ServiceConfiguration()
 service_configuration.log_configurations()
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/_util/constants.py` & `dkist-processing-common-6.1.0/dkist_processing_common/_util/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         The resipe_run_id
     task_name
         The task name
     """
 
     def __init__(self, recipe_run_id: int, task_name: str):
         self.store = TagDB(recipe_run_id, task_name, "constant")
+        self._audit_db = TagDB(
+            recipe_run_id=recipe_run_id, task_name=task_name, namespace="constants_audit"
+        )
+        self._audit_set_tag = f"SET_{task_name}"
 
     @staticmethod
     def extract_value(value: set) -> int | str | float:
         """
         Pop the first (and only) value from set and convert it from a json string.
 
         Parameters
@@ -54,23 +58,41 @@
         self.store.clear_tag(key)
 
     def __setitem__(self, key: str, value: str | int | float | tuple | list):
         """Set a constant key with the specified value. Raise an error if the key already exists."""
         if self.store.all(key):
             raise ValueError(f"Constant {key} already exists")
         self.store.add(key, json.dumps(value))
+        # audit which constant key had a value set
+        self._audit_db.add(tag=self._audit_set_tag, value=key)
 
     def __iter__(self) -> Generator[str, None, None]:
         """Yield the currently defined constants as strings."""
         yield from self.store.tags
 
     def __len__(self):
         """Return the number of constants currently defined."""
         return len(self.store.tags)
 
     def close(self):
         """Close the db connection.  Call on __exit__ of a Task."""
         self.store.close()
+        self._audit_db.close()
 
     def purge(self):
         """Remove all constants associated with the instance recipe run id."""
         self.store.purge()
+        self._audit_db.purge()
+
+    def rollback(self):
+        """Remove all constants associated with the instance recipe run id and task name."""
+        # remove constants
+        for key in self._audit_db.all(tags=self._audit_set_tag):
+            self.store.clear_tag(key)
+        # remove audit
+        self._audit_db.clear_tag(tag=self._audit_set_tag)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-6.1.0/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-6.1.0/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-6.1.0/dkist_processing_common/_util/scratch.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,19 @@
         if not scratch_base_path:
             scratch_base_path = service_configuration.scratch_base_path
         self.scratch_base_path = scratch_base_path
         self.workflow_base_path = Path(self.scratch_base_path) / str(recipe_run_id)
         with self._mask():
             self.workflow_base_path.mkdir(parents=True, exist_ok=True)
         self._tag_db = TagDB(recipe_run_id=self.recipe_run_id, task_name=self.task_name)
+        self._audit_db = TagDB(
+            recipe_run_id=self.recipe_run_id, task_name=self.task_name, namespace="scratch_audit"
+        )
+        self._audit_write_tag = f"WRITE_{self.task_name}"
+        self._audit_tag_tag = f"TAG_{self.task_name}"
 
     @staticmethod
     @contextmanager
     def _mask():
         """Set a permissive umask to allow other users (e.g. globus) to modify resources created by the scratch library."""
         old_mask = umask(0)
         try:
@@ -116,14 +121,16 @@
             if overwrite:
                 mode = "wb"
             else:
                 mode = "xb"
             with path.open(mode=mode) as f:
                 f.write(file_obj)
         self.tag(path, tags)
+        # audit the path that was written to scratch
+        self._audit_db.add(tag=self._audit_write_tag, value=str(path))
 
     def delete(self, path: Path | str):
         """
         Delete the file or path.
 
         Parameters
         ----------
@@ -161,15 +168,19 @@
             raise ValueError(
                 f"Cannot tag paths which are not children of the base path {self.workflow_base_path}"
             )
         if not path.exists():
             raise FileNotFoundError(f"Cannot tag paths which do not exist. {path=}")
 
         for tag in tags:
+            tag_is_new = not bool(self._tag_db.all(tags=tag))
             self._tag_db.add(tag, str(path))
+            # audit the tag that was newly added to the scratch tag db
+            if tag_is_new:
+                self._audit_db.add(tag=self._audit_tag_tag, value=tag)
 
     def tags(self, path: Path | str):
         """
         Return the tags associated with the given file object.
 
         Parameters
         ----------
@@ -258,14 +269,15 @@
         """
         tags = self._parse_tags(tags)
         return len(self._tag_db.all(tags))
 
     def close(self):
         """Close the db connection.  Call on __exit__ of a Task."""
         self._tag_db.close()
+        self._audit_db.close()
 
     def purge(self, ignore_errors: bool = False):
         """
         Remove all data (tags, files, and folders) for the instance.
 
         Call when tearing down a workflow
 
@@ -275,21 +287,42 @@
             If set, errors will be ignored, otherwise stop at the first error
         Returns
         -------
         None
         """
         rmtree(self.workflow_base_path, ignore_errors=ignore_errors)
         self._tag_db.purge()
+        self._audit_db.purge()
+
+    def rollback(self):
+        """Remove all files and new tags associated with the instance recipe run id and task name."""
+        # remove files
+        for path in self._audit_db.all(tags=self._audit_write_tag):
+            path = Path(path)
+            path.unlink(missing_ok=True)
+            self._tag_db.clear_value(path)
+        # remove tags
+        for tag in self._audit_db.all(tags=self._audit_tag_tag):
+            self._tag_db.clear_tag(tag=tag)
+        # remove audit
+        self._audit_db.clear_tag(tag=self._audit_write_tag)
+        self._audit_db.clear_tag(tag=self._audit_tag_tag)
 
     def __repr__(self):
         return f"WorkflowFileSystem(recipe_run_id={self.recipe_run_id}, task_name={self.task_name}, scratch_base_path={self.scratch_base_path})"
 
     def __str__(self):
         return f"{self!r} connected to {self._tag_db}"
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
 
 def _flatten_list(elements: list) -> list:
     """Flatten an arbitrarily nested list."""
     result = []
     for element in elements:
         if isinstance(element, list):
             result.extend(_flatten_list(element))
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/_util/tags.py` & `dkist-processing-common-6.1.0/dkist_processing_common/_util/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     namespace
         The namespace within the recipe_run_id
     """
 
     def __init__(self, recipe_run_id: int, task_name: str, namespace: str = "path"):
         self.recipe_run_id = recipe_run_id
         self.task_name = task_name
-        self._db = self.recipe_run_id % 15
+        self._db = self.recipe_run_id % service_configuration.scratch_inventory_max_db_index
         self.namespace = f"{self.recipe_run_id}:{namespace}:"
         connection_name = f"{self.namespace}{self.task_name}"
         scratch_inventory = service_configuration.scratch_inventory_mesh_service
         self.db = Redis(
             db=self._db,
             host=scratch_inventory.host,
             port=scratch_inventory.port,
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/codecs/asdf.py` & `dkist-processing-common-6.1.0/dkist_processing_common/codecs/asdf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-6.1.0/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-6.1.0/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/codecs/json.py` & `dkist-processing-common-6.1.0/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/codecs/str.py` & `dkist-processing-common-6.1.0/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-6.1.0/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/manual.py` & `dkist-processing-common-6.1.0/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/constants.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 
     def _purge(self):
         self._db_dict.purge()
 
     def _close(self):
         self._db_dict.close()
 
+    def _rollback(self):
+        self._db_dict.rollback()
+
     @property
     def dataset_id(self) -> str:
         """Define the dataset_id constant."""
         return Hashids(min_length=5, alphabet=ascii_uppercase).encode(self._recipe_run_id)
 
     @property
     def proposal_id(self) -> str:
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/graphql.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/message.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/parameters.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/quality.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/tags.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/task_name.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-6.1.0/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/task.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/time.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/parsers/wavelength.py` & `dkist-processing-common-6.1.0/dkist_processing_common/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/__init__.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/base.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -349,17 +349,37 @@
         for tag in tags:
             if not isinstance(tag, str):
                 raise TypeError(f"Tags must be strings. Got {type(tag)} instead.")
             result.append(tag)
         return result
 
     def _purge(self):
-        """Purge the persistent stores associated with a task e.g. when testing."""
+        """Purge the persistent stores associated with the workflow to which this task belongs e.g. when testing."""
         self.scratch.purge()
         self.constants._purge()
         self.filename_counter.purge()
 
+    def rollback(self):
+        """
+
+        Remove changes made by this task from the persistent stores.
+
+        This differs from _purge() in that it attempts to be more surgical.
+
+        Finally, the recipe run is ensured to be in an Inprogress state.
+
+        Scratch: Rolls back files written and tags newly added by this task
+
+        Constants: Rolls back constants whose values were set by this task
+
+        Filename Counter: not rolled back but its purpose of preventing file name collisions is not impacted
+        """
+        super().rollback()
+        self.scratch.rollback()
+        self.constants._rollback()
+        self.metadata_store_change_recipe_run_to_inprogress()
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         super().__exit__(exc_type, exc_val, exc_tb)
         self.scratch.close()
         self.constants._close()
         self.filename_counter.close()
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/l1_output_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,21 @@
     """Subclass of OutputDataBase which encapsulates common level 1 output data methods."""
 
     @property
     def dataset_has_quality_report(self) -> bool:
         """Return True if a quality report has been submitted to the metadata-store."""
         return self.metadata_store_quality_report_exists(dataset_id=self.constants.dataset_id)
 
+    def rollback(self):
+        """Warn that the metadata-store and the interservice bus retain the effect of this tasks execution.  Rolling back this task may not be achievable without other action."""
+        super().rollback()
+        logger.warning(
+            f"Modifications to the metadata store and the interservice bus were not rolled back."
+        )
+
 
 class TransferL1Data(TransferDataBase, GlobusMixin):
     """Task class for transferring Level 1 processed data to the object store."""
 
     def transfer_objects(self):
         """Transfer movie and L1 output frames."""
         with self.apm_task_step("Upload movie"):
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/output_data_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,7 +88,17 @@
         """Remove folder objects that would have been added by the Globus transfer."""
         removed_object_keys = self.object_store_remove_folder_objects(
             bucket=self.destination_bucket, path=self.destination_root_folder
         )
         logger.info(
             f"Removed folder objects in {self.destination_bucket} bucket. {removed_object_keys=}"
         )
+
+    def rollback(self):
+        """
+
+        Rollback a Transfer Task.
+
+        Globus transfers are not dependent upon the task once they are submitted.  Rolling back this task may not be achievable action on the destination.
+        """
+        super().rollback()
+        logger.warning(f"Transferred objects may still exist at the destination.")
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,7 +110,14 @@
                 transfer_items=frame_transfer_items + parameter_transfer_items,
                 label=f"Transfer Inputs for Recipe Run {self.recipe_run_id}",
             )
 
         with self.apm_processing_step("Tag Input Frames and Parameter Files"):
             self.tag_input_frames(transfer_items=frame_transfer_items)
             self.tag_parameter_objects(transfer_items=parameter_transfer_items)
+
+    def rollback(self):
+        """Warn that depending on the progress of the task all data may not be removed because it hadn't been tagged."""
+        super().rollback()
+        logger.warning(
+            f"Rolling back only removes data that has been tagged.  The data persisted by this task may not have been tagged prior to rollback."
+        )
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/trial_catalog.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from dkist_processing_common._util.tags import TagDB
 from dkist_processing_common.models.graphql import InputDatasetInputDatasetPartResponse
 from dkist_processing_common.models.graphql import InputDatasetPartResponse
 from dkist_processing_common.models.graphql import InputDatasetPartTypeResponse
 from dkist_processing_common.models.graphql import InputDatasetResponse
 from dkist_processing_common.models.graphql import RecipeInstanceResponse
 from dkist_processing_common.models.graphql import RecipeRunResponse
+from dkist_processing_common.models.graphql import RecipeRunStatusResponse
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 TILE_SIZE = 64
 
@@ -328,14 +329,16 @@
 
 class FakeGQLClient:
     def __init__(self, *args, **kwargs):
         pass
 
     def execute_gql_query(self, **kwargs):
         query_base = kwargs["query_base"]
+        if query_base == "recipeRunStatuses":
+            return [RecipeRunStatusResponse(recipeRunStatusId=1)]
         if query_base == "recipeRuns":
             return [
                 RecipeRunResponse(
                     recipeInstanceId=1,
                     recipeInstance=RecipeInstanceResponse(
                         recipeId=1,
                         inputDataset=InputDatasetResponse(
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_stems.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_stems.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_task_name.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_teardown.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,16 @@
             )
             task.scratch.workflow_base_path = tmp_path / str(recipe_run_id)
             for filename in filenames:
                 filepath = task.scratch.workflow_base_path / filename
                 filepath.touch()
                 task.tag(filepath, tag_object)
 
+            task.constants._update({"teardown_constant": 1234})
+
             return task, filenames, tag_object
 
     yield factory
 
 
 def test_purge_data(
     teardown_task_factory, make_mock_GQL_with_configuration, config_with_teardown_enabled, mocker
@@ -110,14 +112,17 @@
     for filepath in tagged_data:
         assert filepath.exists()
     task()
     for filepath in tagged_data:
         assert not filepath.exists()
     post_purge_tagged_data = list(task.read(tags=tag_object))
     assert len(post_purge_tagged_data) == 0
+    # audit data removed
+    assert not task.scratch._audit_db.tags
+    assert not task.constants._db_dict._audit_db.tags
 
 
 def test_purge_data_disabled(
     teardown_task_factory, make_mock_GQL_with_configuration, config_with_teardown_disabled, mocker
 ):
     """
     :Given: A Teardown task with files and tags linked to it and teardown disabled
@@ -133,14 +138,17 @@
     for filepath in tagged_data:
         assert filepath.exists()
     task()
     for filepath in tagged_data:
         assert filepath.exists()  # still exists
     post_purge_tagged_data = list(task.read(tags=tag_object))
     assert len(post_purge_tagged_data) == len(tagged_data)
+    # audit data still present
+    assert task.scratch._audit_db.tags
+    assert task.constants._db_dict._audit_db.tags
 
 
 def test_purge_data_no_config(
     teardown_task_factory, make_mock_GQL_with_configuration, config_with_no_teardown, mocker
 ):
     """
     :Given: A Teardown task with files and tags linked and teardown not specified in the configuration
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_trial_catalog.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-6.1.0/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-6.1.0/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.0.4
+Version: 6.1.0
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-6.1.0/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-6.1.0/dkist_processing_common.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 astropy>=5.1.1
 dkist-fits-specifications>=4.0.0
 dkist-header-validator>=5.0.0
-dkist-processing-core==3.0.1
+dkist-processing-core==3.1.0
 dkist-processing-pac>=2.1.1
 dkist-service-configuration>=1.1.0
 dkist-spectral-lines>=2.0.0
 globus-sdk>=3.12.0
 gqlclient==1.0.0
 hashids==1.3.1
 matplotlib>=3.4
```

### Comparing `dkist-processing-common-6.0.4/docs/Makefile` & `dkist-processing-common-6.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/docs/conf.py` & `dkist-processing-common-6.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/docs/make.bat` & `dkist-processing-common-6.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/licenses/LICENSE.rst` & `dkist-processing-common-6.1.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/pyproject.toml` & `dkist-processing-common-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.0.4/setup.cfg` & `dkist-processing-common-6.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	astropy >= 5.1.1
 	dkist-fits-specifications >= 4.0.0
 	dkist-header-validator >= 5.0.0
-	dkist-processing-core == 3.0.1
+	dkist-processing-core == 3.1.0
 	dkist-processing-pac >= 2.1.1
 	dkist-service-configuration >= 1.1.0
 	dkist-spectral-lines >= 2.0.0
 	globus-sdk >= 3.12.0
 	gqlclient == 1.0.0
 	hashids == 1.3.1
 	matplotlib >= 3.4
```

