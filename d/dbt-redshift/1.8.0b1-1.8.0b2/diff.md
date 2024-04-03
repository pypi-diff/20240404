# Comparing `tmp/dbt-redshift-1.8.0b1.tar.gz` & `tmp/dbt-redshift-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.8.0b1.tar", last modified: Sat Mar  2 03:00:01 2024, max compression
+gzip compressed data, was "dbt-redshift-1.8.0b2.tar", last modified: Wed Apr  3 23:44:24 2024, max compression
```

## Comparing `dbt-redshift-1.8.0b1.tar` & `dbt-redshift-1.8.0b2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.783007 dbt-redshift-1.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-02 03:00:01.783007 dbt-redshift-1.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.775006 dbt-redshift-1.8.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.771006 dbt-redshift-1.8.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.775006 dbt-redshift-1.8.0b1/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.775006 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/adapters/redshift/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.771006 dbt-redshift-1.8.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.775006 dbt-redshift-1.8.0b1/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/adapters.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/by_relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/by_schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/incremental_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/metadata/relation_last_modified.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.771006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/describe.sql
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/refresh.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/table/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.779006 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/view/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.783007 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:00:01.783007 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-02 03:00:01.000000 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-02 03:00:01.000000 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 03:00:01.000000 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 03:00:01.000000 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-02 03:00:01.000000 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-02 03:00:01.000000 dbt-redshift-1.8.0b1/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 03:00:01.783007 dbt-redshift-1.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-02 02:59:51.000000 dbt-redshift-1.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.839255 dbt-redshift-1.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-03 23:44:24.839255 dbt-redshift-1.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.827255 dbt-redshift-1.8.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.827255 dbt-redshift-1.8.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/adapters/redshift/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.827255 dbt-redshift-1.8.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/adapters.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/by_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/by_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.831255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/incremental_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.835255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.835255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/metadata/relation_last_modified.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.827255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.835255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/refresh.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.835255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/table/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.835255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/view/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.835255 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:44:24.839255 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-03 23:44:24.000000 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-03 23:44:24.000000 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:44:24.000000 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:44:24.000000 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 23:44:24.000000 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 23:44:24.000000 dbt-redshift-1.8.0b2/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:44:24.839255 dbt-redshift-1.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-03 23:44:13.000000 dbt-redshift-1.8.0b2/setup.py
```

### Comparing `dbt-redshift-1.8.0b1/LICENSE.md` & `dbt-redshift-1.8.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/PKG-INFO` & `dbt-redshift-1.8.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,16 +15,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: dbt-postgres~=1.8.0b1
-Requires-Dist: redshift-connector!=2.0.914,<=2.0.918,>=2.0.913
+Requires-Dist: dbt-postgres~=1.8.0b2
+Requires-Dist: redshift-connector!=2.0.914,<2.0.918,>=2.0.913
+Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: sqlparse<0.5,>=0.2.3
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0b1 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0b2 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: dbt-postgres~=1.8.0b1 Requires-Dist: redshift-
-connector!=2.0.914,<=2.0.918,>=2.0.913 Requires-Dist: sqlparse<0.5,>=0.2.3
-Requires-Dist: agate
+Dist: dbt-postgres~=1.8.0b2 Requires-Dist: redshift-
+connector!=2.0.914,<2.0.918,>=2.0.913 Requires-Dist: dbt-core>=1.8.0a1
+Requires-Dist: sqlparse<0.5,>=0.2.3 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.8.0b1/README.md` & `dbt-redshift-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from dbt.adapters.contracts.relation import RelationConfig
-from typing import Optional
+from typing import FrozenSet, Optional
 
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.relation_configs import (
     RelationConfigBase,
     RelationConfigChangeAction,
     RelationResults,
 )
@@ -26,24 +26,28 @@
 @dataclass(frozen=True, eq=False, repr=False)
 class RedshiftRelation(BaseRelation):
     include_policy = RedshiftIncludePolicy  # type: ignore
     quote_policy = RedshiftQuotePolicy  # type: ignore
     relation_configs = {
         RelationType.MaterializedView.value: RedshiftMaterializedViewConfig,
     }
-    renameable_relations = frozenset(
-        {
-            RelationType.View,
-            RelationType.Table,
-        }
+    renameable_relations: FrozenSet[RelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                RelationType.View,
+                RelationType.Table,
+            }
+        )
     )
