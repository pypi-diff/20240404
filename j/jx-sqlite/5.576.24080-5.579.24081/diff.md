# Comparing `tmp/jx-sqlite-5.576.24080.tar.gz` & `tmp/jx-sqlite-5.579.24081.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx-sqlite-5.576.24080.tar", last modified: Wed Mar 20 02:28:01 2024, max compression
+gzip compressed data, was "jx-sqlite-5.579.24081.tar", last modified: Thu Mar 21 02:53:56 2024, max compression
```

## Comparing `jx-sqlite-5.576.24080.tar` & `jx-sqlite-5.579.24081.tar`

### file list

```diff
@@ -1,121 +1,118 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 02:28:01.394558 jx-sqlite-5.576.24080/
--rw-rw-rw-   0        0        0    16725 2017-02-23 13:51:40.000000 jx-sqlite-5.576.24080/LICENSE
--rw-rw-rw-   0        0        0     6234 2024-03-20 02:28:01.392482 jx-sqlite-5.576.24080/PKG-INFO
--rw-rw-rw-   0        0        0     4907 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/README.md
-drwxrwxrwx   0        0        0        0 2024-03-20 02:28:01.278511 jx-sqlite-5.576.24080/jx_sqlite/
--rw-rw-rw-   0        0        0      706 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/__init__.py
--rw-rw-rw-   0        0        0    30278 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/edges.py
-drwxrwxrwx   0        0        0        0 2024-03-20 02:28:01.375350 jx-sqlite-5.576.24080/jx_sqlite/expressions/
--rw-rw-rw-   0        0        0     3856 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/__init__.py
--rw-rw-rw-   0        0        0     4650 2024-03-20 02:09:03.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/_utils.py
--rw-rw-rw-   0        0        0      855 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/abs_op.py
--rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/add_op.py
--rw-rw-rw-   0        0        0       79 2024-02-02 03:46:38.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/aggregate_op.py
--rw-rw-rw-   0        0        0     1124 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/and_op.py
--rw-rw-rw-   0        0        0      472 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_add_op.py
--rw-rw-rw-   0        0        0      570 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_boolean_op.py
--rw-rw-rw-   0        0        0     1433 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_eq_op.py
--rw-rw-rw-   0        0        0     1745 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_in_op.py
--rw-rw-rw-   0        0        0     2013 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_index_of_op.py
--rw-rw-rw-   0        0        0      472 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_mul_op.py
--rw-rw-rw-   0        0        0      778 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_not_op.py
--rw-rw-rw-   0        0        0     1501 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_starts_with_op.py
--rw-rw-rw-   0        0        0     1066 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_substring_op.py
--rw-rw-rw-   0        0        0      550 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/between_op.py
--rw-rw-rw-   0        0        0     1299 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/case_op.py
--rw-rw-rw-   0        0        0      762 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     2228 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/concat_op.py
--rw-rw-rw-   0        0        0      710 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/count_op.py
--rw-rw-rw-   0        0        0      658 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/date_op.py
--rw-rw-rw-   0        0        0      566 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/default_op.py
--rw-rw-rw-   0        0        0     1037 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/div_op.py
--rw-rw-rw-   0        0        0     2955 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/eq_op.py
--rw-rw-rw-   0        0        0      721 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/exists_op.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/exp_op.py
--rw-rw-rw-   0        0        0      379 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/filter_op.py
--rw-rw-rw-   0        0        0     1781 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/find_op.py
--rw-rw-rw-   0        0        0      993 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/first_op.py
--rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/floor_op.py
--rw-rw-rw-   0        0        0      490 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/format_op.py
--rw-rw-rw-   0        0        0      641 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/from_unix_op.py
--rw-rw-rw-   0        0        0     2424 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/get_op.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/gt_op.py
--rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/gte_op.py
--rw-rw-rw-   0        0        0     1795 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/in_op.py
--rw-rw-rw-   0        0        0      929 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/is_boolean_op.py
--rw-rw-rw-   0        0        0      649 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/is_integer_op.py
--rw-rw-rw-   0        0        0      643 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/is_number_op.py
--rw-rw-rw-   0        0        0     1214 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/is_text_op.py
--rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/last_op.py
--rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/least_op.py
--rw-rw-rw-   0        0        0     1457 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/leaves_op.py
--rw-rw-rw-   0        0        0      922 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/left_op.py
--rw-rw-rw-   0        0        0     1254 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/length_op.py
--rw-rw-rw-   0        0        0      870 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/limit_op.py
--rw-rw-rw-   0        0        0      581 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/literal.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/lt_op.py
--rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/lte_op.py
--rw-rw-rw-   0        0        0      692 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/max_op.py
--rw-rw-rw-   0        0        0      672 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/min_op.py
--rw-rw-rw-   0        0        0     1385 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/missing_op.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/most_op.py
--rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/mul_op.py
--rw-rw-rw-   0        0        0      666 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/ne_op.py
--rw-rw-rw-   0        0        0      868 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/nested_op.py
--rw-rw-rw-   0        0        0     1149 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/not_left_op.py
--rw-rw-rw-   0        0        0      862 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/not_op.py
--rw-rw-rw-   0        0        0     1119 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/not_right_op.py
--rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/offset_op.py
--rw-rw-rw-   0        0        0     1020 2024-03-20 02:09:03.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/or_op.py
--rw-rw-rw-   0        0        0     1061 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/prefix_op.py
--rw-rw-rw-   0        0        0      373 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/range_op.py
--rw-rw-rw-   0        0        0      998 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0     1018 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/right_op.py
--rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/rows_op.py
--rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/script_op.py
--rw-rw-rw-   0        0        0     3123 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/select_op.py
--rw-rw-rw-   0        0        0     1550 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0     1225 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_left_joins_op.py
--rw-rw-rw-   0        0        0      654 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_origins_op.py
--rw-rw-rw-   0        0        0     3755 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_select_all_from_op.py
--rw-rw-rw-   0        0        0     1705 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0     1186 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sub_op.py
--rw-rw-rw-   0        0        0      905 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/suffix_op.py
--rw-rw-rw-   0        0        0      355 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/sum_op.py
--rw-rw-rw-   0        0        0      883 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/tally_op.py
--rw-rw-rw-   0        0        0      725 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0      831 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     1141 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/to_number_op.py
--rw-rw-rw-   0        0        0     2397 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/to_text_op.py
--rw-rw-rw-   0        0        0      794 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/tuple_op.py
--rw-rw-rw-   0        0        0      626 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/unix_op.py
--rw-rw-rw-   0        0        0     2710 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/variable.py
--rw-rw-rw-   0        0        0     1714 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/expressions/when_op.py
--rw-rw-rw-   0        0        0    10200 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/format.py
--rw-rw-rw-   0        0        0     6329 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/group.py
--rw-rw-rw-   0        0        0    17821 2024-03-20 02:09:03.000000 jx-sqlite-5.576.24080/jx_sqlite/insert.py
--rw-rw-rw-   0        0        0    18715 2024-03-17 23:46:53.000000 jx-sqlite-5.576.24080/jx_sqlite/meta_columns.py
-drwxrwxrwx   0        0        0        0 2024-03-20 02:28:01.375350 jx-sqlite-5.576.24080/jx_sqlite/models/
--rw-rw-rw-   0        0        0        0 2024-01-25 04:51:52.000000 jx-sqlite-5.576.24080/jx_sqlite/models/__init__.py
--rw-rw-rw-   0        0        0     7742 2024-03-17 23:46:53.000000 jx-sqlite-5.576.24080/jx_sqlite/models/container.py
--rw-rw-rw-   0        0        0      648 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/models/facts.py
--rw-rw-rw-   0        0        0     1764 2024-03-20 02:09:03.000000 jx-sqlite-5.576.24080/jx_sqlite/models/namespace.py
--rw-rw-rw-   0        0        0      285 2024-02-02 03:46:38.000000 jx-sqlite-5.576.24080/jx_sqlite/models/relation.py
--rw-rw-rw-   0        0        0     8222 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/models/schema.py
--rw-rw-rw-   0        0        0    12962 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/models/snowflake.py
--rw-rw-rw-   0        0        0     1207 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/models/table.py
--rw-rw-rw-   0        0        0     6725 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/query.py
--rw-rw-rw-   0        0        0    17005 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/setop.py
--rw-rw-rw-   0        0        0     7201 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/utils.py
--rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/jx_sqlite/window.py
-drwxrwxrwx   0        0        0        0 2024-03-20 02:28:01.391973 jx-sqlite-5.576.24080/jx_sqlite.egg-info/
--rw-rw-rw-   0        0        0     6234 2024-03-20 02:28:01.000000 jx-sqlite-5.576.24080/jx_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3661 2024-03-20 02:28:01.000000 jx-sqlite-5.576.24080/jx_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 02:28:01.000000 jx-sqlite-5.576.24080/jx_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-03-20 02:28:01.000000 jx-sqlite-5.576.24080/jx_sqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-20 02:28:01.000000 jx-sqlite-5.576.24080/jx_sqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-20 02:28:01.394558 jx-sqlite-5.576.24080/setup.cfg
--rw-rw-rw-   0        0        0     6281 2024-03-20 02:27:56.000000 jx-sqlite-5.576.24080/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 02:28:01.389863 jx-sqlite-5.576.24080/tests/
--rw-rw-rw-   0        0        0     6552 2024-03-18 02:59:49.000000 jx-sqlite-5.576.24080/tests/test_basic.py
--rw-rw-rw-   0        0        0     3889 2024-03-11 07:20:56.000000 jx-sqlite-5.576.24080/tests/test_leaves.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:53:56.272680 jx-sqlite-5.579.24081/
+-rw-rw-rw-   0        0        0    16725 2017-02-23 13:51:40.000000 jx-sqlite-5.579.24081/LICENSE
+-rw-rw-rw-   0        0        0     6234 2024-03-21 02:53:56.272680 jx-sqlite-5.579.24081/PKG-INFO
+-rw-rw-rw-   0        0        0     4907 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/README.md
+drwxrwxrwx   0        0        0        0 2024-03-21 02:53:56.156110 jx-sqlite-5.579.24081/jx_sqlite/
+-rw-rw-rw-   0        0        0      706 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/__init__.py
+-rw-rw-rw-   0        0        0    30278 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/edges.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:53:56.246005 jx-sqlite-5.579.24081/jx_sqlite/expressions/
+-rw-rw-rw-   0        0        0     3856 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4652 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/_utils.py
+-rw-rw-rw-   0        0        0      855 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/abs_op.py
+-rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/add_op.py
+-rw-rw-rw-   0        0        0       79 2024-02-02 03:46:38.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/aggregate_op.py
+-rw-rw-rw-   0        0        0     1124 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/and_op.py
+-rw-rw-rw-   0        0        0      472 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_add_op.py
+-rw-rw-rw-   0        0        0      570 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_boolean_op.py
+-rw-rw-rw-   0        0        0     1433 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_eq_op.py
+-rw-rw-rw-   0        0        0     1745 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_in_op.py
+-rw-rw-rw-   0        0        0     2013 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_index_of_op.py
+-rw-rw-rw-   0        0        0      472 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_mul_op.py
+-rw-rw-rw-   0        0        0      778 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_not_op.py
+-rw-rw-rw-   0        0        0     1501 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_starts_with_op.py
+-rw-rw-rw-   0        0        0     1066 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_substring_op.py
+-rw-rw-rw-   0        0        0      550 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1299 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/case_op.py
+-rw-rw-rw-   0        0        0      762 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     2228 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/concat_op.py
+-rw-rw-rw-   0        0        0      710 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/count_op.py
+-rw-rw-rw-   0        0        0      658 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/date_op.py
+-rw-rw-rw-   0        0        0      566 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/default_op.py
+-rw-rw-rw-   0        0        0     1037 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/div_op.py
+-rw-rw-rw-   0        0        0     2955 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      721 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/exp_op.py
+-rw-rw-rw-   0        0        0      379 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     1781 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/find_op.py
+-rw-rw-rw-   0        0        0      993 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/first_op.py
+-rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/floor_op.py
+-rw-rw-rw-   0        0        0      490 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/format_op.py
+-rw-rw-rw-   0        0        0      641 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/from_unix_op.py
+-rw-rw-rw-   0        0        0     2424 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/get_op.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/gte_op.py
+-rw-rw-rw-   0        0        0     1795 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/in_op.py
+-rw-rw-rw-   0        0        0      929 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/is_boolean_op.py
+-rw-rw-rw-   0        0        0      649 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/is_integer_op.py
+-rw-rw-rw-   0        0        0      643 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/is_number_op.py
+-rw-rw-rw-   0        0        0     1214 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/last_op.py
+-rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/least_op.py
+-rw-rw-rw-   0        0        0     1457 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0      922 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/left_op.py
+-rw-rw-rw-   0        0        0     1254 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/length_op.py
+-rw-rw-rw-   0        0        0      870 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/limit_op.py
+-rw-rw-rw-   0        0        0      581 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/literal.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      692 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/max_op.py
+-rw-rw-rw-   0        0        0      672 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1385 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/most_op.py
+-rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/mul_op.py
+-rw-rw-rw-   0        0        0      666 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/ne_op.py
+-rw-rw-rw-   0        0        0      868 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/nested_op.py
+-rw-rw-rw-   0        0        0     1149 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0      862 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/not_op.py
+-rw-rw-rw-   0        0        0     1119 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/offset_op.py
+-rw-rw-rw-   0        0        0     1025 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/or_op.py
+-rw-rw-rw-   0        0        0     1061 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/range_op.py
+-rw-rw-rw-   0        0        0      998 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0     1018 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/right_op.py
+-rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/rows_op.py
+-rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/script_op.py
+-rw-rw-rw-   0        0        0     3123 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/select_op.py
+-rw-rw-rw-   0        0        0     1550 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0     1225 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_left_joins_op.py
+-rw-rw-rw-   0        0        0      654 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_origins_op.py
+-rw-rw-rw-   0        0        0     3755 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_select_all_from_op.py
+-rw-rw-rw-   0        0        0     1705 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0     1186 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sub_op.py
+-rw-rw-rw-   0        0        0      905 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0      355 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/sum_op.py
+-rw-rw-rw-   0        0        0      883 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/tally_op.py
+-rw-rw-rw-   0        0        0      725 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0      831 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     1141 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0     2397 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0      794 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0      626 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/unix_op.py
+-rw-rw-rw-   0        0        0     2710 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/variable.py
+-rw-rw-rw-   0        0        0     1714 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/expressions/when_op.py
+-rw-rw-rw-   0        0        0    10200 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/format.py
+-rw-rw-rw-   0        0        0     6329 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/group.py
+-rw-rw-rw-   0        0        0    17987 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/insert.py
+-rw-rw-rw-   0        0        0    18964 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/meta_columns.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:53:56.269549 jx-sqlite-5.579.24081/jx_sqlite/models/
+-rw-rw-rw-   0        0        0        0 2024-01-25 04:51:52.000000 jx-sqlite-5.579.24081/jx_sqlite/models/__init__.py
+-rw-rw-rw-   0        0        0     7780 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/models/container.py
+-rw-rw-rw-   0        0        0      648 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/models/facts.py
+-rw-rw-rw-   0        0        0     1917 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/models/namespace.py
+-rw-rw-rw-   0        0        0      285 2024-02-02 03:46:38.000000 jx-sqlite-5.579.24081/jx_sqlite/models/relation.py
+-rw-rw-rw-   0        0        0     8222 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/models/schema.py
+-rw-rw-rw-   0        0        0    12948 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/models/snowflake.py
+-rw-rw-rw-   0        0        0     1207 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/models/table.py
+-rw-rw-rw-   0        0        0     6739 2024-03-21 02:53:47.000000 jx-sqlite-5.579.24081/jx_sqlite/query.py
+-rw-rw-rw-   0        0        0    17005 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/setop.py
+-rw-rw-rw-   0        0        0     7201 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/utils.py
+-rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx-sqlite-5.579.24081/jx_sqlite/window.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:53:56.271638 jx-sqlite-5.579.24081/jx_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     6234 2024-03-21 02:53:56.000000 jx-sqlite-5.579.24081/jx_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3620 2024-03-21 02:53:56.000000 jx-sqlite-5.579.24081/jx_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-21 02:53:56.000000 jx-sqlite-5.579.24081/jx_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-03-21 02:53:56.000000 jx-sqlite-5.579.24081/jx_sqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-21 02:53:56.000000 jx-sqlite-5.579.24081/jx_sqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-21 02:53:56.272680 jx-sqlite-5.579.24081/setup.cfg
+-rw-rw-rw-   0        0        0     6281 2024-03-21 02:53:51.000000 jx-sqlite-5.579.24081/setup.py
```

### Comparing `jx-sqlite-5.576.24080/LICENSE` & `jx-sqlite-5.579.24081/LICENSE`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/PKG-INFO` & `jx-sqlite-5.579.24081/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-sqlite
-Version: 5.576.24080
+Version: 5.579.24081
 Summary: JSON query expressions using SQLite
 Home-page: https://github.com/klahnakoski/jx-sqlite
 Author: Rohit Kumar, Kyle Lahnakoski
 Author-email: rohitkumar.a255@gmail.com, kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: jx-python==4.576.24080
-Requires-Dist: mo-sql==4.576.24080
-Requires-Dist: mo-sqlite==2.576.24080
+Requires-Dist: jx-python==4.579.24081
+Requires-Dist: mo-sql==4.579.24081
+Requires-Dist: mo-sqlite==2.579.24081
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 
 # jx-sqlite 
 
 JSON query expressions using SQLite
```

