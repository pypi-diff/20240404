# Comparing `tmp/oc_ocdm-8.0.1.tar.gz` & `tmp/oc_ocdm-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ocdm-8.0.1.tar", max compression
+gzip compressed data, was "oc_ocdm-8.0.2.tar", max compression
```

## Comparing `oc_ocdm-8.0.1.tar` & `oc_ocdm-8.0.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0      795 2022-12-17 20:42:56.942609 oc_ocdm-8.0.1/LICENSE.md
--rw-r--r--   0        0        0      932 2022-12-17 20:42:56.961650 oc_ocdm-8.0.1/oc_ocdm/__init__.py
--rw-r--r--   0        0        0     8012 2022-12-17 20:42:56.962157 oc_ocdm-8.0.1/oc_ocdm/abstract_entity.py
--rw-r--r--   0        0        0     2890 2022-12-17 20:42:56.962157 oc_ocdm-8.0.1/oc_ocdm/abstract_set.py
--rw-r--r--   0        0        0     1082 2022-12-17 20:42:56.962157 oc_ocdm-8.0.1/oc_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     6500 2024-03-19 17:28:42.852996 oc_ocdm-8.0.1/oc_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0    16948 2024-03-19 17:48:26.059008 oc_ocdm-8.0.1/oc_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0    12624 2024-03-17 19:35:01.946002 oc_ocdm-8.0.1/oc_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3676 2023-04-21 15:37:27.504273 oc_ocdm-8.0.1/oc_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     2647 2022-12-17 20:42:56.964164 oc_ocdm-8.0.1/oc_ocdm/decorators.py
--rw-r--r--   0        0        0      937 2022-12-17 20:42:56.964164 oc_ocdm-8.0.1/oc_ocdm/graph/__init__.py
--rw-r--r--   0        0        0      974 2022-12-17 20:42:56.964164 oc_ocdm-8.0.1/oc_ocdm/graph/entities/__init__.py
--rw-r--r--   0        0        0     1680 2022-12-17 20:42:56.965165 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     8436 2022-12-17 20:42:56.965165 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/agent_role.py
--rw-r--r--   0        0        0     9064 2022-12-17 20:42:56.966166 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
--rw-r--r--   0        0        0    49262 2023-12-20 13:48:38.105696 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
--rw-r--r--   0        0        0    16277 2024-03-19 17:26:56.609028 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/citation.py
--rw-r--r--   0        0        0    21579 2022-12-17 20:42:56.967166 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/discourse_element.py
--rw-r--r--   0        0        0     6313 2022-12-17 20:42:56.967166 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/pointer_list.py
--rw-r--r--   0        0        0     4907 2022-12-17 20:42:56.967166 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
--rw-r--r--   0        0        0    10131 2022-12-17 20:42:56.968163 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
--rw-r--r--   0        0        0    10359 2022-12-17 20:42:56.968163 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
--rw-r--r--   0        0        0     8831 2022-12-17 20:42:56.968163 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
--rw-r--r--   0        0        0     6582 2022-12-17 20:42:56.968163 oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic_entity.py
--rw-r--r--   0        0        0    20380 2023-11-09 16:42:41.366173 oc_ocdm-8.0.1/oc_ocdm/graph/entities/identifier.py
--rw-r--r--   0        0        0    15630 2023-11-09 16:42:41.367172 oc_ocdm-8.0.1/oc_ocdm/graph/graph_entity.py
--rw-r--r--   0        0        0    20240 2024-03-27 14:00:06.254485 oc_ocdm-8.0.1/oc_ocdm/graph/graph_set.py
--rw-r--r--   0        0        0      955 2022-12-17 20:42:56.970162 oc_ocdm-8.0.1/oc_ocdm/metadata/__init__.py
--rw-r--r--   0        0        0      959 2022-12-17 20:42:56.970162 oc_ocdm-8.0.1/oc_ocdm/metadata/entities/__init__.py
--rw-r--r--   0        0        0    19262 2022-12-17 20:42:56.970162 oc_ocdm-8.0.1/oc_ocdm/metadata/entities/dataset.py
--rw-r--r--   0        0        0    12483 2022-12-17 20:42:56.970162 oc_ocdm-8.0.1/oc_ocdm/metadata/entities/distribution.py
--rw-r--r--   0        0        0     7586 2022-12-17 20:42:56.971668 oc_ocdm-8.0.1/oc_ocdm/metadata/metadata_entity.py
--rw-r--r--   0        0        0     6549 2024-03-17 20:00:28.096994 oc_ocdm-8.0.1/oc_ocdm/metadata/metadata_set.py
--rw-r--r--   0        0        0      931 2022-12-17 20:42:56.972674 oc_ocdm-8.0.1/oc_ocdm/prov/__init__.py
--rw-r--r--   0        0        0      905 2022-12-17 20:42:56.972674 oc_ocdm-8.0.1/oc_ocdm/prov/entities/__init__.py
--rw-r--r--   0        0        0    13642 2022-12-17 21:15:23.993253 oc_ocdm-8.0.1/oc_ocdm/prov/entities/snapshot_entity.py
--rw-r--r--   0        0        0     3759 2023-01-26 14:48:48.975521 oc_ocdm-8.0.1/oc_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0    16895 2024-03-18 13:52:02.774526 oc_ocdm-8.0.1/oc_ocdm/prov/prov_set.py
--rw-r--r--   0        0        0    12065 2024-03-27 14:05:48.710473 oc_ocdm-8.0.1/oc_ocdm/reader.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.974673 oc_ocdm-8.0.1/oc_ocdm/resources/__init__.py
--rw-r--r--   0        0        0     1361 2022-12-17 20:42:56.975674 oc_ocdm-8.0.1/oc_ocdm/resources/querymap.txt
--rw-r--r--   0        0        0    22001 2023-04-21 15:22:51.680086 oc_ocdm-8.0.1/oc_ocdm/resources/shacle.ttl
--rw-r--r--   0        0        0    12513 2022-12-17 21:14:27.096784 oc_ocdm-8.0.1/oc_ocdm/resources/shexc.txt
--rw-r--r--   0        0        0    12611 2022-12-17 21:14:16.594827 oc_ocdm-8.0.1/oc_ocdm/resources/shexc_closed.txt
--rw-r--r--   0        0        0    16657 2024-03-19 21:45:03.486875 oc_ocdm-8.0.1/oc_ocdm/storer.py
--rw-r--r--   0        0        0     1354 2022-12-17 20:42:56.976673 oc_ocdm-8.0.1/oc_ocdm/support/__init__.py
--rw-r--r--   0        0        0     3539 2023-04-21 15:22:51.682087 oc_ocdm-8.0.1/oc_ocdm/support/query_utils.py
--rw-r--r--   0        0        0     2615 2022-12-17 20:42:56.977673 oc_ocdm-8.0.1/oc_ocdm/support/reporter.py
--rw-r--r--   0        0        0    15792 2024-03-27 14:16:32.566629 oc_ocdm-8.0.1/oc_ocdm/support/support.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.977673 oc_ocdm-8.0.1/oc_ocdm/test/__init__.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.978673 oc_ocdm-8.0.1/oc_ocdm/test/counter_handler/__init__.py
--rw-r--r--   0        0        0     8681 2022-12-17 20:42:56.978673 oc_ocdm-8.0.1/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
--rw-r--r--   0        0        0    11192 2022-12-17 20:42:56.978673 oc_ocdm-8.0.1/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
--rw-r--r--   0        0        0    69632 2024-03-27 14:19:49.056568 oc_ocdm-8.0.1/oc_ocdm/test/coverage/.coverage
--rw-r--r--   0        0        0      109 2022-12-17 20:42:56.980675 oc_ocdm-8.0.1/oc_ocdm/test/coverage/.coveragerc
--rw-r--r--   0        0        0      925 2024-03-14 13:55:07.972159 oc_ocdm-8.0.1/oc_ocdm/test/coverage/coverage.svg
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.980675 oc_ocdm-8.0.1/oc_ocdm/test/graph/__init__.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.981675 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/__init__.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.981675 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     2679 2022-12-17 20:42:56.982699 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
--rw-r--r--   0        0        0     2209 2022-12-17 20:42:56.982699 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
--rw-r--r--   0        0        0    12671 2022-12-17 20:42:56.983699 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
--rw-r--r--   0        0        0     6887 2024-03-19 17:26:44.224227 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
--rw-r--r--   0        0        0     4915 2022-12-17 20:42:56.983699 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
--rw-r--r--   0        0        0     1908 2022-12-17 20:42:56.983699 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
--rw-r--r--   0        0        0     1740 2022-12-17 20:42:56.984700 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
--rw-r--r--   0        0        0     2501 2022-12-17 20:42:56.984700 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
--rw-r--r--   0        0        0     2990 2022-12-17 20:42:56.984700 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
--rw-r--r--   0        0        0     2535 2022-12-17 20:42:56.984700 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
--rw-r--r--   0        0        0     2980 2022-12-17 20:42:56.985699 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
--rw-r--r--   0        0        0     8109 2023-04-21 15:22:51.693606 oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/test_identifier.py
--rw-r--r--   0        0        0      964 2022-12-17 20:42:56.986698 oc_ocdm-8.0.1/oc_ocdm/test/graph/test_graph_entity.py
--rw-r--r--   0        0        0     6675 2022-12-17 20:42:56.986698 oc_ocdm-8.0.1/oc_ocdm/test/graph/test_graph_set.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.987699 oc_ocdm-8.0.1/oc_ocdm/test/metadata/__init__.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.987699 oc_ocdm-8.0.1/oc_ocdm/test/metadata/entities/__init__.py
--rw-r--r--   0        0        0     4691 2022-12-17 20:42:56.987699 oc_ocdm-8.0.1/oc_ocdm/test/metadata/entities/test_dataset.py
--rw-r--r--   0        0        0     3601 2022-12-17 20:42:56.988700 oc_ocdm-8.0.1/oc_ocdm/test/metadata/entities/test_distribution.py
--rw-r--r--   0        0        0     2738 2022-12-17 20:42:56.988700 oc_ocdm-8.0.1/oc_ocdm/test/metadata/test_metadata_set.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.988700 oc_ocdm-8.0.1/oc_ocdm/test/prov/__init__.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.989699 oc_ocdm-8.0.1/oc_ocdm/test/prov/entities/__init__.py
--rw-r--r--   0        0        0     4248 2022-12-17 20:42:56.989699 oc_ocdm-8.0.1/oc_ocdm/test/prov/entities/test_snapshot_entity.py
--rw-r--r--   0        0        0    12288 2023-04-21 15:22:51.694606 oc_ocdm-8.0.1/oc_ocdm/test/prov/prov_counter.db
--rw-r--r--   0        0        0    13047 2024-03-17 19:48:39.670617 oc_ocdm-8.0.1/oc_ocdm/test/prov/test_prov_set.py
--rw-r--r--   0        0        0        0 2023-04-21 15:22:51.696604 oc_ocdm-8.0.1/oc_ocdm/test/reader/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-21 15:22:51.697605 oc_ocdm-8.0.1/oc_ocdm/test/reader/br.nt
--rw-r--r--   0        0        0     1902 2024-03-17 20:03:04.664111 oc_ocdm-8.0.1/oc_ocdm/test/reader/test_reader.py
--rw-r--r--   0        0        0      837 2023-04-21 15:22:51.698606 oc_ocdm-8.0.1/oc_ocdm/test/resources/__init__.py
--rw-r--r--   0        0        0     6627 2023-04-21 15:22:51.699608 oc_ocdm-8.0.1/oc_ocdm/test/resources/data.json
--rw-r--r--   0        0        0     6627 2023-04-21 15:22:51.699608 oc_ocdm-8.0.1/oc_ocdm/test/resources/data_reader.json
--rw-r--r--   0        0        0     6628 2023-04-21 15:22:51.701366 oc_ocdm-8.0.1/oc_ocdm/test/resources/data_reader_invalid.json
--rw-r--r--   0        0        0     3677 2024-03-27 14:16:45.783492 oc_ocdm-8.0.1/oc_ocdm/test/resources/test_shacle.py
--rw-r--r--   0        0        0      841 2024-03-19 17:52:28.736461 oc_ocdm-8.0.1/oc_ocdm/test/storer/__init__.py
--rw-r--r--   0        0        0    14942 2024-03-19 21:48:30.122504 oc_ocdm-8.0.1/oc_ocdm/test/storer/test_storer.py
--rw-r--r--   0        0        0      837 2022-12-17 20:42:56.990698 oc_ocdm-8.0.1/oc_ocdm/test/support/__init__.py
--rw-r--r--   0        0        0     5485 2023-01-26 14:03:18.904027 oc_ocdm-8.0.1/oc_ocdm/test/support/test_support.py
--rw-r--r--   0        0        0     1611 2024-03-27 14:20:13.109773 oc_ocdm-8.0.1/pyproject.toml
--rw-r--r--   0        0        0     5058 2023-12-06 13:56:17.051639 oc_ocdm-8.0.1/README.md
--rw-r--r--   0        0        0     6391 1970-01-01 00:00:00.000000 oc_ocdm-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-8.0.2/LICENSE.md
+-rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-8.0.2/oc_ocdm/__init__.py
+-rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-8.0.2/oc_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/abstract_set.py
+-rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     6500 2024-04-04 20:59:41.203116 oc_ocdm-8.0.2/oc_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0    16948 2024-04-04 20:59:41.204114 oc_ocdm-8.0.2/oc_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0    12624 2024-04-04 20:59:41.205118 oc_ocdm-8.0.2/oc_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3676 2023-06-08 09:32:26.643046 oc_ocdm-8.0.2/oc_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/decorators.py
+-rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/__init__.py
+-rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/agent_role.py
+-rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
+-rw-r--r--   0        0        0    49262 2023-06-15 09:24:33.053664 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
+-rw-r--r--   0        0        0    16277 2023-03-08 10:55:02.484160 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/citation.py
+-rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/discourse_element.py
+-rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/pointer_list.py
+-rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
+-rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
+-rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
+-rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
+-rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic_entity.py
+-rw-r--r--   0        0        0    20380 2023-09-15 20:24:11.894595 oc_ocdm-8.0.2/oc_ocdm/graph/entities/identifier.py
+-rw-r--r--   0        0        0    15630 2023-09-15 20:22:31.451351 oc_ocdm-8.0.2/oc_ocdm/graph/graph_entity.py
+-rw-r--r--   0        0        0    20240 2024-04-04 20:59:41.206113 oc_ocdm-8.0.2/oc_ocdm/graph/graph_set.py
+-rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/metadata/__init__.py
+-rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/metadata/entities/__init__.py
+-rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/metadata/entities/dataset.py
+-rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/metadata/entities/distribution.py
+-rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/metadata/metadata_entity.py
+-rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/metadata/metadata_set.py
+-rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-8.0.2/oc_ocdm/prov/entities/__init__.py
+-rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-8.0.2/oc_ocdm/prov/entities/snapshot_entity.py
+-rw-r--r--   0        0        0     3759 2023-03-08 15:28:49.049031 oc_ocdm-8.0.2/oc_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0    16895 2024-04-04 20:59:41.207114 oc_ocdm-8.0.2/oc_ocdm/prov/prov_set.py
+-rw-r--r--   0        0        0    12063 2024-04-04 21:05:53.727582 oc_ocdm-8.0.2/oc_ocdm/reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/resources/__init__.py
+-rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/resources/querymap.txt
+-rw-r--r--   0        0        0    22001 2023-03-01 17:12:50.977316 oc_ocdm-8.0.2/oc_ocdm/resources/shacle.ttl
+-rw-r--r--   0        0        0    12513 2023-09-12 19:18:40.048091 oc_ocdm-8.0.2/oc_ocdm/resources/shexc.txt
+-rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/resources/shexc_closed.txt
+-rw-r--r--   0        0        0    16796 2024-04-04 21:06:10.721806 oc_ocdm-8.0.2/oc_ocdm/storer.py
+-rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/support/__init__.py
+-rw-r--r--   0        0        0     3539 2023-03-05 18:46:51.846163 oc_ocdm-8.0.2/oc_ocdm/support/query_utils.py
+-rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/support/reporter.py
+-rw-r--r--   0        0        0    15792 2024-04-04 20:59:41.210113 oc_ocdm-8.0.2/oc_ocdm/support/support.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/counter_handler/__init__.py
+-rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
+-rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
+-rw-r--r--   0        0        0    69632 2024-04-04 20:59:41.211113 oc_ocdm-8.0.2/oc_ocdm/test/coverage/.coverage
+-rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/coverage/.coveragerc
+-rw-r--r--   0        0        0      925 2024-04-04 20:59:41.212113 oc_ocdm-8.0.2/oc_ocdm/test/coverage/coverage.svg
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
+-rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
+-rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
+-rw-r--r--   0        0        0     6887 2023-03-08 14:23:54.735495 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
+-rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
+-rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
+-rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
+-rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
+-rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
+-rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
+-rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
+-rw-r--r--   0        0        0     8109 2023-03-08 11:33:47.672369 oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/test_identifier.py
+-rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/graph/test_graph_entity.py
+-rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-8.0.2/oc_ocdm/test/graph/test_graph_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/metadata/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/metadata/entities/__init__.py
+-rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/metadata/entities/test_dataset.py
+-rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-8.0.2/oc_ocdm/test/metadata/entities/test_distribution.py
+-rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/metadata/test_metadata_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/prov/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/prov/entities/__init__.py
+-rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/prov/entities/test_snapshot_entity.py
+-rw-r--r--   0        0        0    12288 2023-03-08 15:11:17.576967 oc_ocdm-8.0.2/oc_ocdm/test/prov/prov_counter.db
+-rw-r--r--   0        0        0    13047 2024-04-04 20:59:41.213112 oc_ocdm-8.0.2/oc_ocdm/test/prov/test_prov_set.py
+-rw-r--r--   0        0        0        0 2023-03-05 14:27:05.796485 oc_ocdm-8.0.2/oc_ocdm/test/reader/__init__.py
+-rw-r--r--   0        0        0     2542 2023-03-05 17:46:14.507023 oc_ocdm-8.0.2/oc_ocdm/test/reader/br.nt
+-rw-r--r--   0        0        0     1902 2024-04-04 20:59:41.214113 oc_ocdm-8.0.2/oc_ocdm/test/reader/test_reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/resources/__init__.py
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-8.0.2/oc_ocdm/test/resources/data.json
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-8.0.2/oc_ocdm/test/resources/data_reader.json
+-rw-r--r--   0        0        0     6628 2023-03-03 13:05:35.809618 oc_ocdm-8.0.2/oc_ocdm/test/resources/data_reader_invalid.json
+-rw-r--r--   0        0        0     3677 2024-04-04 20:59:41.214113 oc_ocdm-8.0.2/oc_ocdm/test/resources/test_shacle.py
+-rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/storer/__init__.py
+-rw-r--r--   0        0        0    14942 2024-04-04 20:59:41.215113 oc_ocdm-8.0.2/oc_ocdm/test/storer/test_storer.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-8.0.2/oc_ocdm/test/support/__init__.py
+-rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-8.0.2/oc_ocdm/test/support/test_support.py
+-rw-r--r--   0        0        0     1611 2024-04-04 21:07:10.961409 oc_ocdm-8.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5058 2024-04-04 20:59:41.202119 oc_ocdm-8.0.2/README.md
+-rw-r--r--   0        0        0     6391 1970-01-01 00:00:00.000000 oc_ocdm-8.0.2/PKG-INFO
```

### Comparing `oc_ocdm-8.0.1/LICENSE.md` & `oc_ocdm-8.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/abstract_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/abstract_set.py` & `oc_ocdm-8.0.2/oc_ocdm/abstract_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/counter_handler/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/counter_handler/counter_handler.py` & `oc_ocdm-8.0.2/oc_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/counter_handler/filesystem_counter_handler.py` & `oc_ocdm-8.0.2/oc_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/counter_handler/in_memory_counter_handler.py` & `oc_ocdm-8.0.2/oc_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/counter_handler/sqlite_counter_handler.py` & `oc_ocdm-8.0.2/oc_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/decorators.py` & `oc_ocdm-8.0.2/oc_ocdm/decorators.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/agent_role.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/citation.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/discourse_element.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/pointer_list.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/reference_annotation.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/reference_pointer.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic/responsible_agent.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic/responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/bibliographic_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/entities/identifier.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/entities/identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/graph_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/graph/graph_set.py` & `oc_ocdm-8.0.2/oc_ocdm/graph/graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/metadata/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/metadata/entities/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/metadata/entities/dataset.py` & `oc_ocdm-8.0.2/oc_ocdm/metadata/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/metadata/entities/distribution.py` & `oc_ocdm-8.0.2/oc_ocdm/metadata/entities/distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/metadata/metadata_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/metadata/metadata_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/metadata/metadata_set.py` & `oc_ocdm-8.0.2/oc_ocdm/metadata/metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/prov/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/prov/entities/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/prov/entities/snapshot_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/prov/entities/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/prov/prov_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/prov/prov_set.py` & `oc_ocdm-8.0.2/oc_ocdm/prov/prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/reader.py` & `oc_ocdm-8.0.2/oc_ocdm/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import rdflib
 from rdflib import RDF, ConjunctiveGraph, Graph, URIRef
 from SPARQLWrapper import JSON, SPARQLWrapper
 
 from oc_ocdm.graph.graph_entity import GraphEntity
 from oc_ocdm.support.reporter import Reporter
 from oc_ocdm.support.support import build_graph_from_results
