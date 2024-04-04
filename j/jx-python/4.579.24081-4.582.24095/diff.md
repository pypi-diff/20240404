# Comparing `tmp/jx-python-4.579.24081.tar.gz` & `tmp/jx-python-4.582.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx-python-4.579.24081.tar", last modified: Thu Mar 21 02:48:05 2024, max compression
+gzip compressed data, was "jx-python-4.582.24095.tar", last modified: Thu Apr  4 04:16:15 2024, max compression
```

## Comparing `jx-python-4.579.24081.tar` & `jx-python-4.582.24095.tar`

### file list

```diff
@@ -1,287 +1,302 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.823448 jx-python-4.579.24081/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 jx-python-4.579.24081/LICENSE
--rw-rw-rw-   0        0        0     1743 2024-03-21 02:48:05.816895 jx-python-4.579.24081/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-03-08 02:37:16.000000 jx-python-4.579.24081/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.481779 jx-python-4.579.24081/jx_base/
--rw-rw-rw-   0        0        0     1471 2024-03-02 22:12:26.000000 jx-python-4.579.24081/jx_base/__init__.py
--rw-rw-rw-   0        0        0     8710 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/data_class.py
--rw-rw-rw-   0        0        0    25274 2024-02-06 05:15:22.000000 jx-python-4.579.24081/jx_base/domains.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.670904 jx-python-4.579.24081/jx_base/expressions/
--rw-rw-rw-   0        0        0    10592 2024-03-10 19:33:03.000000 jx-python-4.579.24081/jx_base/expressions/__init__.py
--rw-rw-rw-   0        0        0     4925 2024-03-20 02:23:03.000000 jx-python-4.579.24081/jx_base/expressions/_utils.py
--rw-rw-rw-   0        0        0     1027 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/abs_op.py
--rw-rw-rw-   0        0        0      800 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/add_op.py
--rw-rw-rw-   0        0        0     2379 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/aggregate_op.py
--rw-rw-rw-   0        0        0     1277 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/all_op.py
--rw-rw-rw-   0        0        0     3312 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/and_op.py
--rw-rw-rw-   0        0        0     1394 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/any_op.py
--rw-rw-rw-   0        0        0      918 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/array_of_op.py
--rw-rw-rw-   0        0        0      453 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/avg_op.py
--rw-rw-rw-   0        0        0     2183 2024-01-22 13:00:58.000000 jx-python-4.579.24081/jx_base/expressions/base_binary_op.py
--rw-rw-rw-   0        0        0      520 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/base_inequality_op.py
--rw-rw-rw-   0        0        0     2960 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/base_multi_op.py
--rw-rw-rw-   0        0        0      391 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/basic_add_op.py
--rw-rw-rw-   0        0        0     1546 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/basic_boolean_op.py
--rw-rw-rw-   0        0        0     1109 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/basic_eq_op.py
--rw-rw-rw-   0        0        0     3370 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/basic_in_op.py
--rw-rw-rw-   0        0        0     1972 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/basic_index_of_op.py
--rw-rw-rw-   0        0        0      391 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/basic_mul_op.py
--rw-rw-rw-   0        0        0     1966 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/basic_multi_op.py
--rw-rw-rw-   0        0        0     1277 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/basic_not_op.py
--rw-rw-rw-   0        0        0     1666 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/basic_starts_with_op.py
--rw-rw-rw-   0        0        0     1332 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/basic_substring_op.py
--rw-rw-rw-   0        0        0     4493 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/between_op.py
--rw-rw-rw-   0        0        0     1544 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/call_op.py
--rw-rw-rw-   0        0        0      661 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/cardinality_op.py
--rw-rw-rw-   0        0        0     4044 2024-03-21 02:47:56.000000 jx-python-4.579.24081/jx_base/expressions/case_op.py
--rw-rw-rw-   0        0        0     2037 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     1593 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/comment_op.py
--rw-rw-rw-   0        0        0     2890 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/concat_op.py
--rw-rw-rw-   0        0        0     1592 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/count_op.py
--rw-rw-rw-   0        0        0     1250 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/date_op.py
--rw-rw-rw-   0        0        0     2111 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/default_op.py
--rw-rw-rw-   0        0        0     1179 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/div_op.py
--rw-rw-rw-   0        0        0     2754 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/eq_op.py
--rw-rw-rw-   0        0        0      418 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/es_script.py
--rw-rw-rw-   0        0        0     1525 2024-01-28 16:03:01.000000 jx-python-4.579.24081/jx_base/expressions/es_select_op.py
--rw-rw-rw-   0        0        0     1270 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/exists_op.py
--rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/exp_op.py
--rw-rw-rw-   0        0        0     6265 2024-01-22 13:00:58.000000 jx-python-4.579.24081/jx_base/expressions/expression.py
--rw-rw-rw-   0        0        0     1524 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/false_op.py
--rw-rw-rw-   0        0        0     1278 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/filter_op.py
--rw-rw-rw-   0        0        0     2242 2024-01-28 16:03:01.000000 jx-python-4.579.24081/jx_base/expressions/find_op.py
--rw-rw-rw-   0        0        0     2413 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/first_op.py
--rw-rw-rw-   0        0        0      657 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/floor_op.py
--rw-rw-rw-   0        0        0    10147 2024-02-06 05:15:22.000000 jx-python-4.579.24081/jx_base/expressions/format_op.py
--rw-rw-rw-   0        0        0     1577 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/from_op.py
--rw-rw-rw-   0        0        0      807 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/from_unix_op.py
--rw-rw-rw-   0        0        0     3022 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/get_op.py
--rw-rw-rw-   0        0        0     1082 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/group_op.py
--rw-rw-rw-   0        0        0      385 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/gt_op.py
--rw-rw-rw-   0        0        0      386 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/gte_op.py
--rw-rw-rw-   0        0        0     3633 2024-02-15 03:10:30.000000 jx-python-4.579.24081/jx_base/expressions/in_op.py
--rw-rw-rw-   0        0        0     2505 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/inner_join_op.py
--rw-rw-rw-   0        0        0     1322 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/is_boolean_op.py
--rw-rw-rw-   0        0        0      969 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/is_integer_op.py
--rw-rw-rw-   0        0        0     1360 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/is_number_op.py
--rw-rw-rw-   0        0        0     1451 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/is_text_op.py
--rw-rw-rw-   0        0        0     1561 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/last_op.py
--rw-rw-rw-   0        0        0     1761 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/least_op.py
--rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/leaves_op.py
--rw-rw-rw-   0        0        0     2034 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/left_op.py
--rw-rw-rw-   0        0        0     1601 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/length_op.py
--rw-rw-rw-   0        0        0     2593 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/limit_op.py
--rw-rw-rw-   0        0        0     3326 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/literal.py
--rw-rw-rw-   0        0        0      384 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/lt_op.py
--rw-rw-rw-   0        0        0      385 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/lte_op.py
--rw-rw-rw-   0        0        0      507 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/map_op.py
--rw-rw-rw-   0        0        0     1418 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/max_op.py
--rw-rw-rw-   0        0        0     1442 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/min_op.py
--rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/missing_op.py
--rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/mod_op.py
--rw-rw-rw-   0        0        0      845 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/most_op.py
--rw-rw-rw-   0        0        0      882 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/mul_op.py
--rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/name_op.py
--rw-rw-rw-   0        0        0     1643 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/ne_op.py
--rw-rw-rw-   0        0        0     4365 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/nested_op.py
--rw-rw-rw-   0        0        0     2058 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/not_left_op.py
--rw-rw-rw-   0        0        0     1611 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/not_op.py
--rw-rw-rw-   0        0        0     2147 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/not_right_op.py
--rw-rw-rw-   0        0        0     2441 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/null_op.py
--rw-rw-rw-   0        0        0     1059 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/offset_op.py
--rw-rw-rw-   0        0        0     2239 2024-03-02 22:12:26.000000 jx-python-4.579.24081/jx_base/expressions/or_op.py
--rw-rw-rw-   0        0        0     2503 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/outer_join_op.py
--rw-rw-rw-   0        0        0     1387 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/percentile_op.py
--rw-rw-rw-   0        0        0     3282 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/prefix_op.py
--rw-rw-rw-   0        0        0     1585 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/product_op.py
--rw-rw-rw-   0        0        0      460 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/python_function.py
--rw-rw-rw-   0        0        0     1512 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/python_script.py
--rw-rw-rw-   0        0        0    24591 2024-03-21 02:47:56.000000 jx-python-4.579.24081/jx_base/expressions/query_op.py
--rw-rw-rw-   0        0        0     1025 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/range_op.py
--rw-rw-rw-   0        0        0     1575 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0     2244 2024-03-16 21:10:18.000000 jx-python-4.579.24081/jx_base/expressions/right_op.py
--rw-rw-rw-   0        0        0     1478 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/rows_op.py
--rw-rw-rw-   0        0        0     1247 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/script_op.py
--rw-rw-rw-   0        0        0    12251 2024-02-15 03:10:30.000000 jx-python-4.579.24081/jx_base/expressions/select_op.py
--rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/split_op.py
--rw-rw-rw-   0        0        0     1295 2024-02-15 03:10:30.000000 jx-python-4.579.24081/jx_base/expressions/sql_alias_op.py
--rw-rw-rw-   0        0        0     1027 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_and_op.py
--rw-rw-rw-   0        0        0     1010 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/sql_cast_op.py
--rw-rw-rw-   0        0        0     1361 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_concat_op.py
--rw-rw-rw-   0        0        0     1490 2024-03-10 19:33:03.000000 jx-python-4.579.24081/jx_base/expressions/sql_eq_op.py
--rw-rw-rw-   0        0        0     1082 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.579.24081/jx_base/expressions/sql_gt_op.py
--rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.579.24081/jx_base/expressions/sql_gte_op.py
--rw-rw-rw-   0        0        0      343 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_in_op.py
--rw-rw-rw-   0        0        0      428 2024-01-22 13:00:58.000000 jx-python-4.579.24081/jx_base/expressions/sql_inner_join_op.py
--rw-rw-rw-   0        0        0     1192 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/expressions/sql_instr_op.py
--rw-rw-rw-   0        0        0      832 2024-03-10 19:33:03.000000 jx-python-4.579.24081/jx_base/expressions/sql_is_null_op.py
--rw-rw-rw-   0        0        0     3313 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/sql_left_joins_op.py
--rw-rw-rw-   0        0        0      499 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_limit_op.py
--rw-rw-rw-   0        0        0      360 2024-02-15 03:10:30.000000 jx-python-4.579.24081/jx_base/expressions/sql_literal.py
--rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.579.24081/jx_base/expressions/sql_lt_op.py
--rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.579.24081/jx_base/expressions/sql_lte_op.py
--rw-rw-rw-   0        0        0     1448 2024-03-21 02:47:56.000000 jx-python-4.579.24081/jx_base/expressions/sql_not_op.py
--rw-rw-rw-   0        0        0     2371 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_or_op.py
--rw-rw-rw-   0        0        0      781 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_order_by_op.py
--rw-rw-rw-   0        0        0     1057 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/sql_origins_op.py
--rw-rw-rw-   0        0        0      427 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/expressions/sql_script.py
--rw-rw-rw-   0        0        0      958 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/sql_select_all_from_op.py
--rw-rw-rw-   0        0        0     2012 2024-02-15 03:10:30.000000 jx-python-4.579.24081/jx_base/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0      911 2024-03-10 19:33:03.000000 jx-python-4.579.24081/jx_base/expressions/sql_substr_op.py
--rw-rw-rw-   0        0        0     1583 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sql_variable.py
--rw-rw-rw-   0        0        0      611 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/sub_op.py
--rw-rw-rw-   0        0        0     3011 2024-03-02 22:12:26.000000 jx-python-4.579.24081/jx_base/expressions/suffix_op.py
--rw-rw-rw-   0        0        0     1556 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/sum_op.py
--rw-rw-rw-   0        0        0      721 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/tally_op.py
--rw-rw-rw-   0        0        0     1594 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/to_array_op.py
--rw-rw-rw-   0        0        0     1304 2024-03-02 22:12:26.000000 jx-python-4.579.24081/jx_base/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0     2708 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     2874 2024-03-02 22:12:26.000000 jx-python-4.579.24081/jx_base/expressions/to_number_op.py
--rw-rw-rw-   0        0        0     2043 2024-03-10 19:33:03.000000 jx-python-4.579.24081/jx_base/expressions/to_text_op.py
--rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/to_value_op.py
--rw-rw-rw-   0        0        0     1626 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/true_op.py
--rw-rw-rw-   0        0        0     1678 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/tuple_op.py
--rw-rw-rw-   0        0        0     2000 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/union_op.py
--rw-rw-rw-   0        0        0      826 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/expressions/unix_op.py
--rw-rw-rw-   0        0        0     6146 2024-01-24 02:03:18.000000 jx-python-4.579.24081/jx_base/expressions/variable.py
--rw-rw-rw-   0        0        0     3270 2024-03-21 02:47:56.000000 jx-python-4.579.24081/jx_base/expressions/when_op.py
--rw-rw-rw-   0        0        0    14462 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_base/language.py
--rw-rw-rw-   0        0        0    13555 2024-03-21 02:47:56.000000 jx-python-4.579.24081/jx_base/meta_columns.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.673699 jx-python-4.579.24081/jx_base/models/
--rw-rw-rw-   0        0        0        0 2022-11-12 15:14:28.000000 jx-python-4.579.24081/jx_base/models/__init__.py
--rw-rw-rw-   0        0        0     2369 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/models/container.py
--rw-rw-rw-   0        0        0    13016 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/models/dimensions.py
--rw-rw-rw-   0        0        0      945 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/models/facts.py
--rw-rw-rw-   0        0        0     1656 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/models/namespace.py
--rw-rw-rw-   0        0        0      294 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/models/nested_path.py
--rw-rw-rw-   0        0        0      408 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_base/models/relation.py
--rw-rw-rw-   0        0        0     5523 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/models/schema.py
--rw-rw-rw-   0        0        0      833 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/models/snowflake.py
--rw-rw-rw-   0        0        0      687 2024-03-16 21:27:51.000000 jx-python-4.579.24081/jx_base/models/table.py
--rw-rw-rw-   0        0        0      791 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_base/queries.py
--rw-rw-rw-   0        0        0     2520 2024-02-15 03:10:30.000000 jx-python-4.579.24081/jx_base/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.692774 jx-python-4.579.24081/jx_python/
--rw-rw-rw-   0        0        0      614 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.718438 jx-python-4.579.24081/jx_python/containers/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.579.24081/jx_python/containers/__init__.py
--rw-rw-rw-   0        0        0    16625 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/containers/cube.py
--rw-rw-rw-   0        0        0    10036 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/containers/list.py
--rw-rw-rw-   0        0        0     1836 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/convert.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.720773 jx-python-4.579.24081/jx_python/cubes/
--rw-rw-rw-   0        0        0        0 2020-01-29 00:24:56.000000 jx-python-4.579.24081/jx_python/cubes/__init__.py
--rw-rw-rw-   0        0        0     3647 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/cubes/aggs.py
--rw-rw-rw-   0        0        0     1920 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expression_compiler.py
--rw-rw-rw-   0        0        0     1735 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expression_factory.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.810060 jx-python-4.579.24081/jx_python/expressions/
--rw-rw-rw-   0        0        0     3954 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/__init__.py
--rw-rw-rw-   0        0        0     4641 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/_utils.py
--rw-rw-rw-   0        0        0      440 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/add_op.py
--rw-rw-rw-   0        0        0      945 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_python/expressions/and_op.py
--rw-rw-rw-   0        0        0      857 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/array_of_op.py
--rw-rw-rw-   0        0        0      714 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/avg_op.py
--rw-rw-rw-   0        0        0      884 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/basic_add_op.py
--rw-rw-rw-   0        0        0      846 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/basic_eq_op.py
--rw-rw-rw-   0        0        0      866 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/basic_index_of_op.py
--rw-rw-rw-   0        0        0      907 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/expressions/basic_starts_with_op.py
--rw-rw-rw-   0        0        0      993 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/expressions/basic_substring_op.py
--rw-rw-rw-   0        0        0      372 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/between_op.py
--rw-rw-rw-   0        0        0     1285 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/call_op.py
--rw-rw-rw-   0        0        0      673 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/cardinality_op.py
--rw-rw-rw-   0        0        0      716 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/case_op.py
--rw-rw-rw-   0        0        0      976 2024-01-21 21:27:17.000000 jx-python-4.579.24081/jx_python/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     1146 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/concat_op.py
--rw-rw-rw-   0        0        0      786 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/count_op.py
--rw-rw-rw-   0        0        0      554 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/date_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/div_op.py
--rw-rw-rw-   0        0        0     1605 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/eq_op.py
--rw-rw-rw-   0        0        0      750 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/exists_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/exp_op.py
--rw-rw-rw-   0        0        0      635 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/false_op.py
--rw-rw-rw-   0        0        0     1110 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/filter_op.py
--rw-rw-rw-   0        0        0     1689 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_python/expressions/find_op.py
--rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/first_op.py
--rw-rw-rw-   0        0        0      647 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/floor_op.py
--rw-rw-rw-   0        0        0      368 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/format_op.py
--rw-rw-rw-   0        0        0     1823 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/get_op.py
--rw-rw-rw-   0        0        0     1707 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/group_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/gt_op.py
--rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/gte_op.py
--rw-rw-rw-   0        0        0      831 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/in_op.py
--rw-rw-rw-   0        0        0      787 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/is_text_op.py
--rw-rw-rw-   0        0        0     1109 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/last_op.py
--rw-rw-rw-   0        0        0     1026 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_python/expressions/least_op.py
--rw-rw-rw-   0        0        0      559 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/leaves_op.py
--rw-rw-rw-   0        0        0      692 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/length_op.py
--rw-rw-rw-   0        0        0      953 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/limit_op.py
--rw-rw-rw-   0        0        0      618 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/literal.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/lt_op.py
--rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/lte_op.py
--rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/max_op.py
--rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/min_op.py
--rw-rw-rw-   0        0        0     1045 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/missing_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/mod_op.py
--rw-rw-rw-   0        0        0      981 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/most_op.py
--rw-rw-rw-   0        0        0      533 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/mul_op.py
--rw-rw-rw-   0        0        0      992 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/name_op.py
--rw-rw-rw-   0        0        0      733 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/ne_op.py
--rw-rw-rw-   0        0        0      773 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/not_left_op.py
--rw-rw-rw-   0        0        0      680 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/not_op.py
--rw-rw-rw-   0        0        0      999 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/not_right_op.py
--rw-rw-rw-   0        0        0      556 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/offset_op.py
--rw-rw-rw-   0        0        0      930 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/or_op.py
--rw-rw-rw-   0        0        0      468 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/percentile_op.py
--rw-rw-rw-   0        0        0      651 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/prefix_op.py
--rw-rw-rw-   0        0        0     1303 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/product_op.py
--rw-rw-rw-   0        0        0     1139 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/python_function.py
--rw-rw-rw-   0        0        0     1443 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/python_script.py
--rw-rw-rw-   0        0        0      364 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/range_op.py
--rw-rw-rw-   0        0        0      946 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0      699 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/right_op.py
--rw-rw-rw-   0        0        0     1022 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/rows_op.py
--rw-rw-rw-   0        0        0      594 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/script_op.py
--rw-rw-rw-   0        0        0     2105 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/select_op.py
--rw-rw-rw-   0        0        0      643 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/split_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/sub_op.py
--rw-rw-rw-   0        0        0      742 2024-02-27 03:13:49.000000 jx-python-4.579.24081/jx_python/expressions/suffix_op.py
--rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/sum_op.py
--rw-rw-rw-   0        0        0     1056 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/tally_op.py
--rw-rw-rw-   0        0        0      835 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/to_array_op.py
--rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0      606 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     1034 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/to_number_op.py
--rw-rw-rw-   0        0        0      800 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/to_text_op.py
--rw-rw-rw-   0        0        0      957 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/to_value_op.py
--rw-rw-rw-   0        0        0      628 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/true_op.py
--rw-rw-rw-   0        0        0      812 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/tuple_op.py
--rw-rw-rw-   0        0        0     1328 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/expressions/variable.py
--rw-rw-rw-   0        0        0      968 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/expressions/when_op.py
--rw-rw-rw-   0        0        0     4434 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/flat_list.py
--rw-rw-rw-   0        0        0     4439 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/group_by.py
--rw-rw-rw-   0        0        0    34076 2024-01-25 04:46:12.000000 jx-python-4.579.24081/jx_python/jx.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.812570 jx-python-4.579.24081/jx_python/lists/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.579.24081/jx_python/lists/__init__.py
--rw-rw-rw-   0        0        0     4978 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/lists/aggs.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.814502 jx-python-4.579.24081/jx_python/namespace/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.579.24081/jx_python/namespace/__init__.py
--rw-rw-rw-   0        0        0     8745 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/namespace/normal.py
--rw-rw-rw-   0        0        0      768 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/records.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.816895 jx-python-4.579.24081/jx_python/streams/
--rw-rw-rw-   0        0        0     4178 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/streams/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/streams/expression_compiler.py
--rw-rw-rw-   0        0        0     4727 2024-01-20 18:36:41.000000 jx-python-4.579.24081/jx_python/streams/expression_factory.py
--rw-rw-rw-   0        0        0      713 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/streams/inspects.py
--rw-rw-rw-   0        0        0      807 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/streams/type_parser.py
--rw-rw-rw-   0        0        0     5515 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/streams/typers.py
--rw-rw-rw-   0        0        0     1622 2024-03-16 21:32:01.000000 jx-python-4.579.24081/jx_python/streams.py
--rw-rw-rw-   0        0        0      564 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/table.py
--rw-rw-rw-   0        0        0     1431 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/utils.py
--rw-rw-rw-   0        0        0     7410 2023-06-17 11:25:18.000000 jx-python-4.579.24081/jx_python/windows.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:48:05.816895 jx-python-4.579.24081/jx_python.egg-info/
--rw-rw-rw-   0        0        0     1743 2024-03-21 02:48:05.000000 jx-python-4.579.24081/jx_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8866 2024-03-21 02:48:05.000000 jx-python-4.579.24081/jx_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 02:48:05.000000 jx-python-4.579.24081/jx_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2024-03-21 02:48:05.000000 jx-python-4.579.24081/jx_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-21 02:48:05.000000 jx-python-4.579.24081/jx_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 02:48:05.824476 jx-python-4.579.24081/setup.cfg
--rw-rw-rw-   0        0        0     1872 2024-03-21 02:48:00.000000 jx-python-4.579.24081/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.067338 jx-python-4.582.24095/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 jx-python-4.582.24095/LICENSE
+-rw-rw-rw-   0        0        0     1743 2024-04-04 04:16:15.066336 jx-python-4.582.24095/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-03-08 02:37:16.000000 jx-python-4.582.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.597650 jx-python-4.582.24095/jx_base/
+-rw-rw-rw-   0        0        0     1553 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/__init__.py
+-rw-rw-rw-   0        0        0     8710 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/data_class.py
+-rw-rw-rw-   0        0        0    25274 2024-02-06 05:15:22.000000 jx-python-4.582.24095/jx_base/domains.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.878298 jx-python-4.582.24095/jx_base/expressions/
+-rw-rw-rw-   0        0        0    10593 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4925 2024-03-20 02:23:03.000000 jx-python-4.582.24095/jx_base/expressions/_utils.py
+-rw-rw-rw-   0        0        0     1027 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/abs_op.py
+-rw-rw-rw-   0        0        0      800 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/add_op.py
+-rw-rw-rw-   0        0        0     2379 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/aggregate_op.py
+-rw-rw-rw-   0        0        0     1277 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/all_op.py
+-rw-rw-rw-   0        0        0     3312 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/and_op.py
+-rw-rw-rw-   0        0        0     1394 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/any_op.py
+-rw-rw-rw-   0        0        0      918 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/array_of_op.py
+-rw-rw-rw-   0        0        0      453 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/avg_op.py
+-rw-rw-rw-   0        0        0     2183 2024-01-22 13:00:58.000000 jx-python-4.582.24095/jx_base/expressions/base_binary_op.py
+-rw-rw-rw-   0        0        0      520 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/base_inequality_op.py
+-rw-rw-rw-   0        0        0     2960 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/base_multi_op.py
+-rw-rw-rw-   0        0        0      391 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/basic_add_op.py
+-rw-rw-rw-   0        0        0     1546 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_boolean_op.py
+-rw-rw-rw-   0        0        0     1109 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/basic_eq_op.py
+-rw-rw-rw-   0        0        0     3370 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_in_op.py
+-rw-rw-rw-   0        0        0     1972 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/basic_index_of_op.py
+-rw-rw-rw-   0        0        0      391 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/basic_mul_op.py
+-rw-rw-rw-   0        0        0     1966 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_multi_op.py
+-rw-rw-rw-   0        0        0     1277 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_not_op.py
+-rw-rw-rw-   0        0        0     1666 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_starts_with_op.py
+-rw-rw-rw-   0        0        0     1332 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/basic_substring_op.py
+-rw-rw-rw-   0        0        0     4496 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1544 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/call_op.py
+-rw-rw-rw-   0        0        0      661 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/cardinality_op.py
+-rw-rw-rw-   0        0        0     4044 2024-03-21 02:47:56.000000 jx-python-4.582.24095/jx_base/expressions/case_op.py
+-rw-rw-rw-   0        0        0     2037 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     1593 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/comment_op.py
+-rw-rw-rw-   0        0        0     2890 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/concat_op.py
+-rw-rw-rw-   0        0        0     1592 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/count_op.py
+-rw-rw-rw-   0        0        0     1250 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/date_op.py
+-rw-rw-rw-   0        0        0     2111 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/default_op.py
+-rw-rw-rw-   0        0        0     1179 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/div_op.py
+-rw-rw-rw-   0        0        0     2757 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      418 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/es_script.py
+-rw-rw-rw-   0        0        0     1525 2024-01-28 16:03:01.000000 jx-python-4.582.24095/jx_base/expressions/es_select_op.py
+-rw-rw-rw-   0        0        0     1270 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/exp_op.py
+-rw-rw-rw-   0        0        0     6265 2024-01-22 13:00:58.000000 jx-python-4.582.24095/jx_base/expressions/expression.py
+-rw-rw-rw-   0        0        0     1524 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/false_op.py
+-rw-rw-rw-   0        0        0     1278 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     2242 2024-01-28 16:03:01.000000 jx-python-4.582.24095/jx_base/expressions/find_op.py
+-rw-rw-rw-   0        0        0     2413 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/first_op.py
+-rw-rw-rw-   0        0        0      657 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/floor_op.py
+-rw-rw-rw-   0        0        0    10147 2024-02-06 05:15:22.000000 jx-python-4.582.24095/jx_base/expressions/format_op.py
+-rw-rw-rw-   0        0        0     1577 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/from_op.py
+-rw-rw-rw-   0        0        0      807 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/from_unix_op.py
+-rw-rw-rw-   0        0        0     3022 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/get_op.py
+-rw-rw-rw-   0        0        0     1082 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/group_op.py
+-rw-rw-rw-   0        0        0      385 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      386 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/gte_op.py
+-rw-rw-rw-   0        0        0     3648 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/in_op.py
+-rw-rw-rw-   0        0        0     2505 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/inner_join_op.py
+-rw-rw-rw-   0        0        0     1322 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_boolean_op.py
+-rw-rw-rw-   0        0        0      969 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_integer_op.py
+-rw-rw-rw-   0        0        0     1360 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_number_op.py
+-rw-rw-rw-   0        0        0     1451 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0     1561 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/last_op.py
+-rw-rw-rw-   0        0        0     1761 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/least_op.py
+-rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0     2037 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/left_op.py
+-rw-rw-rw-   0        0        0     1601 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/length_op.py
+-rw-rw-rw-   0        0        0     2593 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/limit_op.py
+-rw-rw-rw-   0        0        0     3326 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/literal.py
+-rw-rw-rw-   0        0        0      384 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      385 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      507 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/map_op.py
+-rw-rw-rw-   0        0        0     1418 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/max_op.py
+-rw-rw-rw-   0        0        0     1442 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1861 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/mod_op.py
+-rw-rw-rw-   0        0        0      845 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/most_op.py
+-rw-rw-rw-   0        0        0      882 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/mul_op.py
+-rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/name_op.py
+-rw-rw-rw-   0        0        0     1647 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/ne_op.py
+-rw-rw-rw-   0        0        0     4366 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/nested_op.py
+-rw-rw-rw-   0        0        0     2061 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0     1612 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/not_op.py
+-rw-rw-rw-   0        0        0     2150 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0     2442 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/null_op.py
+-rw-rw-rw-   0        0        0     1059 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/offset_op.py
+-rw-rw-rw-   0        0        0     2239 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/or_op.py
+-rw-rw-rw-   0        0        0     2503 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/outer_join_op.py
+-rw-rw-rw-   0        0        0     1387 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/percentile_op.py
+-rw-rw-rw-   0        0        0     3285 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0     1585 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/product_op.py
+-rw-rw-rw-   0        0        0      460 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/python_function.py
+-rw-rw-rw-   0        0        0     1512 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/python_script.py
+-rw-rw-rw-   0        0        0    24585 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/query_op.py
+-rw-rw-rw-   0        0        0     1025 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/range_op.py
+-rw-rw-rw-   0        0        0     1575 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0     2247 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/right_op.py
+-rw-rw-rw-   0        0        0     1478 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/rows_op.py
+-rw-rw-rw-   0        0        0     1247 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/script_op.py
+-rw-rw-rw-   0        0        0    12251 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/select_op.py
+-rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/split_op.py
+-rw-rw-rw-   0        0        0     1295 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/sql_alias_op.py
+-rw-rw-rw-   0        0        0     1027 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_and_op.py
+-rw-rw-rw-   0        0        0     1010 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/sql_cast_op.py
+-rw-rw-rw-   0        0        0     1361 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_concat_op.py
+-rw-rw-rw-   0        0        0     1490 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/sql_eq_op.py
+-rw-rw-rw-   0        0        0     1082 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_gt_op.py
+-rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_gte_op.py
+-rw-rw-rw-   0        0        0      343 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_in_op.py
+-rw-rw-rw-   0        0        0      428 2024-01-22 13:00:58.000000 jx-python-4.582.24095/jx_base/expressions/sql_inner_join_op.py
+-rw-rw-rw-   0        0        0     1192 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/expressions/sql_instr_op.py
+-rw-rw-rw-   0        0        0      832 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/sql_is_null_op.py
+-rw-rw-rw-   0        0        0     3313 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sql_left_joins_op.py
+-rw-rw-rw-   0        0        0      499 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_limit_op.py
+-rw-rw-rw-   0        0        0      360 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/sql_literal.py
+-rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_lt_op.py
+-rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx-python-4.582.24095/jx_base/expressions/sql_lte_op.py
+-rw-rw-rw-   0        0        0     1449 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/sql_not_op.py
+-rw-rw-rw-   0        0        0     2371 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_or_op.py
+-rw-rw-rw-   0        0        0      781 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_order_by_op.py
+-rw-rw-rw-   0        0        0     1057 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sql_origins_op.py
+-rw-rw-rw-   0        0        0      427 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/expressions/sql_script.py
+-rw-rw-rw-   0        0        0      958 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sql_select_all_from_op.py
+-rw-rw-rw-   0        0        0     2012 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0      911 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/sql_substr_op.py
+-rw-rw-rw-   0        0        0     1583 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sql_variable.py
+-rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0     1549 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_boolean_op.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0     3378 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_in_op.py
+-rw-rw-rw-   0        0        0     1976 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_mul_op.py
+-rw-rw-rw-   0        0        0     1967 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_multi_op.py
+-rw-rw-rw-   0        0        0     1281 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_not_op.py
+-rw-rw-rw-   0        0        0     1671 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0     1335 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0      611 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/sub_op.py
+-rw-rw-rw-   0        0        0     3011 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0     1556 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/sum_op.py
+-rw-rw-rw-   0        0        0      721 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/tally_op.py
+-rw-rw-rw-   0        0        0     1594 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/to_array_op.py
+-rw-rw-rw-   0        0        0     1304 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0     2708 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     2874 2024-03-02 22:12:26.000000 jx-python-4.582.24095/jx_base/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0     2043 2024-03-10 19:33:03.000000 jx-python-4.582.24095/jx_base/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/to_value_op.py
+-rw-rw-rw-   0        0        0     1626 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/true_op.py
+-rw-rw-rw-   0        0        0     1678 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0     2000 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/union_op.py
+-rw-rw-rw-   0        0        0      826 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/expressions/unix_op.py
+-rw-rw-rw-   0        0        0     6148 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/expressions/variable.py
+-rw-rw-rw-   0        0        0     3270 2024-03-21 02:47:56.000000 jx-python-4.582.24095/jx_base/expressions/when_op.py
+-rw-rw-rw-   0        0        0    14462 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_base/language.py
+-rw-rw-rw-   0        0        0    15169 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_base/meta_columns.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.886703 jx-python-4.582.24095/jx_base/models/
+-rw-rw-rw-   0        0        0        0 2022-11-12 15:14:28.000000 jx-python-4.582.24095/jx_base/models/__init__.py
+-rw-rw-rw-   0        0        0     2369 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/container.py
+-rw-rw-rw-   0        0        0    13016 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/dimensions.py
+-rw-rw-rw-   0        0        0      945 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/facts.py
+-rw-rw-rw-   0        0        0     1656 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/namespace.py
+-rw-rw-rw-   0        0        0      294 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/nested_path.py
+-rw-rw-rw-   0        0        0      408 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_base/models/relation.py
+-rw-rw-rw-   0        0        0     5523 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/schema.py
+-rw-rw-rw-   0        0        0      833 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/snowflake.py
+-rw-rw-rw-   0        0        0      687 2024-03-16 21:27:51.000000 jx-python-4.582.24095/jx_base/models/table.py
+-rw-rw-rw-   0        0        0      791 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_base/queries.py
+-rw-rw-rw-   0        0        0     2520 2024-02-15 03:10:30.000000 jx-python-4.582.24095/jx_base/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.898849 jx-python-4.582.24095/jx_python/
+-rw-rw-rw-   0        0        0      614 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.934413 jx-python-4.582.24095/jx_python/containers/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.582.24095/jx_python/containers/__init__.py
+-rw-rw-rw-   0        0        0    16625 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/containers/cube.py
+-rw-rw-rw-   0        0        0     9580 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/containers/list.py
+-rw-rw-rw-   0        0        0     1836 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/convert.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:14.936838 jx-python-4.582.24095/jx_python/cubes/
+-rw-rw-rw-   0        0        0        0 2020-01-29 00:24:56.000000 jx-python-4.582.24095/jx_python/cubes/__init__.py
+-rw-rw-rw-   0        0        0     3647 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/cubes/aggs.py
+-rw-rw-rw-   0        0        0     1920 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expression_compiler.py
+-rw-rw-rw-   0        0        0     1735 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expression_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.051797 jx-python-4.582.24095/jx_python/expressions/
+-rw-rw-rw-   0        0        0     3964 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4641 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/_utils.py
+-rw-rw-rw-   0        0        0      440 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/add_op.py
+-rw-rw-rw-   0        0        0      945 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_python/expressions/and_op.py
+-rw-rw-rw-   0        0        0      857 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/array_of_op.py
+-rw-rw-rw-   0        0        0      714 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/avg_op.py
+-rw-rw-rw-   0        0        0      884 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/basic_add_op.py
+-rw-rw-rw-   0        0        0      846 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/basic_eq_op.py
+-rw-rw-rw-   0        0        0      866 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/basic_index_of_op.py
+-rw-rw-rw-   0        0        0      907 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/expressions/basic_starts_with_op.py
+-rw-rw-rw-   0        0        0      993 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/expressions/basic_substring_op.py
+-rw-rw-rw-   0        0        0      372 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1285 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/call_op.py
+-rw-rw-rw-   0        0        0      673 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/cardinality_op.py
+-rw-rw-rw-   0        0        0      716 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/case_op.py
+-rw-rw-rw-   0        0        0      976 2024-01-21 21:27:17.000000 jx-python-4.582.24095/jx_python/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     1146 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/concat_op.py
+-rw-rw-rw-   0        0        0      786 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/count_op.py
+-rw-rw-rw-   0        0        0      554 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/date_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/div_op.py
+-rw-rw-rw-   0        0        0     1608 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      750 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/exp_op.py
+-rw-rw-rw-   0        0        0      635 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/false_op.py
+-rw-rw-rw-   0        0        0     1110 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     1692 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/find_op.py
+-rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/first_op.py
+-rw-rw-rw-   0        0        0      647 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/floor_op.py
+-rw-rw-rw-   0        0        0      368 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/format_op.py
+-rw-rw-rw-   0        0        0     1823 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/get_op.py
+-rw-rw-rw-   0        0        0     1707 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/group_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/gte_op.py
+-rw-rw-rw-   0        0        0      831 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/in_op.py
+-rw-rw-rw-   0        0        0      787 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0     1109 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/last_op.py
+-rw-rw-rw-   0        0        0     1026 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_python/expressions/least_op.py
+-rw-rw-rw-   0        0        0      559 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0      692 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/length_op.py
+-rw-rw-rw-   0        0        0      953 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/limit_op.py
+-rw-rw-rw-   0        0        0      618 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/literal.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/max_op.py
+-rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1045 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/mod_op.py
+-rw-rw-rw-   0        0        0      981 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/most_op.py
+-rw-rw-rw-   0        0        0      533 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/mul_op.py
+-rw-rw-rw-   0        0        0      992 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/name_op.py
+-rw-rw-rw-   0        0        0      733 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/ne_op.py
+-rw-rw-rw-   0        0        0      773 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0      680 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/not_op.py
+-rw-rw-rw-   0        0        0      999 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0      556 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/offset_op.py
+-rw-rw-rw-   0        0        0      930 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/or_op.py
+-rw-rw-rw-   0        0        0      468 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/percentile_op.py
+-rw-rw-rw-   0        0        0      651 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0     1303 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/product_op.py
+-rw-rw-rw-   0        0        0     1139 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/python_function.py
+-rw-rw-rw-   0        0        0     1443 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/python_script.py
+-rw-rw-rw-   0        0        0      364 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/range_op.py
+-rw-rw-rw-   0        0        0      946 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0      699 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/right_op.py
+-rw-rw-rw-   0        0        0     1022 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/rows_op.py
+-rw-rw-rw-   0        0        0      594 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/script_op.py
+-rw-rw-rw-   0        0        0     2105 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/select_op.py
+-rw-rw-rw-   0        0        0      643 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/split_op.py
+-rw-rw-rw-   0        0        0      888 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0      850 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0      870 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      912 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0      998 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/sub_op.py
+-rw-rw-rw-   0        0        0      742 2024-02-27 03:13:49.000000 jx-python-4.582.24095/jx_python/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/sum_op.py
+-rw-rw-rw-   0        0        0     1056 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/tally_op.py
+-rw-rw-rw-   0        0        0      835 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/to_array_op.py
+-rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0      606 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     1034 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0      800 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0      957 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/to_value_op.py
+-rw-rw-rw-   0        0        0      628 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/true_op.py
+-rw-rw-rw-   0        0        0      812 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0     1328 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/expressions/variable.py
+-rw-rw-rw-   0        0        0      968 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/expressions/when_op.py
+-rw-rw-rw-   0        0        0     4434 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/flat_list.py
+-rw-rw-rw-   0        0        0     4439 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/group_by.py
+-rw-rw-rw-   0        0        0    34076 2024-01-25 04:46:12.000000 jx-python-4.582.24095/jx_python/jx.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.054808 jx-python-4.582.24095/jx_python/lists/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.582.24095/jx_python/lists/__init__.py
+-rw-rw-rw-   0        0        0     5009 2024-04-04 04:16:05.000000 jx-python-4.582.24095/jx_python/lists/aggs.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.056805 jx-python-4.582.24095/jx_python/namespace/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx-python-4.582.24095/jx_python/namespace/__init__.py
+-rw-rw-rw-   0        0        0     8745 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/namespace/normal.py
+-rw-rw-rw-   0        0        0      768 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/records.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.062323 jx-python-4.582.24095/jx_python/streams/
+-rw-rw-rw-   0        0        0     4178 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/streams/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/expression_compiler.py
+-rw-rw-rw-   0        0        0     4727 2024-01-20 18:36:41.000000 jx-python-4.582.24095/jx_python/streams/expression_factory.py
+-rw-rw-rw-   0        0        0      713 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/inspects.py
+-rw-rw-rw-   0        0        0      807 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/type_parser.py
+-rw-rw-rw-   0        0        0     5515 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/streams/typers.py
+-rw-rw-rw-   0        0        0     1622 2024-03-16 21:32:01.000000 jx-python-4.582.24095/jx_python/streams.py
+-rw-rw-rw-   0        0        0      564 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/table.py
+-rw-rw-rw-   0        0        0     1431 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/utils.py
+-rw-rw-rw-   0        0        0     7410 2023-06-17 11:25:18.000000 jx-python-4.582.24095/jx_python/windows.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:16:15.064339 jx-python-4.582.24095/jx_python.egg-info/
+-rw-rw-rw-   0        0        0     1743 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9472 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      265 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-04 04:16:14.000000 jx-python-4.582.24095/jx_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 04:16:15.067338 jx-python-4.582.24095/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2024-04-04 04:16:09.000000 jx-python-4.582.24095/setup.py
```

### Comparing `jx-python-4.579.24081/LICENSE` & `jx-python-4.582.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/PKG-INFO` & `jx-python-4.582.24095/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-python
-Version: 4.579.24081
+Version: 4.582.24095
 Summary: JSON query expressions using Python
 Home-page: https://github.com/klahnakoski/jx-python
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,24 +12,24 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.579.24081
-Requires-Dist: mo-dots==9.578.24081
+Requires-Dist: mo-collections==5.582.24095
+Requires-Dist: mo-dots==9.582.24095
 Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-json==6.579.24081