-    replaceable_relations = frozenset(
-        {
-            RelationType.View,
-        }
+    replaceable_relations: FrozenSet[RelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                RelationType.View,
+            }
+        )
     )
 
     def __post_init__(self):
         # Check for length of Redshift table/view names.
         # Check self.type to exclude test relation identifiers
         if (
             self.identifier is not None
```

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/__init__.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/base.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/dist.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/dist.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/materialized_view.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/relation_configs/sort.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/relation_configs/sort.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/adapters/redshift/utility.py` & `dbt-redshift-1.8.0b2/dbt/adapters/redshift/utility.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/by_relation.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/by_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/by_schema.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/by_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/catalog/catalog.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/catalog/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/incremental_merge.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/incremental_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/seeds/helpers.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/table.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/materializations/view.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/metadata/relation_last_modified.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/metadata/relation_last_modified.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/alter.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/create.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/create.sql`

 * *Files 1% similar despite different names*

```diff
@@ -6,10 +6,10 @@
         backup {% if materialized_view.backup %}yes{% else %}no{% endif %}
         diststyle {{ materialized_view.dist.diststyle }}
         {% if materialized_view.dist.distkey %}distkey ({{ materialized_view.dist.distkey }}){% endif %}
         {% if materialized_view.sort.sortkey %}sortkey ({{ ','.join(materialized_view.sort.sortkey) }}){% endif %}
         auto refresh {% if materialized_view.autorefresh %}yes{% else %}no{% endif %}
     as (
         {{ materialized_view.query }}
-    );
+    )
 
 {% endmacro %}
```

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations/materialized_view/describe.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations/materialized_view/describe.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/relations.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.8.0b2/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.8.0b2/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.8.0b2/dbt_redshift.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,16 +15,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: dbt-postgres~=1.8.0b1
-Requires-Dist: redshift-connector!=2.0.914,<=2.0.918,>=2.0.913
+Requires-Dist: dbt-postgres~=1.8.0b2
+Requires-Dist: redshift-connector!=2.0.914,<2.0.918,>=2.0.913
+Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: sqlparse<0.5,>=0.2.3
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0b1 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0b2 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: dbt-postgres~=1.8.0b1 Requires-Dist: redshift-
-connector!=2.0.914,<=2.0.918,>=2.0.913 Requires-Dist: sqlparse<0.5,>=0.2.3
-Requires-Dist: agate
+Dist: dbt-postgres~=1.8.0b2 Requires-Dist: redshift-
+connector!=2.0.914,<2.0.918,>=2.0.913 Requires-Dist: dbt-core>=1.8.0a1
+Requires-Dist: sqlparse<0.5,>=0.2.3 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.8.0b1/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.8.0b2/dbt_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.8.0b1/setup.py` & `dbt-redshift-1.8.0b2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+import re
 import sys
 
 if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
     print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
@@ -32,32 +33,44 @@
     Pull the package version from the main package version file
     """
     attributes = {}
     exec(VERSION.read_text(), attributes)
     return attributes["version"]
 
 
+def _plugin_version_trim() -> str:
+    """
+    Pull the package version from the main package version file
+    """
+    attributes = {}
+    exec(VERSION.read_text(), attributes)
+    pattern = r"\+build\d+$"
+    return re.sub(pattern, "", attributes["version"])
+
+
 setup(
     name="dbt-redshift",
     version=_plugin_version(),
     description="The Redshift adapter plugin for dbt",
     long_description=README.read_text(),
     long_description_content_type="text/markdown",
     author="dbt Labs",
     author_email="info@dbtlabs.com",
     url="https://github.com/dbt-labs/dbt-redshift",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-common>=0.1.0a1,<2.0",
         "dbt-adapters>=0.1.0a1,<2.0",
-        f"dbt-postgres~={_plugin_version()}",
+        f"dbt-postgres~={_plugin_version_trim()}",
         # dbt-redshift depends deeply on this package. it does not follow SemVer, therefore there have been breaking changes in previous patch releases
         # Pin to the patch or minor version, and bump in each new minor version of dbt-redshift.
-        "redshift-connector<=2.0.918, >=2.0.913, !=2.0.914",
+        "redshift-connector<2.0.918,>=2.0.913,!=2.0.914",
+        # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
+        "dbt-core>=1.8.0a1",
         # installed via dbt-core but referenced directly; don't pin to avoid version conflicts with dbt-core
         "sqlparse>=0.2.3,<0.5",
         "agate",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