-
 if TYPE_CHECKING:
     from typing import Any, Dict, List, Optional, Set
     from oc_ocdm.graph.graph_set import GraphSet
 
 from pyshacl import validate
```

### Comparing `oc_ocdm-8.0.1/oc_ocdm/resources/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/resources/querymap.txt` & `oc_ocdm-8.0.2/oc_ocdm/resources/querymap.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/resources/shacle.ttl` & `oc_ocdm-8.0.2/oc_ocdm/resources/shacle.ttl`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/resources/shexc.txt` & `oc_ocdm-8.0.2/oc_ocdm/resources/shexc.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/resources/shexc_closed.txt` & `oc_ocdm-8.0.2/oc_ocdm/resources/shexc_closed.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/storer.py` & `oc_ocdm-8.0.2/oc_ocdm/storer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from oc_ocdm.graph.graph_entity import GraphEntity
 from oc_ocdm.metadata.metadata_entity import MetadataEntity
 from oc_ocdm.prov.prov_entity import ProvEntity
 from oc_ocdm.reader import Reader
 from oc_ocdm.support.query_utils import get_update_query
 from oc_ocdm.support.reporter import Reporter
 from oc_ocdm.support.support import find_paths
+from filelock import FileLock
 
 if TYPE_CHECKING:
     from typing import Any, Dict, List, Optional, Set, Tuple
 
     from rdflib import URIRef
 
     from oc_ocdm.abstract_entity import AbstractEntity
@@ -165,21 +166,23 @@
                 relevant_paths.setdefault(cur_file_path, list())
                 relevant_paths[cur_file_path].append(entity)
 
         for relevant_path, entities_in_path in relevant_paths.items():
             stored_g = None
             # Here we try to obtain a reference to the currently stored graph
             output_filepath = relevant_path.replace(os.path.splitext(relevant_path)[1], ".zip") if self.zip_output else relevant_path
-            if os.path.exists(output_filepath):
-                stored_g = Reader(context_map=self.context_map).load(output_filepath)
-            if stored_g is None:
-                stored_g = ConjunctiveGraph()
-            for entity_in_path in entities_in_path:
-                self.store(entity_in_path, stored_g, relevant_path, context_path, False)
-            self._store_in_file(stored_g, relevant_path, context_path)
+            lock = FileLock(f"{output_filepath}.lock")
+            with lock:
+                if os.path.exists(output_filepath):
+                    stored_g = Reader(context_map=self.context_map).load(output_filepath)
+                if stored_g is None:
+                    stored_g = ConjunctiveGraph()
+                for entity_in_path in entities_in_path:
+                    self.store(entity_in_path, stored_g, relevant_path, context_path, False)
+                self._store_in_file(stored_g, relevant_path, context_path)
 
         return list(relevant_paths.keys())
 
     def store(self, entity: AbstractEntity, destination_g: ConjunctiveGraph, cur_file_path: str, context_path: str = None, store_now: bool = True) -> ConjunctiveGraph:
         self.repok.new_article()
         self.reperr.new_article()
```