-Requires-Dist: mo-json-config==4.579.24081
-Requires-Dist: mo-kwargs==7.578.24081
-Requires-Dist: mo-logs==8.579.24081
-Requires-Dist: mo-math==7.579.24081
-Requires-Dist: mo-threads==6.579.24081
-Requires-Dist: mo-times==5.579.24081
+Requires-Dist: mo-json==6.582.24095
+Requires-Dist: mo-json-config==4.582.24095
+Requires-Dist: mo-kwargs==7.582.24095
+Requires-Dist: mo-logs==8.582.24095
+Requires-Dist: mo-math==7.582.24095
+Requires-Dist: mo-threads==6.582.24095
+Requires-Dist: mo-times==5.582.24095
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 
 # jx-python
 
 Python library for JSON Expressions
```

### Comparing `jx-python-4.579.24081/jx_base/__init__.py` & `jx-python-4.582.24095/jx_base/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from jx_base.expressions import jx_expression
 from jx_base.expressions._utils import JX, simplified, builtin_ops
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.null_op import NULL
 from jx_base.expressions.true_op import TRUE
 from jx_base.expressions.when_op import WhenOp
 from jx_base.language import is_op
+from jx_base.meta_columns import get_schema_from_list
 from jx_base.models.container import Container
 from jx_base.models.facts import Facts
 from jx_base.models.namespace import Namespace
 from jx_base.models.nested_path import NestedPath
 from jx_base.models.relation import Relation
 from jx_base.models.schema import Schema
 from jx_base.models.snowflake import Snowflake
