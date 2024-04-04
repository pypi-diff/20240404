# Comparing `tmp/pixeltable-0.2.0.tar.gz` & `tmp/pixeltable-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.2.0.tar", max compression
+gzip compressed data, was "pixeltable-0.2.1.tar", max compression
```

## Comparing `pixeltable-0.2.0.tar` & `pixeltable-0.2.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0      746 2024-01-15 22:21:10.025602 pixeltable-0.2.0/LICENSE
--rw-r--r--   0        0        0     4193 2024-04-03 21:21:55.982423 pixeltable-0.2.0/README.md
--rw-r--r--   0        0        0      959 2024-04-03 21:21:04.612709 pixeltable-0.2.0/pixeltable/__init__.py
--rw-r--r--   0        0        0      453 2024-03-29 02:10:24.349472 pixeltable-0.2.0/pixeltable/catalog/__init__.py
--rw-r--r--   0        0        0     7908 2024-04-02 22:13:56.668343 pixeltable-0.2.0/pixeltable/catalog/catalog.py
--rw-r--r--   0        0        0     8661 2024-04-03 17:26:04.851919 pixeltable-0.2.0/pixeltable/catalog/column.py
--rw-r--r--   0        0        0      919 2024-03-29 02:10:24.350840 pixeltable-0.2.0/pixeltable/catalog/dir.py
--rw-r--r--   0        0        0      943 2024-03-29 02:10:24.351032 pixeltable-0.2.0/pixeltable/catalog/globals.py
--rw-r--r--   0        0        0     8280 2024-04-03 17:26:04.852785 pixeltable-0.2.0/pixeltable/catalog/insertable_table.py
--rw-r--r--   0        0        0     1147 2024-03-29 02:10:24.351974 pixeltable-0.2.0/pixeltable/catalog/named_function.py
--rw-r--r--   0        0        0     1677 2024-04-03 17:26:04.853184 pixeltable-0.2.0/pixeltable/catalog/path.py
--rw-r--r--   0        0        0     5941 2024-04-03 17:26:04.853564 pixeltable-0.2.0/pixeltable/catalog/path_dict.py
--rw-r--r--   0        0        0     1059 2024-03-29 02:10:24.352764 pixeltable-0.2.0/pixeltable/catalog/schema_object.py
--rw-r--r--   0        0        0    25499 2024-04-03 21:21:04.613051 pixeltable-0.2.0/pixeltable/catalog/table.py
--rw-r--r--   0        0        0    35680 2024-04-03 21:21:04.613924 pixeltable-0.2.0/pixeltable/catalog/table_version.py
--rw-r--r--   0        0        0     5461 2024-04-03 17:26:04.855707 pixeltable-0.2.0/pixeltable/catalog/table_version_path.py
--rw-r--r--   0        0        0     9734 2024-04-02 22:13:56.672469 pixeltable-0.2.0/pixeltable/catalog/view.py
--rw-r--r--   0        0        0    20548 2024-04-03 21:21:04.614493 pixeltable-0.2.0/pixeltable/client.py
--rw-r--r--   0        0        0    28327 2024-04-03 21:21:04.615036 pixeltable-0.2.0/pixeltable/dataframe.py
--rw-r--r--   0        0        0    16225 2024-04-03 21:21:04.615583 pixeltable-0.2.0/pixeltable/env.py
--rw-r--r--   0        0        0      376 2024-01-15 22:21:10.095679 pixeltable-0.2.0/pixeltable/exceptions.py
--rw-r--r--   0        0        0      412 2024-01-15 22:21:10.095882 pixeltable-0.2.0/pixeltable/exec/__init__.py
--rw-r--r--   0        0        0     3321 2024-04-02 22:13:56.674688 pixeltable-0.2.0/pixeltable/exec/aggregation_node.py
--rw-r--r--   0        0        0     5104 2024-03-29 02:10:24.358353 pixeltable-0.2.0/pixeltable/exec/cache_prefetch_node.py
--rw-r--r--   0        0        0     4069 2024-03-29 02:10:24.358711 pixeltable-0.2.0/pixeltable/exec/component_iteration_node.py
--rw-r--r--   0        0        0     3505 2024-03-29 02:10:24.359053 pixeltable-0.2.0/pixeltable/exec/data_row_batch.py
--rw-r--r--   0        0        0      924 2024-03-29 02:10:24.359224 pixeltable-0.2.0/pixeltable/exec/exec_context.py
--rw-r--r--   0        0        0     2170 2024-01-15 22:21:10.096673 pixeltable-0.2.0/pixeltable/exec/exec_node.py
--rw-r--r--   0        0        0    10810 2024-04-02 22:13:56.675099 pixeltable-0.2.0/pixeltable/exec/expr_eval_node.py
--rw-r--r--   0        0        0     2949 2024-03-29 02:10:24.359831 pixeltable-0.2.0/pixeltable/exec/in_memory_data_node.py
--rw-r--r--   0        0        0     1514 2024-01-15 22:21:10.097303 pixeltable-0.2.0/pixeltable/exec/media_validation_node.py
--rw-r--r--   0        0        0    10318 2024-03-29 02:10:24.360143 pixeltable-0.2.0/pixeltable/exec/sql_scan_node.py
--rw-r--r--   0        0        0      935 2024-04-03 17:26:04.856752 pixeltable-0.2.0/pixeltable/exprs/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-29 02:10:24.360769 pixeltable-0.2.0/pixeltable/exprs/arithmetic_expr.py
--rw-r--r--   0        0        0     2131 2024-03-29 02:10:24.361026 pixeltable-0.2.0/pixeltable/exprs/array_slice.py
--rw-r--r--   0        0        0     2706 2024-03-29 02:10:24.361259 pixeltable-0.2.0/pixeltable/exprs/column_property_ref.py
--rw-r--r--   0        0        0     4794 2024-03-29 02:10:24.361503 pixeltable-0.2.0/pixeltable/exprs/column_ref.py
--rw-r--r--   0        0        0     3000 2024-03-29 02:10:24.361847 pixeltable-0.2.0/pixeltable/exprs/comparison.py
--rw-r--r--   0        0        0     3830 2024-03-29 02:10:24.362201 pixeltable-0.2.0/pixeltable/exprs/compound_predicate.py
--rw-r--r--   0        0        0     7535 2024-01-15 22:21:10.098798 pixeltable-0.2.0/pixeltable/exprs/data_row.py
--rw-r--r--   0        0        0    23748 2024-04-02 22:13:56.676458 pixeltable-0.2.0/pixeltable/exprs/expr.py
--rw-r--r--   0        0        0     1222 2024-01-15 22:21:10.099182 pixeltable-0.2.0/pixeltable/exprs/expr_set.py
--rw-r--r--   0        0        0    16961 2024-04-03 17:26:04.857185 pixeltable-0.2.0/pixeltable/exprs/function_call.py
--rw-r--r--   0        0        0     1537 2024-01-15 22:21:10.099445 pixeltable-0.2.0/pixeltable/exprs/globals.py
--rw-r--r--   0        0        0     4663 2024-03-29 02:10:24.364993 pixeltable-0.2.0/pixeltable/exprs/image_member_access.py
--rw-r--r--   0        0        0     1906 2024-03-29 02:10:24.365419 pixeltable-0.2.0/pixeltable/exprs/image_similarity_predicate.py
--rw-r--r--   0        0        0     4312 2024-03-29 02:10:24.366065 pixeltable-0.2.0/pixeltable/exprs/inline_array.py
--rw-r--r--   0        0        0     3695 2024-03-29 02:10:24.366678 pixeltable-0.2.0/pixeltable/exprs/inline_dict.py
--rw-r--r--   0        0        0     1041 2024-03-29 02:10:24.367023 pixeltable-0.2.0/pixeltable/exprs/is_null.py
--rw-r--r--   0        0        0     4559 2024-03-29 02:10:24.368455 pixeltable-0.2.0/pixeltable/exprs/json_mapper.py
--rw-r--r--   0        0        0     6526 2024-03-29 02:10:24.368997 pixeltable-0.2.0/pixeltable/exprs/json_path.py
--rw-r--r--   0        0        0     1885 2024-03-29 02:10:24.369311 pixeltable-0.2.0/pixeltable/exprs/literal.py
--rw-r--r--   0        0        0     1250 2024-01-15 22:21:10.100425 pixeltable-0.2.0/pixeltable/exprs/object_ref.py
--rw-r--r--   0        0        0     1859 2024-03-29 02:10:24.374640 pixeltable-0.2.0/pixeltable/exprs/predicate.py
--rw-r--r--   0        0        0    16992 2024-04-02 22:13:56.677709 pixeltable-0.2.0/pixeltable/exprs/row_builder.py
--rw-r--r--   0        0        0     4268 2024-03-29 02:10:24.376127 pixeltable-0.2.0/pixeltable/exprs/rowid_ref.py
--rw-r--r--   0        0        0     1793 2024-03-29 02:10:24.376650 pixeltable-0.2.0/pixeltable/exprs/type_cast.py
--rw-r--r--   0        0        0     1361 2024-04-03 17:26:04.857483 pixeltable-0.2.0/pixeltable/exprs/variable.py
--rw-r--r--   0        0        0      457 2024-04-03 17:26:04.858004 pixeltable-0.2.0/pixeltable/func/__init__.py
--rw-r--r--   0        0        0     9177 2024-04-03 17:26:04.858396 pixeltable-0.2.0/pixeltable/func/aggregate_function.py
--rw-r--r--   0        0        0     2350 2024-04-03 17:26:04.858718 pixeltable-0.2.0/pixeltable/func/batched_function.py
--rw-r--r--   0        0        0     2357 2024-04-03 21:21:04.616017 pixeltable-0.2.0/pixeltable/func/callable_function.py
--rw-r--r--   0        0        0     3392 2024-04-03 17:26:04.859226 pixeltable-0.2.0/pixeltable/func/expr_template_function.py
--rw-r--r--   0        0        0     4023 2024-04-03 21:21:04.616348 pixeltable-0.2.0/pixeltable/func/function.py
--rw-r--r--   0        0        0    11456 2024-04-03 21:21:04.616669 pixeltable-0.2.0/pixeltable/func/function_registry.py
--rw-r--r--   0        0        0     1220 2024-04-03 21:21:04.616973 pixeltable-0.2.0/pixeltable/func/globals.py
--rw-r--r--   0        0        0     9650 2024-04-03 17:26:04.859586 pixeltable-0.2.0/pixeltable/func/nos_function.py
--rw-r--r--   0        0        0     7107 2024-04-03 17:26:04.859944 pixeltable-0.2.0/pixeltable/func/signature.py
--rw-r--r--   0        0        0     6457 2024-04-03 21:21:04.617376 pixeltable-0.2.0/pixeltable/func/udf.py
--rw-r--r--   0        0        0     3419 2024-04-03 21:21:04.617766 pixeltable-0.2.0/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0     8453 2024-04-02 22:13:56.685253 pixeltable-0.2.0/pixeltable/functions/eval.py
--rw-r--r--   0        0        0     1595 2024-04-03 21:21:04.618117 pixeltable-0.2.0/pixeltable/functions/fireworks.py
--rw-r--r--   0        0        0     4804 2024-04-03 17:26:04.860757 pixeltable-0.2.0/pixeltable/functions/huggingface.py
--rw-r--r--   0        0        0      431 2024-04-03 17:26:04.861025 pixeltable-0.2.0/pixeltable/functions/image.py
--rw-r--r--   0        0        0     2863 2024-04-03 21:21:04.618487 pixeltable-0.2.0/pixeltable/functions/openai.py
--rw-r--r--   0        0        0     6217 2024-04-03 17:26:04.861910 pixeltable-0.2.0/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      516 2024-04-02 22:13:56.687559 pixeltable-0.2.0/pixeltable/functions/string.py
--rw-r--r--   0        0        0      650 2024-04-03 21:21:04.618764 pixeltable-0.2.0/pixeltable/functions/together.py
--rw-r--r--   0        0        0     1596 2024-04-02 22:13:56.688834 pixeltable-0.2.0/pixeltable/functions/util.py
--rw-r--r--   0        0        0     2403 2024-04-02 22:13:56.689676 pixeltable-0.2.0/pixeltable/functions/video.py
--rw-r--r--   0        0        0       70 2024-01-15 22:21:10.104617 pixeltable-0.2.0/pixeltable/iterators/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-29 02:10:24.389524 pixeltable-0.2.0/pixeltable/iterators/base.py
--rw-r--r--   0        0        0    13088 2024-03-29 02:10:24.390315 pixeltable-0.2.0/pixeltable/iterators/document.py
--rw-r--r--   0        0        0     3444 2024-03-29 02:10:24.390700 pixeltable-0.2.0/pixeltable/iterators/video.py
--rw-r--r--   0        0        0     2083 2024-04-03 17:26:04.862244 pixeltable-0.2.0/pixeltable/metadata/__init__.py
--rw-r--r--   0        0        0      733 2024-03-29 02:10:24.391424 pixeltable-0.2.0/pixeltable/metadata/converters/convert_10.py
--rw-r--r--   0        0        0     7761 2024-04-02 22:13:56.690669 pixeltable-0.2.0/pixeltable/metadata/schema.py
--rw-r--r--   0        0        0    34710 2024-04-03 17:26:04.862980 pixeltable-0.2.0/pixeltable/plan.py
--rw-r--r--   0        0        0    19230 2024-04-02 22:13:56.691931 pixeltable-0.2.0/pixeltable/store.py
--rw-r--r--   0        0        0     6581 2024-04-03 17:26:04.864000 pixeltable-0.2.0/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0     3186 2024-04-03 17:26:04.864518 pixeltable-0.2.0/pixeltable/tests/test_audio.py
--rw-r--r--   0        0        0     1189 2024-01-15 22:21:10.632434 pixeltable-0.2.0/pixeltable/tests/test_catalog.py
--rw-r--r--   0        0        0      531 2024-04-03 17:26:04.864987 pixeltable-0.2.0/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0    17704 2024-04-03 17:26:04.865583 pixeltable-0.2.0/pixeltable/tests/test_component_view.py
--rw-r--r--   0        0        0    17686 2024-04-03 17:26:04.866459 pixeltable-0.2.0/pixeltable/tests/test_dataframe.py
--rw-r--r--   0        0        0     3611 2024-04-03 17:26:04.866972 pixeltable-0.2.0/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0     5657 2024-04-03 17:26:04.867386 pixeltable-0.2.0/pixeltable/tests/test_document.py
--rw-r--r--   0        0        0    32695 2024-04-03 17:26:04.868024 pixeltable-0.2.0/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0    12817 2024-04-03 21:21:04.619175 pixeltable-0.2.0/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0    14477 2024-04-03 17:26:04.869252 pixeltable-0.2.0/pixeltable/tests/test_functions.py
--rw-r--r--   0        0        0     1535 2024-04-03 17:26:04.869854 pixeltable-0.2.0/pixeltable/tests/test_migration.py
--rw-r--r--   0        0        0     2649 2024-04-03 17:26:04.870509 pixeltable-0.2.0/pixeltable/tests/test_nos.py
--rw-r--r--   0        0        0     9297 2024-04-03 17:26:04.871225 pixeltable-0.2.0/pixeltable/tests/test_snapshot.py
--rw-r--r--   0        0        0    48202 2024-04-03 21:21:04.619933 pixeltable-0.2.0/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     1308 2024-04-03 17:26:04.872718 pixeltable-0.2.0/pixeltable/tests/test_transactional_directory.py
--rw-r--r--   0        0        0      970 2024-04-03 17:26:04.873099 pixeltable-0.2.0/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     7676 2024-04-03 17:26:04.873582 pixeltable-0.2.0/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0    21859 2024-04-03 17:26:04.874060 pixeltable-0.2.0/pixeltable/tests/test_view.py
--rw-r--r--   0        0        0     9914 2024-04-03 17:26:04.874467 pixeltable-0.2.0/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     5148 2024-04-03 17:26:04.875028 pixeltable-0.2.0/pixeltable/tool/create_test_db_dump.py
--rw-r--r--   0        0        0    31781 2024-04-03 17:26:04.875632 pixeltable-0.2.0/pixeltable/type_system.py
--rw-r--r--   0        0        0      439 2024-01-15 22:21:10.635863 pixeltable-0.2.0/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0      720 2024-01-15 22:21:10.635981 pixeltable-0.2.0/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     5604 2024-03-29 02:10:24.462374 pixeltable-0.2.0/pixeltable/utils/coco.py
--rw-r--r--   0        0        0     1094 2024-03-29 02:10:24.462842 pixeltable-0.2.0/pixeltable/utils/documents.py
--rw-r--r--   0        0        0     7839 2024-03-29 02:10:24.463396 pixeltable-0.2.0/pixeltable/utils/filecache.py
--rw-r--r--   0        0        0      252 2024-01-15 22:21:10.636442 pixeltable-0.2.0/pixeltable/utils/help.py
--rw-r--r--   0        0        0     3116 2024-03-29 02:10:24.463930 pixeltable-0.2.0/pixeltable/utils/media_store.py
--rw-r--r--   0        0        0     5775 2024-01-15 22:21:10.636686 pixeltable-0.2.0/pixeltable/utils/parquet.py
--rw-r--r--   0        0        0     6515 2024-04-03 17:26:04.876346 pixeltable-0.2.0/pixeltable/utils/pytorch.py
--rw-r--r--   0        0        0      432 2024-01-15 22:21:10.636985 pixeltable-0.2.0/pixeltable/utils/s3.py
--rw-r--r--   0        0        0      765 2024-01-15 22:21:10.637081 pixeltable-0.2.0/pixeltable/utils/sql.py
--rw-r--r--   0        0        0     1349 2024-04-03 17:26:04.876793 pixeltable-0.2.0/pixeltable/utils/transactional_directory.py
--rw-r--r--   0        0        0     3240 2024-04-03 21:22:30.194178 pixeltable-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 pixeltable-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-01-15 22:21:10.025602 pixeltable-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4193 2024-04-04 01:37:06.313845 pixeltable-0.2.1/README.md
+-rw-r--r--   0        0        0      959 2024-04-04 01:37:07.019405 pixeltable-0.2.1/pixeltable/__init__.py
+-rw-r--r--   0        0        0      453 2024-03-29 02:10:24.349472 pixeltable-0.2.1/pixeltable/catalog/__init__.py
+-rw-r--r--   0        0        0     7908 2024-04-02 22:13:56.668343 pixeltable-0.2.1/pixeltable/catalog/catalog.py
+-rw-r--r--   0        0        0     8661 2024-04-03 17:26:04.851919 pixeltable-0.2.1/pixeltable/catalog/column.py
+-rw-r--r--   0        0        0      919 2024-03-29 02:10:24.350840 pixeltable-0.2.1/pixeltable/catalog/dir.py
+-rw-r--r--   0        0        0      943 2024-03-29 02:10:24.351032 pixeltable-0.2.1/pixeltable/catalog/globals.py
+-rw-r--r--   0        0        0     8280 2024-04-03 17:26:04.852785 pixeltable-0.2.1/pixeltable/catalog/insertable_table.py
+-rw-r--r--   0        0        0     1147 2024-03-29 02:10:24.351974 pixeltable-0.2.1/pixeltable/catalog/named_function.py
+-rw-r--r--   0        0        0     1677 2024-04-03 17:26:04.853184 pixeltable-0.2.1/pixeltable/catalog/path.py
+-rw-r--r--   0        0        0     5941 2024-04-03 17:26:04.853564 pixeltable-0.2.1/pixeltable/catalog/path_dict.py
+-rw-r--r--   0        0        0     1059 2024-03-29 02:10:24.352764 pixeltable-0.2.1/pixeltable/catalog/schema_object.py
+-rw-r--r--   0        0        0    25499 2024-04-04 00:19:02.760665 pixeltable-0.2.1/pixeltable/catalog/table.py
+-rw-r--r--   0        0        0    35680 2024-04-04 01:37:07.020191 pixeltable-0.2.1/pixeltable/catalog/table_version.py
+-rw-r--r--   0        0        0     5461 2024-04-03 17:26:04.855707 pixeltable-0.2.1/pixeltable/catalog/table_version_path.py
+-rw-r--r--   0        0        0     9734 2024-04-02 22:13:56.672469 pixeltable-0.2.1/pixeltable/catalog/view.py
+-rw-r--r--   0        0        0    20548 2024-04-04 01:37:07.040061 pixeltable-0.2.1/pixeltable/client.py
+-rw-r--r--   0        0        0    28327 2024-04-04 01:37:07.059370 pixeltable-0.2.1/pixeltable/dataframe.py
+-rw-r--r--   0        0        0    16225 2024-04-04 01:37:07.060269 pixeltable-0.2.1/pixeltable/env.py
+-rw-r--r--   0        0        0      376 2024-01-15 22:21:10.095679 pixeltable-0.2.1/pixeltable/exceptions.py
+-rw-r--r--   0        0        0      412 2024-01-15 22:21:10.095882 pixeltable-0.2.1/pixeltable/exec/__init__.py
+-rw-r--r--   0        0        0     3321 2024-04-02 22:13:56.674688 pixeltable-0.2.1/pixeltable/exec/aggregation_node.py
+-rw-r--r--   0        0        0     5104 2024-03-29 02:10:24.358353 pixeltable-0.2.1/pixeltable/exec/cache_prefetch_node.py
+-rw-r--r--   0        0        0     4069 2024-03-29 02:10:24.358711 pixeltable-0.2.1/pixeltable/exec/component_iteration_node.py
+-rw-r--r--   0        0        0     3505 2024-03-29 02:10:24.359053 pixeltable-0.2.1/pixeltable/exec/data_row_batch.py
+-rw-r--r--   0        0        0      924 2024-03-29 02:10:24.359224 pixeltable-0.2.1/pixeltable/exec/exec_context.py
+-rw-r--r--   0        0        0     2170 2024-01-15 22:21:10.096673 pixeltable-0.2.1/pixeltable/exec/exec_node.py
+-rw-r--r--   0        0        0    10810 2024-04-02 22:13:56.675099 pixeltable-0.2.1/pixeltable/exec/expr_eval_node.py
+-rw-r--r--   0        0        0     2949 2024-03-29 02:10:24.359831 pixeltable-0.2.1/pixeltable/exec/in_memory_data_node.py
+-rw-r--r--   0        0        0     1514 2024-01-15 22:21:10.097303 pixeltable-0.2.1/pixeltable/exec/media_validation_node.py
+-rw-r--r--   0        0        0    10318 2024-03-29 02:10:24.360143 pixeltable-0.2.1/pixeltable/exec/sql_scan_node.py
+-rw-r--r--   0        0        0      935 2024-04-03 17:26:04.856752 pixeltable-0.2.1/pixeltable/exprs/__init__.py
+-rw-r--r--   0        0        0     4386 2024-03-29 02:10:24.360769 pixeltable-0.2.1/pixeltable/exprs/arithmetic_expr.py
+-rw-r--r--   0        0        0     2131 2024-03-29 02:10:24.361026 pixeltable-0.2.1/pixeltable/exprs/array_slice.py
+-rw-r--r--   0        0        0     2706 2024-03-29 02:10:24.361259 pixeltable-0.2.1/pixeltable/exprs/column_property_ref.py
+-rw-r--r--   0        0        0     4794 2024-03-29 02:10:24.361503 pixeltable-0.2.1/pixeltable/exprs/column_ref.py
+-rw-r--r--   0        0        0     3000 2024-03-29 02:10:24.361847 pixeltable-0.2.1/pixeltable/exprs/comparison.py
+-rw-r--r--   0        0        0     3830 2024-03-29 02:10:24.362201 pixeltable-0.2.1/pixeltable/exprs/compound_predicate.py
+-rw-r--r--   0        0        0     7535 2024-01-15 22:21:10.098798 pixeltable-0.2.1/pixeltable/exprs/data_row.py
+-rw-r--r--   0        0        0    23748 2024-04-02 22:13:56.676458 pixeltable-0.2.1/pixeltable/exprs/expr.py
+-rw-r--r--   0        0        0     1222 2024-01-15 22:21:10.099182 pixeltable-0.2.1/pixeltable/exprs/expr_set.py
+-rw-r--r--   0        0        0    16961 2024-04-03 17:26:04.857185 pixeltable-0.2.1/pixeltable/exprs/function_call.py
+-rw-r--r--   0        0        0     1537 2024-01-15 22:21:10.099445 pixeltable-0.2.1/pixeltable/exprs/globals.py
+-rw-r--r--   0        0        0     4663 2024-03-29 02:10:24.364993 pixeltable-0.2.1/pixeltable/exprs/image_member_access.py
+-rw-r--r--   0        0        0     1906 2024-03-29 02:10:24.365419 pixeltable-0.2.1/pixeltable/exprs/image_similarity_predicate.py
+-rw-r--r--   0        0        0     4312 2024-03-29 02:10:24.366065 pixeltable-0.2.1/pixeltable/exprs/inline_array.py
+-rw-r--r--   0        0        0     3695 2024-03-29 02:10:24.366678 pixeltable-0.2.1/pixeltable/exprs/inline_dict.py
+-rw-r--r--   0        0        0     1041 2024-03-29 02:10:24.367023 pixeltable-0.2.1/pixeltable/exprs/is_null.py
+-rw-r--r--   0        0        0     4559 2024-03-29 02:10:24.368455 pixeltable-0.2.1/pixeltable/exprs/json_mapper.py
+-rw-r--r--   0        0        0     6526 2024-03-29 02:10:24.368997 pixeltable-0.2.1/pixeltable/exprs/json_path.py
+-rw-r--r--   0        0        0     1885 2024-03-29 02:10:24.369311 pixeltable-0.2.1/pixeltable/exprs/literal.py
+-rw-r--r--   0        0        0     1250 2024-01-15 22:21:10.100425 pixeltable-0.2.1/pixeltable/exprs/object_ref.py
+-rw-r--r--   0        0        0     1859 2024-03-29 02:10:24.374640 pixeltable-0.2.1/pixeltable/exprs/predicate.py
+-rw-r--r--   0        0        0    16992 2024-04-02 22:13:56.677709 pixeltable-0.2.1/pixeltable/exprs/row_builder.py
+-rw-r--r--   0        0        0     4268 2024-03-29 02:10:24.376127 pixeltable-0.2.1/pixeltable/exprs/rowid_ref.py
+-rw-r--r--   0        0        0     1793 2024-03-29 02:10:24.376650 pixeltable-0.2.1/pixeltable/exprs/type_cast.py
+-rw-r--r--   0        0        0     1361 2024-04-03 17:26:04.857483 pixeltable-0.2.1/pixeltable/exprs/variable.py
+-rw-r--r--   0        0        0      457 2024-04-03 17:26:04.858004 pixeltable-0.2.1/pixeltable/func/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-03 17:26:04.858396 pixeltable-0.2.1/pixeltable/func/aggregate_function.py
+-rw-r--r--   0        0        0     2350 2024-04-03 17:26:04.858718 pixeltable-0.2.1/pixeltable/func/batched_function.py
+-rw-r--r--   0        0        0     2357 2024-04-04 01:37:07.078107 pixeltable-0.2.1/pixeltable/func/callable_function.py
+-rw-r--r--   0        0        0     3392 2024-04-03 17:26:04.859226 pixeltable-0.2.1/pixeltable/func/expr_template_function.py
+-rw-r--r--   0        0        0     4023 2024-04-04 01:37:07.098368 pixeltable-0.2.1/pixeltable/func/function.py
+-rw-r--r--   0        0        0    11456 2024-04-04 01:37:07.099391 pixeltable-0.2.1/pixeltable/func/function_registry.py
+-rw-r--r--   0        0        0     1220 2024-04-04 01:37:07.119033 pixeltable-0.2.1/pixeltable/func/globals.py
+-rw-r--r--   0        0        0     9650 2024-04-03 17:26:04.859586 pixeltable-0.2.1/pixeltable/func/nos_function.py
+-rw-r--r--   0        0        0     7107 2024-04-03 17:26:04.859944 pixeltable-0.2.1/pixeltable/func/signature.py
+-rw-r--r--   0        0        0     6457 2024-04-04 01:37:07.138326 pixeltable-0.2.1/pixeltable/func/udf.py
+-rw-r--r--   0        0        0     3419 2024-04-04 01:37:07.139301 pixeltable-0.2.1/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0     8453 2024-04-02 22:13:56.685253 pixeltable-0.2.1/pixeltable/functions/eval.py
+-rw-r--r--   0        0        0     1596 2024-04-04 02:03:58.915636 pixeltable-0.2.1/pixeltable/functions/fireworks.py
+-rw-r--r--   0        0        0     4804 2024-04-03 17:26:04.860757 pixeltable-0.2.1/pixeltable/functions/huggingface.py
+-rw-r--r--   0        0        0      431 2024-04-03 17:26:04.861025 pixeltable-0.2.1/pixeltable/functions/image.py
+-rw-r--r--   0        0        0     2863 2024-04-04 01:37:07.159142 pixeltable-0.2.1/pixeltable/functions/openai.py
+-rw-r--r--   0        0        0     6217 2024-04-03 17:26:04.861910 pixeltable-0.2.1/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      516 2024-04-02 22:13:56.687559 pixeltable-0.2.1/pixeltable/functions/string.py
+-rw-r--r--   0        0        0      650 2024-04-04 01:37:07.179442 pixeltable-0.2.1/pixeltable/functions/together.py
+-rw-r--r--   0        0        0     1596 2024-04-02 22:13:56.688834 pixeltable-0.2.1/pixeltable/functions/util.py
+-rw-r--r--   0        0        0     2403 2024-04-02 22:13:56.689676 pixeltable-0.2.1/pixeltable/functions/video.py
+-rw-r--r--   0        0        0       70 2024-01-15 22:21:10.104617 pixeltable-0.2.1/pixeltable/iterators/__init__.py
+-rw-r--r--   0        0        0     1545 2024-03-29 02:10:24.389524 pixeltable-0.2.1/pixeltable/iterators/base.py
+-rw-r--r--   0        0        0    13088 2024-03-29 02:10:24.390315 pixeltable-0.2.1/pixeltable/iterators/document.py
+-rw-r--r--   0        0        0     3444 2024-03-29 02:10:24.390700 pixeltable-0.2.1/pixeltable/iterators/video.py
+-rw-r--r--   0        0        0     2083 2024-04-03 17:26:04.862244 pixeltable-0.2.1/pixeltable/metadata/__init__.py
+-rw-r--r--   0        0        0      733 2024-03-29 02:10:24.391424 pixeltable-0.2.1/pixeltable/metadata/converters/convert_10.py
+-rw-r--r--   0        0        0     7761 2024-04-02 22:13:56.690669 pixeltable-0.2.1/pixeltable/metadata/schema.py
+-rw-r--r--   0        0        0    34710 2024-04-03 17:26:04.862980 pixeltable-0.2.1/pixeltable/plan.py
+-rw-r--r--   0        0        0    19230 2024-04-02 22:13:56.691931 pixeltable-0.2.1/pixeltable/store.py
+-rw-r--r--   0        0        0     6581 2024-04-03 17:26:04.864000 pixeltable-0.2.1/pixeltable/tests/conftest.py
+-rw-r--r--   0        0        0     3186 2024-04-03 17:26:04.864518 pixeltable-0.2.1/pixeltable/tests/test_audio.py
+-rw-r--r--   0        0        0     1189 2024-01-15 22:21:10.632434 pixeltable-0.2.1/pixeltable/tests/test_catalog.py
+-rw-r--r--   0        0        0      531 2024-04-03 17:26:04.864987 pixeltable-0.2.1/pixeltable/tests/test_client.py
+-rw-r--r--   0        0        0    17704 2024-04-03 17:26:04.865583 pixeltable-0.2.1/pixeltable/tests/test_component_view.py
+-rw-r--r--   0        0        0    17686 2024-04-03 17:26:04.866459 pixeltable-0.2.1/pixeltable/tests/test_dataframe.py
+-rw-r--r--   0        0        0     3611 2024-04-03 17:26:04.866972 pixeltable-0.2.1/pixeltable/tests/test_dirs.py
+-rw-r--r--   0        0        0     5657 2024-04-03 17:26:04.867386 pixeltable-0.2.1/pixeltable/tests/test_document.py
+-rw-r--r--   0        0        0    32695 2024-04-03 17:26:04.868024 pixeltable-0.2.1/pixeltable/tests/test_exprs.py
+-rw-r--r--   0        0        0    12817 2024-04-04 01:37:07.199475 pixeltable-0.2.1/pixeltable/tests/test_function.py
+-rw-r--r--   0        0        0    14477 2024-04-03 17:26:04.869252 pixeltable-0.2.1/pixeltable/tests/test_functions.py
+-rw-r--r--   0        0        0     1535 2024-04-03 17:26:04.869854 pixeltable-0.2.1/pixeltable/tests/test_migration.py
+-rw-r--r--   0        0        0     2649 2024-04-03 17:26:04.870509 pixeltable-0.2.1/pixeltable/tests/test_nos.py
+-rw-r--r--   0        0        0     9297 2024-04-03 17:26:04.871225 pixeltable-0.2.1/pixeltable/tests/test_snapshot.py
+-rw-r--r--   0        0        0    48202 2024-04-04 01:37:07.200583 pixeltable-0.2.1/pixeltable/tests/test_table.py
+-rw-r--r--   0        0        0     1308 2024-04-03 17:26:04.872718 pixeltable-0.2.1/pixeltable/tests/test_transactional_directory.py
+-rw-r--r--   0        0        0      970 2024-04-03 17:26:04.873099 pixeltable-0.2.1/pixeltable/tests/test_types.py
+-rw-r--r--   0        0        0     7676 2024-04-03 17:26:04.873582 pixeltable-0.2.1/pixeltable/tests/test_video.py
+-rw-r--r--   0        0        0    21859 2024-04-03 17:26:04.874060 pixeltable-0.2.1/pixeltable/tests/test_view.py
+-rw-r--r--   0        0        0     9914 2024-04-03 17:26:04.874467 pixeltable-0.2.1/pixeltable/tests/utils.py
+-rw-r--r--   0        0        0     5148 2024-04-03 17:26:04.875028 pixeltable-0.2.1/pixeltable/tool/create_test_db_dump.py
+-rw-r--r--   0        0        0    31781 2024-04-03 17:26:04.875632 pixeltable-0.2.1/pixeltable/type_system.py
+-rw-r--r--   0        0        0      439 2024-01-15 22:21:10.635863 pixeltable-0.2.1/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0      720 2024-01-15 22:21:10.635981 pixeltable-0.2.1/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     5604 2024-03-29 02:10:24.462374 pixeltable-0.2.1/pixeltable/utils/coco.py
+-rw-r--r--   0        0        0     1094 2024-03-29 02:10:24.462842 pixeltable-0.2.1/pixeltable/utils/documents.py
+-rw-r--r--   0        0        0     7839 2024-03-29 02:10:24.463396 pixeltable-0.2.1/pixeltable/utils/filecache.py
+-rw-r--r--   0        0        0      252 2024-01-15 22:21:10.636442 pixeltable-0.2.1/pixeltable/utils/help.py
+-rw-r--r--   0        0        0     3116 2024-03-29 02:10:24.463930 pixeltable-0.2.1/pixeltable/utils/media_store.py
+-rw-r--r--   0        0        0     5775 2024-01-15 22:21:10.636686 pixeltable-0.2.1/pixeltable/utils/parquet.py
+-rw-r--r--   0        0        0     6515 2024-04-03 17:26:04.876346 pixeltable-0.2.1/pixeltable/utils/pytorch.py
+-rw-r--r--   0        0        0      432 2024-01-15 22:21:10.636985 pixeltable-0.2.1/pixeltable/utils/s3.py
+-rw-r--r--   0        0        0      765 2024-01-15 22:21:10.637081 pixeltable-0.2.1/pixeltable/utils/sql.py
+-rw-r--r--   0        0        0     1349 2024-04-03 17:26:04.876793 pixeltable-0.2.1/pixeltable/utils/transactional_directory.py
+-rw-r--r--   0        0        0     3280 2024-04-04 05:03:44.713584 pixeltable-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 pixeltable-0.2.1/PKG-INFO
```

### Comparing `pixeltable-0.2.0/LICENSE` & `pixeltable-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/README.md` & `pixeltable-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/__init__.py` & `pixeltable-0.2.1/pixeltable/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/catalog.py` & `pixeltable-0.2.1/pixeltable/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/column.py` & `pixeltable-0.2.1/pixeltable/catalog/column.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/dir.py` & `pixeltable-0.2.1/pixeltable/catalog/dir.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/globals.py` & `pixeltable-0.2.1/pixeltable/catalog/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/insertable_table.py` & `pixeltable-0.2.1/pixeltable/catalog/insertable_table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/named_function.py` & `pixeltable-0.2.1/pixeltable/catalog/named_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/path.py` & `pixeltable-0.2.1/pixeltable/catalog/path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/path_dict.py` & `pixeltable-0.2.1/pixeltable/catalog/path_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/schema_object.py` & `pixeltable-0.2.1/pixeltable/catalog/schema_object.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/table.py` & `pixeltable-0.2.1/pixeltable/catalog/table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/table_version.py` & `pixeltable-0.2.1/pixeltable/catalog/table_version.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/table_version_path.py` & `pixeltable-0.2.1/pixeltable/catalog/table_version_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/catalog/view.py` & `pixeltable-0.2.1/pixeltable/catalog/view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/client.py` & `pixeltable-0.2.1/pixeltable/client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/dataframe.py` & `pixeltable-0.2.1/pixeltable/dataframe.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/env.py` & `pixeltable-0.2.1/pixeltable/env.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/aggregation_node.py` & `pixeltable-0.2.1/pixeltable/exec/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/cache_prefetch_node.py` & `pixeltable-0.2.1/pixeltable/exec/cache_prefetch_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/component_iteration_node.py` & `pixeltable-0.2.1/pixeltable/exec/component_iteration_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/data_row_batch.py` & `pixeltable-0.2.1/pixeltable/exec/data_row_batch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/exec_context.py` & `pixeltable-0.2.1/pixeltable/exec/exec_context.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/exec_node.py` & `pixeltable-0.2.1/pixeltable/exec/exec_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/expr_eval_node.py` & `pixeltable-0.2.1/pixeltable/exec/expr_eval_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/in_memory_data_node.py` & `pixeltable-0.2.1/pixeltable/exec/in_memory_data_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/media_validation_node.py` & `pixeltable-0.2.1/pixeltable/exec/media_validation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exec/sql_scan_node.py` & `pixeltable-0.2.1/pixeltable/exec/sql_scan_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/__init__.py` & `pixeltable-0.2.1/pixeltable/exprs/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/arithmetic_expr.py` & `pixeltable-0.2.1/pixeltable/exprs/arithmetic_expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/array_slice.py` & `pixeltable-0.2.1/pixeltable/exprs/array_slice.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/column_property_ref.py` & `pixeltable-0.2.1/pixeltable/exprs/column_property_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/column_ref.py` & `pixeltable-0.2.1/pixeltable/exprs/column_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/comparison.py` & `pixeltable-0.2.1/pixeltable/exprs/comparison.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/compound_predicate.py` & `pixeltable-0.2.1/pixeltable/exprs/compound_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/data_row.py` & `pixeltable-0.2.1/pixeltable/exprs/data_row.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/expr.py` & `pixeltable-0.2.1/pixeltable/exprs/expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/expr_set.py` & `pixeltable-0.2.1/pixeltable/exprs/expr_set.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/function_call.py` & `pixeltable-0.2.1/pixeltable/exprs/function_call.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/globals.py` & `pixeltable-0.2.1/pixeltable/exprs/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/image_member_access.py` & `pixeltable-0.2.1/pixeltable/exprs/image_member_access.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/image_similarity_predicate.py` & `pixeltable-0.2.1/pixeltable/exprs/image_similarity_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/inline_array.py` & `pixeltable-0.2.1/pixeltable/exprs/inline_array.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/inline_dict.py` & `pixeltable-0.2.1/pixeltable/exprs/inline_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/is_null.py` & `pixeltable-0.2.1/pixeltable/exprs/is_null.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/json_mapper.py` & `pixeltable-0.2.1/pixeltable/exprs/json_mapper.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/json_path.py` & `pixeltable-0.2.1/pixeltable/exprs/json_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/literal.py` & `pixeltable-0.2.1/pixeltable/exprs/literal.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/object_ref.py` & `pixeltable-0.2.1/pixeltable/exprs/object_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/predicate.py` & `pixeltable-0.2.1/pixeltable/exprs/predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/row_builder.py` & `pixeltable-0.2.1/pixeltable/exprs/row_builder.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/rowid_ref.py` & `pixeltable-0.2.1/pixeltable/exprs/rowid_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/type_cast.py` & `pixeltable-0.2.1/pixeltable/exprs/type_cast.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/exprs/variable.py` & `pixeltable-0.2.1/pixeltable/exprs/variable.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/aggregate_function.py` & `pixeltable-0.2.1/pixeltable/func/aggregate_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/batched_function.py` & `pixeltable-0.2.1/pixeltable/func/batched_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/callable_function.py` & `pixeltable-0.2.1/pixeltable/func/callable_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/expr_template_function.py` & `pixeltable-0.2.1/pixeltable/func/expr_template_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/function.py` & `pixeltable-0.2.1/pixeltable/func/function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/function_registry.py` & `pixeltable-0.2.1/pixeltable/func/function_registry.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/globals.py` & `pixeltable-0.2.1/pixeltable/func/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/nos_function.py` & `pixeltable-0.2.1/pixeltable/func/nos_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/signature.py` & `pixeltable-0.2.1/pixeltable/func/signature.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/func/udf.py` & `pixeltable-0.2.1/pixeltable/func/udf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/__init__.py` & `pixeltable-0.2.1/pixeltable/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/eval.py` & `pixeltable-0.2.1/pixeltable/functions/eval.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/fireworks.py` & `pixeltable-0.2.1/pixeltable/functions/fireworks.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         'max_tokens': max_tokens,
         'repetition_penalty': repetition_penalty,
         'top_k': top_k,
         'top_p': top_p,
         'temperature': temperature
     }
     kwargs_not_none = dict(filter(lambda x: x[1] is not None, kwargs.items()))