### Comparing `oc_ocdm-8.0.1/oc_ocdm/support/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/support/query_utils.py` & `oc_ocdm-8.0.2/oc_ocdm/support/query_utils.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/support/reporter.py` & `oc_ocdm-8.0.2/oc_ocdm/support/reporter.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/support/support.py` & `oc_ocdm-8.0.2/oc_ocdm/support/support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/counter_handler/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py` & `oc_ocdm-8.0.2/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py` & `oc_ocdm-8.0.2/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/coverage/.coverage` & `oc_ocdm-8.0.2/oc_ocdm/test/coverage/.coverage`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -14,15 +14,15 @@
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
 INSERT INTO meta VALUES('sys_argv','[''python -m unittest'', ''discover'', ''-s'', ''oc_ocdm/test'', ''-p'', ''test_*.py'']');
 INSERT INTO meta VALUES('version','6.5.0');
-INSERT INTO meta VALUES('when','2024-03-27 14:18:42');
+INSERT INTO meta VALUES('when','2024-03-27 14:21:27');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
@@ -122,29 +122,29 @@
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'0000cb77affbfdbbffffefdffbfbfbbffd7dfdfdaff704');
 INSERT INTO line_bits VALUES(3,1,X'00000d');
-INSERT INTO line_bits VALUES(4,1,X'00007dfb0bd0a1f81b03630420fe3ab50137d7f57edbd7fd670c5f6200807bc0e55bf6805b01c15f17');
+INSERT INTO line_bits VALUES(4,1,X'00007dfb0b50a0f81b03630420fe3ab50137d7f57edbd7fd27045f2200807bc0e55bf6805b01415f17');
 INSERT INTO line_bits VALUES(5,1,X'000006');
