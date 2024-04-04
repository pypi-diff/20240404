# Comparing `tmp/jx-python-4.582.24095.tar.gz` & `tmp/jx-python-4.583.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx-python-4.582.24095.tar", last modified: Thu Apr  4 04:16:15 2024, max compression
+gzip compressed data, was "jx-python-4.583.24095.tar", last modified: Thu Apr  4 12:04:51 2024, max compression
```

## Comparing `jx-python-4.582.24095.tar` & `jx-python-4.583.24095.tar`

### file list

```diff
@@ -1,302 +1,287 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.067338 jx-python-4.582.24095/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 jx-python-4.582.24095/LICENSE
--rw-rw-rw-   0        0        0     1743 2024-04-04 04:16:15.066336 jx-python-4.582.24095/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-03-08 02:37:16.000000 jx-python-4.582.24095/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.597650 jx-python-4.582.24095/jx_base/
--rw-rw-rw-   0        0        0     1553 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/__init__.py
--rw-rw-rw-   0        0        0     8710 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/data_class.py
--rw-rw-rw-   0        0        0    25274 2024-02-06 05:15:22.000000 jx-python-4.582.24095/jx_base/domains.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.878298 jx-python-4.582.24095/jx_base/expressions/
--rw-rw-rw-   0        0        0    10593 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/__init__.py
--rw-rw-rw-   0        0        0     4925 2024-03-20 02:23:03.000000 jx-python-4.582.24095/jx_base/expressions/_utils.py
--rw-rw-rw-   0        0        0     1027 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/abs_op.py
--rw-rw-rw-   0        0        0      800 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/add_op.py
--rw-rw-rw-   0        0        0     2379 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/aggregate_op.py
--rw-rw-rw-   0        0        0     1277 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/all_op.py
--rw-rw-rw-   0        0        0     3312 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/and_op.py
--rw-rw-rw-   0        0        0     1394 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/any_op.py
--rw-rw-rw-   0        0        0      918 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/array_of_op.py
--rw-rw-rw-   0        0        0      453 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/avg_op.py
--rw-rw-rw-   0        0        0     2183 2024-01-22 13:00:58.000000 jx-python-4.582.24095/jx_base/expressions/base_binary_op.py
--rw-rw-rw-   0        0        0      520 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/base_inequality_op.py
--rw-rw-rw-   0        0        0     2960 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/base_multi_op.py
--rw-rw-rw-   0        0        0      391 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/basic_add_op.py
--rw-rw-rw-   0        0        0     1546 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_boolean_op.py
--rw-rw-rw-   0        0        0     1109 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/basic_eq_op.py
--rw-rw-rw-   0        0        0     3370 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_in_op.py
--rw-rw-rw-   0        0        0     1972 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/basic_index_of_op.py
--rw-rw-rw-   0        0        0      391 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/basic_mul_op.py
--rw-rw-rw-   0        0        0     1966 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_multi_op.py
--rw-rw-rw-   0        0        0     1277 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_not_op.py
--rw-rw-rw-   0        0        0     1666 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_starts_with_op.py
--rw-rw-rw-   0        0        0     1332 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_substring_op.py
--rw-rw-rw-   0        0        0     4496 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/between_op.py
--rw-rw-rw-   0        0        0     1544 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/call_op.py
--rw-rw-rw-   0        0        0      661 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/cardinality_op.py
--rw-rw-rw-   0        0        0     4044 2024-03-21 02:47:56.000000 jx-python-4.582.24095/jx_base/expressions/case_op.py
--rw-rw-rw-   0        0        0     2037 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     1593 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/comment_op.py
--rw-rw-rw-   0        0        0     2890 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/concat_op.py
--rw-rw-rw-   0        0        0     1592 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/count_op.py
--rw-rw-rw-   0        0        0     1250 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/date_op.py
--rw-rw-rw-   0        0        0     2111 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/default_op.py
--rw-rw-rw-   0        0        0     1179 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/div_op.py
--rw-rw-rw-   0        0        0     2757 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/eq_op.py
--rw-rw-rw-   0        0        0      418 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/es_script.py
--rw-rw-rw-   0        0        0     1525 2024-01-28 16:03:01.000000 jx-python-4.582.24095/jx_base/expressions/es_select_op.py
--rw-rw-rw-   0        0        0     1270 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/exists_op.py
--rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/exp_op.py
--rw-rw-rw-   0        0        0     6265 2024-01-22 13:00:58.000000 jx-python-4.582.24095/jx_base/expressions/expression.py
--rw-rw-rw-   0        0        0     1524 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/false_op.py
--rw-rw-rw-   0        0        0     1278 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/filter_op.py
--rw-rw-rw-   0        0        0     2242 2024-01-28 16:03:01.000000 jx-python-4.582.24095/jx_base/expressions/find_op.py
--rw-rw-rw-   0        0        0     2413 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/first_op.py
--rw-rw-rw-   0        0        0      657 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/floor_op.py
--rw-rw-rw-   0        0        0    10147 2024-02-06 05:15:22.000000 jx-python-4.582.24095/jx_base/expressions/format_op.py
--rw-rw-rw-   0        0        0     1577 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/from_op.py
--rw-rw-rw-   0        0        0      807 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/from_unix_op.py
--rw-rw-rw-   0        0        0     3022 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/get_op.py
--rw-rw-rw-   0        0        0     1082 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/group_op.py
--rw-rw-rw-   0        0        0      385 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/gt_op.py
--rw-rw-rw-   0        0        0      386 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/gte_op.py
--rw-rw-rw-   0        0        0     3648 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/in_op.py
--rw-rw-rw-   0        0        0     2505 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/inner_join_op.py
--rw-rw-rw-   0        0        0     1322 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_boolean_op.py
--rw-rw-rw-   0        0        0      969 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_integer_op.py
--rw-rw-rw-   0        0        0     1360 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_number_op.py
--rw-rw-rw-   0        0        0     1451 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_text_op.py
--rw-rw-rw-   0        0        0     1561 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/last_op.py
--rw-rw-rw-   0        0        0     1761 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/least_op.py
--rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/leaves_op.py
--rw-rw-rw-   0        0        0     2037 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/left_op.py
--rw-rw-rw-   0        0        0     1601 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/length_op.py
--rw-rw-rw-   0        0        0     2593 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/limit_op.py
--rw-rw-rw-   0        0        0     3326 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/literal.py
--rw-rw-rw-   0        0        0      384 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/lt_op.py
--rw-rw-rw-   0        0        0      385 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/lte_op.py
--rw-rw-rw-   0        0        0      507 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/map_op.py
--rw-rw-rw-   0        0        0     1418 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/max_op.py
--rw-rw-rw-   0        0        0     1442 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/min_op.py
--rw-rw-rw-   0        0        0     1861 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/missing_op.py
--rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/mod_op.py
--rw-rw-rw-   0        0        0      845 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/most_op.py
--rw-rw-rw-   0        0        0      882 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/mul_op.py
--rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/name_op.py
--rw-rw-rw-   0        0        0     1647 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/ne_op.py
--rw-rw-rw-   0        0        0     4366 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/nested_op.py
--rw-rw-rw-   0        0        0     2061 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/not_left_op.py
--rw-rw-rw-   0        0        0     1612 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/not_op.py
--rw-rw-rw-   0        0        0     2150 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/not_right_op.py
--rw-rw-rw-   0        0        0     2442 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/null_op.py
--rw-rw-rw-   0        0        0     1059 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/offset_op.py
--rw-rw-rw-   0        0        0     2239 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/or_op.py
--rw-rw-rw-   0        0        0     2503 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/outer_join_op.py
--rw-rw-rw-   0        0        0     1387 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/percentile_op.py
--rw-rw-rw-   0        0        0     3285 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/prefix_op.py
--rw-rw-rw-   0        0        0     1585 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/product_op.py
--rw-rw-rw-   0        0        0      460 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/python_function.py
--rw-rw-rw-   0        0        0     1512 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/python_script.py
--rw-rw-rw-   0        0        0    24585 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/query_op.py
--rw-rw-rw-   0        0        0     1025 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/range_op.py
--rw-rw-rw-   0        0        0     1575 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0     2247 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/right_op.py
--rw-rw-rw-   0        0        0     1478 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/rows_op.py
--rw-rw-rw-   0        0        0     1247 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/script_op.py
--rw-rw-rw-   0        0        0    12251 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/select_op.py
--rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/split_op.py
--rw-rw-rw-   0        0        0     1295 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/sql_alias_op.py
--rw-rw-rw-   0        0        0     1027 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_and_op.py
--rw-rw-rw-   0        0        0     1010 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/sql_cast_op.py
--rw-rw-rw-   0        0        0     1361 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_concat_op.py
--rw-rw-rw-   0        0        0     1490 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/sql_eq_op.py
--rw-rw-rw-   0        0        0     1082 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_gt_op.py
--rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_gte_op.py
--rw-rw-rw-   0        0        0      343 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_in_op.py
--rw-rw-rw-   0        0        0      428 2024-01-22 13:00:58.000000 jx-python-4.582.24095/jx_base/expressions/sql_inner_join_op.py
--rw-rw-rw-   0        0        0     1192 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/sql_instr_op.py
--rw-rw-rw-   0        0        0      832 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/sql_is_null_op.py
--rw-rw-rw-   0        0        0     3313 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sql_left_joins_op.py
--rw-rw-rw-   0        0        0      499 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_limit_op.py
--rw-rw-rw-   0        0        0      360 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/sql_literal.py
--rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_lt_op.py
--rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_lte_op.py
--rw-rw-rw-   0        0        0     1449 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/sql_not_op.py
--rw-rw-rw-   0        0        0     2371 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_or_op.py
--rw-rw-rw-   0        0        0      781 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_order_by_op.py
--rw-rw-rw-   0        0        0     1057 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sql_origins_op.py
--rw-rw-rw-   0        0        0      427 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/sql_script.py
--rw-rw-rw-   0        0        0      958 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sql_select_all_from_op.py
--rw-rw-rw-   0        0        0     2012 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0      911 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/sql_substr_op.py
--rw-rw-rw-   0        0        0     1583 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_variable.py
--rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_add_op.py
--rw-rw-rw-   0        0        0     1549 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_boolean_op.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_eq_op.py
--rw-rw-rw-   0        0        0     3378 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_in_op.py
--rw-rw-rw-   0        0        0     1976 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_index_of_op.py
--rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_mul_op.py
--rw-rw-rw-   0        0        0     1967 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_multi_op.py
--rw-rw-rw-   0        0        0     1281 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_not_op.py
--rw-rw-rw-   0        0        0     1671 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_starts_with_op.py
--rw-rw-rw-   0        0        0     1335 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_substring_op.py
--rw-rw-rw-   0        0        0      611 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sub_op.py
--rw-rw-rw-   0        0        0     3011 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/suffix_op.py
--rw-rw-rw-   0        0        0     1556 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sum_op.py
--rw-rw-rw-   0        0        0      721 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/tally_op.py
--rw-rw-rw-   0        0        0     1594 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/to_array_op.py
--rw-rw-rw-   0        0        0     1304 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0     2708 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     2874 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/to_number_op.py
--rw-rw-rw-   0        0        0     2043 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/to_text_op.py
--rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/to_value_op.py
--rw-rw-rw-   0        0        0     1626 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/true_op.py
--rw-rw-rw-   0        0        0     1678 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/tuple_op.py
--rw-rw-rw-   0        0        0     2000 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/union_op.py
--rw-rw-rw-   0        0        0      826 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/unix_op.py
--rw-rw-rw-   0        0        0     6148 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/variable.py
--rw-rw-rw-   0        0        0     3270 2024-03-21 02:47:56.000000 jx-python-4.582.24095/jx_base/expressions/when_op.py
--rw-rw-rw-   0        0        0    14462 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/language.py
--rw-rw-rw-   0        0        0    15169 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/meta_columns.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.886703 jx-python-4.582.24095/jx_base/models/
--rw-rw-rw-   0        0        0        0 2022-11-12 15:14:28.000000 jx-python-4.582.24095/jx_base/models/__init__.py
--rw-rw-rw-   0        0        0     2369 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/container.py
--rw-rw-rw-   0        0        0    13016 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/dimensions.py
--rw-rw-rw-   0        0        0      945 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/facts.py
--rw-rw-rw-   0        0        0     1656 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/namespace.py
--rw-rw-rw-   0        0        0      294 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/nested_path.py
--rw-rw-rw-   0        0        0      408 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/relation.py
--rw-rw-rw-   0        0        0     5523 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/schema.py
--rw-rw-rw-   0        0        0      833 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/snowflake.py
--rw-rw-rw-   0        0        0      687 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/table.py
--rw-rw-rw-   0        0        0      791 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/queries.py
--rw-rw-rw-   0        0        0     2520 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.898849 jx-python-4.582.24095/jx_python/
--rw-rw-rw-   0        0        0      614 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.934413 jx-python-4.582.24095/jx_python/containers/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.582.24095/jx_python/containers/__init__.py
--rw-rw-rw-   0        0        0    16625 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/containers/cube.py
--rw-rw-rw-   0        0        0     9580 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/containers/list.py
--rw-rw-rw-   0        0        0     1836 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/convert.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.936838 jx-python-4.582.24095/jx_python/cubes/
--rw-rw-rw-   0        0        0        0 2020-01-29 00:24:56.000000 jx-python-4.582.24095/jx_python/cubes/__init__.py
--rw-rw-rw-   0        0        0     3647 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/cubes/aggs.py
--rw-rw-rw-   0        0        0     1920 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expression_compiler.py
--rw-rw-rw-   0        0        0     1735 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expression_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.051797 jx-python-4.582.24095/jx_python/expressions/
--rw-rw-rw-   0        0        0     3964 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/__init__.py
--rw-rw-rw-   0        0        0     4641 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/_utils.py
--rw-rw-rw-   0        0        0      440 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/add_op.py
--rw-rw-rw-   0        0        0      945 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_python/expressions/and_op.py
--rw-rw-rw-   0        0        0      857 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/array_of_op.py
--rw-rw-rw-   0        0        0      714 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/avg_op.py
--rw-rw-rw-   0        0        0      884 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/basic_add_op.py
--rw-rw-rw-   0        0        0      846 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/basic_eq_op.py
--rw-rw-rw-   0        0        0      866 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/basic_index_of_op.py
--rw-rw-rw-   0        0        0      907 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/expressions/basic_starts_with_op.py
--rw-rw-rw-   0        0        0      993 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/expressions/basic_substring_op.py
--rw-rw-rw-   0        0        0      372 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/between_op.py
--rw-rw-rw-   0        0        0     1285 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/call_op.py
--rw-rw-rw-   0        0        0      673 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/cardinality_op.py
--rw-rw-rw-   0        0        0      716 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/case_op.py
--rw-rw-rw-   0        0        0      976 2024-01-21 21:27:17.000000 jx-python-4.582.24095/jx_python/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     1146 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/concat_op.py
--rw-rw-rw-   0        0        0      786 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/count_op.py
--rw-rw-rw-   0        0        0      554 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/date_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/div_op.py
--rw-rw-rw-   0        0        0     1608 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/eq_op.py
--rw-rw-rw-   0        0        0      750 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/exists_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/exp_op.py
--rw-rw-rw-   0        0        0      635 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/false_op.py
--rw-rw-rw-   0        0        0     1110 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/filter_op.py
--rw-rw-rw-   0        0        0     1692 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/find_op.py
--rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/first_op.py
--rw-rw-rw-   0        0        0      647 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/floor_op.py
--rw-rw-rw-   0        0        0      368 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/format_op.py
--rw-rw-rw-   0        0        0     1823 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/get_op.py
--rw-rw-rw-   0        0        0     1707 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/group_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/gt_op.py
--rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/gte_op.py
--rw-rw-rw-   0        0        0      831 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/in_op.py
--rw-rw-rw-   0        0        0      787 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/is_text_op.py
--rw-rw-rw-   0        0        0     1109 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/last_op.py
--rw-rw-rw-   0        0        0     1026 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_python/expressions/least_op.py
--rw-rw-rw-   0        0        0      559 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/leaves_op.py
--rw-rw-rw-   0        0        0      692 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/length_op.py
--rw-rw-rw-   0        0        0      953 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/limit_op.py
--rw-rw-rw-   0        0        0      618 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/literal.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/lt_op.py
--rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/lte_op.py
--rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/max_op.py
--rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/min_op.py
--rw-rw-rw-   0        0        0     1045 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/missing_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/mod_op.py
--rw-rw-rw-   0        0        0      981 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/most_op.py
--rw-rw-rw-   0        0        0      533 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/mul_op.py
--rw-rw-rw-   0        0        0      992 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/name_op.py
--rw-rw-rw-   0        0        0      733 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/ne_op.py
--rw-rw-rw-   0        0        0      773 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/not_left_op.py
--rw-rw-rw-   0        0        0      680 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/not_op.py
--rw-rw-rw-   0        0        0      999 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/not_right_op.py
--rw-rw-rw-   0        0        0      556 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/offset_op.py
--rw-rw-rw-   0        0        0      930 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/or_op.py
--rw-rw-rw-   0        0        0      468 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/percentile_op.py
--rw-rw-rw-   0        0        0      651 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/prefix_op.py
--rw-rw-rw-   0        0        0     1303 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/product_op.py
--rw-rw-rw-   0        0        0     1139 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/python_function.py
--rw-rw-rw-   0        0        0     1443 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/python_script.py
--rw-rw-rw-   0        0        0      364 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/range_op.py
--rw-rw-rw-   0        0        0      946 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0      699 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/right_op.py
--rw-rw-rw-   0        0        0     1022 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/rows_op.py
--rw-rw-rw-   0        0        0      594 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/script_op.py
--rw-rw-rw-   0        0        0     2105 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/select_op.py
--rw-rw-rw-   0        0        0      643 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/split_op.py
--rw-rw-rw-   0        0        0      888 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_add_op.py
--rw-rw-rw-   0        0        0      850 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_eq_op.py
--rw-rw-rw-   0        0        0      870 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_index_of_op.py
--rw-rw-rw-   0        0        0      912 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_starts_with_op.py
--rw-rw-rw-   0        0        0      998 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_substring_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/sub_op.py
--rw-rw-rw-   0        0        0      742 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_python/expressions/suffix_op.py
--rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/sum_op.py
--rw-rw-rw-   0        0        0     1056 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/tally_op.py
--rw-rw-rw-   0        0        0      835 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/to_array_op.py
--rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0      606 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     1034 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/to_number_op.py
--rw-rw-rw-   0        0        0      800 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/to_text_op.py
--rw-rw-rw-   0        0        0      957 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/to_value_op.py
--rw-rw-rw-   0        0        0      628 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/true_op.py
--rw-rw-rw-   0        0        0      812 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/tuple_op.py
--rw-rw-rw-   0        0        0     1328 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/variable.py
--rw-rw-rw-   0        0        0      968 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/when_op.py
--rw-rw-rw-   0        0        0     4434 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/flat_list.py
--rw-rw-rw-   0        0        0     4439 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/group_by.py
--rw-rw-rw-   0        0        0    34076 2024-01-25 04:46:12.000000 jx-python-4.582.24095/jx_python/jx.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.054808 jx-python-4.582.24095/jx_python/lists/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.582.24095/jx_python/lists/__init__.py
--rw-rw-rw-   0        0        0     5009 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/lists/aggs.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.056805 jx-python-4.582.24095/jx_python/namespace/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.582.24095/jx_python/namespace/__init__.py
--rw-rw-rw-   0        0        0     8745 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/namespace/normal.py
--rw-rw-rw-   0        0        0      768 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/records.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.062323 jx-python-4.582.24095/jx_python/streams/
--rw-rw-rw-   0        0        0     4178 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/streams/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/expression_compiler.py
--rw-rw-rw-   0        0        0     4727 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/streams/expression_factory.py
--rw-rw-rw-   0        0        0      713 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/inspects.py
--rw-rw-rw-   0        0        0      807 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/type_parser.py
--rw-rw-rw-   0        0        0     5515 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/typers.py
--rw-rw-rw-   0        0        0     1622 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/streams.py
--rw-rw-rw-   0        0        0      564 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/table.py
--rw-rw-rw-   0        0        0     1431 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/utils.py
--rw-rw-rw-   0        0        0     7410 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/windows.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.064339 jx-python-4.582.24095/jx_python.egg-info/
--rw-rw-rw-   0        0        0     1743 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9472 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 04:16:15.067338 jx-python-4.582.24095/setup.cfg
--rw-rw-rw-   0        0        0     1872 2024-04-04 04:16:09.000000 jx-python-4.582.24095/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.818856 jx-python-4.583.24095/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 jx-python-4.583.24095/LICENSE
+-rw-rw-rw-   0        0        0     1743 2024-04-04 12:04:51.817814 jx-python-4.583.24095/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-03-08 02:37:16.000000 jx-python-4.583.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.539322 jx-python-4.583.24095/jx_base/
+-rw-rw-rw-   0        0        0     1553 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/__init__.py
+-rw-rw-rw-   0        0        0     8710 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/data_class.py
+-rw-rw-rw-   0        0        0    25274 2024-02-06 05:15:22.000000 jx-python-4.583.24095/jx_base/domains.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.676572 jx-python-4.583.24095/jx_base/expressions/
+-rw-rw-rw-   0        0        0    10593 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4925 2024-03-20 02:23:03.000000 jx-python-4.583.24095/jx_base/expressions/_utils.py
+-rw-rw-rw-   0        0        0     1027 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/abs_op.py
+-rw-rw-rw-   0        0        0      800 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/add_op.py
+-rw-rw-rw-   0        0        0     2379 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/aggregate_op.py
+-rw-rw-rw-   0        0        0     1277 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/all_op.py
+-rw-rw-rw-   0        0        0     3312 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/and_op.py
+-rw-rw-rw-   0        0        0     1394 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/any_op.py
+-rw-rw-rw-   0        0        0      918 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/expressions/array_of_op.py
+-rw-rw-rw-   0        0        0      453 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/avg_op.py
+-rw-rw-rw-   0        0        0     2183 2024-01-22 13:00:58.000000 jx-python-4.583.24095/jx_base/expressions/base_binary_op.py
+-rw-rw-rw-   0        0        0      520 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/base_inequality_op.py
+-rw-rw-rw-   0        0        0     2960 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/base_multi_op.py
+-rw-rw-rw-   0        0        0     4496 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1544 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/call_op.py
+-rw-rw-rw-   0        0        0      661 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/cardinality_op.py
+-rw-rw-rw-   0        0        0     4044 2024-03-21 02:47:56.000000 jx-python-4.583.24095/jx_base/expressions/case_op.py
+-rw-rw-rw-   0        0        0     2037 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_base/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     1593 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/comment_op.py
+-rw-rw-rw-   0        0        0     2890 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/concat_op.py
+-rw-rw-rw-   0        0        0     1592 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/count_op.py
+-rw-rw-rw-   0        0        0     1250 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/date_op.py
+-rw-rw-rw-   0        0        0     2111 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_base/expressions/default_op.py
+-rw-rw-rw-   0        0        0     1179 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/div_op.py
+-rw-rw-rw-   0        0        0     2757 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      418 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/expressions/es_script.py
+-rw-rw-rw-   0        0        0     1525 2024-01-28 16:03:01.000000 jx-python-4.583.24095/jx_base/expressions/es_select_op.py
+-rw-rw-rw-   0        0        0     1270 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/exp_op.py
+-rw-rw-rw-   0        0        0     6265 2024-01-22 13:00:58.000000 jx-python-4.583.24095/jx_base/expressions/expression.py
+-rw-rw-rw-   0        0        0     1524 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/false_op.py
+-rw-rw-rw-   0        0        0     1278 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     2242 2024-01-28 16:03:01.000000 jx-python-4.583.24095/jx_base/expressions/find_op.py
+-rw-rw-rw-   0        0        0     2413 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/first_op.py
+-rw-rw-rw-   0        0        0      657 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/floor_op.py
+-rw-rw-rw-   0        0        0    10147 2024-02-06 05:15:22.000000 jx-python-4.583.24095/jx_base/expressions/format_op.py
+-rw-rw-rw-   0        0        0     1577 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/from_op.py
+-rw-rw-rw-   0        0        0      807 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/from_unix_op.py
+-rw-rw-rw-   0        0        0     3022 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/get_op.py
+-rw-rw-rw-   0        0        0     1082 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/group_op.py
+-rw-rw-rw-   0        0        0      385 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      386 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/gte_op.py
+-rw-rw-rw-   0        0        0     3648 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/in_op.py
+-rw-rw-rw-   0        0        0     2505 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/inner_join_op.py
+-rw-rw-rw-   0        0        0     1322 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/is_boolean_op.py
+-rw-rw-rw-   0        0        0      969 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/is_integer_op.py
+-rw-rw-rw-   0        0        0     1360 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/is_number_op.py
+-rw-rw-rw-   0        0        0     1451 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0     1561 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/last_op.py
+-rw-rw-rw-   0        0        0     1761 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/least_op.py
+-rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0     2037 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/left_op.py
+-rw-rw-rw-   0        0        0     1601 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_base/expressions/length_op.py
+-rw-rw-rw-   0        0        0     2593 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/limit_op.py
+-rw-rw-rw-   0        0        0     3326 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/literal.py
+-rw-rw-rw-   0        0        0      384 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      385 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      507 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/expressions/map_op.py
+-rw-rw-rw-   0        0        0     1418 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/max_op.py
+-rw-rw-rw-   0        0        0     1442 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1861 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/mod_op.py
+-rw-rw-rw-   0        0        0      845 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/most_op.py
+-rw-rw-rw-   0        0        0      882 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/mul_op.py
+-rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/name_op.py
+-rw-rw-rw-   0        0        0     1647 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/ne_op.py
+-rw-rw-rw-   0        0        0     4366 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/nested_op.py
+-rw-rw-rw-   0        0        0     2061 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0     1612 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/not_op.py
+-rw-rw-rw-   0        0        0     2150 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0     2442 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/null_op.py
+-rw-rw-rw-   0        0        0     1059 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/offset_op.py
+-rw-rw-rw-   0        0        0     2239 2024-03-02 22:12:26.000000 jx-python-4.583.24095/jx_base/expressions/or_op.py
+-rw-rw-rw-   0        0        0     2503 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/outer_join_op.py
+-rw-rw-rw-   0        0        0     1387 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/percentile_op.py
+-rw-rw-rw-   0        0        0     3285 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0     1585 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/product_op.py
+-rw-rw-rw-   0        0        0      460 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/expressions/python_function.py
+-rw-rw-rw-   0        0        0     1512 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/python_script.py
+-rw-rw-rw-   0        0        0    24585 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/query_op.py
+-rw-rw-rw-   0        0        0     1025 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/range_op.py
+-rw-rw-rw-   0        0        0     1575 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0     2247 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/right_op.py
+-rw-rw-rw-   0        0        0     1478 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/rows_op.py
+-rw-rw-rw-   0        0        0     1247 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/script_op.py
+-rw-rw-rw-   0        0        0    12251 2024-02-15 03:10:30.000000 jx-python-4.583.24095/jx_base/expressions/select_op.py
+-rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/split_op.py
+-rw-rw-rw-   0        0        0     1295 2024-02-15 03:10:30.000000 jx-python-4.583.24095/jx_base/expressions/sql_alias_op.py
+-rw-rw-rw-   0        0        0     1027 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_and_op.py
+-rw-rw-rw-   0        0        0     1010 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_base/expressions/sql_cast_op.py
+-rw-rw-rw-   0        0        0     1361 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_concat_op.py
+-rw-rw-rw-   0        0        0     1490 2024-03-10 19:33:03.000000 jx-python-4.583.24095/jx_base/expressions/sql_eq_op.py
+-rw-rw-rw-   0        0        0     1082 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.583.24095/jx_base/expressions/sql_gt_op.py
+-rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.583.24095/jx_base/expressions/sql_gte_op.py
+-rw-rw-rw-   0        0        0      343 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_in_op.py
+-rw-rw-rw-   0        0        0      428 2024-01-22 13:00:58.000000 jx-python-4.583.24095/jx_base/expressions/sql_inner_join_op.py
+-rw-rw-rw-   0        0        0     1192 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_base/expressions/sql_instr_op.py
+-rw-rw-rw-   0        0        0      832 2024-03-10 19:33:03.000000 jx-python-4.583.24095/jx_base/expressions/sql_is_null_op.py
+-rw-rw-rw-   0        0        0     3313 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/sql_left_joins_op.py
+-rw-rw-rw-   0        0        0      499 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_limit_op.py
+-rw-rw-rw-   0        0        0      360 2024-02-15 03:10:30.000000 jx-python-4.583.24095/jx_base/expressions/sql_literal.py
+-rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.583.24095/jx_base/expressions/sql_lt_op.py
+-rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.583.24095/jx_base/expressions/sql_lte_op.py
+-rw-rw-rw-   0        0        0     1449 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/sql_not_op.py
+-rw-rw-rw-   0        0        0     2371 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_or_op.py
+-rw-rw-rw-   0        0        0      781 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_order_by_op.py
+-rw-rw-rw-   0        0        0     1057 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/sql_origins_op.py
+-rw-rw-rw-   0        0        0      427 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/expressions/sql_script.py
+-rw-rw-rw-   0        0        0      958 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/sql_select_all_from_op.py
+-rw-rw-rw-   0        0        0     2012 2024-02-15 03:10:30.000000 jx-python-4.583.24095/jx_base/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0      911 2024-03-10 19:33:03.000000 jx-python-4.583.24095/jx_base/expressions/sql_substr_op.py
+-rw-rw-rw-   0        0        0     1583 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sql_variable.py
+-rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0     1549 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_boolean_op.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0     3378 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_in_op.py
+-rw-rw-rw-   0        0        0     1976 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_mul_op.py
+-rw-rw-rw-   0        0        0     1967 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_multi_op.py
+-rw-rw-rw-   0        0        0     1281 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_not_op.py
+-rw-rw-rw-   0        0        0     1671 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0     1335 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0      611 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/sub_op.py
+-rw-rw-rw-   0        0        0     3011 2024-03-02 22:12:26.000000 jx-python-4.583.24095/jx_base/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0     1556 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/sum_op.py
+-rw-rw-rw-   0        0        0      721 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/tally_op.py
+-rw-rw-rw-   0        0        0     1594 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/to_array_op.py
+-rw-rw-rw-   0        0        0     1304 2024-03-02 22:12:26.000000 jx-python-4.583.24095/jx_base/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0     2708 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     2874 2024-03-02 22:12:26.000000 jx-python-4.583.24095/jx_base/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0     2043 2024-03-10 19:33:03.000000 jx-python-4.583.24095/jx_base/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/to_value_op.py
+-rw-rw-rw-   0        0        0     1626 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/true_op.py
+-rw-rw-rw-   0        0        0     1678 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0     2000 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/union_op.py
+-rw-rw-rw-   0        0        0      826 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/expressions/unix_op.py
+-rw-rw-rw-   0        0        0     6148 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/expressions/variable.py
+-rw-rw-rw-   0        0        0     3270 2024-03-21 02:47:56.000000 jx-python-4.583.24095/jx_base/expressions/when_op.py
+-rw-rw-rw-   0        0        0    14462 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_base/language.py
+-rw-rw-rw-   0        0        0    15169 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_base/meta_columns.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.686061 jx-python-4.583.24095/jx_base/models/
+-rw-rw-rw-   0        0        0        0 2022-11-12 15:14:28.000000 jx-python-4.583.24095/jx_base/models/__init__.py
+-rw-rw-rw-   0        0        0     2369 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/models/container.py
+-rw-rw-rw-   0        0        0    13016 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/models/dimensions.py
+-rw-rw-rw-   0        0        0      945 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/models/facts.py
+-rw-rw-rw-   0        0        0     1656 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/models/namespace.py
+-rw-rw-rw-   0        0        0      294 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/models/nested_path.py
+-rw-rw-rw-   0        0        0      408 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_base/models/relation.py
+-rw-rw-rw-   0        0        0     5523 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/models/schema.py
+-rw-rw-rw-   0        0        0      833 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/models/snowflake.py
+-rw-rw-rw-   0        0        0      687 2024-03-16 21:27:51.000000 jx-python-4.583.24095/jx_base/models/table.py
+-rw-rw-rw-   0        0        0      791 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_base/queries.py
+-rw-rw-rw-   0        0        0     2520 2024-02-15 03:10:30.000000 jx-python-4.583.24095/jx_base/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.697650 jx-python-4.583.24095/jx_python/
+-rw-rw-rw-   0        0        0      614 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.722732 jx-python-4.583.24095/jx_python/containers/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.583.24095/jx_python/containers/__init__.py
+-rw-rw-rw-   0        0        0    16625 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/containers/cube.py
+-rw-rw-rw-   0        0        0     9580 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/containers/list.py
+-rw-rw-rw-   0        0        0     1836 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/convert.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.724829 jx-python-4.583.24095/jx_python/cubes/
+-rw-rw-rw-   0        0        0        0 2020-01-29 00:24:56.000000 jx-python-4.583.24095/jx_python/cubes/__init__.py
+-rw-rw-rw-   0        0        0     3647 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/cubes/aggs.py
+-rw-rw-rw-   0        0        0     1920 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expression_compiler.py
+-rw-rw-rw-   0        0        0     1735 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expression_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.805055 jx-python-4.583.24095/jx_python/expressions/
+-rw-rw-rw-   0        0        0     3964 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4641 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/_utils.py
+-rw-rw-rw-   0        0        0      440 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/add_op.py
+-rw-rw-rw-   0        0        0      945 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_python/expressions/and_op.py
+-rw-rw-rw-   0        0        0      857 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/array_of_op.py
+-rw-rw-rw-   0        0        0      714 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/avg_op.py
+-rw-rw-rw-   0        0        0      372 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1285 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/call_op.py
+-rw-rw-rw-   0        0        0      673 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/cardinality_op.py
+-rw-rw-rw-   0        0        0      716 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/case_op.py
+-rw-rw-rw-   0        0        0      976 2024-01-21 21:27:17.000000 jx-python-4.583.24095/jx_python/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     1146 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/concat_op.py
+-rw-rw-rw-   0        0        0      786 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/count_op.py
+-rw-rw-rw-   0        0        0      554 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/date_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/div_op.py
+-rw-rw-rw-   0        0        0     1608 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      750 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/exp_op.py
+-rw-rw-rw-   0        0        0      635 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/false_op.py
+-rw-rw-rw-   0        0        0     1110 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     1692 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/find_op.py
+-rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/first_op.py
+-rw-rw-rw-   0        0        0      647 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/floor_op.py
+-rw-rw-rw-   0        0        0      368 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/format_op.py
+-rw-rw-rw-   0        0        0     1823 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/get_op.py
+-rw-rw-rw-   0        0        0     1707 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/group_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/gte_op.py
+-rw-rw-rw-   0        0        0      831 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/in_op.py
+-rw-rw-rw-   0        0        0      787 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0     1109 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/last_op.py
+-rw-rw-rw-   0        0        0     1026 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_python/expressions/least_op.py
+-rw-rw-rw-   0        0        0      559 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0      692 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/length_op.py
+-rw-rw-rw-   0        0        0      953 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/limit_op.py
+-rw-rw-rw-   0        0        0      618 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/literal.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/max_op.py
+-rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1045 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/mod_op.py
+-rw-rw-rw-   0        0        0      981 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/most_op.py
+-rw-rw-rw-   0        0        0      533 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/mul_op.py
+-rw-rw-rw-   0        0        0      992 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/name_op.py
+-rw-rw-rw-   0        0        0      733 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/ne_op.py
+-rw-rw-rw-   0        0        0      773 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0      680 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/not_op.py
+-rw-rw-rw-   0        0        0      999 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0      556 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/offset_op.py
+-rw-rw-rw-   0        0        0      930 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/or_op.py
+-rw-rw-rw-   0        0        0      468 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/percentile_op.py
+-rw-rw-rw-   0        0        0      651 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0     1303 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/product_op.py
+-rw-rw-rw-   0        0        0     1139 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/python_function.py
+-rw-rw-rw-   0        0        0     1443 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/python_script.py
+-rw-rw-rw-   0        0        0      364 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/range_op.py
+-rw-rw-rw-   0        0        0      946 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0      699 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/right_op.py
+-rw-rw-rw-   0        0        0     1022 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/rows_op.py
+-rw-rw-rw-   0        0        0      594 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/script_op.py
+-rw-rw-rw-   0        0        0     2105 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/select_op.py
+-rw-rw-rw-   0        0        0      643 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/split_op.py
+-rw-rw-rw-   0        0        0      888 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0      850 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0      870 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      912 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0      998 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/sub_op.py
+-rw-rw-rw-   0        0        0      742 2024-02-27 03:13:49.000000 jx-python-4.583.24095/jx_python/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/sum_op.py
+-rw-rw-rw-   0        0        0     1056 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/tally_op.py
+-rw-rw-rw-   0        0        0      835 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/to_array_op.py
+-rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0      606 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     1034 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0      800 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0      957 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/to_value_op.py
+-rw-rw-rw-   0        0        0      628 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/true_op.py
+-rw-rw-rw-   0        0        0      812 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0     1328 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/expressions/variable.py
+-rw-rw-rw-   0        0        0      968 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/expressions/when_op.py
+-rw-rw-rw-   0        0        0     4434 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/flat_list.py
+-rw-rw-rw-   0        0        0     4439 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/group_by.py
+-rw-rw-rw-   0        0        0    34076 2024-01-25 04:46:12.000000 jx-python-4.583.24095/jx_python/jx.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.807139 jx-python-4.583.24095/jx_python/lists/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.583.24095/jx_python/lists/__init__.py
+-rw-rw-rw-   0        0        0     5009 2024-04-04 04:16:05.000000 jx-python-4.583.24095/jx_python/lists/aggs.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.809206 jx-python-4.583.24095/jx_python/namespace/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.583.24095/jx_python/namespace/__init__.py
+-rw-rw-rw-   0        0        0     8745 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/namespace/normal.py
+-rw-rw-rw-   0        0        0      768 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/records.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.814492 jx-python-4.583.24095/jx_python/streams/
+-rw-rw-rw-   0        0        0     4178 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/streams/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/streams/expression_compiler.py
+-rw-rw-rw-   0        0        0     4727 2024-01-20 18:36:41.000000 jx-python-4.583.24095/jx_python/streams/expression_factory.py
+-rw-rw-rw-   0        0        0      713 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/streams/inspects.py
+-rw-rw-rw-   0        0        0      807 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/streams/type_parser.py
+-rw-rw-rw-   0        0        0     5515 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/streams/typers.py
+-rw-rw-rw-   0        0        0     1622 2024-03-16 21:32:01.000000 jx-python-4.583.24095/jx_python/streams.py
+-rw-rw-rw-   0        0        0      564 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/table.py
+-rw-rw-rw-   0        0        0     1431 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/utils.py
+-rw-rw-rw-   0        0        0     7410 2023-06-17 11:25:18.000000 jx-python-4.583.24095/jx_python/windows.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:51.815785 jx-python-4.583.24095/jx_python.egg-info/
+-rw-rw-rw-   0        0        0     1743 2024-04-04 12:04:51.000000 jx-python-4.583.24095/jx_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8881 2024-04-04 12:04:51.000000 jx-python-4.583.24095/jx_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:04:51.000000 jx-python-4.583.24095/jx_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      265 2024-04-04 12:04:51.000000 jx-python-4.583.24095/jx_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-04 12:04:51.000000 jx-python-4.583.24095/jx_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:04:51.818856 jx-python-4.583.24095/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2024-04-04 12:04:46.000000 jx-python-4.583.24095/setup.py
```

### Comparing `jx-python-4.582.24095/LICENSE` & `jx-python-4.583.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/PKG-INFO` & `jx-python-4.583.24095/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-python
-Version: 4.582.24095
+Version: 4.583.24095
 Summary: JSON query expressions using Python
 Home-page: https://github.com/klahnakoski/jx-python
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `jx-python-4.582.24095/jx_base/__init__.py` & `jx-python-4.583.24095/jx_base/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/data_class.py` & `jx-python-4.583.24095/jx_base/data_class.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/domains.py` & `jx-python-4.583.24095/jx_base/domains.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/__init__.py` & `jx-python-4.583.24095/jx_base/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/_utils.py` & `jx-python-4.583.24095/jx_base/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/abs_op.py` & `jx-python-4.583.24095/jx_base/expressions/abs_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/add_op.py` & `jx-python-4.583.24095/jx_base/expressions/add_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/aggregate_op.py` & `jx-python-4.583.24095/jx_base/expressions/aggregate_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/all_op.py` & `jx-python-4.583.24095/jx_base/expressions/all_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/and_op.py` & `jx-python-4.583.24095/jx_base/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/any_op.py` & `jx-python-4.583.24095/jx_base/expressions/any_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/array_of_op.py` & `jx-python-4.583.24095/jx_base/expressions/array_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/base_binary_op.py` & `jx-python-4.583.24095/jx_base/expressions/base_binary_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/base_inequality_op.py` & `jx-python-4.583.24095/jx_base/expressions/base_inequality_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/base_multi_op.py` & `jx-python-4.583.24095/jx_base/expressions/base_multi_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_boolean_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_boolean_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.null_op import NULL
 from jx_base.expressions.not_op import NotOp
 from mo_json.types import JX_BOOLEAN
 
 
-class BasicBooleanOp(Expression):
+class StrictBooleanOp(Expression):
     """
     FORCE VALUE TO BOOLEAN, USING COMMON SENSE
     * NULL IS FALSE
     * EMPTY STRING IS FALSE
     * ZERO IS FALSE
     """
 
     _jx_type = JX_BOOLEAN
 
     def __init__(self, term):
         Expression.__init__(self, term)
         self.term = term
 
     def __data__(self):
-        return {"basic.boolean": self.term.__data__()}
+        return {"strict.boolean": self.term.__data__()}
 
     def vars(self):
         return self.term.vars()
 
     def map(self, map_):
-        return BasicBooleanOp(self.term.map(map_))
+        return StrictBooleanOp(self.term.map(map_))
 
     def missing(self, lang):
         return FALSE
 
     def partial_eval(self, lang):
         term = self.term.partial_eval(lang)
         if term is NULL:
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_eq_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_eq_op.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #
 from jx_base.expressions.base_inequality_op import BaseInequalityOp
 from jx_base.expressions.literal import is_literal
 from jx_base.expressions.not_op import NotOp
 from mo_json import JX_BOOLEAN
 
 
-class BasicEqOp(BaseInequalityOp):
+class StrictEqOp(BaseInequalityOp):
     """
     STRICT `==` OPERATOR (CAN NOT DEAL WITH NULLS)
     """
-    op = "basic.eq"
+    op = "strict.eq"
 
     def __call__(self, row, rownum=None, rows=None):
         return self.lhs(row, rownum, rows) == self.rhs(row, rownum, rows)
 
     def partial_eval(self, lang):
         lhs = self.lhs.partial_eval(lang)
         rhs = self.rhs.partial_eval(lang)
         if is_literal(rhs) and rhs.value == 0:
             lhs._jx_type = JX_BOOLEAN
             return NotOp(lhs)
         if is_literal(lhs) and lhs.value == 0:
             rhs._jx_type = JX_BOOLEAN
             return NotOp(rhs)
-        return lang.BasicEqOp(lhs, rhs)
+        return lang.StrictEqOp(lhs, rhs)
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_in_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_in_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from mo_logs import Log
 
 EqOp, MissingOp, NestedOp, NotOp, NULL, Variable, is_variable = expect(
     "EqOp", "MissingOp", "NestedOp", "NotOp", "NULL", "Variable", "is_variable"
 )
 
 
-class BasicInOp(Expression):
+class StrictInOp(Expression):
     has_simple_form = True
     _jx_type = JX_BOOLEAN
 
     def __new__(cls, value, superset):
         if is_variable(value) and is_op(superset, Literal) and not is_many(superset.value):
             return EqOp(value, Literal(superset.value))
         return object.__new__(cls)
@@ -37,46 +37,46 @@
         self.value = value
         self.superset = superset
         if self.value is None:
             Log.error("Should not happpen")
 
     def __data__(self):
         if is_variable(self.value) and is_literal(self.superset):
-            return {"basic.in": {self.value.var: self.superset.value}}
+            return {"strict.in": {self.value.var: self.superset.value}}
         else:
-            return {"basic.in": [self.value.__data__(), self.superset.__data__()]}
+            return {"strict.in": [self.value.__data__(), self.superset.__data__()]}
 
     def __eq__(self, other):
-        if is_op(other, BasicInOp):
+        if is_op(other, StrictInOp):
             return self.value == other.value and self.superset == other.superset
         return False
 
     def vars(self):
         return self.value.vars()
 
     def map(self, map_):
-        return BasicInOp(self.value.map(map_), self.superset.map(map_))
+        return StrictInOp(self.value.map(map_), self.superset.map(map_))
 
     def partial_eval(self, lang):
         value = self.value.partial_eval(lang)
         superset = self.superset.partial_eval(lang)
         if superset is NULL:
             return FALSE
         elif value is NULL:
             return NULL
         elif is_literal(value) and is_literal(superset):
             return Literal(value() in superset())
         elif is_op(value, NestedOp):
             return (
-                NestedOp(value.nested_path, None, lang.AndOp(BasicInOp(value.select, superset), value.where),)
+                NestedOp(value.nested_path, None, lang.AndOp(StrictInOp(value.select, superset), value.where),)
                 .exists()
                 .partial_eval(lang)
             )
         else:
-            return lang.BasicInOp(value, superset)
+            return lang.StrictInOp(value, superset)
 
     def __call__(self, row, rownum=None, rows=None):
         value = self.value(row)
         superset = self.superset(row)
         if value == None:
             return None
         if superset == None:
@@ -84,15 +84,15 @@
         return value in superset
 
     def missing(self, lang):
         return FALSE
 
     def invert(self, lang):
         this = self.partial_eval(lang)
-        if is_op(this, BasicInOp):
+        if is_op(this, StrictInOp):
             inv = NotOp(this)
             inv.simplified = True
             return inv
         else:
             return this.invert(lang)
 
     def __rcontains__(self, superset):
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_index_of_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_index_of_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from jx_base.expressions.literal import ZERO
 from jx_base.expressions.max_op import MaxOp
 from jx_base.expressions.to_text_op import ToTextOp
 from jx_base.language import is_op
 from mo_json import JX_INTEGER
 
 
-class BasicIndexOfOp(Expression):
+class StrictIndexOfOp(Expression):
     """
     PLACEHOLDER FOR STRICT value.indexOf(find, start) (CAN NOT DEAL WITH NULLS)
     RETURN -1 IF NOT FOUND
     """
 
     _jx_type = JX_INTEGER
 
@@ -36,28 +36,28 @@
     def __call__(self, row, rownum=None, rows=None):
         value = self.value(row)
         find = self.find(row)
         start = self.start(row)
         return value.find(find, start)
 
     def __data__(self):
-        return {"basic.indexOf": [self.value.__data__(), self.find.__data__(), self.start.__data__()]}
+        return {"strict.indexOf": [self.value.__data__(), self.find.__data__(), self.start.__data__()]}
 
     def vars(self):
         return self.value.vars() | self.find.vars() | self.start.vars()
 
     def missing(self, lang):
         return FALSE
 
     def invert(self, lang):
         return FALSE
 
     def partial_eval(self, lang):
         start = ToIntegerOp(MaxOp(ZERO, self.start)).partial_eval(lang)
-        return self.lang.BasicIndexOfOp(
+        return self.lang.StrictIndexOfOp(
             ToTextOp(self.value).partial_eval(lang), ToTextOp(self.find).partial_eval(lang), start,
         )
 
     def __eq__(self, other):
-        if not is_op(other, BasicIndexOfOp):
+        if not is_op(other, StrictIndexOfOp):
             return False
         return self.value == self.value and self.find == other.find and self.start == other.start
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_multi_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_multi_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.literal import Literal
 from jx_base.expressions.null_op import NULL
 from jx_base.language import is_op
 from mo_json.types import JX_NUMBER
 
 
-class BasicMultiOp(Expression):
+class StrictMultiOp(Expression):
     """
     PLACEHOLDER FOR STRICT MULTI-VALUED OPERATIONS (CAN NOT DEAL WITH NULLS)
     """
 
     _jx_type = JX_NUMBER
     op = None
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_not_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_not_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 
 from jx_base.expressions.expression import Expression
 from jx_base.language import is_op
 from mo_json.types import JX_BOOLEAN
 
 
-class BasicNotOp(Expression):
+class StrictNotOp(Expression):
     _jx_type = JX_BOOLEAN
 
     def __init__(self, term):
         Expression.__init__(self, term)
         self.term = term
 
     def __data__(self):
-        return {"basic.not": self.term.__data__()}
+        return {"strict.not": self.term.__data__()}
 
     def __call__(self, row, rownum=None, rows=None):
         return not self.term(row, rownum, rows)
 
     def __eq__(self, other):
-        if not is_op(other, BasicNotOp):
+        if not is_op(other, StrictNotOp):
             return False
         return self.term == other.term
 
     def vars(self):
         return self.term.vars()
 
     def map(self, map_):
@@ -41,11 +41,11 @@
     def missing(self, lang):
         return (self.term).missing(lang)
 
     def invert(self, lang):
         return self.term.partial_eval(lang)
 
     def partial_eval(self, lang):
-        if is_op(self.term, BasicNotOp):
+        if is_op(self.term, StrictNotOp):
             return self.term
         else:
             return self
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_starts_with_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_starts_with_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.is_text_op import IsTextOp
 from jx_base.language import is_op
 from mo_json.types import JX_BOOLEAN
 
 
-class BasicStartsWithOp(Expression):
+class StrictStartsWithOp(Expression):
     """
     PLACEHOLDER FOR BASIC value.startsWith(find, start) (CAN NOT DEAL WITH NULLS)
     """
 
     _jx_type = JX_BOOLEAN
 
     def __init__(self, *params):
@@ -30,26 +30,26 @@
     def __call__(self, row, rownum=None, rows=None):
         if self.value(row, rownum, rows).startswith(self.prefix(row, rownum, rows)):
             return True
         else:
             return False
 
     def __data__(self):
-        return {"basic.startsWith": [self.value.__data__(), self.prefix.__data__()]}
+        return {"strict.startsWith": [self.value.__data__(), self.prefix.__data__()]}
 
     def __eq__(self, other):
-        if is_op(other, BasicStartsWithOp):
+        if is_op(other, StrictStartsWithOp):
             return self.value == other.value and self.prefix == other.prefix
 
     def vars(self):
         return self.value.vars() | self.prefix.vars()
 
     def map(self, map_):
-        return self.lang.BasicStartsWithOp(self.value.map(map_), self.prefix.map(map_),)
+        return self.lang.StrictStartsWithOp(self.value.map(map_), self.prefix.map(map_),)
 
     def missing(self, lang):
         return FALSE
 
     def partial_eval(self, lang):
-        return lang.BasicStartsWithOp(
+        return lang.StrictStartsWithOp(
             IsTextOp(self.value).partial_eval(lang), IsTextOp(self.prefix).partial_eval(lang),
         )
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/basic_substring_op.py` & `jx-python-4.583.24095/jx_base/expressions/strict_substring_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.false_op import FALSE
 from mo_json.types import JX_TEXT
 
 
-class BasicSubstringOp(Expression):
+class StrictSubstringOp(Expression):
     """
     PLACEHOLDER FOR BASIC value.substring(start, end) (CAN NOT DEAL WITH NULLS)
     """
 
     _jx_type = JX_TEXT
 
     def __init__(self, value, start, end):
         Expression.__init__(self, value, start, end)
         self.value, self.start, self.end = value, start, end
 
     def __call__(self, row, rownum=None, rows=None):
         return self.value(row, rownum, rows)[self.start(row, rownum, rows) : self.end(row, rownum, rows)]
 
     def __data__(self):
-        return {"basic.substring": [self.value.__data__(), self.start.__data__(), self.end.__data__()]}
+        return {"strict.substring": [self.value.__data__(), self.start.__data__(), self.end.__data__()]}
 
     def map(self, map_):
-        return BasicSubstringOp(self.value.map(map_), self.start.map(map_), self.end.map(map_),)
+        return StrictSubstringOp(self.value.map(map_), self.start.map(map_), self.end.map(map_),)
 
     def vars(self):
         return self.value.vars() | self.start.vars() | self.end.vars()
 
     def missing(self, lang):
         return FALSE
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/between_op.py` & `jx-python-4.583.24095/jx_base/expressions/between_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/call_op.py` & `jx-python-4.583.24095/jx_base/expressions/call_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/cardinality_op.py` & `jx-python-4.583.24095/jx_base/expressions/cardinality_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/case_op.py` & `jx-python-4.583.24095/jx_base/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/coalesce_op.py` & `jx-python-4.583.24095/jx_base/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/comment_op.py` & `jx-python-4.583.24095/jx_base/expressions/comment_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/concat_op.py` & `jx-python-4.583.24095/jx_base/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/count_op.py` & `jx-python-4.583.24095/jx_base/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/date_op.py` & `jx-python-4.583.24095/jx_base/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/default_op.py` & `jx-python-4.583.24095/jx_base/expressions/default_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/div_op.py` & `jx-python-4.583.24095/jx_base/expressions/div_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/eq_op.py` & `jx-python-4.583.24095/jx_base/expressions/eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/es_select_op.py` & `jx-python-4.583.24095/jx_base/expressions/es_select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/exists_op.py` & `jx-python-4.583.24095/jx_base/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/expression.py` & `jx-python-4.583.24095/jx_base/expressions/expression.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/false_op.py` & `jx-python-4.583.24095/jx_base/expressions/false_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/filter_op.py` & `jx-python-4.583.24095/jx_base/expressions/filter_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/find_op.py` & `jx-python-4.583.24095/jx_base/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/first_op.py` & `jx-python-4.583.24095/jx_base/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/floor_op.py` & `jx-python-4.583.24095/jx_base/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/format_op.py` & `jx-python-4.583.24095/jx_base/expressions/format_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/from_op.py` & `jx-python-4.583.24095/jx_base/expressions/from_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/from_unix_op.py` & `jx-python-4.583.24095/jx_base/expressions/from_unix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/get_op.py` & `jx-python-4.583.24095/jx_base/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/group_op.py` & `jx-python-4.583.24095/jx_base/expressions/group_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/in_op.py` & `jx-python-4.583.24095/jx_base/expressions/in_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/inner_join_op.py` & `jx-python-4.583.24095/jx_base/expressions/inner_join_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/is_boolean_op.py` & `jx-python-4.583.24095/jx_base/expressions/is_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/is_integer_op.py` & `jx-python-4.583.24095/jx_base/expressions/is_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/is_number_op.py` & `jx-python-4.583.24095/jx_base/expressions/is_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/is_text_op.py` & `jx-python-4.583.24095/jx_base/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/last_op.py` & `jx-python-4.583.24095/jx_base/expressions/last_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/least_op.py` & `jx-python-4.583.24095/jx_base/expressions/least_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/leaves_op.py` & `jx-python-4.583.24095/jx_base/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/left_op.py` & `jx-python-4.583.24095/jx_base/expressions/left_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/length_op.py` & `jx-python-4.583.24095/jx_base/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/limit_op.py` & `jx-python-4.583.24095/jx_base/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/literal.py` & `jx-python-4.583.24095/jx_base/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/max_op.py` & `jx-python-4.583.24095/jx_base/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/min_op.py` & `jx-python-4.583.24095/jx_base/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/missing_op.py` & `jx-python-4.583.24095/jx_base/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/most_op.py` & `jx-python-4.583.24095/jx_base/expressions/most_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/mul_op.py` & `jx-python-4.583.24095/jx_base/expressions/mul_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/name_op.py` & `jx-python-4.583.24095/jx_base/expressions/name_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/ne_op.py` & `jx-python-4.583.24095/jx_base/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/nested_op.py` & `jx-python-4.583.24095/jx_base/expressions/nested_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/not_left_op.py` & `jx-python-4.583.24095/jx_base/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/not_op.py` & `jx-python-4.583.24095/jx_base/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/not_right_op.py` & `jx-python-4.583.24095/jx_base/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/null_op.py` & `jx-python-4.583.24095/jx_base/expressions/null_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/offset_op.py` & `jx-python-4.583.24095/jx_base/expressions/offset_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/or_op.py` & `jx-python-4.583.24095/jx_base/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/outer_join_op.py` & `jx-python-4.583.24095/jx_base/expressions/outer_join_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/percentile_op.py` & `jx-python-4.583.24095/jx_base/expressions/percentile_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/prefix_op.py` & `jx-python-4.583.24095/jx_base/expressions/prefix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/product_op.py` & `jx-python-4.583.24095/jx_base/expressions/product_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/python_script.py` & `jx-python-4.583.24095/jx_base/expressions/python_script.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/query_op.py` & `jx-python-4.583.24095/jx_base/expressions/query_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/range_op.py` & `jx-python-4.583.24095/jx_base/expressions/range_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/reg_exp_op.py` & `jx-python-4.583.24095/jx_base/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/right_op.py` & `jx-python-4.583.24095/jx_base/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/rows_op.py` & `jx-python-4.583.24095/jx_base/expressions/rows_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/script_op.py` & `jx-python-4.583.24095/jx_base/expressions/script_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/select_op.py` & `jx-python-4.583.24095/jx_base/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/split_op.py` & `jx-python-4.583.24095/jx_base/expressions/split_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_alias_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_alias_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_and_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_and_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_cast_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_cast_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_concat_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_eq_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_group_by_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_group_by_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_instr_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_instr_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_is_null_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_is_null_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_left_joins_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_left_joins_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_not_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_not_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_or_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_or_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_order_by_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_order_by_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_origins_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_origins_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_select_all_from_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_select_all_from_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_select_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_substr_op.py` & `jx-python-4.583.24095/jx_base/expressions/sql_substr_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sql_variable.py` & `jx-python-4.583.24095/jx_base/expressions/sql_variable.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/strict_boolean_op.py` & `jx-python-4.583.24095/jx_python/expressions/eq_op.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,57 +3,43 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
-from mo_imports import export
-from jx_base.expressions.expression import Expression
-from jx_base.expressions.false_op import FALSE
-from jx_base.expressions.null_op import NULL
-from jx_base.expressions.not_op import NotOp
-from mo_json.types import JX_BOOLEAN
-
-
-class StrictBooleanOp(Expression):
-    """
-    FORCE VALUE TO BOOLEAN, USING COMMON SENSE
-    * NULL IS FALSE
-    * EMPTY STRING IS FALSE
-    * ZERO IS FALSE
-    """
-
-    _jx_type = JX_BOOLEAN
-
-    def __init__(self, term):
-        Expression.__init__(self, term)
-        self.term = term
-
-    def __data__(self):
-        return {"strict.boolean": self.term.__data__()}
-
-    def vars(self):
-        return self.term.vars()
-
-    def map(self, map_):
-        return StrictBooleanOp(self.term.map(map_))
-
-    def missing(self, lang):
-        return FALSE
+from jx_base.expressions import EqOp as _EqOp, is_literal, FALSE, TRUE, ToArrayOp
+from jx_base.expressions.python_script import PythonScript
+from jx_base.language import value_compare
+from jx_python.expressions import Python
+from jx_python.expressions.strict_eq_op import StrictEqOp
+from jx_python.expressions.case_op import CaseOp
+from jx_python.expressions.when_op import WhenOp
+from jx_python.utils import merge_locals
+from mo_json import JX_BOOLEAN
+
+
+class EqOp(_EqOp):
+    def to_python(self, loop_depth=0):
+        lhs = ToArrayOp(self.lhs).partial_eval(Python).to_python(loop_depth)
+        rhs = self.rhs.to_python(loop_depth)
+        return PythonScript(
+            merge_locals(rhs.locals, lhs.locals),
+            loop_depth,
+            JX_BOOLEAN,
+            f"({rhs.source}) in ({lhs.source})",
+            self,
+            FALSE,
+        )
 
     def partial_eval(self, lang):
-        term = self.term.partial_eval(lang)
-        if term is NULL:
-            return FALSE
-        elif term.jx_type is JX_BOOLEAN:
-            return term
-        elif term is self.term:
-            return self
+        lhs = self.lhs.partial_eval(lang)
+        rhs = self.rhs.partial_eval(lang)
 
-        truthy = AndOp(
-            NotOp(term.missing(lang)),
-            NotOp(InOp(term, [Literal(""), Literal("F"), Literal("false"), NeOp(term, ZERO)])),
-        ).partial_eval(lang)
-        return truthy
+        if is_literal(lhs) and is_literal(rhs):
+            return FALSE if value_compare(lhs.value, rhs.value) else TRUE
+        else:
+            return CaseOp(
+                WhenOp(lhs.missing(lang), then=rhs.missing(lang)),
+                WhenOp(rhs.missing(lang), then=FALSE),
+                StrictEqOp(lhs, rhs),
+            ).partial_eval(lang)
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/strict_eq_op.py` & `jx-python-4.583.24095/jx_base/expressions/to_boolean_op.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,32 +3,49 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from jx_base.expressions.base_inequality_op import BaseInequalityOp
-from jx_base.expressions.literal import is_literal
-from jx_base.expressions.not_op import NotOp
+
+from jx_base.expressions.expression import Expression, TRUE
+from mo_imports import export
 from mo_json import JX_BOOLEAN
 
 
-class StrictEqOp(BaseInequalityOp):
+class ToBooleanOp(Expression):
     """
-    STRICT `==` OPERATOR (CAN NOT DEAL WITH NULLS)
+    CONVERT VALUE TO BOOLEAN, OR KEEP AS BOOLEAN
     """
-    op = "strict.eq"
 
-    def __call__(self, row, rownum=None, rows=None):
-        return self.lhs(row, rownum, rows) == self.rhs(row, rownum, rows)
+    _jx_type = JX_BOOLEAN
+
+    def __init__(self, term):
+        Expression.__init__(self, term)
+        self.term = term
+
+    def __data__(self):
+        return {"boolean": self.term.__data__()}
+
+    def __eq__(self, other):
+        return isinstance(other, ToBooleanOp) and self.term == other.term
+
+    def vars(self):
+        return self.term.vars()
+
+    def map(self, map_):
+        return ToBooleanOp(self.term.map(map_))
+
+    def missing(self, lang):
+        return self.term.missing(lang)
 
     def partial_eval(self, lang):
-        lhs = self.lhs.partial_eval(lang)
-        rhs = self.rhs.partial_eval(lang)
-        if is_literal(rhs) and rhs.value == 0:
-            lhs._jx_type = JX_BOOLEAN
-            return NotOp(lhs)
-        if is_literal(lhs) and lhs.value == 0:
-            rhs._jx_type = JX_BOOLEAN
-            return NotOp(rhs)
-        return lang.StrictEqOp(lhs, rhs)
+        term = self.term.partial_eval(lang)
+        if term.jx_type == JX_BOOLEAN or term.missing(lang) is TRUE:
+            return term
+        elif term is self.term:
+            return self
+        return ToBooleanOp(term)
+
+
+export("jx_base.expressions.and_op", ToBooleanOp)
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/strict_multi_op.py` & `jx-python-4.583.24095/jx_base/expressions/to_array_op.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,69 +3,54 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
-from jx_base.expressions._utils import builtin_ops
 from jx_base.expressions.expression import Expression
-from jx_base.expressions.false_op import FALSE
-from jx_base.expressions.literal import Literal
-from jx_base.expressions.null_op import NULL
+from jx_base.expressions.filter_op import FilterOp
+from jx_base.expressions.group_op import GroupOp
+from jx_base.expressions.literal import NULL, Literal
+from jx_base.expressions.select_op import SelectOp
 from jx_base.language import is_op
-from mo_json.types import JX_NUMBER
+from mo_json import ARRAY
+from mo_json.types import array_of
 
 
-class StrictMultiOp(Expression):
+class ToArrayOp(Expression):
     """
-    PLACEHOLDER FOR STRICT MULTI-VALUED OPERATIONS (CAN NOT DEAL WITH NULLS)
+    Ensure the result is an array, or Null
     """
 
-    _jx_type = JX_NUMBER
-    op = None
+    def __init__(self, term):
+        Expression.__init__(self, term)
+        self.term = term
 
-    def __init__(self, *terms):
-        Expression.__init__(self, *terms)
-        self.terms = terms
+    def __data__(self):
+        return {"to_array": self.term.__data__()}
 
-    def vars(self):
-        output = set()
-        for t in self.terms:
-            output.update(t.vars())
-        return output
+    @property
+    def jx_type(self):
+        if self.term.jx_type == ARRAY:
+            return self.term.jx_type
+        else:
+            return array_of(self.term.jx_type)
 
-    def map(self, map):
-        return self.__class__([t.map(map) for t in self.terms])
+    def vars(self):
+        return self.term.vars()
 
-    def __data__(self):
-        return {self.op: [t.__data__() for t in self.terms]}
+    def map(self, map_):
+        return ToArrayOp(self.term.map(map_))
 
     def missing(self, lang):
-        return FALSE
+        return self.term.missing(lang)
 
     def partial_eval(self, lang):
-        acc = None
-        terms = []
-        for t in self.terms:
-            simple = t.partial_eval(lang)
-            if simple is NULL:
-                pass
-            elif is_op(simple, Literal):
-                if acc is None:
-                    acc = simple.value
-                else:
-                    acc = builtin_ops[self.op](acc, simple.value)
-            else:
-                terms.append(simple)
-        if len(terms) == 0:
-            if acc == None:
-                return self.default.partial_eval(lang)
-            else:
-                return Literal(acc)
-        else:
-            if acc is not None:
-                terms.append(Literal(acc))
-
-            return self.__class__(*terms)
+        term = self.term.partial_eval(lang)
+        if any(is_op(term, t) for t in [ToArrayOp, SelectOp, GroupOp, FilterOp]):
+            return term
+        if term is NULL:
+            return Literal([])
+        if self.term.jx_type == ARRAY:
+            return term
+        return ToArrayOp(term)
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/strict_not_op.py` & `jx-python-4.583.24095/jx_base/expressions/to_value_op.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,49 +3,43 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
 from jx_base.expressions.expression import Expression
-from jx_base.language import is_op
-from mo_json.types import JX_BOOLEAN
+from mo_json import ARRAY
+from mo_json.types import array_of, ARRAY_KEY
 
 
-class StrictNotOp(Expression):
-    _jx_type = JX_BOOLEAN
+class ToValueOp(Expression):
+    """
+    Try to cast the result to a value (or None), not an array
+    """
 
     def __init__(self, term):
         Expression.__init__(self, term)
         self.term = term
 
     def __data__(self):
-        return {"strict.not": self.term.__data__()}
-
-    def __call__(self, row, rownum=None, rows=None):
-        return not self.term(row, rownum, rows)
+        return {"to_value": self.term.__data__()}
 
-    def __eq__(self, other):
-        if not is_op(other, StrictNotOp):
-            return False
-        return self.term == other.term
+    @property
+    def jx_type(self):
+        if self.term.jx_type == ARRAY:
+            return self.term.jx_type[ARRAY_KEY]
+        else:
+            return array_of(self.term.jx_type)
 
     def vars(self):
         return self.term.vars()
 
     def map(self, map_):
-        return NotOp(self.term.map(map_))
+        return ToValueOp(self.term.map(map_))
 
     def missing(self, lang):
-        return (self.term).missing(lang)
-
-    def invert(self, lang):
-        return self.term.partial_eval(lang)
+        return self.term.missing(lang)
 
     def partial_eval(self, lang):
-        if is_op(self.term, StrictNotOp):
-            return self.term
-        else:
-            return self
+        term = self.term.partial_eval(lang)
+        return ToValueOp(term)
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/strict_substring_op.py` & `jx-python-4.583.24095/jx_python/expressions/python_script.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,41 +4,51 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
+from jx_base.expressions import FALSE, TRUE, PythonScript as _PythonScript
+from jx_python.expressions import Python
 
-from jx_base.expressions.expression import Expression
-from jx_base.expressions.false_op import FALSE
-from mo_json.types import JX_TEXT
 
+class PythonScript(_PythonScript):
+    def __str__(self):
+        missing = self.miss.partial_eval(Python)
+        if missing is FALSE:
+            return self.partial_eval(Python).to_python(self.loop_depth).source
+        elif missing is TRUE:
+            return "None"
+
+        missing = missing.to_python(self.loop_depth)
+
+        return f"None if {missing.source}) else ({self.source})"
+
+    def __add__(self, other):
+        return str(self) + str(other)
+
+    def __radd__(self, other):
+        try:
+            a = str(other)
+            b = str(self)
+            return a + b
+        except Exception as cause:
+            b = str(self)
+            return ""
 
-class StrictSubstringOp(Expression):
-    """
-    PLACEHOLDER FOR BASIC value.substring(start, end) (CAN NOT DEAL WITH NULLS)
-    """
+    def to_python(self, loop_depth=0):
+        return self
 
-    _jx_type = JX_TEXT
-
-    def __init__(self, value, start, end):
-        Expression.__init__(self, value, start, end)
-        self.value, self.start, self.end = value, start, end
-
-    def __call__(self, row, rownum=None, rows=None):
-        return self.value(row, rownum, rows)[self.start(row, rownum, rows) : self.end(row, rownum, rows)]
+    def missing(self, lang):
+        return self.miss
 
     def __data__(self):
-        return {"strict.substring": [self.value.__data__(), self.start.__data__(), self.end.__data__()]}
-
-    def map(self, map_):
-        return StrictSubstringOp(self.value.map(map_), self.start.map(map_), self.end.map(map_),)
-
-    def vars(self):
-        return self.value.vars() | self.start.vars() | self.end.vars()
-
-    def missing(self, lang):
-        return FALSE
+        return {"script": self.script}
 
-    def invert(self, lang):
-        return FALSE
+    def __eq__(self, other):
+        if not isinstance(other, _PythonScript):
+            return False
+        elif self.expr == other.frum:
+            return True
+        else:
+            return False
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/sub_op.py` & `jx-python-4.583.24095/jx_base/expressions/sub_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/suffix_op.py` & `jx-python-4.583.24095/jx_base/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/sum_op.py` & `jx-python-4.583.24095/jx_base/expressions/sum_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/tally_op.py` & `jx-python-4.583.24095/jx_base/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/to_array_op.py` & `jx-python-4.583.24095/jx_base/expressions/true_op.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,54 +3,76 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from jx_base.expressions.expression import Expression
-from jx_base.expressions.filter_op import FilterOp
-from jx_base.expressions.group_op import GroupOp
-from jx_base.expressions.literal import NULL, Literal
-from jx_base.expressions.select_op import SelectOp
-from jx_base.language import is_op
-from mo_json import ARRAY
-from mo_json.types import array_of
-
-
-class ToArrayOp(Expression):
-    """
-    Ensure the result is an array, or Null
-    """
-
-    def __init__(self, term):
-        Expression.__init__(self, term)
-        self.term = term
 
-    def __data__(self):
-        return {"to_array": self.term.__data__()}
 
-    @property
-    def jx_type(self):
-        if self.term.jx_type == ARRAY:
-            return self.term.jx_type
-        else:
-            return array_of(self.term.jx_type)
+from jx_base.expressions.false_op import FALSE
+from jx_base.expressions.literal import Literal
+from mo_imports import export
+from mo_json.types import JX_BOOLEAN
+
+
+class TrueOp(Literal):
+    _jx_type = JX_BOOLEAN
+
+    def __new__(cls, *args, **kwargs):
+        return object.__new__(cls)
+
+    def __init__(self, op=None, term=None):
+        Literal.__init__(self, True)
+
+    @classmethod
+    def define(cls, expr):
+        return TRUE
+
+    def __nonzero__(self):
+        return True
+
+    def __eq__(self, other):
+        return (other is TRUE) or (other is True)
+
+    def __data__(self):
+        return True
 
     def vars(self):
-        return self.term.vars()
+        return set()
 
     def map(self, map_):
-        return ToArrayOp(self.term.map(map_))
+        return self
 
     def missing(self, lang):
-        return self.term.missing(lang)
+        return FALSE
+
+    def invert(self, lang):
+        return FALSE
+
+    @property
+    def jx_type(self):
+        return JX_BOOLEAN
+
+    def __call__(self, row=None, rownum=None, rows=None):
+        return True
+
+    def __str__(self):
+        return "true"
+
+    def __bool__(self):
+        return True
+
+    def __rcontains__(self, superset):
+        return self is superset
+
+    def __nonzero__(self):
+        return True
+
+
+TRUE = TrueOp()
+
 
-    def partial_eval(self, lang):
-        term = self.term.partial_eval(lang)
-        if any(is_op(term, t) for t in [ToArrayOp, SelectOp, GroupOp, FilterOp]):
-            return term
-        if term is NULL:
-            return Literal([])
-        if self.term.jx_type == ARRAY:
-            return term
-        return ToArrayOp(term)
+export("jx_base.expressions.literal", TRUE)
+export("jx_base.expressions.false_op", TRUE)
+export("jx_base.expressions._utils", TRUE)
+export("jx_base.expressions.expression", TRUE)
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/to_integer_op.py` & `jx-python-4.583.24095/jx_base/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/to_number_op.py` & `jx-python-4.583.24095/jx_base/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/to_text_op.py` & `jx-python-4.583.24095/jx_base/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/to_value_op.py` & `jx-python-4.583.24095/jx_python/expression_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,59 @@
-# encoding: utf-8
-#
-#
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this file,
-# You can obtain one at http:# mozilla.org/MPL/2.0/.
-#
-# Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
-#
-from jx_base.expressions.expression import Expression
-from mo_json import ARRAY
-from mo_json.types import array_of, ARRAY_KEY
+from jx_base import jx_expression
+from jx_base.expressions import Expression, Variable, GetOp, EqOp, Literal
+from jx_python.expression_compiler import compile_expression
+from jx_python.expressions import Python
+from jx_python.streams.typers import UnknownTyper, Typer, LazyTyper
+from mo_logs import logger
 
 
-class ToValueOp(Expression):
+class ExpressionFactory:
+    def __init__(self, expr, domain):
+        self.expr: Expression = expr
+        self.domain: Typer = domain or LazyTyper()
+
+    def build(self):
+        return compile_expression(self.expr.partial_eval(Python).to_python(), "some_function")
+
+    def __getattr__(self, item):
+        item_type = getattr(self.domain, item)
+
+        return ExpressionFactory(GetOp(self.expr, factory(item).expr), item_type)
+
+    def __eq__(self, other):
+        other = factory(other)
+        return ExpressionFactory(EqOp(self, other), Typer(python_type=bool))
+
+    def to_list(self):
+        self.build()(None)
+
+
+def factory(expr, typer=None) -> ExpressionFactory:
     """
-    Try to cast the result to a value (or None), not an array
+    assemble the expression
     """
+    if isinstance(expr, ExpressionFactory):
+        return ExpressionFactory(expr.expr, typer)
+
+    if not isinstance(expr, Expression):
+        expr = jx_expression(expr)
+
+    return ExpressionFactory(expr, typer)
+
+
+class TopExpressionFactory(ExpressionFactory):
+    """
+    it(x)  RETURNS A FunctionFactory FOR x
+    """
+
+    def __call__(self, value):
+        # much like an import of a value
+        if isinstance(value, ExpressionFactory):
+            logger.error("don't do this")
+
+        return ExpressionFactory(Literal("."), Typer(python_type=type(value)), f"{value}")
+
+    def __str__(self):
+        return "it"
+
 
-    def __init__(self, term):
-        Expression.__init__(self, term)
-        self.term = term
-
-    def __data__(self):
-        return {"to_value": self.term.__data__()}
-
-    @property
-    def jx_type(self):
-        if self.term.jx_type == ARRAY:
-            return self.term.jx_type[ARRAY_KEY]
-        else:
-            return array_of(self.term.jx_type)
-
-    def vars(self):
-        return self.term.vars()
-
-    def map(self, map_):
-        return ToValueOp(self.term.map(map_))
-
-    def missing(self, lang):
-        return self.term.missing(lang)
-
-    def partial_eval(self, lang):
-        term = self.term.partial_eval(lang)
-        return ToValueOp(term)
+it = TopExpressionFactory(Variable("."), UnknownTyper(Exception("unknonwn type")))
```