@@ -31,14 +32,15 @@
     "builtin_ops",
     "Container",
     "Column",
     "DataClass",
     "enlist",
     "Facts",
     "FALSE",
+    "get_schema_from_list",
     "is_op",
     "jx_expression",
     "JX",
     "Namespace",
     "NestedPath",
     "NULL",
     "Python",
```

### Comparing `jx-python-4.579.24081/jx_base/data_class.py` & `jx-python-4.582.24095/jx_base/data_class.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/domains.py` & `jx-python-4.582.24095/jx_base/domains.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/__init__.py` & `jx-python-4.582.24095/jx_base/expressions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-from jx_base.expressions._utils import (
-    jx_expression,
-    merge_types,
-    operators,
-    JX,
-    _jx_expression,
-)
+from jx_base.expressions._utils import jx_expression, merge_types, operators, JX, _jx_expression
 from jx_base.expressions.abs_op import AbsOp
 from jx_base.expressions.add_op import AddOp
 from jx_base.expressions.aggregate_op import AggregateOp
 from jx_base.expressions.all_op import AllOp
 from jx_base.expressions.and_op import AndOp
 from jx_base.expressions.any_op import AnyOp
 from jx_base.expressions.array_of_op import ArrayOfOp
 from jx_base.expressions.avg_op import AvgOp
 from jx_base.expressions.base_binary_op import BaseBinaryOp
 from jx_base.expressions.base_inequality_op import BaseInequalityOp
 from jx_base.expressions.base_multi_op import BaseMultiOp