-INSERT INTO line_bits VALUES(6,1,X'000055c1fffffeffffffffffffffffffffffffffffdffff37f63b5e099bbbb9c0200879ba1f301');
+INSERT INTO line_bits VALUES(6,1,X'000055c1fffffeffffffffffffffffffffffffffffdfff937f63b5e099bbbb9c0200879ba1f301');
 INSERT INTO line_bits VALUES(7,1,X'00006d61282e00090a604101408205c002340b00fe029fbbcf06');
 INSERT INTO line_bits VALUES(8,1,X'000062');
-INSERT INTO line_bits VALUES(9,1,X'00007d410900a8f195feafc11bf7defdffa45ce6cc98978097879387938097006060415ef4fae55e0600000080e2ef73');
+INSERT INTO line_bits VALUES(9,1,X'00007d410900a8f195feafc11bf7defdffa45ce6cc98978097879387938097002060411ad4f8e55e0600000080e2ef73');
 INSERT INTO line_bits VALUES(10,1,X'000015fbfdfc121001');
 INSERT INTO line_bits VALUES(11,1,X'000015cc03e73c9cee6b');
-INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5f4ffdc87ff5be77af7bbdef5ee77bdfb5def7af7bbdefd5fe9df5700c0f3ffffff02fe02020202020202fe02');
+INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5f4ffd487ff5ba77af5ab5ef5ea57bdfa55af7af5abdefd5fe9df5700c0f3ffffff02fe02020202020202fe02');
 INSERT INTO line_bits VALUES(13,1,X'0000ad301405be011880');