### Comparing `jx-sqlite-5.576.24080/README.md` & `jx-sqlite-5.579.24081/README.md`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/__init__.py` & `jx-sqlite-5.579.24081/jx_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/edges.py` & `jx-sqlite-5.579.24081/jx_sqlite/edges.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/__init__.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/_utils.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         return NULL.to_sql(schema)
 
     if self.decisive:
         miss = AndOp(*(t.missing(SQLang) for t in self.terms))
         temp = [SqlCoalesceOp(t, zero).partial_eval(SQLang).to_sql(schema).expr for t in self.terms]
         expr = iso(sign.join(sql_iso(t) for t in temp))
     else:
-        miss = OrOp(*(t.missing(SQLang) for t in self.terms), nulls=True)
+        miss = OrOp(*(t.missing(SQLang) for t in self.terms), nulls=False)
         expr = iso(sign.join(sql_iso(t.partial_eval(SQLang).to_sql(schema)) for t in self.terms))
 
     return SqlScript(jx_type=jx_type, expr=expr, frum=self, miss=miss, schema=schema)
 
 
 def with_var(var, expression, eval):
     """
@@ -99,15 +99,15 @@
 def basic_multiop_to_sql(self, schema, many=False):
     iso, op, identity, jx_type = _sql_operators[self.op.split("basic.")[1]]
     sql = iso(op.join(sql_iso(t.partial_eval(SQLang).to_sql(schema)) for t in self.terms))
     return SqlScript(jx_type=jx_type, frum=self, expr=sql, miss=FALSE, schema=schema,)  # basic operations are "strict"
 
 
 _sql_operators = {
-    # (operator, zero-array default value) PAIR
+    # (operator, zero-array default value) TUPLE
     "add": (sql_iso, SQL_PLUS, ZERO, JX_NUMBER),
     "sum": (sql_iso, SQL_PLUS, ZERO, JX_NUMBER),
     "mul": (sql_iso, SQL_STAR, ONE, JX_NUMBER),
     "sub": (sql_iso, SQL(" - "), None, JX_NUMBER),
     "div": (sql_iso, SQL_DIV, NULL, JX_NUMBER),
     "exp": (sql_iso, SQL(" ** "), NULL, JX_NUMBER),
     "mod": (sql_iso, SQL(" % "), NULL, JX_NUMBER),
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/abs_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/abs_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/and_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_boolean_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_eq_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_in_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_in_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_index_of_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_not_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_not_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_starts_with_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_starts_with_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/basic_substring_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/basic_substring_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/between_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/between_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/case_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/coalesce_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/concat_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/count_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/date_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/default_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/default_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/div_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/div_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/eq_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/eq_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/exists_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/find_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/first_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/floor_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/from_unix_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/from_unix_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/get_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/in_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/in_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/is_boolean_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/is_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/is_integer_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/is_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/is_number_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/is_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/is_text_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/leaves_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/left_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/left_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/length_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/limit_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/literal.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/max_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/min_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/missing_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/ne_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/nested_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/nested_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/not_left_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/not_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/not_right_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/or_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/or_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     def to_sql(self, schema) -> SqlScript:
         this = self.partial_eval(SQLang)
         if not is_op(this, OrOp):
             return this.to_sql(schema)
         return SqlScript(
             jx_type=JX_BOOLEAN,
             miss=FALSE,
-            expr=SqlOrOp(*(t.to_sql(schema) for t in self.terms)),
+            expr=SqlOrOp(*(t.to_sql(schema).expr for t in self.terms)),
             frum=self,
             schema=schema,
         )
 
 
 export("jx_sqlite.expressions._utils", OrOp)
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/prefix_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/prefix_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/reg_exp_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/right_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/select_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_group_by_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_group_by_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_left_joins_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_left_joins_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_origins_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_origins_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_select_all_from_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_select_all_from_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/sql_select_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/sub_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/sub_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/suffix_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/tally_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/to_boolean_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/to_integer_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/to_number_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/to_text_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/tuple_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/unix_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/unix_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/variable.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/expressions/when_op.py` & `jx-sqlite-5.579.24081/jx_sqlite/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/format.py` & `jx-sqlite-5.579.24081/jx_sqlite/format.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/group.py` & `jx-sqlite-5.579.24081/jx_sqlite/group.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/insert.py` & `jx-sqlite-5.579.24081/jx_sqlite/insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from_data,
     is_many,
     is_data,
     to_data,
     relative_field, exists,
 )
 from mo_future import text, first, extend
-from mo_json import STRUCT, ARRAY, OBJECT, value_to_json_type, get_if_type
+from mo_json import STRUCT, ARRAY, OBJECT, value_to_json_type, get_if_type, jx_type_to_json_type, base_type
 from mo_logs import logger
 from mo_sql.utils import json_type_to_sql_type_key
 from mo_sqlite import (
     SQL_AND,
     SQL_FROM,
     SQL_INNER_JOIN,
     SQL_NULL,
@@ -89,35 +89,38 @@
     # REJECT DEEP UPDATES
     touched_columns = command.set.keys() | clear_columns
     for c in self.schema.columns:
         if c.name in touched_columns and len(c.nested_path) > 1:
             logger.error("Deep update not supported")
 
     # ADD NEW COLUMNS
-    where = jx_expression(command.where) or TRUE
+    where = jx_expression(command.where) if command.where else TRUE
     _vars = where.vars()
     _map = {v: c.es_column for v in _vars for _, c in self.schema.leaves(v) if c.json_type not in STRUCT}
     where_sql = where.map(_map).to_sql(self.schema)
     new_columns = set(command.set.keys()) - set(c.name for c in self.schema.columns)
     for new_column_name in new_columns:
-        nested_value = command.set[new_column_name]
-        ctype = value_to_json_type(nested_value)
+        expr = jx_expression(command.set[new_column_name])
+        json_type = jx_type_to_json_type(expr.jx_type)
         column = Column(
             name=new_column_name,
-            json_type=ctype,
+            json_type=json_type,
             es_index=self.name,
-            es_type=json_type_to_sqlite_type(ctype),
-            es_column=typed_column(new_column_name, ctype),
+            es_type=json_type_to_sqlite_type[json_type],
+            es_column=typed_column(new_column_name, json_type_to_sql_type_key[json_type]),
+            nested_path=[self.name],
+            multi=1,
+            cardinality=1,
             last_updated=Date.now(),
         )
-        self.add_column(column)
+        self.snowflake._add_column(column)
 
     # UPDATE THE ARRAY VALUES
-    for nested_column_name, nested_value in command.set.items():
-        if value_to_json_type(nested_value) == "nested":
+    for nested_column_name, expr in command.set.items():
+        if value_to_json_type(expr) == "nested":
             nested_table_name = concat_field(self.name, nested_column_name)
             nested_table = nested_tables[nested_column_name]
             self_primary_key = sql_list(quote_column(c.es_column) for u in self.uid for c in self.columns[u])
             extra_key_name = UID + str(len(self.uid))
             extra_key = [e for e in nested_table.columns[extra_key_name]][0]
 
             sql_command = ConcatSQL(
@@ -143,19 +146,19 @@
                         for c in self.columns[u]
                     ),
                 ),
             )
             self.container.db.execute(sql_command)
 
             # INSERT NEW RECORDS
-            if not nested_value:
+            if not expr:
                 continue
 
             doc_collection = {}
-            for d in listwrap(nested_value):
+            for d in listwrap(expr):
                 nested_table.flatten(d, Data(), doc_collection, path=nested_column_name)
 
             prefix = ConcatSQL(
                 SQL_INSERT,
                 quote_column(nested_table.name),
                 sql_iso(sql_list(
                     [self_primary_key]
@@ -234,33 +237,33 @@
             # PROBABLY A DELETE AND INSERT
             logger.error("do not know how to handle")
 
     command = ConcatSQL(
         SQL_UPDATE,
         quote_column(self.name),
         SQL_SET,
-        sql_list(
-            [
-                ConcatSQL(quote_column(c.es_column), SQL_EQ, quote_value(get_if_type(v, c.json_type)),)
+        sql_list([
+            *(
+                ConcatSQL(quote_column(c.es_column), SQL_EQ, jx_expression(v).to_sql(self.schema))
                 for c in self.schema.columns
                 if c.json_type != ARRAY and len(c.nested_path) == 1
                 for v in [command.set[c.name]]
                 if v != None
-            ]
-            + [
+            ),
+            *(
                 ConcatSQL(quote_column(c.es_column), SQL_EQ, SQL_NULL)
                 for c in self.schema.columns
                 if (
                     c.name in clear_columns
                     and command.set[c.name] != None
                     and c.json_type != ARRAY
                     and len(c.nested_path) == 1
                 )
-            ]
-        ),
+            )
+        ]),
         SQL_WHERE,
         where_sql,
     )
 
     with self.container.db.transaction() as t:
         t.execute(command)
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/meta_columns.py` & `jx-sqlite-5.579.24081/jx_sqlite/meta_columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 # You can obtain one at http:# mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 from copy import copy
 
 import jx_base
-from jx_base import Schema, Table, Container, Column, Snowflake
+from jx_base import Schema, Container, Column, Snowflake
 from jx_base.meta_columns import (
     META_COLUMNS_DESC,
     META_COLUMNS_NAME,
     SIMPLE_METADATA_COLUMNS,
+    META_TABLES_NAME,
 )
 from jx_python import jx
+from jx_sqlite.models.table import Table
 from jx_sqlite.utils import untyped_column, untype_field
-from mo_dots import Data, Null, coalesce, is_data, is_list, startswith_field, unwraplist, wrap, list_to_data
+from mo_dots import Data, Null, coalesce, is_data, is_list, startswith_field, unwraplist, list_to_data, to_data
 from mo_future import first
 from mo_json import STRUCT, IS_NULL
 from mo_json.typed_encoder import detype
 from mo_logs import Log, logger
 from mo_sql.utils import sql_type_key_to_json_type, SQL_ARRAY_KEY
 from mo_threads import Queue, Lock
 from mo_times.dates import Date
@@ -50,15 +52,15 @@
         return output
 
     def __init__(self, db):
         with CACHE_LOCKER:
             if hasattr(self, "db"):
                 return
             self.db = db
-        Table.__init__(self, META_COLUMNS_NAME)
+        Table.__init__(self, [META_COLUMNS_NAME], self)
         self.data = {}  # MAP FROM fact_name TO (abs_column_name to COLUMNS)
         self.locker = Lock()
         self._schema = None
         self.dirty = False
         self.es_index = None
         self.last_load = Null
         self.todo = Queue("update columns to es")  # HOLD (action, column) PAIR, WHERE action in ['insert', 'update']
@@ -441,17 +443,21 @@
         return self._schema
 
     @property
     def namespace(self):
         return self
 
     def get_table(self, table_name):
-        if table_name != META_COLUMNS_NAME:
-            Log.error("this container has only the " + META_COLUMNS_NAME)
-        return self
+        if table_name in (META_TABLES_NAME, META_COLUMNS_NAME):
+            return Table([table_name], self)
+        Log.error("this container has only the " + META_COLUMNS_NAME)
+
+    def find_snowflake(self, fact_name):
+        if fact_name in (META_TABLES_NAME, META_COLUMNS_NAME):
+            return [fact_name]
 
     def get_columns(self, table_name):
         if table_name != META_COLUMNS_NAME:
             Log.error("this container has only the " + META_COLUMNS_NAME)
         return self._all_columns()
 
     def get_nested_path(self, table_name):
@@ -499,20 +505,20 @@
                 for c in cs
                 if c.json_type not in STRUCT  # and c.es_column != "_id"
             ]
 
         from jx_python.containers.list import ListContainer
 
         return ListContainer(
-            self.name, data=output, schema=jx_base.Schema(META_COLUMNS_NAME, SIMPLE_METADATA_COLUMNS),
+            self.name, data=output, schema=jx_base.Schema([META_COLUMNS_NAME], SIMPLE_METADATA_COLUMNS),
         )
 
 
 def doc_to_column(doc):
-    return Column(**wrap(detype(doc)))
+    return Column(**to_data(detype(doc)))
 
 
 def mark_as_deleted(col):
     col.count = 0
     col.cardinality = 0
     col.multi = 0
     col.partitions = None
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/models/container.py` & `jx-sqlite-5.579.24081/jx_sqlite/models/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     def drop(self, item):
         if isinstance(item, Facts):
             self.drop_facts(item.name)
         else:
             logger.error("do not know how to handle {item}", item=item)
 
     def drop_facts(self, fact_name):
-        paths = self.namespace.columns._snowflakes.get(fact_name)
+        paths = self.namespace.find_snowflake(fact_name)
         if paths:
             with self.db.transaction() as t:
                 for p in paths:
                     t.execute("DROP TABLE " + quote_column(p))
             self.namespace.columns.remove_table(fact_name)
 
     def get_or_create_facts(self, fact_name, uid=UID):
@@ -189,14 +189,16 @@
             command = sql_create(fact_name, {UID: "INTEGER PRIMARY KEY", GUID: "TEXT"}, unique=UID)
 
             with self.db.transaction() as t:
                 t.execute(command)
 
         return Facts(fact_name, self)
 
+    get_or_create_table = get_or_create_facts
+
     def get_table(self, table_name):
         nested_path = self.namespace.columns.get_nested_path(table_name)
         return Table(nested_path, self)
 
     def get_snowflake(self, table_name):
         fact_name = first(
             fact for fact, nps in self.namespace.columns._snowflakes.items() for np in nps if np[0] == table_name
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/models/facts.py` & `jx-sqlite-5.579.24081/jx_sqlite/models/facts.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/models/namespace.py` & `jx-sqlite-5.579.24081/jx_sqlite/models/namespace.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,16 +34,19 @@
 
     def rename_tables(self, name_map):
         output = object.__new__(Namespace)
         output.db = None
         output.columns = self.columns.rename_tables(name_map)
         return output
 
-
-
+    def find_snowflake(self, fact_name):
+        """
+        RETURN ALL PATHS IF EXISTS
+        """
+        return self.columns._snowflakes.get(fact_name)
 
     def get_facts(self, fact_name):
         snowflake = Snowflake(fact_name, self)
         return Facts(self, snowflake)
 
     def get_schema(self, fact_name):
         # TODO: HOW TO REDUCE RELATIONS TO JUST THIS TREE? (AVOID CYCLES)
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/models/schema.py` & `jx-sqlite-5.579.24081/jx_sqlite/models/schema.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/models/snowflake.py` & `jx-sqlite-5.579.24081/jx_sqlite/models/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 class Snowflake(jx_base.Snowflake):
     """
     MANAGE SINGLE HIERARCHY IN SQLITE DATABASE
     """
 
     def __init__(self, fact_name, namespace):
-        if not namespace.columns._snowflakes.get(fact_name):
+        if not namespace.find_snowflake(fact_name):
             Log.error("{name} does not exist", name=fact_name)
         self.fact_name = fact_name  # THE CENTRAL FACT TABLE
         self.namespace = namespace
 
     @property
     def query_paths(self):
         return self.namespace.columns.get_query_paths(self.fact_name)
@@ -301,15 +301,15 @@
             # NOTE: c HAS ALREADY BEEN MOVED TO active_columns
             all_columns.remove(c)
             c.es_column = new_es_column(c)
             c.nested_path = new_nested_path(c)
             all_columns.add(c)
 
     def add_table(self, nested_path):
-        query_paths = self.namespace.columns._snowflakes[self.fact_name]
+        query_paths = self.namespace.find_snowflake(self.fact_name)
         if nested_path in query_paths:
             Log.error("table exists")
         query_paths.append(nested_path[0])
         return Table(nested_path, self)
 
     @property
     def tables(self):
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/models/table.py` & `jx-sqlite-5.579.24081/jx_sqlite/models/table.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/query.py` & `jx-sqlite-5.579.24081/jx_sqlite/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,34 +150,35 @@
     if startswith_field(table_name, self.name):
         return Facts(table_name, self.container)
     Log.error("programmer error")
 
 
 @extend(Facts)
 def query_metadata(self, query):
-    frum, query["from"] = query["from"], self
-    columns = self.snowflake.columns
+    container = self.container.namespace.columns.denormalized()
+    query = QueryOp.wrap(query, container, JX)
 
-    query = QueryOp.wrap(query, self.container, JX)
     where = query.where
     table_name = None
     column_name = None
 
     if query.edges or query.groupby:
         raise Log.error("Aggregates(groupby or edge) are not supported")
 
     if where.op == "eq" and where.lhs.var == "table":
         table_name = mo_json.json2value(where.rhs.json)
     elif where.op == "eq" and where.lhs.var == "name":
         column_name = mo_json.json2value(where.rhs.json)
     else:
         raise Log.error('Only simple filters are expected like: "eq" on table and column name')
 
+
     tables = [concat_field(self.snowflake.fact_name, i) for i in self.tables.keys()]
 
+    columns = self.snowflake.columns
     metadata = []
     if columns[-1].es_column != GUID:
         columns.append(Column(
             name=GUID, json_type=STRING, es_column=GUID, es_index=self.snowflake.fact_name, nested_path=["."],
         ))
 
     for tname, table in zip(t, tables):
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/setop.py` & `jx-sqlite-5.579.24081/jx_sqlite/setop.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/utils.py` & `jx-sqlite-5.579.24081/jx_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite/window.py` & `jx-sqlite-5.579.24081/jx_sqlite/window.py`

 * *Files identical despite different names*

### Comparing `jx-sqlite-5.576.24080/jx_sqlite.egg-info/PKG-INFO` & `jx-sqlite-5.579.24081/jx_sqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-sqlite
-Version: 5.576.24080
+Version: 5.579.24081
 Summary: JSON query expressions using SQLite
 Home-page: https://github.com/klahnakoski/jx-sqlite
 Author: Rohit Kumar, Kyle Lahnakoski
 Author-email: rohitkumar.a255@gmail.com, kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: jx-python==4.576.24080
-Requires-Dist: mo-sql==4.576.24080
-Requires-Dist: mo-sqlite==2.576.24080
+Requires-Dist: jx-python==4.579.24081
+Requires-Dist: mo-sql==4.579.24081
+Requires-Dist: mo-sqlite==2.579.24081
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 
 # jx-sqlite 
 
 JSON query expressions using SQLite
```

### Comparing `jx-sqlite-5.576.24080/jx_sqlite.egg-info/SOURCES.txt` & `jx-sqlite-5.579.24081/jx_sqlite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -104,10 +104,8 @@
 jx_sqlite/models/__init__.py
 jx_sqlite/models/container.py
 jx_sqlite/models/facts.py
 jx_sqlite/models/namespace.py
 jx_sqlite/models/relation.py
 jx_sqlite/models/schema.py
 jx_sqlite/models/snowflake.py
-jx_sqlite/models/table.py
-tests/test_basic.py
-tests/test_leaves.py
+jx_sqlite/models/table.py
```

### Comparing `jx-sqlite-5.576.24080/setup.py` & `jx-sqlite-5.579.24081/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 setup(
     author='Rohit Kumar, Kyle Lahnakoski',
     author_email='rohitkumar.a255@gmail.com, kyle@lahnakoski.com',
     classifiers=["Development Status :: 3 - Alpha","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Topic :: Database","Topic :: Utilities","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='JSON query expressions using SQLite',
     extras_require={"tests":["mo-testing>=7.562.24075"]},
     include_package_data=True,
-    install_requires=["hjson","jx-python==4.576.24080","mo-sql==4.576.24080","mo-sqlite==2.576.24080","requests"],
+    install_requires=["hjson","jx-python==4.579.24081","mo-sql==4.579.24081","mo-sqlite==2.579.24081","requests"],
     license='MPL 2.0',
     long_description='# jx-sqlite \n\nJSON query expressions using SQLite\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/jx-sqlite/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/jx-sqlite.svg?branch=master)](https://travis-ci.com/github/klahnakoski/jx-sqlite)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/jx-sqlite/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/jx-sqlite?branch=dev)\n\n## Summary\n\nThis library will manage your database schema to store JSON documents. You get all the speed of a well-formed database schema without the schema migration headaches. \n\n\n## Status\n\nSignificant updates to the supporting libraries has broken this code.  It still works for the simple cases that require it\n\n**Jan 2024** - 118 of 334 tests ignored\n\n\n## Installation\n\n    pip install jx-sqlite\n\n## Code Example\n\nThe smoke test, found in the `tests` is a simple example of how to use this library.\n\n```python\nimport jx_sqlite\n\ntable = (\n    jx_sqlite\n    .Container(filename="my.db")\n    .get_or_create_facts("my_table")\n    .insert([{"os": "linux", "value": 42}])\n    .query({\n        "select": "os",\n        "where": {"gt": {"value": 0}}\n    })\n)\n```\n\n## More\n\nThis project is an attempt to store JSON documents in SQLite so that they are accessible via SQL. The hope is this will serve a basis for a general document-relational map (DRM), and leverage the database\'s query optimizer.\n`jx-sqlite` is responsible for expanding the schema dynamically as new JSON documents are encountered.  It also strives to ensure old queries against the new schema have the same meaning; the same results.\n\nThe most interesting, and most important feature is that we query nested object arrays as if they were just another table.  This is important for two reasons:\n\n1. Inner objects `{"a": {"b": 0}}` are a shortcut for nested arrays `{"a": [{"b": 0}]}`, plus\n2. Schemas can be expanded from one-to-one  to one-to-many `{"a": [{"b": 0}, {"b": 1}]}`.\n\n\n## Motivation\n\nJSON is a nice format to store data, and it has become quite prevalent. Unfortunately, databases do not handle it well, often a human is required to declare a schema that can hold the JSON before it can be queried. If we are not overwhelmed by the diversity of JSON now, we soon will be. There will be more JSON, of more different shapes, as the number of connected devices( and the information they generate) continues to increase.\n\n## Contributing\n\nContributions are always welcome! The best thing to do is find a failing test, and try to fix it.\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n    $ git clone https://github.com/klahnakoski/jx-sqlite\n    $ cd jx-sqlite\n\n### Running tests\n\nThere are over 300 tests used to confirm the expected behaviour: They test a variety of JSON forms, and the queries that can be performed on them. Most tests are further split into three different output formats ( list, table and cube).\n\nThe `requirements.lock` file is the last successful combination that passed all tests, despite the version conflicts.\n\n    python.exe -m pip install --no-deps -r tests\\requirements.lock\n\n\nLinux\n\n    export PYTHONPATH=.:vendor\n    python -m unittest discover -v -s tests\n\nWindows\n\n    set PYTHONPATH=.;vendor\n    python -m unittest discover -v -s tests\n\n\n### Technical Docs\n\n* [Json Query Expression](https://github.com/klahnakoski/ActiveData/blob/dev/docs/jx.md)\n* [Nomenclature](https://github.com/mozilla/jx-sqlite/blob/master/docs/Nomenclature.md)\n* [Snowflake](https://github.com/mozilla/jx-sqlite/blob/master/docs/Perspective.md)\n* [JSON in Database](https://github.com/mozilla/jx-sqlite/blob/master/docs/JSON%20in%20Database.md)\n* [The Future](https://github.com/mozilla/jx-sqlite/blob/master/docs/The%20Future.md)\n\n## License\n\nThis project is licensed under Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed with this file, You can obtain one at http://mozilla.org/MPL/2.0/.\n\n\n## History\n\n*Jan 2024* - Attempt to resurrect this project (118 of 334 tests ignored)\n\n*Sep 2018* - Upgrade libs, start refactoring to work with other libs\n\n*Dec 2017* - A number of tests were added, but they do not pass.\n\n*Sep 2017* - GSoC work completed, all but a few tests pass.\n \n\n## GSOC\n\nGood work by Rohit Kumar.  You may see the end result on [gsoc branch](https://github.com/klahnakoski/jx-sqlite/tree/gsoc).  Installation requires python2.7,  and will require some version fixing to get running.\n\nSee [the demonstration video](https://www.youtube.com/watch?v=0_YLzb7BegI&list=PLSE8ODhjZXja7K1hjZ01UTVDnGQdx5v5U&index=26&t=260s)\n\n\nWork done up to the deadline of GSoC\'17:\n\n* [Pull Requests](https://github.com/mozilla/jx-sqlite/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Arohit-rk)\n* [Commits](https://github.com/mozilla/jx-sqlite/commits?author=rohit-rk)\n\n\n\n',
     long_description_content_type='text/markdown',
     name='jx-sqlite',
     package_dir={},
     packages=["jx_sqlite","jx_sqlite.models","jx_sqlite.expressions"],
     url='https://github.com/klahnakoski/jx-sqlite',
-    version='5.576.24080'
+    version='5.579.24081'
 )
```