-from jx_base.expressions.basic_add_op import BasicAddOp
-from jx_base.expressions.basic_boolean_op import BasicBooleanOp
-from jx_base.expressions.basic_eq_op import BasicEqOp
-from jx_base.expressions.basic_in_op import BasicInOp
-from jx_base.expressions.basic_index_of_op import BasicIndexOfOp
-from jx_base.expressions.basic_mul_op import BasicMulOp
-from jx_base.expressions.basic_multi_op import BasicMultiOp
-from jx_base.expressions.basic_not_op import BasicNotOp
-from jx_base.expressions.basic_starts_with_op import BasicStartsWithOp
-from jx_base.expressions.basic_substring_op import BasicSubstringOp
 from jx_base.expressions.between_op import BetweenOp
 from jx_base.expressions.call_op import CallOp
 from jx_base.expressions.cardinality_op import CardinalityOp
 from jx_base.expressions.case_op import CaseOp
 from jx_base.expressions.coalesce_op import CoalesceOp
 from jx_base.expressions.comment_op import CommentOp
 from jx_base.expressions.concat_op import ConcatOp
@@ -120,14 +104,24 @@
 from jx_base.expressions.sql_order_by_op import SqlOrderByOp
 from jx_base.expressions.sql_origins_op import SqlOriginsOp
 from jx_base.expressions.sql_script import SqlScript
 from jx_base.expressions.sql_select_all_from_op import SqlSelectAllFromOp
 from jx_base.expressions.sql_select_op import SqlSelectOp
 from jx_base.expressions.sql_substr_op import SqlSubstrOp
 from jx_base.expressions.sql_variable import SqlVariable
+from jx_base.expressions.strict_add_op import StrictAddOp
+from jx_base.expressions.strict_boolean_op import StrictBooleanOp
+from jx_base.expressions.strict_eq_op import StrictEqOp
+from jx_base.expressions.strict_in_op import StrictInOp
+from jx_base.expressions.strict_index_of_op import StrictIndexOfOp
+from jx_base.expressions.strict_mul_op import StrictMulOp
+from jx_base.expressions.strict_multi_op import StrictMultiOp
+from jx_base.expressions.strict_not_op import StrictNotOp
+from jx_base.expressions.strict_starts_with_op import StrictStartsWithOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp
 from jx_base.expressions.sub_op import SubOp
 from jx_base.expressions.suffix_op import SuffixOp
 from jx_base.expressions.sum_op import SumOp
 from jx_base.expressions.tally_op import TallyOp
 from jx_base.expressions.to_array_op import ToArrayOp
 from jx_base.expressions.to_boolean_op import ToBooleanOp
 from jx_base.expressions.to_integer_op import ToIntegerOp
@@ -147,17 +141,17 @@
     {
         "abs": AbsOp,
         "add": AddOp,
         "aggregate": AggregateOp,
         "and": AndOp,
         "array": ArrayOfOp,
         "avg": AvgOp,
-        "basic.add": BasicAddOp,
-        "basic.boolean": BasicBooleanOp,
-        "basic.mul": BasicMulOp,
+        "strict.add": StrictAddOp,
+        "strict.boolean": StrictBooleanOp,
+        "strict.mul": StrictMulOp,
         "between": BetweenOp,
         "cardinality": CardinalityOp,
         "case": CaseOp,
         "coalesce": CoalesceOp,
         "comment": CommentOp,
         "meta": CommentOp,
         "concat": ConcatOp,
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/_utils.py` & `jx-python-4.582.24095/jx_base/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/abs_op.py` & `jx-python-4.582.24095/jx_base/expressions/abs_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/add_op.py` & `jx-python-4.582.24095/jx_base/expressions/add_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/aggregate_op.py` & `jx-python-4.582.24095/jx_base/expressions/aggregate_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/all_op.py` & `jx-python-4.582.24095/jx_base/expressions/all_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/and_op.py` & `jx-python-4.582.24095/jx_base/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/any_op.py` & `jx-python-4.582.24095/jx_base/expressions/any_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/array_of_op.py` & `jx-python-4.582.24095/jx_base/expressions/array_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/base_binary_op.py` & `jx-python-4.582.24095/jx_base/expressions/base_binary_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/base_inequality_op.py` & `jx-python-4.582.24095/jx_base/expressions/base_inequality_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/base_multi_op.py` & `jx-python-4.582.24095/jx_base/expressions/base_multi_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_boolean_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_eq_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_in_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_in_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_index_of_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_multi_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_multi_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_not_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_not_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_starts_with_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_starts_with_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/basic_substring_op.py` & `jx-python-4.582.24095/jx_base/expressions/basic_substring_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/between_op.py` & `jx-python-4.582.24095/jx_base/expressions/between_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 from jx_base.expressions._utils import jx_expression
 from jx_base.expressions.add_op import AddOp
-from jx_base.expressions.basic_substring_op import BasicSubstringOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp
 from jx_base.expressions.case_op import CaseOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.find_op import FindOp
 from jx_base.expressions.is_number_op import IsNumberOp
 from jx_base.expressions.length_op import LengthOp
 from jx_base.expressions.literal import Literal, ZERO, is_literal
 from jx_base.expressions.max_op import MaxOp
@@ -104,12 +104,12 @@
             WhenOp(start_index.missing(lang), then=NULL),
             WhenOp(self.suffix.missing(lang), then=LengthOp(value)),
             WhenOp(IsNumberOp(self.suffix), then=MinOp(self.suffix, LengthOp(value))),
             FindOp(value, self.suffix, AddOp(start_index, len_prefix)),
         ).partial_eval(lang)
 
         start_index = AddOp(start_index, len_prefix).partial_eval(lang)