### Comparing `jx-python-4.582.24095/jx_base/expressions/tuple_op.py` & `jx-python-4.583.24095/jx_base/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/union_op.py` & `jx-python-4.583.24095/jx_base/expressions/union_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/unix_op.py` & `jx-python-4.583.24095/jx_base/expressions/unix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/variable.py` & `jx-python-4.583.24095/jx_base/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/expressions/when_op.py` & `jx-python-4.583.24095/jx_base/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/language.py` & `jx-python-4.583.24095/jx_base/language.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/meta_columns.py` & `jx-python-4.583.24095/jx_base/meta_columns.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/container.py` & `jx-python-4.583.24095/jx_base/models/container.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/dimensions.py` & `jx-python-4.583.24095/jx_base/models/dimensions.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/facts.py` & `jx-python-4.583.24095/jx_base/models/facts.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/namespace.py` & `jx-python-4.583.24095/jx_base/models/namespace.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/schema.py` & `jx-python-4.583.24095/jx_base/models/schema.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/snowflake.py` & `jx-python-4.583.24095/jx_base/models/snowflake.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/models/table.py` & `jx-python-4.583.24095/jx_base/models/table.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/queries.py` & `jx-python-4.583.24095/jx_base/queries.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_base/utils.py` & `jx-python-4.583.24095/jx_base/utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/__init__.py` & `jx-python-4.583.24095/jx_python/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/containers/cube.py` & `jx-python-4.583.24095/jx_python/containers/cube.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/containers/list.py` & `jx-python-4.583.24095/jx_python/containers/list.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/convert.py` & `jx-python-4.583.24095/jx_python/convert.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/cubes/aggs.py` & `jx-python-4.583.24095/jx_python/cubes/aggs.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expression_compiler.py` & `jx-python-4.583.24095/jx_python/expression_compiler.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/__init__.py` & `jx-python-4.583.24095/jx_python/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/_utils.py` & `jx-python-4.583.24095/jx_python/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/and_op.py` & `jx-python-4.583.24095/jx_python/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/array_of_op.py` & `jx-python-4.583.24095/jx_python/expressions/array_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/avg_op.py` & `jx-python-4.583.24095/jx_python/expressions/avg_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/basic_add_op.py` & `jx-python-4.583.24095/jx_python/expressions/strict_add_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import BasicAddOp as _BasicAddOp, FALSE
+from jx_base.expressions import StrictAddOp as _StrictAddOp, FALSE
 from jx_base.expressions.python_script import PythonScript
 from jx_python.expressions import Python
 from jx_python.utils import merge_locals
 from mo_json import JX_BOOLEAN
 
 