-INSERT INTO line_bits VALUES(14,1,X'0000bdbb4865608c00000800000400c0eff7fcffbfff171717717197fe3f01');
+INSERT INTO line_bits VALUES(14,1,X'0000bdbb4865608c00000800000400c0eff7fcffbffd171717717197f63f01');
 INSERT INTO line_bits VALUES(15,1,X'00000e');
 INSERT INTO line_bits VALUES(16,1,X'0000d9010060000006006000c00060');
-INSERT INTO line_bits VALUES(17,1,X'0000bdcc2c20fb6f0000000200b60080edbdddbbfe8faebd7fb77a7fffa974f7277bf3bd00000002b02100db');
-INSERT INTO line_bits VALUES(18,1,X'0000954cfc0d00c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
+INSERT INTO line_bits VALUES(17,1,X'0000bdcc2c20fb2f0000000200b60080edbdddbbfe8faebd7fb77a7fffa974f7277bf3bc00000002b02100db');
+INSERT INTO line_bits VALUES(18,1,X'0000954cfc0500c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
 INSERT INTO line_bits VALUES(19,1,X'000006');
 INSERT INTO line_bits VALUES(20,1,X'0000556401d020c137003400a40020e1df0d');
 INSERT INTO line_bits VALUES(21,1,X'0000ad1200d03f0c');
 INSERT INTO line_bits VALUES(22,1,X'00002dce1800809ea060030006000d001800a00100038006000d00e006006800001a0034006800d000a00140030006000d001a00f40506');
 INSERT INTO line_bits VALUES(23,1,X'0000fe07');
 INSERT INTO line_bits VALUES(24,1,X'000055cc0600000000821b002c487003c082040bc002b0002c08');
 INSERT INTO line_bits VALUES(25,1,X'00005598c1000000000206008005098001d000000430002c08');
@@ -153,22 +153,22 @@
 INSERT INTO line_bits VALUES(28,1,X'00005598610000000000000103c08204c00068000002180016240006400300100003a0010008180016246000106000001000140014001400140014001400140004');
 INSERT INTO line_bits VALUES(29,1,X'000055cc18000000040cc08204c00068');
 INSERT INTO line_bits VALUES(30,1,X'000055cc800100000430005810');
 INSERT INTO line_bits VALUES(31,1,X'00005598610000000010300058900006000b12c000604102600068');
 INSERT INTO line_bits VALUES(32,1,X'00002dce0c00000000020c000b123000c02948c00000a7200106800509000580');
 INSERT INTO line_bits VALUES(33,1,X'000055660c000000000206000b1230002c48c000b02001064003');
 INSERT INTO line_bits VALUES(34,1,X'000006');
-INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff3bffbff1d102605e3313400000000010');
-INSERT INTO line_bits VALUES(36,1,X'0000f54bd3d935eec2bbde5b004bc11710');
+INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff3bf1bff1d102605e3313400000000010');
+INSERT INTO line_bits VALUES(36,1,X'0000f54bd3d935aec2ab5e5b004bc11710');
 INSERT INTO line_bits VALUES(37,1,X'000006');
 INSERT INTO line_bits VALUES(38,1,X'000075c10c000000000000000206800509180016246000b02001038005091880060020c0003400000103c08204c0003400000106800509800168');
 INSERT INTO line_bits VALUES(39,1,X'0000d5c20c00000000002060005890800160410206000b123000589080016041020680050918001604');
 INSERT INTO line_bits VALUES(40,1,X'000006');
-INSERT INTO line_bits VALUES(41,1,X'0000d58241ffcdef633477');
-INSERT INTO line_bits VALUES(42,1,X'0000dd45ebd1bcffd771fbfbeeef9f6d59766fbfff992e77fbdb0f00006f01807cb7eee7bd02');
+INSERT INTO line_bits VALUES(41,1,X'0000d58241ff4dec633477');
+INSERT INTO line_bits VALUES(42,1,X'0000dd45ebd1bcffd771fbfbeeef9f6d19766fbfff992e77fbdb0f00006d01807cb7eee7bd02');
 INSERT INTO line_bits VALUES(43,1,X'000002');
 INSERT INTO line_bits VALUES(44,1,X'0000d50583a0018005091a00b020c102c08204b701d000000418002c48d00060418206002c48b001b020');
 INSERT INTO line_bits VALUES(45,1,X'0000ca041e0100023e080092');
 INSERT INTO line_bits VALUES(46,1,X'0000a5bdbffffdefbff7fbefbfbff7f7bffffdfbfefe7dbfdff7f727');
 INSERT INTO line_bits VALUES(47,1,X'02');
 INSERT INTO line_bits VALUES(48,1,X'02');
 INSERT INTO line_bits VALUES(49,1,X'02');
```

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/coverage/coverage.svg` & `oc_ocdm-8.0.2/oc_ocdm/test/coverage/coverage.svg`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_citation.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/test_bibliographic_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/test_bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/entities/test_identifier.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/entities/test_identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/test_graph_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/test_graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/graph/test_graph_set.py` & `oc_ocdm-8.0.2/oc_ocdm/test/graph/test_graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/metadata/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/metadata/entities/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/metadata/entities/test_dataset.py` & `oc_ocdm-8.0.2/oc_ocdm/test/metadata/entities/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/metadata/entities/test_distribution.py` & `oc_ocdm-8.0.2/oc_ocdm/test/metadata/entities/test_distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/metadata/test_metadata_set.py` & `oc_ocdm-8.0.2/oc_ocdm/test/metadata/test_metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/prov/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/prov/entities/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/prov/entities/test_snapshot_entity.py` & `oc_ocdm-8.0.2/oc_ocdm/test/prov/entities/test_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/prov/prov_counter.db` & `oc_ocdm-8.0.2/oc_ocdm/test/prov/prov_counter.db`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/prov/test_prov_set.py` & `oc_ocdm-8.0.2/oc_ocdm/test/prov/test_prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/reader/br.nt` & `oc_ocdm-8.0.2/oc_ocdm/test/reader/br.nt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/reader/test_reader.py` & `oc_ocdm-8.0.2/oc_ocdm/test/reader/test_reader.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/resources/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/resources/data.json` & `oc_ocdm-8.0.2/oc_ocdm/test/resources/data.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/resources/data_reader.json` & `oc_ocdm-8.0.2/oc_ocdm/test/resources/data_reader.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/resources/data_reader_invalid.json` & `oc_ocdm-8.0.2/oc_ocdm/test/resources/data_reader_invalid.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/resources/test_shacle.py` & `oc_ocdm-8.0.2/oc_ocdm/test/resources/test_shacle.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/storer/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/storer/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/storer/test_storer.py` & `oc_ocdm-8.0.2/oc_ocdm/test/storer/test_storer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/support/__init__.py` & `oc_ocdm-8.0.2/oc_ocdm/test/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/oc_ocdm/test/support/test_support.py` & `oc_ocdm-8.0.2/oc_ocdm/test/support/test_support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/pyproject.toml` & `oc_ocdm-8.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc_ocdm"
-version = "8.0.1"
+version = "8.0.2"
 description = "Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel."
 authors = [
     "Silvio Peroni <essepuntato@gmail.com>",
     "Marilena Daquino <marilena.daquino2@unibo.it>",
     "Fabio Mariani <fabio.mariani6@studio.unibo.it>",
     "Simone Persiani <iosonopersia@gmail.com>",
     "Arcangelo Massari <arcangelo.massari@unibo.it>"
```

### Comparing `oc_ocdm-8.0.1/README.md` & `oc_ocdm-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.0.1/PKG-INFO` & `oc_ocdm-8.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc_ocdm
-Version: 8.0.1
+Version: 8.0.2
 Summary: Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.
 Home-page: https://opencitations.net
 License: ISC
 Keywords: opencitations,openscience,datamodel,mapping
 Author: Silvio Peroni
 Author-email: essepuntato@gmail.com
 Requires-Python: >=3.8,<4.0
```