-        substring = BasicSubstringOp(value, start_index, end_index).partial_eval(lang)
+        substring = StrictSubstringOp(value, start_index, end_index).partial_eval(lang)
 
         between = WhenOp(end_index.missing(lang), **{"else": substring}).partial_eval(lang)
 
         return between
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/call_op.py` & `jx-python-4.582.24095/jx_base/expressions/call_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/cardinality_op.py` & `jx-python-4.582.24095/jx_base/expressions/cardinality_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/case_op.py` & `jx-python-4.582.24095/jx_base/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/coalesce_op.py` & `jx-python-4.582.24095/jx_base/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/comment_op.py` & `jx-python-4.582.24095/jx_base/expressions/comment_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/concat_op.py` & `jx-python-4.582.24095/jx_base/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/count_op.py` & `jx-python-4.582.24095/jx_base/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/date_op.py` & `jx-python-4.582.24095/jx_base/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/default_op.py` & `jx-python-4.582.24095/jx_base/expressions/default_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/div_op.py` & `jx-python-4.582.24095/jx_base/expressions/div_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/eq_op.py` & `jx-python-4.582.24095/jx_base/expressions/eq_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 from jx_base.expressions._utils import _jx_expression
 from jx_base.expressions.and_op import AndOp
 from jx_base.expressions.base_inequality_op import BaseInequalityOp
-from jx_base.expressions.basic_eq_op import BasicEqOp
+from jx_base.expressions.strict_eq_op import StrictEqOp
 from jx_base.expressions.case_op import CaseOp
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.literal import is_literal, Literal
 from jx_base.expressions.true_op import TRUE
 from jx_base.expressions.variable import Variable
 from jx_base.language import value_compare
 from mo_dots import is_many, is_data
@@ -76,8 +76,8 @@
 
         if is_literal(lhs) and is_literal(rhs):
             return FALSE if value_compare(lhs.value, rhs.value) else TRUE
         else:
             return lang.EqOp(lhs, rhs)
 
 
-export("jx_base.expressions.basic_in_op", EqOp)
+export("jx_base.expressions.strict_in_op", EqOp)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/es_select_op.py` & `jx-python-4.582.24095/jx_base/expressions/es_select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/exists_op.py` & `jx-python-4.582.24095/jx_base/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/expression.py` & `jx-python-4.582.24095/jx_base/expressions/expression.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/false_op.py` & `jx-python-4.582.24095/jx_base/expressions/false_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/filter_op.py` & `jx-python-4.582.24095/jx_base/expressions/filter_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/find_op.py` & `jx-python-4.582.24095/jx_base/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/first_op.py` & `jx-python-4.582.24095/jx_base/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/floor_op.py` & `jx-python-4.582.24095/jx_base/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/format_op.py` & `jx-python-4.582.24095/jx_base/expressions/format_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/from_op.py` & `jx-python-4.582.24095/jx_base/expressions/from_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/from_unix_op.py` & `jx-python-4.582.24095/jx_base/expressions/from_unix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/get_op.py` & `jx-python-4.582.24095/jx_base/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/group_op.py` & `jx-python-4.582.24095/jx_base/expressions/group_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/in_op.py` & `jx-python-4.582.24095/jx_base/expressions/in_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions import BasicInOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.get_op import GetOp
 from jx_base.expressions.literal import Literal
 from jx_base.expressions.literal import is_literal
 from jx_base.expressions.missing_op import MissingOp
 from jx_base.expressions.nested_op import NestedOp
 from jx_base.expressions.not_op import NotOp
 from jx_base.expressions.null_op import NULL
 from jx_base.expressions.or_op import OrOp
+from jx_base.expressions.strict_in_op import StrictInOp
 from jx_base.expressions.variable import is_variable
 from jx_base.language import is_op
 from mo_dots import is_many
 from mo_imports import export
 from mo_json.types import JX_BOOLEAN
 
 
@@ -87,15 +87,15 @@
 
     def missing(self, lang):
         return FALSE
 
     def invert(self, lang):
         this = self.partial_eval(lang)
         if is_op(this, InOp):
-            inv = NotOp(BasicInOp(this.value, this.superset))
+            inv = NotOp(StrictInOp(this.value, this.superset))
             inv.simplified = True
             return OrOp(MissingOp(this.value), inv)
         else:
             return this.invert(lang)
 
     def __rcontains__(self, superset):
         if (
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/inner_join_op.py` & `jx-python-4.582.24095/jx_base/expressions/inner_join_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/is_boolean_op.py` & `jx-python-4.582.24095/jx_base/expressions/is_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/is_integer_op.py` & `jx-python-4.582.24095/jx_base/expressions/is_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/is_number_op.py` & `jx-python-4.582.24095/jx_base/expressions/is_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/is_text_op.py` & `jx-python-4.582.24095/jx_base/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/last_op.py` & `jx-python-4.582.24095/jx_base/expressions/last_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/least_op.py` & `jx-python-4.582.24095/jx_base/expressions/least_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/leaves_op.py` & `jx-python-4.582.24095/jx_base/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/left_op.py` & `jx-python-4.582.24095/jx_base/expressions/left_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.basic_substring_op import BasicSubstringOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.length_op import LengthOp
 from jx_base.expressions.literal import ZERO
 from jx_base.expressions.literal import is_literal
 from jx_base.expressions.max_op import MaxOp
 from jx_base.expressions.min_op import MinOp
 from jx_base.expressions.or_op import OrOp
@@ -52,9 +52,9 @@
 
     def partial_eval(self, lang):
         value = (self.value).partial_eval(lang)
         length = (self.length).partial_eval(lang)
         max_length = LengthOp(value)
 
         return WhenOp(
-            self.missing(lang), **{"else": BasicSubstringOp(value, ZERO, MaxOp(ZERO, MinOp(length, max_length)),)}
+            self.missing(lang), **{"else": StrictSubstringOp(value, ZERO, MaxOp(ZERO, MinOp(length, max_length)),)}
         ).partial_eval(lang)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/length_op.py` & `jx-python-4.582.24095/jx_base/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/limit_op.py` & `jx-python-4.582.24095/jx_base/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/literal.py` & `jx-python-4.582.24095/jx_base/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/max_op.py` & `jx-python-4.582.24095/jx_base/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/min_op.py` & `jx-python-4.582.24095/jx_base/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/missing_op.py` & `jx-python-4.582.24095/jx_base/expressions/missing_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,8 @@
         if is_op(output, MissingOp):
             return output
         else:
             return output.partial_eval(lang)
 
 
 export("jx_base.expressions.expression", MissingOp)
-export("jx_base.expressions.basic_in_op", MissingOp)
+export("jx_base.expressions.strict_in_op", MissingOp)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/most_op.py` & `jx-python-4.582.24095/jx_base/expressions/most_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/mul_op.py` & `jx-python-4.582.24095/jx_base/expressions/mul_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/name_op.py` & `jx-python-4.582.24095/jx_base/expressions/name_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/ne_op.py` & `jx-python-4.582.24095/jx_base/expressions/ne_op.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 from jx_base.expressions.base_inequality_op import BaseInequalityOp
 
-from jx_base.expressions.basic_eq_op import BasicEqOp
+from jx_base.expressions.strict_eq_op import StrictEqOp
 from jx_base.expressions.nested_op import NestedOp
 from jx_base.expressions.not_op import NotOp
 from jx_base.expressions.or_op import OrOp
 from jx_base.expressions.variable import IDENTITY
 from jx_base.language import is_op
 
 
@@ -23,24 +23,24 @@
         v1 = self.lhs(row, rownum, rows)
         v2 = self.rhs(row, rownum, rows)
         if v1 == None or v2 == None:
             return False
         return v1 != v2
 
     def invert(self, lang):
-        return OrOp(self.lhs.missing(lang), self.rhs.missing(lang), BasicEqOp(self.lhs, self.rhs),).partial_eval(lang)
+        return OrOp(self.lhs.missing(lang), self.rhs.missing(lang), StrictEqOp(self.lhs, self.rhs),).partial_eval(lang)
 
     def partial_eval(self, lang):
         lhs = self.lhs.partial_eval(lang)
         rhs = self.rhs.partial_eval(lang)
 
         if is_op(lhs, NestedOp):
             return NestedOp(
                 path=lhs.nested_path.partial_eval(lang),
                 select=IDENTITY,
                 where=lang.AndOp(lhs.where, NeOp(lhs.select, rhs)).partial_eval(lang),
                 sort=lhs.sort.partial_eval(lang),
                 limit=lhs.limit.partial_eval(lang),
             ).partial_eval(lang)
 
-        output = lang.AndOp(lhs.exists(), rhs.exists(), NotOp(BasicEqOp(lhs, rhs))).partial_eval(lang)
+        output = lang.AndOp(lhs.exists(), rhs.exists(), NotOp(StrictEqOp(lhs, rhs))).partial_eval(lang)
         return output
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/nested_op.py` & `jx-python-4.582.24095/jx_base/expressions/nested_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,8 +122,8 @@
             NotOp(self.where),
             # self.path.missing(lang), ASSUME PATH TO TABLES, WHICH ASSUMED TO HAVE DATA (EXISTS)
             # self.select.missing(lang),
             EqOp(self.limit, ZERO),
         ).partial_eval(lang)
 
 
-export("jx_base.expressions.basic_in_op", NestedOp)
+export("jx_base.expressions.strict_in_op", NestedOp)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/not_left_op.py` & `jx-python-4.582.24095/jx_base/expressions/not_left_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.basic_substring_op import BasicSubstringOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp
 from jx_base.expressions.coalesce_op import CoalesceOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.length_op import LengthOp
 from jx_base.expressions.literal import ZERO
 from jx_base.expressions.literal import is_literal
 from jx_base.expressions.max_op import MaxOp
 from jx_base.expressions.min_op import MinOp
@@ -52,10 +52,10 @@
 
         if length is ZERO:
             return value
 
         max_length = CoalesceOp(LengthOp(value), ZERO)
         output = WhenOp(
             self.missing(lang),
-            **{"else": BasicSubstringOp(value, MaxOp(ZERO, MinOp(length, max_length)), max_length)}
+            **{"else": StrictSubstringOp(value, MaxOp(ZERO, MinOp(length, max_length)), max_length)}
         ).partial_eval(lang)
         return output
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/not_op.py` & `jx-python-4.582.24095/jx_base/expressions/not_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
         return self.term.partial_eval(lang)
 
     def partial_eval(self, lang):
         return self.term.invert(lang)
 
 
 export("jx_base.expressions.and_op", NotOp)
-export("jx_base.expressions.basic_in_op", NotOp)
+export("jx_base.expressions.strict_in_op", NotOp)
 export("jx_base.expressions.exists_op", NotOp)
 export("jx_base.expressions.expression", NotOp)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/not_right_op.py` & `jx-python-4.582.24095/jx_base/expressions/not_right_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.basic_substring_op import BasicSubstringOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.length_op import LengthOp
 from jx_base.expressions.literal import ZERO
 from jx_base.expressions.literal import is_literal
 from jx_base.expressions.max_op import MaxOp
 from jx_base.expressions.min_op import MinOp
 from jx_base.expressions.or_op import OrOp