-class BasicAddOp(_BasicAddOp):
+class StrictAddOp(_StrictAddOp):
     def to_python(self, loop_depth=0):
         terms = [t.partial_eval(Python).to_python(loop_depth) for t in self.terms]
         return PythonScript(
             merge_locals(*(t.locals for t in terms)),
             loop_depth,
             JX_BOOLEAN,
             " + ".join(f"({t.source})" for t in terms),
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/basic_eq_op.py` & `jx-python-4.583.24095/jx_python/expressions/strict_starts_with_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import BasicEqOp as _BasicEqOp, FALSE
+from jx_base.expressions.strict_starts_with_op import StrictStartsWithOp as _StrictStartsWithOp
 from jx_base.expressions.python_script import PythonScript
 from jx_python.utils import merge_locals
 from mo_json import JX_BOOLEAN
 
 
-class BasicEqOp(_BasicEqOp):
+class StrictStartsWithOp(_StrictStartsWithOp):
     def to_python(self, loop_depth=0):
-        lhs = self.lhs.to_python(loop_depth)
-        rhs = self.rhs.to_python(loop_depth)
+        value = self.value.to_python(loop_depth)
+        prefix = self.prefix.to_python(loop_depth)
         return PythonScript(
-            merge_locals(lhs.locals, rhs.locals),
+            merge_locals(value.locals, prefix.locals),
             loop_depth,
             JX_BOOLEAN,
-            "(" + lhs.source + ") == (" + rhs.source + ")",
-            FALSE,
+            f"({value.source}).startswith({prefix.source})",
+            self,
         )
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/basic_index_of_op.py` & `jx-python-4.583.24095/jx_python/expressions/in_op.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import BasicIndexOfOp as _BasicIndexOfOp
-from jx_python.expressions._utils import with_var, PythonScript
+from jx_base.expressions import InOp as _InOp
+from jx_base.expressions.python_script import PythonScript
 from jx_python.utils import merge_locals
-from mo_json import JX_INTEGER
+from mo_json import JX_BOOLEAN
 
 
-class BasicIndexOfOp(_BasicIndexOfOp):
+class InOp(_InOp):
     def to_python(self, loop_depth=0):
-        find = self.find.to_python(loop_depth)
         value = self.value.to_python(loop_depth)
-
+        superset = self.superset.to_python(loop_depth)
         return PythonScript(
-            merge_locals(value.locals, find.locals),
+            merge_locals(value.locals, superset.locals),
             loop_depth,
-            JX_INTEGER,
-            f"({value.source}).find({find.source})",
+            JX_BOOLEAN,
+            f"{value.source} in {superset.source}",
             self,
         )
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/basic_starts_with_op.py` & `jx-python-4.583.24095/jx_python/expressions/strict_eq_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.basic_starts_with_op import BasicStartsWithOp as _BasicStartsWithOp
+from jx_base.expressions import StrictEqOp as _StrictEqOp, FALSE
 from jx_base.expressions.python_script import PythonScript
 from jx_python.utils import merge_locals
 from mo_json import JX_BOOLEAN
 
 
-class BasicStartsWithOp(_BasicStartsWithOp):
+class StrictEqOp(_StrictEqOp):
     def to_python(self, loop_depth=0):
-        value = self.value.to_python(loop_depth)
-        prefix = self.prefix.to_python(loop_depth)
+        lhs = self.lhs.to_python(loop_depth)
+        rhs = self.rhs.to_python(loop_depth)
         return PythonScript(
-            merge_locals(value.locals, prefix.locals),
+            merge_locals(lhs.locals, rhs.locals),
             loop_depth,
             JX_BOOLEAN,
-            f"({value.source}).startswith({prefix.source})",
-            self,
+            "(" + lhs.source + ") == (" + rhs.source + ")",
+            FALSE,
         )
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/basic_substring_op.py` & `jx-python-4.583.24095/jx_python/expressions/strict_substring_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.basic_substring_op import BasicSubstringOp as _BasicSubstringOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp as _StrictSubstringOp
 from jx_base.expressions.python_script import PythonScript
 from jx_python.utils import merge_locals
 from mo_json import JX_TEXT
 
 
-class BasicSubstringOp(_BasicSubstringOp):
+class StrictSubstringOp(_StrictSubstringOp):
     def to_python(self, loop_depth=0):
         value = self.value.to_python(loop_depth)
         start = self.start.to_python(loop_depth)
         end = self.end.to_python(loop_depth)
         return PythonScript(
             merge_locals(value.locals, start.locals, end.locals),
             loop_depth,
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/call_op.py` & `jx-python-4.583.24095/jx_python/expressions/call_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/cardinality_op.py` & `jx-python-4.583.24095/jx_python/expressions/cardinality_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/case_op.py` & `jx-python-4.583.24095/jx_python/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/coalesce_op.py` & `jx-python-4.583.24095/jx_python/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/concat_op.py` & `jx-python-4.583.24095/jx_python/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/count_op.py` & `jx-python-4.583.24095/jx_python/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/date_op.py` & `jx-python-4.583.24095/jx_python/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/eq_op.py` & `jx-python-4.583.24095/jx_python/expressions/group_op.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,43 +3,49 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from jx_base.expressions import EqOp as _EqOp, is_literal, FALSE, TRUE, ToArrayOp
+import itertools
+
+from mo_dots import is_data
+from mo_json.typed_object import TypedObject
+
+from jx_base.expressions import GroupOp as _GroupOp, ToArrayOp
 from jx_base.expressions.python_script import PythonScript
 from jx_base.language import value_compare
+from jx_base.utils import enlist
 from jx_python.expressions import Python
-from jx_python.expressions.strict_eq_op import StrictEqOp
-from jx_python.expressions.case_op import CaseOp
-from jx_python.expressions.when_op import WhenOp
 from jx_python.utils import merge_locals
-from mo_json import JX_BOOLEAN
+from mo_future import sort_using_cmp
+from mo_json.typed_encoder import detype
+from mo_json.types import JxType, array_of, ARRAY_KEY
 
+ARRAY_KEY = ARRAY_KEY
 
-class EqOp(_EqOp):
+
+class GroupOp(_GroupOp):
     def to_python(self, loop_depth=0):
-        lhs = ToArrayOp(self.lhs).partial_eval(Python).to_python(loop_depth)
-        rhs = self.rhs.to_python(loop_depth)
+        frum = ToArrayOp(self.frum).partial_eval(Python).to_python(loop_depth)
+        group = self.group.partial_eval(Python).to_python(loop_depth)
+
         return PythonScript(
-            merge_locals(rhs.locals, lhs.locals),
+            merge_locals(frum.locals, group.locals, groupby=groupby, enlist=enlist),
             loop_depth,
-            JX_BOOLEAN,
-            f"({rhs.source}) in ({lhs.source})",
+            array_of(frum.jx_type) | JxType(group=group.jx_type),
+            f"""groupby({frum.source}, lambda row{loop_depth}: {group.source})""",
             self,
-            FALSE,
         )
 
-    def partial_eval(self, lang):
-        lhs = self.lhs.partial_eval(lang)
-        rhs = self.rhs.partial_eval(lang)
 
-        if is_literal(lhs) and is_literal(rhs):
-            return FALSE if value_compare(lhs.value, rhs.value) else TRUE
+def groupby(values, func):
+    output = []
+    cmp = lambda a, b: value_compare(detype(func(a)), detype(func(b)))
+    for g, rows in itertools.groupby(sort_using_cmp(values, cmp=cmp), func):
+        row = list(rows)
+        if is_data(g):
+            output.append(TypedObject(row, **g))
         else:
-            return CaseOp(
-                WhenOp(lhs.missing(lang), then=rhs.missing(lang)),
-                WhenOp(rhs.missing(lang), then=FALSE),
-                StrictEqOp(lhs, rhs),
-            ).partial_eval(lang)
+            output.append(TypedObject(row, group=g))
+    return output
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/exists_op.py` & `jx-python-4.583.24095/jx_python/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/false_op.py` & `jx-python-4.583.24095/jx_python/expressions/false_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/filter_op.py` & `jx-python-4.583.24095/jx_python/expressions/filter_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/find_op.py` & `jx-python-4.583.24095/jx_python/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/first_op.py` & `jx-python-4.583.24095/jx_python/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/floor_op.py` & `jx-python-4.583.24095/jx_python/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/get_op.py` & `jx-python-4.583.24095/jx_python/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/in_op.py` & `jx-python-4.583.24095/jx_python/expressions/prefix_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,18 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import InOp as _InOp
+from jx_base.expressions import PrefixOp as _PrefixOp
 from jx_base.expressions.python_script import PythonScript
-from jx_python.utils import merge_locals
-from mo_json import JX_BOOLEAN
 
 
-class InOp(_InOp):
+class PrefixOp(_PrefixOp):
     def to_python(self, loop_depth=0):
-        value = self.value.to_python(loop_depth)
-        superset = self.superset.to_python(loop_depth)
         return PythonScript(
-            merge_locals(value.locals, superset.locals),
+            {},
             loop_depth,
-            JX_BOOLEAN,
-            f"{value.source} in {superset.source}",
-            self,
+            ("(" + self.expr.to_python(loop_depth) + ").startswith(" + (self.prefix).to_python(loop_depth) + ")"),
         )
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/is_text_op.py` & `jx-python-4.583.24095/jx_python/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/last_op.py` & `jx-python-4.583.24095/jx_python/expressions/last_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/least_op.py` & `jx-python-4.583.24095/jx_python/expressions/least_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/leaves_op.py` & `jx-python-4.583.24095/jx_python/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/length_op.py` & `jx-python-4.583.24095/jx_python/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/limit_op.py` & `jx-python-4.583.24095/jx_python/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/literal.py` & `jx-python-4.583.24095/jx_python/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/max_op.py` & `jx-python-4.583.24095/jx_python/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/min_op.py` & `jx-python-4.583.24095/jx_python/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/missing_op.py` & `jx-python-4.583.24095/jx_python/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/most_op.py` & `jx-python-4.583.24095/jx_python/expressions/most_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/mul_op.py` & `jx-python-4.583.24095/jx_python/expressions/mul_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/name_op.py` & `jx-python-4.583.24095/jx_python/expressions/name_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/ne_op.py` & `jx-python-4.583.24095/jx_python/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/not_left_op.py` & `jx-python-4.583.24095/jx_python/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/not_op.py` & `jx-python-4.583.24095/jx_python/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/not_right_op.py` & `jx-python-4.583.24095/jx_python/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/offset_op.py` & `jx-python-4.583.24095/jx_python/expressions/offset_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/or_op.py` & `jx-python-4.583.24095/jx_python/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/prefix_op.py` & `jx-python-4.583.24095/jx_python/expressions/to_integer_op.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import PrefixOp as _PrefixOp
+from jx_base.expressions import ToIntegerOp as _IntegerOp
 from jx_base.expressions.python_script import PythonScript
+from mo_json import JX_INTEGER
 
 
-class PrefixOp(_PrefixOp):
+class ToIntegerOp(_IntegerOp):
     def to_python(self, loop_depth=0):
-        return PythonScript(
-            {},
-            loop_depth,
-            ("(" + self.expr.to_python(loop_depth) + ").startswith(" + (self.prefix).to_python(loop_depth) + ")"),
-        )
+        return PythonScript({}, loop_depth, JX_INTEGER, "int(" + self.term.to_python(loop_depth) + ")", self)
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/product_op.py` & `jx-python-4.583.24095/jx_python/expressions/product_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/python_function.py` & `jx-python-4.583.24095/jx_python/expressions/python_function.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/reg_exp_op.py` & `jx-python-4.583.24095/jx_python/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/right_op.py` & `jx-python-4.583.24095/jx_python/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/rows_op.py` & `jx-python-4.583.24095/jx_python/expressions/rows_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/script_op.py` & `jx-python-4.583.24095/jx_python/expressions/script_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/select_op.py` & `jx-python-4.583.24095/jx_python/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/split_op.py` & `jx-python-4.583.24095/jx_python/expressions/split_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/strict_add_op.py` & `jx-python-4.583.24095/jx_python/expressions/to_array_op.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
-from jx_base.expressions import StrictAddOp as _StrictAddOp, FALSE
-from jx_base.expressions.python_script import PythonScript
+from jx_base.expressions import ToArrayOp as _ToArrayOp, PythonScript
+from jx_base.utils import enlist
 from jx_python.expressions import Python
 from jx_python.utils import merge_locals
-from mo_json import JX_BOOLEAN
+from mo_json import array_of
 
 
-class StrictAddOp(_StrictAddOp):
+class ToArrayOp(_ToArrayOp):
     def to_python(self, loop_depth=0):
-        terms = [t.partial_eval(Python).to_python(loop_depth) for t in self.terms]
+        term = self.term.partial_eval(Python).to_python(loop_depth)
         return PythonScript(
-            merge_locals(*(t.locals for t in terms)),
+            merge_locals(term.locals, enlist=enlist),
             loop_depth,
-            JX_BOOLEAN,
-            " + ".join(f"({t.source})" for t in terms),
-            FALSE,
+            array_of(term.jx_type),
+            f"enlist({term.source})",
+            self,
         )
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/strict_eq_op.py` & `jx-python-4.583.24095/jx_python/expressions/when_op.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
+from mo_imports import export
 
-
-from jx_base.expressions import StrictEqOp as _StrictEqOp, FALSE
+from jx_base.expressions import WhenOp as _WhenOp
 from jx_base.expressions.python_script import PythonScript
 from jx_python.utils import merge_locals
-from mo_json import JX_BOOLEAN
 
 
-class StrictEqOp(_StrictEqOp):
+class WhenOp(_WhenOp):
     def to_python(self, loop_depth=0):
-        lhs = self.lhs.to_python(loop_depth)
-        rhs = self.rhs.to_python(loop_depth)
+        when = self.when.to_python(loop_depth)
+        then = self.then.to_python(loop_depth)
+        els_ = self.els_.to_python(loop_depth)
         return PythonScript(
-            merge_locals(lhs.locals, rhs.locals),
+            merge_locals(when.locals, then.locals, els_.locals),
             loop_depth,
-            JX_BOOLEAN,
-            "(" + lhs.source + ") == (" + rhs.source + ")",
-            FALSE,
+            then.jx_type | els_.jx_type,
+            f"({then.source}) if ({when.source}) else ({els_.source})",
+            self,
         )
+
+
+export("jx_python.expressions._utils", WhenOp)
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/strict_index_of_op.py` & `jx-python-4.583.24095/jx_python/expressions/strict_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/strict_starts_with_op.py` & `jx-python-4.583.24095/jx_python/expressions/suffix_op.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.strict_starts_with_op import StrictStartsWithOp as _StrictStartsWithOp
+from jx_base.expressions import SuffixOp as _SuffixOp
 from jx_base.expressions.python_script import PythonScript
-from jx_python.utils import merge_locals
 from mo_json import JX_BOOLEAN
 
 
-class StrictStartsWithOp(_StrictStartsWithOp):
+class SuffixOp(_SuffixOp):
     def to_python(self, loop_depth=0):
-        value = self.value.to_python(loop_depth)
-        prefix = self.prefix.to_python(loop_depth)
         return PythonScript(
-            merge_locals(value.locals, prefix.locals),
-            loop_depth,
-            JX_BOOLEAN,
-            f"({value.source}).startswith({prefix.source})",
-            self,
+            locals={},
+            loop_depth=loop_depth,
+            type=JX_BOOLEAN,
+            source=f"({self.expr.to_python(loop_depth)}).endswith({self.suffix.to_python(loop_depth)})",
+            frum=self,
         )
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/suffix_op.py` & `jx-python-4.583.24095/jx_python/expressions/tally_op.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,21 +5,35 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import SuffixOp as _SuffixOp
+from jx_base.expressions import TallyOp as _TallyOp
 from jx_base.expressions.python_script import PythonScript
-from mo_json import JX_BOOLEAN
+from jx_python.expressions import Python
+from jx_python.utils import merge_locals
+from mo_dots import is_missing
+from mo_json import JX_INTEGER
 
 
-class SuffixOp(_SuffixOp):
+class TallyOp(_TallyOp):
     def to_python(self, loop_depth=0):
+        terms = [t.partial_eval(Python).to_python(loop_depth) for t in self.terms]
+
         return PythonScript(
-            locals={},
-            loop_depth=loop_depth,
-            type=JX_BOOLEAN,
-            source=f"({self.expr.to_python(loop_depth)}).endswith({self.suffix.to_python(loop_depth)})",
-            frum=self,
+            merge_locals(*(t.locals for t in terms), tally=tally),
+            loop_depth,
+            JX_INTEGER,
+            f"tally({','.join(t.source for t in terms)})",
+            self,
         )
+
+
+def tally(*terms):
+    output = 0
+    for t in terms:
+        if is_missing(t):
+            return None
+        output += 1
+    return output
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/sum_op.py` & `jx-python-4.583.24095/jx_python/expressions/sum_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/to_array_op.py` & `jx-python-4.583.24095/jx_python/expressions/to_number_op.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,38 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from jx_base.expressions import ToArrayOp as _ToArrayOp, PythonScript
-from jx_base.utils import enlist
-from jx_python.expressions import Python
+from mo_imports import export
+
+from jx_base.expressions.python_script import PythonScript
+from jx_base.expressions.to_number_op import ToNumberOp as _NumberOp
 from jx_python.utils import merge_locals
-from mo_json import array_of
+from mo_json.types import JX_NUMBER
 
 
-class ToArrayOp(_ToArrayOp):
+class ToNumberOp(_NumberOp):
     def to_python(self, loop_depth=0):
-        term = self.term.partial_eval(Python).to_python(loop_depth)
+        exists = self.term.exists()
+        value = self.term.to_python(loop_depth)
+
         return PythonScript(
-            merge_locals(term.locals, enlist=enlist),
+            merge_locals(value.locals, to_float=to_float),
             loop_depth,
-            array_of(term.jx_type),
-            f"enlist({term.source})",
+            JX_NUMBER,
+            f"to_float({value.source})",
             self,
+            exists,
         )
+
+
+def to_float(value):
+    try:
+        return float(value)
+    except:
+        return None
+
+
+export("jx_python.expressions._utils", ToNumberOp)
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/to_boolean_op.py` & `jx-python-4.583.24095/jx_python/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/to_number_op.py` & `jx-python-4.583.24095/jx_python/expressions/to_text_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,21 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from mo_imports import export
-
 from jx_base.expressions.python_script import PythonScript
-from jx_base.expressions.to_number_op import ToNumberOp as _NumberOp
-from jx_python.utils import merge_locals
-from mo_json.types import JX_NUMBER
+
+from jx_base.expressions import ToTextOp as _ToTextOp
+from jx_python.expressions._utils import Python
+from mo_json import JX_TEXT
 
 
-class ToNumberOp(_NumberOp):
+class ToTextOp(_ToTextOp):
     def to_python(self, loop_depth=0):
-        exists = self.term.exists()
+        missing = self.term.missing(Python).to_python(loop_depth)
         value = self.term.to_python(loop_depth)
-
         return PythonScript(
-            merge_locals(value.locals, to_float=to_float),
-            loop_depth,
-            JX_NUMBER,
-            f"to_float({value.source})",
-            self,
-            exists,
+            locals=value.locals, loop_depth=loop_depth, type=JX_TEXT, source=value.source, frum=self, miss=missing
         )
-
-
-def to_float(value):
-    try:
-        return float(value)
-    except:
-        return None
-
-
-export("jx_python.expressions._utils", ToNumberOp)
```

### Comparing `jx-python-4.582.24095/jx_python/expressions/to_value_op.py` & `jx-python-4.583.24095/jx_python/expressions/to_value_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/true_op.py` & `jx-python-4.583.24095/jx_python/expressions/true_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/tuple_op.py` & `jx-python-4.583.24095/jx_python/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/expressions/variable.py` & `jx-python-4.583.24095/jx_python/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/flat_list.py` & `jx-python-4.583.24095/jx_python/flat_list.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/group_by.py` & `jx-python-4.583.24095/jx_python/group_by.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/jx.py` & `jx-python-4.583.24095/jx_python/jx.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/lists/aggs.py` & `jx-python-4.583.24095/jx_python/lists/aggs.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/namespace/normal.py` & `jx-python-4.583.24095/jx_python/namespace/normal.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/records.py` & `jx-python-4.583.24095/jx_python/records.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams/__init__.py` & `jx-python-4.583.24095/jx_python/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams/expression_compiler.py` & `jx-python-4.583.24095/jx_python/streams/expression_compiler.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams/expression_factory.py` & `jx-python-4.583.24095/jx_python/streams/expression_factory.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams/inspects.py` & `jx-python-4.583.24095/jx_python/streams/inspects.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams/type_parser.py` & `jx-python-4.583.24095/jx_python/streams/type_parser.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams/typers.py` & `jx-python-4.583.24095/jx_python/streams/typers.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/streams.py` & `jx-python-4.583.24095/jx_python/streams.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/table.py` & `jx-python-4.583.24095/jx_python/table.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/utils.py` & `jx-python-4.583.24095/jx_python/utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python/windows.py` & `jx-python-4.583.24095/jx_python/windows.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.582.24095/jx_python.egg-info/PKG-INFO` & `jx-python-4.583.24095/jx_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-python
-Version: 4.582.24095
+Version: 4.583.24095
 Summary: JSON query expressions using Python
 Home-page: https://github.com/klahnakoski/jx-python
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `jx-python-4.582.24095/jx_python.egg-info/SOURCES.txt` & `jx-python-4.583.24095/jx_python.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,14 @@
 jx_base/expressions/and_op.py
 jx_base/expressions/any_op.py
 jx_base/expressions/array_of_op.py
 jx_base/expressions/avg_op.py
 jx_base/expressions/base_binary_op.py
 jx_base/expressions/base_inequality_op.py
 jx_base/expressions/base_multi_op.py
-jx_base/expressions/basic_add_op.py
-jx_base/expressions/basic_boolean_op.py
-jx_base/expressions/basic_eq_op.py
-jx_base/expressions/basic_in_op.py
-jx_base/expressions/basic_index_of_op.py
-jx_base/expressions/basic_mul_op.py
-jx_base/expressions/basic_multi_op.py
-jx_base/expressions/basic_not_op.py
-jx_base/expressions/basic_starts_with_op.py
-jx_base/expressions/basic_substring_op.py
 jx_base/expressions/between_op.py
 jx_base/expressions/call_op.py
 jx_base/expressions/cardinality_op.py
 jx_base/expressions/case_op.py
 jx_base/expressions/coalesce_op.py
 jx_base/expressions/comment_op.py
 jx_base/expressions/concat_op.py
@@ -191,19 +181,14 @@
 jx_python/cubes/aggs.py
 jx_python/expressions/__init__.py
 jx_python/expressions/_utils.py
 jx_python/expressions/add_op.py
 jx_python/expressions/and_op.py
 jx_python/expressions/array_of_op.py
 jx_python/expressions/avg_op.py
-jx_python/expressions/basic_add_op.py
-jx_python/expressions/basic_eq_op.py
-jx_python/expressions/basic_index_of_op.py
-jx_python/expressions/basic_starts_with_op.py
-jx_python/expressions/basic_substring_op.py
 jx_python/expressions/between_op.py
 jx_python/expressions/call_op.py
 jx_python/expressions/cardinality_op.py
 jx_python/expressions/case_op.py
 jx_python/expressions/coalesce_op.py
 jx_python/expressions/concat_op.py
 jx_python/expressions/count_op.py
```

### Comparing `jx-python-4.582.24095/setup.py` & `jx-python-4.583.24095/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     install_requires=["mo-collections==5.582.24095","mo-dots==9.582.24095","mo-future==7.546.24057","mo-json==6.582.24095","mo-json-config==4.582.24095","mo-kwargs==7.582.24095","mo-logs==8.582.24095","mo-math==7.582.24095","mo-threads==6.582.24095","mo-times==5.582.24095"],
     license='MPL 2.0',
     long_description='# jx-python\n\nPython library for JSON Expressions \n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-python.svg)](https://pypi.org/project/jx-python/)\n[![Build Status](https://github.com/klahnakoski/jx-python/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/jx-python/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/jx-python/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/jx-python?branch=dev)\n',
     long_description_content_type='text/markdown',
     name='jx-python',
     packages=["jx_base","jx_base.expressions","jx_base.models","jx_python.expressions","jx_python.containers","jx_python.cubes","jx_python.lists","jx_python.namespace","jx_python","jx_python.streams"],
     url='https://github.com/klahnakoski/jx-python',
-    version='4.582.24095'
+    version='4.583.24095'
 )
```