-    print(kwargs_not_none)
+    import fireworks.client
     return fireworks.client.Completion.create(
         model=model,
         prompt_or_messages=prompt,
         **kwargs_not_none
     ).dict()
```

### Comparing `pixeltable-0.2.0/pixeltable/functions/huggingface.py` & `pixeltable-0.2.1/pixeltable/functions/huggingface.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/openai.py` & `pixeltable-0.2.1/pixeltable/functions/openai.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/pil/image.py` & `pixeltable-0.2.1/pixeltable/functions/pil/image.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/string.py` & `pixeltable-0.2.1/pixeltable/functions/string.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/together.py` & `pixeltable-0.2.1/pixeltable/functions/together.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/util.py` & `pixeltable-0.2.1/pixeltable/functions/util.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/functions/video.py` & `pixeltable-0.2.1/pixeltable/functions/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/iterators/base.py` & `pixeltable-0.2.1/pixeltable/iterators/base.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/iterators/document.py` & `pixeltable-0.2.1/pixeltable/iterators/document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/iterators/video.py` & `pixeltable-0.2.1/pixeltable/iterators/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/metadata/__init__.py` & `pixeltable-0.2.1/pixeltable/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/metadata/converters/convert_10.py` & `pixeltable-0.2.1/pixeltable/metadata/converters/convert_10.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/metadata/schema.py` & `pixeltable-0.2.1/pixeltable/metadata/schema.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/plan.py` & `pixeltable-0.2.1/pixeltable/plan.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/store.py` & `pixeltable-0.2.1/pixeltable/store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/conftest.py` & `pixeltable-0.2.1/pixeltable/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_audio.py` & `pixeltable-0.2.1/pixeltable/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_catalog.py` & `pixeltable-0.2.1/pixeltable/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_client.py` & `pixeltable-0.2.1/pixeltable/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_component_view.py` & `pixeltable-0.2.1/pixeltable/tests/test_component_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_dataframe.py` & `pixeltable-0.2.1/pixeltable/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_dirs.py` & `pixeltable-0.2.1/pixeltable/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_document.py` & `pixeltable-0.2.1/pixeltable/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_exprs.py` & `pixeltable-0.2.1/pixeltable/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_function.py` & `pixeltable-0.2.1/pixeltable/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_functions.py` & `pixeltable-0.2.1/pixeltable/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_migration.py` & `pixeltable-0.2.1/pixeltable/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_nos.py` & `pixeltable-0.2.1/pixeltable/tests/test_nos.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_snapshot.py` & `pixeltable-0.2.1/pixeltable/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_table.py` & `pixeltable-0.2.1/pixeltable/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_transactional_directory.py` & `pixeltable-0.2.1/pixeltable/tests/test_transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_types.py` & `pixeltable-0.2.1/pixeltable/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_video.py` & `pixeltable-0.2.1/pixeltable/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/test_view.py` & `pixeltable-0.2.1/pixeltable/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tests/utils.py` & `pixeltable-0.2.1/pixeltable/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/tool/create_test_db_dump.py` & `pixeltable-0.2.1/pixeltable/tool/create_test_db_dump.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/type_system.py` & `pixeltable-0.2.1/pixeltable/type_system.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/clip.py` & `pixeltable-0.2.1/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/coco.py` & `pixeltable-0.2.1/pixeltable/utils/coco.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/documents.py` & `pixeltable-0.2.1/pixeltable/utils/documents.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/filecache.py` & `pixeltable-0.2.1/pixeltable/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/media_store.py` & `pixeltable-0.2.1/pixeltable/utils/media_store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/parquet.py` & `pixeltable-0.2.1/pixeltable/utils/parquet.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/pytorch.py` & `pixeltable-0.2.1/pixeltable/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/sql.py` & `pixeltable-0.2.1/pixeltable/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pixeltable/utils/transactional_directory.py` & `pixeltable-0.2.1/pixeltable/utils/transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.0/pyproject.toml` & `pixeltable-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pixeltable"
-version = "0.2.0"
+version = "0.2.1"
 description = "Pixeltable: The Multimodal AI Data Plane"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
     "pixeltable/.pytest_cache",
     "pixeltable/tests/data"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = ">=3.9,<4.0"
 numpy = "^1.24.1"
 pandas = "^1.5.3"
 pillow = "^9.4.0"
 opencv-python-headless = "^4.7.0.68"
 tqdm = "^4.64.1"
 jmespath = "^1.0.1"
 regex = "^2022.10.31"
 cloudpickle = "^2.2.1"
 psycopg2-binary = "^2.9.5"
 psutil = "^5.9.5"
 sqlalchemy = {extras = ["mypy"], version = "^2.0.23"}
 sqlalchemy-utils = "^0.41.1"
 pgvector = "^0.2.1"
 av = ">=10.0.0"
+pyyaml = "^6.0.1"
+jinja2 = "^3.1.3"
 pgserver = "0.0.5"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # pytest-related
```

### Comparing `pixeltable-0.2.0/PKG-INFO` & `pixeltable-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pixeltable
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pixeltable: The Multimodal AI Data Plane
 Author: Marcel Kornacker
 Author-email: marcelk@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: av (>=10.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pgserver (==0.0.5)
 Requires-Dist: pgvector (>=0.2.1,<0.3.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: regex (>=2022.10.31,<2023.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[mypy] (>=2.0.23,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img src="docs/pixeltable-banner.png" width="45%"/>
```