@@ -55,9 +55,9 @@
         value = (self.value).partial_eval(lang)
         length = self.length.partial_eval(lang)
 
         if length is ZERO:
             return value
 
         max_length = LengthOp(value)
-        part = BasicSubstringOp(value, ZERO, MaxOp(ZERO, MinOp(max_length, SubOp(max_length, length))),)
+        part = StrictSubstringOp(value, ZERO, MaxOp(ZERO, MinOp(max_length, SubOp(max_length, length))),)
         return (WhenOp(self.missing(lang), **{"else": part})).partial_eval(lang)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/null_op.py` & `jx-python-4.582.24095/jx_base/expressions/null_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,10 +99,10 @@
 
 NULL = NullOp()
 TYPE_ORDER[NullOp] = 9
 TYPE_ORDER[NULL] = 9
 
 export("jx_base.expressions._utils", NULL)
 export("jx_base.expressions.expression", NULL)
-export("jx_base.expressions.basic_in_op", NULL)
+export("jx_base.expressions.strict_in_op", NULL)
 export("jx_base.expressions.literal", NULL)
 export("jx_base.expressions.base_multi_op", NULL)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/offset_op.py` & `jx-python-4.582.24095/jx_base/expressions/offset_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/or_op.py` & `jx-python-4.582.24095/jx_base/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/outer_join_op.py` & `jx-python-4.582.24095/jx_base/expressions/outer_join_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/percentile_op.py` & `jx-python-4.582.24095/jx_base/expressions/percentile_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/prefix_op.py` & `jx-python-4.582.24095/jx_base/expressions/prefix_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 from mo_dots import is_data, is_missing
 
 from jx_base.expressions._utils import jx_expression
-from jx_base.expressions.basic_starts_with_op import BasicStartsWithOp
+from jx_base.expressions.strict_starts_with_op import StrictStartsWithOp
 from jx_base.expressions.case_op import CaseOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.false_op import FALSE
 from jx_base.expressions.is_text_op import IsTextOp
 from jx_base.expressions.literal import is_literal, Literal
 from jx_base.expressions.null_op import NULL
 from jx_base.expressions.true_op import TRUE
@@ -87,14 +87,14 @@
 
     def partial_eval(self, lang):
         prefix = IsTextOp(self.prefix).partial_eval(lang)
         expr = IsTextOp(self.expr).partial_eval(lang)
         return CaseOp(
             WhenOp(prefix.missing(lang), then=TRUE),
             WhenOp(expr.missing(lang), then=FALSE),
-            BasicStartsWithOp(expr, prefix),
+            StrictStartsWithOp(expr, prefix),
         ).partial_eval(lang)
 
     def __eq__(self, other):
         if not is_op(other, PrefixOp):
             return False
         return self.expr == other.frum and self.prefix == other.prefix
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/product_op.py` & `jx-python-4.582.24095/jx_base/expressions/product_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/python_script.py` & `jx-python-4.582.24095/jx_base/expressions/python_script.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/query_op.py` & `jx-python-4.582.24095/jx_base/expressions/query_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         elif query.format == "list" and (select or is_data(select)) and not is_many(select):
             output.select = normalize_one(Null, select, query.format)
             output.select.terms = (output.select.terms[0].set_name("."),)
         elif is_value:
             output.select = _normalize_selects(Null, [select or "."], query.format)
 
         output.select.frum = frum.schema
-        output.where = _normalize_where(query.where, lang)
+        output.where = _normalize_where(query.where)
         output.window = [_normalize_window(w) for w in enlist(query.window)]
         output.sort = _normalize_sort(query.sort)
 
         return output
 
 
     def __data__(self):
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/range_op.py` & `jx-python-4.582.24095/jx_base/expressions/range_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/reg_exp_op.py` & `jx-python-4.582.24095/jx_base/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/right_op.py` & `jx-python-4.582.24095/jx_base/expressions/right_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-from jx_base.expressions.basic_substring_op import BasicSubstringOp
+from jx_base.expressions.strict_substring_op import StrictSubstringOp
 from jx_base.expressions.expression import Expression
 from jx_base.expressions.length_op import LengthOp
 from jx_base.expressions.literal import ZERO
 from jx_base.expressions.literal import is_literal
 from jx_base.expressions.max_op import MaxOp
 from jx_base.expressions.min_op import MinOp
 from jx_base.expressions.or_op import OrOp
@@ -56,9 +56,9 @@
     def partial_eval(self, lang):
         value = self.value.partial_eval(lang)
         length = self.length.partial_eval(lang)
         max_length = LengthOp(value).partial_eval(lang)
 
         return WhenOp(
             self.missing(lang),
-            **{"else": BasicSubstringOp(value, MaxOp(ZERO, MinOp(max_length, SubOp(max_length, length))), max_length,)}
+            **{"else": StrictSubstringOp(value, MaxOp(ZERO, MinOp(max_length, SubOp(max_length, length))), max_length,)}
         ).partial_eval(lang)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/rows_op.py` & `jx-python-4.582.24095/jx_base/expressions/rows_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/script_op.py` & `jx-python-4.582.24095/jx_base/expressions/script_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/select_op.py` & `jx-python-4.582.24095/jx_base/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/split_op.py` & `jx-python-4.582.24095/jx_base/expressions/split_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_alias_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_alias_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_and_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_and_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_cast_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_cast_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_concat_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_eq_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_group_by_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_group_by_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_instr_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_instr_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_is_null_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_is_null_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_left_joins_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_left_joins_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_not_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_not_op.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def missing(self, lang):
         return FALSE
 
     def invert(self, lang):
         return (
             WhenOp(
-                OrOp(self.term.missing(lang), BasicEqOp(self.term, ZERO)),
+                OrOp(self.term.missing(lang), StrictEqOp(self.term, ZERO)),
                 *{"then": self, "else": ToBoolean(self.term)}
             )
             .term
             .partial_eval(lang)
         )
 
     def partial_eval(self, lang):
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_or_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_or_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_order_by_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_order_by_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_origins_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_origins_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_select_all_from_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_select_all_from_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_select_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_substr_op.py` & `jx-python-4.582.24095/jx_base/expressions/sql_substr_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sql_variable.py` & `jx-python-4.582.24095/jx_base/expressions/sql_variable.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sub_op.py` & `jx-python-4.582.24095/jx_base/expressions/sub_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/suffix_op.py` & `jx-python-4.582.24095/jx_base/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/sum_op.py` & `jx-python-4.582.24095/jx_base/expressions/sum_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/tally_op.py` & `jx-python-4.582.24095/jx_base/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/to_array_op.py` & `jx-python-4.582.24095/jx_base/expressions/to_array_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/to_boolean_op.py` & `jx-python-4.582.24095/jx_base/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/to_integer_op.py` & `jx-python-4.582.24095/jx_base/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/to_number_op.py` & `jx-python-4.582.24095/jx_base/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/to_text_op.py` & `jx-python-4.582.24095/jx_base/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/to_value_op.py` & `jx-python-4.582.24095/jx_base/expressions/to_value_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/true_op.py` & `jx-python-4.582.24095/jx_base/expressions/true_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/tuple_op.py` & `jx-python-4.582.24095/jx_base/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/union_op.py` & `jx-python-4.582.24095/jx_base/expressions/union_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/unix_op.py` & `jx-python-4.582.24095/jx_base/expressions/unix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/expressions/variable.py` & `jx-python-4.582.24095/jx_base/expressions/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,10 +182,10 @@
 ROW = Variable("row")
 
 
 export("jx_base.expressions._utils", Variable)
 export("jx_base.expressions.expression", Variable)
 export("jx_base.expressions.base_binary_op", Variable)
 export("jx_base.expressions.base_binary_op", is_variable)
-export("jx_base.expressions.basic_in_op", Variable)
-export("jx_base.expressions.basic_in_op", is_variable)
+export("jx_base.expressions.strict_in_op", Variable)
+export("jx_base.expressions.strict_in_op", is_variable)
 export("jx_base.expressions.from_op", Variable)
```

### Comparing `jx-python-4.579.24081/jx_base/expressions/when_op.py` & `jx-python-4.582.24095/jx_base/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/language.py` & `jx-python-4.582.24095/jx_base/language.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/meta_columns.py` & `jx-python-4.582.24095/jx_base/meta_columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,40 +9,41 @@
 #
 
 
 import datetime
 from dataclasses import dataclass
 from typing import List, Optional
 
+from jx_base.expressions.variable import QueryOp
 from mo_dots.datas import register_data
 
 from jx_base.expressions._utils import JX, _jx_expression as jx_expression
 from jx_base.models.namespace import Namespace
 from jx_base.models.schema import Schema
 from jx_base.models.snowflake import Snowflake
 from mo_collections import UniqueIndex
 from mo_dots import (
     Data,
     FlatList,
     NullType,
     concat_field,
     to_data,
     is_many,
-    is_missing, relative_field, last,
+    is_missing, relative_field, last, endswith_field, join_field, split_field,
 )
-from mo_future import Mapping
+from mo_future import Mapping, first
 from mo_future import binary_type, items, long, none_type, text
 from mo_imports import export
 from mo_json import (
     INTEGER,
     NUMBER,
     STRING,
     OBJECT,
     EXISTS,
-    ARRAY, python_type_to_json_type, ARRAY_KEY,
+    ARRAY, python_type_to_json_type, ARRAY_KEY, jx_type_to_json_type,
 )
 from mo_json.typed_encoder import EXISTS_KEY
 from mo_logs import logger
 from mo_times.dates import Date
 
 _get = object.__getattribute__
 _set = object.__setattr__
@@ -193,20 +194,56 @@
 
     def __bool__(self):
         return True
 
 register_data(Column)
 
 
+def get_schema_from_jx_type(table_name, jx_type):
+    """
+    ASSUME THE VALUES DO NOT HAVE TYPED PROPERTIES
+    :param table_name:
+    :param jx_type:
+    :return:
+    """
+    paths, columns = _get_columns_from_jx_type([table_name], jx_type)
+    schema = Schema([table_name], Snowflake(None, paths, columns))
+    schema.snowflake.namespace = schema.snowflake
+    return schema
+
+def _get_columns_from_jx_type(nested_path, jx_type):
+    paths = [nested_path[0]]
+    columns = []
+    for path, type in jx_type.leaves():
+        if endswith_field(path, ARRAY_KEY):
+            child = concat_field(nested_path[0], join_field(split_field(path)[:-1]))
+            more_paths, more_columns = _get_columns_from_jx_type([child, *nested_path], type)
+            paths = [*paths, *more_paths]
+            columns.extend(more_columns)
+            continue
+        name = concat_field(relative_field(nested_path[0], nested_path[-1]), path)
+        columns.append(Column(
+            name=name,  # ABS NAME OF COLUMN
+            es_column=name,
+            es_index=nested_path[0],
+            es_type=type,
+            json_type=jx_type_to_json_type(type),
+            nested_path=nested_path,
+            multi=1,
+            last_updated=Date.now()
+        ))
+    return paths, columns
+
 def get_schema_from_list(table_name, frum, native_type_to_json_type=python_type_to_json_type):
     """
     SCAN THE LIST FOR COLUMN TYPES
     """
     columns = UniqueIndex(keys=("es_column",))
-    snowflake = Snowflake(Namespace(), [table_name], columns)
+    snowflake = Snowflake(None, [table_name], columns)
+    snowflake.namespace = snowflake
 
     _get_schema_from_list(
         frum,
         prefix=".",
         nested_path=[table_name],
         snowflake=snowflake,
         native_type_to_json_type=native_type_to_json_type,
@@ -458,10 +495,15 @@
 
     if isinstance(output, str):
         return output
     else:
         return output.__name__
 
 
+def query_metadata(container, query):
+    container = container.namespace.columns.denormalized()
+    normalized = QueryOp.wrap(query, container, JX)
+    return container.query(normalized)
+
 export("jx_base.expressions.query_op", Column)
 export("jx_python.containers.list", Column)
 export("jx_python.containers.list", get_schema_from_list)
```

### Comparing `jx-python-4.579.24081/jx_base/models/container.py` & `jx-python-4.582.24095/jx_base/models/container.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/models/dimensions.py` & `jx-python-4.582.24095/jx_base/models/dimensions.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/models/facts.py` & `jx-python-4.582.24095/jx_base/models/facts.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/models/namespace.py` & `jx-python-4.582.24095/jx_base/models/namespace.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/models/schema.py` & `jx-python-4.582.24095/jx_base/models/schema.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/models/snowflake.py` & `jx-python-4.582.24095/jx_base/models/snowflake.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/models/table.py` & `jx-python-4.582.24095/jx_base/models/table.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/queries.py` & `jx-python-4.582.24095/jx_base/queries.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_base/utils.py` & `jx-python-4.582.24095/jx_base/utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/__init__.py` & `jx-python-4.582.24095/jx_python/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/containers/cube.py` & `jx-python-4.582.24095/jx_python/containers/cube.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/containers/list.py` & `jx-python-4.582.24095/jx_python/containers/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 import itertools
 
+from jx_base.expressions._utils import jx_expression
+
 from jx_base.expressions import TRUE
 from jx_base.expressions.variable import is_variable
 from jx_base.language import is_expression
+from jx_base.meta_columns import get_schema_from_jx_type
 from jx_base.models.container import Container
 from jx_base.models.namespace import Namespace
 from jx_base.models.schema import Schema
 from jx_base.models.snowflake import Snowflake
 from jx_base.models.table import Table
 from jx_base.utils import delist, enlist
 from jx_python.convert import list2cube, list2table
 from jx_python.expressions import jx_expression_to_function
+from jx_python.expressions._utils import compile_expression, JXExpression
 from jx_python.lists.aggs import is_aggs, list_aggs
 from mo_collections import UniqueIndex
 from mo_dots import (
     Data,
     Null,
     is_data,
     is_list,
@@ -34,15 +38,15 @@
     coalesce,
     dict_to_data,
     last,
     startswith_field,
 )
 from mo_future import first, sort_using_key
 from mo_imports import export, expect
-from mo_json import ARRAY
+from mo_json import ARRAY, JX_IS_NULL, value_to_json_type, value_to_jx_type
 from mo_logs import Log
 from mo_threads import Lock
 
 jx, get_schema_from_list, Column = expect("jx", "get_schema_from_list", "Column")
 
 
 class ListContainer(Container, Namespace, Table):
@@ -52,14 +56,15 @@
     """
 
     def __init__(self, name, data, schema=None):
         # TODO: STORE THIS LIKE A CUBE FOR FASTER ACCESS AND TRANSFORMATION
         Container.__init__(self)
         self.name = name = coalesce(name, ".")
         self.data = data = list(from_data(data))
+        self.container = self
         self.schema = schema or get_schema_from_list(name, data)
         self.locker = Lock()  # JUST IN CASE YOU WANT TO DO MORE THAN ONE THING
 
     @property
     def nested_path(self):
         return [self.name]
 
@@ -97,54 +102,54 @@
 
     def last(self):
         """
         :return:  Last element in the list, or Null
         """
         last(self.data)
 
-    def query(self, q):
-        q = to_data(q)
+    def query(self, query: "QueryOp"):
+        query = to_data(query)
         output = self
-        if is_aggs(q):
-            output = list_aggs(output.data, q)
+        if is_aggs(query):
+            output = list_aggs(output.data, query)
         else:
-            if q.where is not TRUE:
-                output = output.where(q.where)
+            if query.where is not TRUE:
+                output = output.where(query.where)
 
-            if q.sort:
-                output = output.sort(q.sort)
+            if query.sort:
+                output = output.sort(query.sort)
 
-            if q.select:
-                output = output.select(q.select)
+            if query.select:
+                output = output.select(query.select)
 
         # TODO: ADD EXTRA COLUMN DESCRIPTIONS TO RESULTING SCHEMA
-        for param in q.window:
+        for param in query.window:
             output.window(param)
 
-        if q.format:
-            if q.format == "list":
+        if query.format:
+            if query.format == "list":
                 return Data(data=output.data, meta={"format": "list"})
-            elif q.format == "table":
-                head = [c.name for c in output.schema.columns]
+            elif query.format == "table":
+                head = [c.name for c in output.schema.snowflake.columns]
                 data = [[r if h == "." else r[h] for h in head] for r in output.data]
                 return Data(header=head, data=data, meta={"format": "table"})
-            elif q.format == "cube":
-                head = [c.name for c in output.schema.columns]
+            elif query.format == "cube":
+                head = [c.name for c in output.schema.snowflake.columns]
                 rows = [[r[h] for h in head] for r in output.data]
                 data = {h: c for h, c in zip(head, zip(*rows))}
                 return Data(
                     data=data,
                     meta={"format": "cube"},
                     edges=[{
                         "name": "rownum",
                         "domain": {"type": "rownum", "min": 0, "max": len(rows), "interval": 1},
                     }],
                 )
             else:
-                Log.error("unknown format {{format}}", format=q.format)
+                Log.error("unknown format {{format}}", format=query.format)
         else:
             return output
 
     def update(self, command):
         """
         EXPECTING command == {"set":term, "clear":term, "where":where}
         THE set CLAUSE IS A DICT MAPPING NAMES TO VALUES
@@ -182,52 +187,32 @@
         """
         if is_list(select):
             return [(d[s] for s in select) for d in self.data]
         else:
             return [d[select] for d in self.data]
 
     def select(self, select):
-        selects = enlist(select)
-
-        if len(selects) == 1 and is_variable(selects[0].value) and selects[0].value.var == ".":
-            new_schema = self.schema
-            if selects[0].name == ".":
-                return self
-        else:
-            new_schema = None
-
-        if is_list(select):
-            if all(is_variable(s.value) and s.name == s.value.var for s in select):
-                names = set(s.value.var for s in select)
-                new_schema = Schema(".", [c for c in self.schema.columns if c.name in names])
-
-            push_and_pull = [(s.name, jx_expression_to_function(s.value)) for s in selects]
-
-            def selector(d):
-                output = Data()
-                for n, p in push_and_pull:
-                    output[n] = delist(p(to_data(d)))
-                return from_data(output)
-
-            new_data = list(map(selector, self.data))
-        else:
-            select_value = jx_expression_to_function(select.value)
-            new_data = list(map(select_value, self.data))
-            if is_variable(select.value):
-                column = dict(**first(c for c in self.schema.columns if c.name == select.value.var))
-                column.update({
-                    "name": ".",
-                    "json_type": ARRAY,
-                    "es_type": "nested",
-                    "multi": 1001,
-                    "cardinality": 1,
-                })
-                new_schema = Schema("from " + self.name, [Column(**column)])
-
-        return ListContainer("from " + self.name, data=new_data, schema=new_schema)
+        selects= select.terms
+        if len(selects) == 1 and is_variable(selects[0].value) and selects[0].value.var == "." and selects[0].name == ".":
+            return self
+
+        exprs = [jx_expression(s.value) for s in selects]
+        jx_type = JX_IS_NULL
+        new_data = []
+        for row in self.data:
+            result = Data()
+            for s, e in zip(selects, exprs):
+                value = e(row)
+                result[s.name] = e(row)
+                jx_type = jx_type | s.name+value_to_jx_type(value)
+            new_data.append(from_data(result))
+
+        new_name = f"from {self.name}"
+        new_schema = get_schema_from_jx_type(new_name, jx_type)
+        return ListContainer(new_name, data=new_data, schema=new_schema)
 
     def window(self, window):
         # _ = window
         jx.window(self.data, window)
         return self
 
     def format(self, format):
```

### Comparing `jx-python-4.579.24081/jx_python/convert.py` & `jx-python-4.582.24095/jx_python/convert.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/cubes/aggs.py` & `jx-python-4.582.24095/jx_python/cubes/aggs.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expression_compiler.py` & `jx-python-4.582.24095/jx_python/expression_compiler.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expression_factory.py` & `jx-python-4.582.24095/jx_python/expression_factory.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/__init__.py` & `jx-python-4.582.24095/jx_python/expressions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from jx_python.expressions._utils import jx_expression_to_function, Python
 from jx_python.expressions.add_op import AddOp
 from jx_python.expressions.and_op import AndOp
 from jx_python.expressions.array_of_op import ArrayOfOp
-from jx_python.expressions.basic_add_op import BasicAddOp
-from jx_python.expressions.basic_eq_op import BasicEqOp
-from jx_python.expressions.basic_index_of_op import BasicIndexOfOp
-from jx_python.expressions.basic_starts_with_op import BasicStartsWithOp
-from jx_python.expressions.basic_substring_op import BasicSubstringOp
 from jx_python.expressions.between_op import BetweenOp
 from jx_python.expressions.call_op import CallOp
 from jx_python.expressions.case_op import CaseOp
 from jx_python.expressions.coalesce_op import CoalesceOp
 from jx_python.expressions.concat_op import ConcatOp
 from jx_python.expressions.count_op import CountOp
 from jx_python.expressions.date_op import DateOp
@@ -56,14 +51,19 @@
 from jx_python.expressions.range_op import RangeOp
 from jx_python.expressions.reg_exp_op import RegExpOp
 from jx_python.expressions.right_op import RightOp
 from jx_python.expressions.rows_op import RowsOp
 from jx_python.expressions.script_op import ScriptOp
 from jx_python.expressions.select_op import SelectOp
 from jx_python.expressions.split_op import SplitOp
+from jx_python.expressions.strict_add_op import StrictAddOp
+from jx_python.expressions.strict_eq_op import StrictEqOp
+from jx_python.expressions.strict_index_of_op import StrictIndexOfOp
+from jx_python.expressions.strict_starts_with_op import StrictStartsWithOp
+from jx_python.expressions.strict_substring_op import StrictSubstringOp
 from jx_python.expressions.sub_op import SubOp
 from jx_python.expressions.suffix_op import SuffixOp
 from jx_python.expressions.sum_op import SumOp
 from jx_python.expressions.to_array_op import ToArrayOp
 from jx_python.expressions.to_boolean_op import ToBooleanOp
 from jx_python.expressions.to_integer_op import ToIntegerOp
 from jx_python.expressions.to_number_op import ToNumberOp
```

### Comparing `jx-python-4.579.24081/jx_python/expressions/_utils.py` & `jx-python-4.582.24095/jx_python/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/and_op.py` & `jx-python-4.582.24095/jx_python/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/array_of_op.py` & `jx-python-4.582.24095/jx_python/expressions/array_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/avg_op.py` & `jx-python-4.582.24095/jx_python/expressions/avg_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/basic_add_op.py` & `jx-python-4.582.24095/jx_python/expressions/basic_add_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/basic_eq_op.py` & `jx-python-4.582.24095/jx_python/expressions/basic_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/basic_index_of_op.py` & `jx-python-4.582.24095/jx_python/expressions/basic_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/basic_starts_with_op.py` & `jx-python-4.582.24095/jx_python/expressions/basic_starts_with_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/basic_substring_op.py` & `jx-python-4.582.24095/jx_python/expressions/basic_substring_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/call_op.py` & `jx-python-4.582.24095/jx_python/expressions/call_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/cardinality_op.py` & `jx-python-4.582.24095/jx_python/expressions/cardinality_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/case_op.py` & `jx-python-4.582.24095/jx_python/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/coalesce_op.py` & `jx-python-4.582.24095/jx_python/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/concat_op.py` & `jx-python-4.582.24095/jx_python/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/count_op.py` & `jx-python-4.582.24095/jx_python/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/date_op.py` & `jx-python-4.582.24095/jx_python/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/eq_op.py` & `jx-python-4.582.24095/jx_python/expressions/eq_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 from jx_base.expressions import EqOp as _EqOp, is_literal, FALSE, TRUE, ToArrayOp
 from jx_base.expressions.python_script import PythonScript
 from jx_base.language import value_compare
 from jx_python.expressions import Python
-from jx_python.expressions.basic_eq_op import BasicEqOp
+from jx_python.expressions.strict_eq_op import StrictEqOp
 from jx_python.expressions.case_op import CaseOp
 from jx_python.expressions.when_op import WhenOp
 from jx_python.utils import merge_locals
 from mo_json import JX_BOOLEAN
 
 
 class EqOp(_EqOp):
@@ -37,9 +37,9 @@
 
         if is_literal(lhs) and is_literal(rhs):
             return FALSE if value_compare(lhs.value, rhs.value) else TRUE
         else:
             return CaseOp(
                 WhenOp(lhs.missing(lang), then=rhs.missing(lang)),
                 WhenOp(rhs.missing(lang), then=FALSE),
-                BasicEqOp(lhs, rhs),
+                StrictEqOp(lhs, rhs),
             ).partial_eval(lang)
```

### Comparing `jx-python-4.579.24081/jx_python/expressions/exists_op.py` & `jx-python-4.582.24095/jx_python/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/false_op.py` & `jx-python-4.582.24095/jx_python/expressions/false_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/filter_op.py` & `jx-python-4.582.24095/jx_python/expressions/filter_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/find_op.py` & `jx-python-4.582.24095/jx_python/expressions/find_op.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 from jx_python.expressions.literal import Literal
 from jx_python.utils import merge_locals
 from mo_json import JX_INTEGER
 
 
 class FindOp(_FindOp):
     def partial_eval(self, lang):
-        index = lang.BasicIndexOfOp(self.value, self.find, self.start).partial_eval(lang)
+        index = lang.StrictIndexOfOp(self.value, self.find, self.start).partial_eval(lang)
 
         output = (
             lang
             .WhenOp(
-                lang.OrOp(self.value.missing(Python), self.find.missing(Python), lang.BasicEqOp(index, Literal(-1))),
+                lang.OrOp(self.value.missing(Python), self.find.missing(Python), lang.StrictEqOp(index, Literal(-1))),
                 **{"else": index},
             )
             .partial_eval(lang)
         )
         return output
 
     def missing(self, lang):
         output = (
             lang
             .OrOp(
                 self.value.missing(Python),
                 self.find.missing(Python),
-                lang.EqOp(lang.BasicIndexOfOp(self.value, self.find, self.start), Literal(-1)),
+                lang.EqOp(lang.StrictIndexOfOp(self.value, self.find, self.start), Literal(-1)),
             )
             .partial_eval(lang)
         )
         return output
 
     def to_python(self, loop_depth=0):
         value = self.value.to_python(loop_depth)
```

### Comparing `jx-python-4.579.24081/jx_python/expressions/first_op.py` & `jx-python-4.582.24095/jx_python/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/floor_op.py` & `jx-python-4.582.24095/jx_python/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/get_op.py` & `jx-python-4.582.24095/jx_python/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/group_op.py` & `jx-python-4.582.24095/jx_python/expressions/group_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/in_op.py` & `jx-python-4.582.24095/jx_python/expressions/in_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/is_text_op.py` & `jx-python-4.582.24095/jx_python/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/last_op.py` & `jx-python-4.582.24095/jx_python/expressions/last_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/least_op.py` & `jx-python-4.582.24095/jx_python/expressions/least_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/leaves_op.py` & `jx-python-4.582.24095/jx_python/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/length_op.py` & `jx-python-4.582.24095/jx_python/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/limit_op.py` & `jx-python-4.582.24095/jx_python/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/literal.py` & `jx-python-4.582.24095/jx_python/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/max_op.py` & `jx-python-4.582.24095/jx_python/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/min_op.py` & `jx-python-4.582.24095/jx_python/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/missing_op.py` & `jx-python-4.582.24095/jx_python/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/most_op.py` & `jx-python-4.582.24095/jx_python/expressions/most_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/mul_op.py` & `jx-python-4.582.24095/jx_python/expressions/mul_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/name_op.py` & `jx-python-4.582.24095/jx_python/expressions/name_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/ne_op.py` & `jx-python-4.582.24095/jx_python/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/not_left_op.py` & `jx-python-4.582.24095/jx_python/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/not_op.py` & `jx-python-4.582.24095/jx_python/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/not_right_op.py` & `jx-python-4.582.24095/jx_python/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/offset_op.py` & `jx-python-4.582.24095/jx_python/expressions/offset_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/or_op.py` & `jx-python-4.582.24095/jx_python/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/prefix_op.py` & `jx-python-4.582.24095/jx_python/expressions/prefix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/product_op.py` & `jx-python-4.582.24095/jx_python/expressions/product_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/python_function.py` & `jx-python-4.582.24095/jx_python/expressions/python_function.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/python_script.py` & `jx-python-4.582.24095/jx_python/expressions/python_script.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/reg_exp_op.py` & `jx-python-4.582.24095/jx_python/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/right_op.py` & `jx-python-4.582.24095/jx_python/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/rows_op.py` & `jx-python-4.582.24095/jx_python/expressions/rows_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/script_op.py` & `jx-python-4.582.24095/jx_python/expressions/script_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/select_op.py` & `jx-python-4.582.24095/jx_python/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/split_op.py` & `jx-python-4.582.24095/jx_python/expressions/split_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/suffix_op.py` & `jx-python-4.582.24095/jx_python/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/sum_op.py` & `jx-python-4.582.24095/jx_python/expressions/sum_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/tally_op.py` & `jx-python-4.582.24095/jx_python/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/to_array_op.py` & `jx-python-4.582.24095/jx_python/expressions/to_array_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/to_boolean_op.py` & `jx-python-4.582.24095/jx_python/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/to_integer_op.py` & `jx-python-4.582.24095/jx_python/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/to_number_op.py` & `jx-python-4.582.24095/jx_python/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/to_text_op.py` & `jx-python-4.582.24095/jx_python/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/to_value_op.py` & `jx-python-4.582.24095/jx_python/expressions/to_value_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/true_op.py` & `jx-python-4.582.24095/jx_python/expressions/true_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/tuple_op.py` & `jx-python-4.582.24095/jx_python/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/variable.py` & `jx-python-4.582.24095/jx_python/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/expressions/when_op.py` & `jx-python-4.582.24095/jx_python/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/flat_list.py` & `jx-python-4.582.24095/jx_python/flat_list.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/group_by.py` & `jx-python-4.582.24095/jx_python/group_by.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/jx.py` & `jx-python-4.582.24095/jx_python/jx.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/lists/aggs.py` & `jx-python-4.582.24095/jx_python/lists/aggs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 import itertools
 
 from jx_base.domains import DefaultDomain, SimpleSetDomain
+from jx_base.expressions.literal import NULL
 from jx_python import windows
 from jx_python.expressions import jx_expression_to_function
 from mo_collections.matrix import Matrix
 from mo_dots import to_data
 from jx_base.utils import coalesce, enlist
 from mo_logs import Log
 from mo_math import UNION
 from mo_times.dates import Date
 
 _ = Date
 
 
 def is_aggs(query):
-    if query.edges or query.groupby or any(a != None and a != "none" for a in enlist(query.select).aggregate):
+    if query.edges or query.groupby or any(s.aggregate is not NULL for s in query.select.terms):
         return True
     return False
 
 
 def list_aggs(frum, query):
     frum = to_data(frum)
     select = enlist(query.select)
```

### Comparing `jx-python-4.579.24081/jx_python/namespace/normal.py` & `jx-python-4.582.24095/jx_python/namespace/normal.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/records.py` & `jx-python-4.582.24095/jx_python/records.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams/__init__.py` & `jx-python-4.582.24095/jx_python/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams/expression_compiler.py` & `jx-python-4.582.24095/jx_python/streams/expression_compiler.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams/expression_factory.py` & `jx-python-4.582.24095/jx_python/streams/expression_factory.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams/inspects.py` & `jx-python-4.582.24095/jx_python/streams/inspects.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams/type_parser.py` & `jx-python-4.582.24095/jx_python/streams/type_parser.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams/typers.py` & `jx-python-4.582.24095/jx_python/streams/typers.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/streams.py` & `jx-python-4.582.24095/jx_python/streams.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/table.py` & `jx-python-4.582.24095/jx_python/table.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/utils.py` & `jx-python-4.582.24095/jx_python/utils.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python/windows.py` & `jx-python-4.582.24095/jx_python/windows.py`

 * *Files identical despite different names*

### Comparing `jx-python-4.579.24081/jx_python.egg-info/PKG-INFO` & `jx-python-4.582.24095/jx_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-python
-Version: 4.579.24081
+Version: 4.582.24095
 Summary: JSON query expressions using Python
 Home-page: https://github.com/klahnakoski/jx-python
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,24 +12,24 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.579.24081
-Requires-Dist: mo-dots==9.578.24081
+Requires-Dist: mo-collections==5.582.24095
+Requires-Dist: mo-dots==9.582.24095
 Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-json==6.579.24081
-Requires-Dist: mo-json-config==4.579.24081
-Requires-Dist: mo-kwargs==7.578.24081
-Requires-Dist: mo-logs==8.579.24081
-Requires-Dist: mo-math==7.579.24081
-Requires-Dist: mo-threads==6.579.24081
-Requires-Dist: mo-times==5.579.24081
+Requires-Dist: mo-json==6.582.24095
+Requires-Dist: mo-json-config==4.582.24095
+Requires-Dist: mo-kwargs==7.582.24095
+Requires-Dist: mo-logs==8.582.24095
+Requires-Dist: mo-math==7.582.24095
+Requires-Dist: mo-threads==6.582.24095
+Requires-Dist: mo-times==5.582.24095
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 
 # jx-python
 
 Python library for JSON Expressions
```

### Comparing `jx-python-4.579.24081/jx_python.egg-info/SOURCES.txt` & `jx-python-4.582.24095/jx_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -127,14 +127,24 @@
 jx_base/expressions/sql_order_by_op.py
 jx_base/expressions/sql_origins_op.py
 jx_base/expressions/sql_script.py
 jx_base/expressions/sql_select_all_from_op.py
 jx_base/expressions/sql_select_op.py
 jx_base/expressions/sql_substr_op.py
 jx_base/expressions/sql_variable.py
+jx_base/expressions/strict_add_op.py
+jx_base/expressions/strict_boolean_op.py
+jx_base/expressions/strict_eq_op.py
+jx_base/expressions/strict_in_op.py
+jx_base/expressions/strict_index_of_op.py
+jx_base/expressions/strict_mul_op.py
+jx_base/expressions/strict_multi_op.py
+jx_base/expressions/strict_not_op.py
+jx_base/expressions/strict_starts_with_op.py
+jx_base/expressions/strict_substring_op.py
 jx_base/expressions/sub_op.py
 jx_base/expressions/suffix_op.py
 jx_base/expressions/sum_op.py
 jx_base/expressions/tally_op.py
 jx_base/expressions/to_array_op.py
 jx_base/expressions/to_boolean_op.py
 jx_base/expressions/to_integer_op.py
@@ -243,14 +253,19 @@
 jx_python/expressions/range_op.py
 jx_python/expressions/reg_exp_op.py
 jx_python/expressions/right_op.py
 jx_python/expressions/rows_op.py
 jx_python/expressions/script_op.py
 jx_python/expressions/select_op.py
 jx_python/expressions/split_op.py
+jx_python/expressions/strict_add_op.py
+jx_python/expressions/strict_eq_op.py
+jx_python/expressions/strict_index_of_op.py
+jx_python/expressions/strict_starts_with_op.py
+jx_python/expressions/strict_substring_op.py
 jx_python/expressions/sub_op.py
 jx_python/expressions/suffix_op.py
 jx_python/expressions/sum_op.py
 jx_python/expressions/tally_op.py
 jx_python/expressions/to_array_op.py
 jx_python/expressions/to_boolean_op.py
 jx_python/expressions/to_integer_op.py
```

### Comparing `jx-python-4.579.24081/setup.py` & `jx-python-4.582.24095/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='JSON query expressions using Python',
     extras_require={"tests":["mo-testing>=7.562.24075"]},
     include_package_data=True,
-    install_requires=["mo-collections==5.579.24081","mo-dots==9.578.24081","mo-future==7.546.24057","mo-json==6.579.24081","mo-json-config==4.579.24081","mo-kwargs==7.578.24081","mo-logs==8.579.24081","mo-math==7.579.24081","mo-threads==6.579.24081","mo-times==5.579.24081"],
+    install_requires=["mo-collections==5.582.24095","mo-dots==9.582.24095","mo-future==7.546.24057","mo-json==6.582.24095","mo-json-config==4.582.24095","mo-kwargs==7.582.24095","mo-logs==8.582.24095","mo-math==7.582.24095","mo-threads==6.582.24095","mo-times==5.582.24095"],
     license='MPL 2.0',
     long_description='# jx-python\n\nPython library for JSON Expressions \n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-python.svg)](https://pypi.org/project/jx-python/)\n[![Build Status](https://github.com/klahnakoski/jx-python/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/jx-python/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/jx-python/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/jx-python?branch=dev)\n',
     long_description_content_type='text/markdown',
     name='jx-python',
     packages=["jx_base","jx_base.expressions","jx_base.models","jx_python.expressions","jx_python.containers","jx_python.cubes","jx_python.lists","jx_python.namespace","jx_python","jx_python.streams"],
     url='https://github.com/klahnakoski/jx-python',
-    version='4.579.24081'
+    version='4.582.24095'
 )
```

