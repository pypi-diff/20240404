# Comparing `tmp/nisystemlink_clients-1.1.1.tar.gz` & `tmp/nisystemlink_clients-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nisystemlink_clients-1.1.1.tar", max compression
+gzip compressed data, was "nisystemlink_clients-1.1.2.tar", max compression
```

## Comparing `nisystemlink_clients-1.1.1.tar` & `nisystemlink_clients-1.1.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1071 2023-09-22 18:58:43.497864 nisystemlink_clients-1.1.1/LICENSE
--rw-r--r--   0        0        0     2335 2023-09-22 18:58:43.497864 nisystemlink_clients-1.1.1/README.rst
--rw-r--r--   0        0        0       15 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/__init__.py
--rw-r--r--   0        0        0       15 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/__init__.py
--rw-r--r--   0        0        0      360 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/__init__.py
--rw-r--r--   0        0        0      835 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_api_error.py
--rw-r--r--   0        0        0     2501 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_api_exception.py
--rw-r--r--   0        0        0      654 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_cloud_http_configuration.py
--rw-r--r--   0        0        0     4791 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_http_configuration.py
--rw-r--r--   0        0        0     7128 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_http_configuration_manager.py
--rw-r--r--   0        0        0       39 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/__init__.py
--rw-r--r--   0        0        0     1223 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_classproperty_support.py
--rw-r--r--   0        0        0    10921 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_http_client.py
--rw-r--r--   0        0        0     2955 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_http_configuration_file.py
--rw-r--r--   0        0        0     2482 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_path_constants.py
--rw-r--r--   0        0        0     2048 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_timestamp_utilities.py
--rw-r--r--   0        0        0    10778 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_winpaths.py
--rw-r--r--   0        0        0     3764 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_winpaths.pyi
--rw-r--r--   0        0        0      772 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_jupyter_http_configuration.py
--rw-r--r--   0        0        0       15 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/__init__.py
--rw-r--r--   0        0        0     2982 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_base_client.py
--rw-r--r--   0        0        0      444 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_json_model.py
--rw-r--r--   0        0        0     1968 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_methods.py
--rw-r--r--   0        0        0      615 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_with_paging.py
--rw-r--r--   0        0        0       66 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/helpers/__init__.py
--rw-r--r--   0        0        0      981 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/core/helpers/_iterator_file_like.py
--rw-r--r--   0        0        0       64 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/__init__.py
--rw-r--r--   0        0        0    10781 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/_data_frame_client.py
--rw-r--r--   0        0        0     1365 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/__init__.py
--rw-r--r--   0        0        0     1093 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_api_info.py
--rw-r--r--   0        0        0      537 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_append_table_data_request.py
--rw-r--r--   0        0        0      625 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column.py
--rw-r--r--   0        0        0     1367 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column_filter.py
--rw-r--r--   0        0        0      364 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column_order_by.py
--rw-r--r--   0        0        0      645 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column_type.py
--rw-r--r--   0        0        0      809 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_create_table_request.py
--rw-r--r--   0        0        0     3065 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_data_frame.py
--rw-r--r--   0        0        0      599 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_data_type.py
--rw-r--r--   0        0        0      553 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_delete_tables_partial_success.py
--rw-r--r--   0        0        0     1553 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_export_table_data_request.py
--rw-r--r--   0        0        0     1940 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_modify_table_request.py
--rw-r--r--   0        0        0      653 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_modify_tables_partial_success.py
--rw-r--r--   0        0        0     1821 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_modify_tables_request.py
--rw-r--r--   0        0        0      627 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_order_by.py
--rw-r--r--   0        0        0      388 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_paged_table_rows.py
--rw-r--r--   0        0        0      329 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_paged_tables.py
--rw-r--r--   0        0        0     2448 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_decimated_data_request.py
--rw-r--r--   0        0        0      894 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_table_data_base.py
--rw-r--r--   0        0        0      877 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_table_data_request.py
--rw-r--r--   0        0        0     3454 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_tables_request.py
--rw-r--r--   0        0        0     1195 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_table_metadata.py
--rw-r--r--   0        0        0      279 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_table_rows.py
--rw-r--r--   0        0        0      830 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/__init__.py
--rw-r--r--   0        0        0     3849 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_async_tag_query_result_collection.py
--rw-r--r--   0        0        0    13155 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_buffered_tag_writer.py
--rw-r--r--   0        0        0       39 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/__init__.py
--rw-r--r--   0        0        0      489 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_itime_stamper.py
--rw-r--r--   0        0        0     5787 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_manual_reset_timer.py
--rw-r--r--   0        0        0     3938 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates.py
--rw-r--r--   0        0        0     3053 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates_reader.py
--rw-r--r--   0        0        0     1065 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_system_time_stamper.py
--rw-r--r--   0        0        0     2048 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_data_type.py
--rw-r--r--   0        0        0       39 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/__init__.py
--rw-r--r--   0        0        0     2591 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_async_tag_query_result_collection.py
--rw-r--r--   0        0        0     2336 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_buffered_tag_writer.py
--rw-r--r--   0        0        0     2498 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_tag_query_result_collection.py
--rw-r--r--   0        0        0    15418 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_tag_selection.py
--rw-r--r--   0        0        0     9988 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_tag_subscription.py
--rw-r--r--   0        0        0     4577 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_temporary_tag_selection.py
--rw-r--r--   0        0        0     9900 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_itag_reader.py
--rw-r--r--   0        0        0     9391 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_itag_writer.py
--rw-r--r--   0        0        0      744 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_retention_type.py
--rw-r--r--   0        0        0    11515 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_data.py
--rw-r--r--   0        0        0     5856 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_data_update.py
--rw-r--r--   0        0        0    33150 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_manager.py
--rw-r--r--   0        0        0     1699 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_path_utilities.py
--rw-r--r--   0        0        0     2733 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_query_result_collection.py
--rw-r--r--   0        0        0    30845 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_selection.py
--rw-r--r--   0        0        0     8684 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_subscription.py
--rw-r--r--   0        0        0     1347 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_update_fields.py
--rw-r--r--   0        0        0     3800 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_value_reader.py
--rw-r--r--   0        0        0     2753 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_value_writer.py
--rw-r--r--   0        0        0     4423 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_with_aggregates.py
--rw-r--r--   0        0        0        0 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/py.typed
--rw-r--r--   0        0        0      960 2023-09-22 18:58:43.501864 nisystemlink_clients-1.1.1/nisystemlink/stubs/events.pyi
--rw-r--r--   0        0        0     2594 2023-09-22 18:59:04.393518 nisystemlink_clients-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 nisystemlink_clients-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2335 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/README.rst
+-rw-r--r--   0        0        0       15 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/__init__.py
+-rw-r--r--   0        0        0       15 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/__init__.py
+-rw-r--r--   0        0        0      360 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/__init__.py
+-rw-r--r--   0        0        0      835 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_api_error.py
+-rw-r--r--   0        0        0     2501 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_api_exception.py
+-rw-r--r--   0        0        0      654 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_cloud_http_configuration.py
+-rw-r--r--   0        0        0     4791 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_http_configuration.py
+-rw-r--r--   0        0        0     7128 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_http_configuration_manager.py
+-rw-r--r--   0        0        0       39 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/__init__.py
+-rw-r--r--   0        0        0     1223 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_classproperty_support.py
+-rw-r--r--   0        0        0    10921 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_http_client.py
+-rw-r--r--   0        0        0     2955 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_http_configuration_file.py
+-rw-r--r--   0        0        0     2482 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_path_constants.py
+-rw-r--r--   0        0        0     2048 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_timestamp_utilities.py
+-rw-r--r--   0        0        0    10778 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_winpaths.py
+-rw-r--r--   0        0        0     3764 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_winpaths.pyi
+-rw-r--r--   0        0        0      772 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_jupyter_http_configuration.py
+-rw-r--r--   0        0        0       15 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/__init__.py
+-rw-r--r--   0        0        0     2982 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_base_client.py
+-rw-r--r--   0        0        0      444 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_json_model.py
+-rw-r--r--   0        0        0     1968 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_methods.py
+-rw-r--r--   0        0        0      615 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_with_paging.py
+-rw-r--r--   0        0        0       66 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/helpers/__init__.py
+-rw-r--r--   0        0        0      981 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/core/helpers/_iterator_file_like.py
+-rw-r--r--   0        0        0       64 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/__init__.py
+-rw-r--r--   0        0        0    10781 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/_data_frame_client.py
+-rw-r--r--   0        0        0     1365 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/__init__.py
+-rw-r--r--   0        0        0     1093 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_api_info.py
+-rw-r--r--   0        0        0      537 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_append_table_data_request.py
+-rw-r--r--   0        0        0      625 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column.py
+-rw-r--r--   0        0        0     1367 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column_filter.py
+-rw-r--r--   0        0        0      364 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column_order_by.py
+-rw-r--r--   0        0        0      645 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column_type.py
+-rw-r--r--   0        0        0      809 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_create_table_request.py
+-rw-r--r--   0        0        0     3065 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_data_frame.py
+-rw-r--r--   0        0        0      599 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_data_type.py
+-rw-r--r--   0        0        0      553 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_delete_tables_partial_success.py
+-rw-r--r--   0        0        0     1553 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_export_table_data_request.py
+-rw-r--r--   0        0        0     1940 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_modify_table_request.py
+-rw-r--r--   0        0        0      653 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_modify_tables_partial_success.py
+-rw-r--r--   0        0        0     1821 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_modify_tables_request.py
+-rw-r--r--   0        0        0      627 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_order_by.py
+-rw-r--r--   0        0        0      388 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_paged_table_rows.py
+-rw-r--r--   0        0        0      329 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_paged_tables.py
+-rw-r--r--   0        0        0     2448 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_decimated_data_request.py
+-rw-r--r--   0        0        0      894 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_table_data_base.py
+-rw-r--r--   0        0        0      877 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_table_data_request.py
+-rw-r--r--   0        0        0     3454 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_tables_request.py
+-rw-r--r--   0        0        0     1195 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_table_metadata.py
+-rw-r--r--   0        0        0      279 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_table_rows.py
+-rw-r--r--   0        0        0      830 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/__init__.py
+-rw-r--r--   0        0        0     3849 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_async_tag_query_result_collection.py
+-rw-r--r--   0        0        0    13155 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_buffered_tag_writer.py
+-rw-r--r--   0        0        0       39 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/__init__.py
+-rw-r--r--   0        0        0      489 2023-10-03 13:15:00.376538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_itime_stamper.py
+-rw-r--r--   0        0        0     5787 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_manual_reset_timer.py
+-rw-r--r--   0        0        0     3938 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates.py
+-rw-r--r--   0        0        0     3053 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates_reader.py
+-rw-r--r--   0        0        0     1065 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_system_time_stamper.py
+-rw-r--r--   0        0        0     2048 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_data_type.py
+-rw-r--r--   0        0        0       39 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/__init__.py
+-rw-r--r--   0        0        0     2591 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_async_tag_query_result_collection.py
+-rw-r--r--   0        0        0     2336 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_buffered_tag_writer.py
+-rw-r--r--   0        0        0     2498 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_tag_query_result_collection.py
+-rw-r--r--   0        0        0    15418 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_tag_selection.py
+-rw-r--r--   0        0        0     9988 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_tag_subscription.py
+-rw-r--r--   0        0        0     4577 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_temporary_tag_selection.py
+-rw-r--r--   0        0        0     9900 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_itag_reader.py
+-rw-r--r--   0        0        0     9391 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_itag_writer.py
+-rw-r--r--   0        0        0      744 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_retention_type.py
+-rw-r--r--   0        0        0    11515 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_data.py
+-rw-r--r--   0        0        0     5856 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_data_update.py
+-rw-r--r--   0        0        0    33150 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_manager.py
+-rw-r--r--   0        0        0     1699 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_path_utilities.py
+-rw-r--r--   0        0        0     2733 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_query_result_collection.py
+-rw-r--r--   0        0        0    30845 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_selection.py
+-rw-r--r--   0        0        0     8684 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_subscription.py
+-rw-r--r--   0        0        0     1347 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_update_fields.py
+-rw-r--r--   0        0        0     3800 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_value_reader.py
+-rw-r--r--   0        0        0     2753 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_value_writer.py
+-rw-r--r--   0        0        0     4423 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_with_aggregates.py
+-rw-r--r--   0        0        0        0 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/py.typed
+-rw-r--r--   0        0        0      960 2023-10-03 13:15:00.380538 nisystemlink_clients-1.1.2/nisystemlink/stubs/events.pyi
+-rw-r--r--   0        0        0     2594 2023-10-03 13:15:30.424943 nisystemlink_clients-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 nisystemlink_clients-1.1.2/PKG-INFO
```

### Comparing `nisystemlink_clients-1.1.1/LICENSE` & `nisystemlink_clients-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/README.rst` & `nisystemlink_clients-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_api_error.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_api_error.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_api_exception.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_api_exception.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_cloud_http_configuration.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_cloud_http_configuration.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_http_configuration.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_http_configuration.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_http_configuration_manager.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_http_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_classproperty_support.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_classproperty_support.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_http_client.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_http_client.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_http_configuration_file.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_http_configuration_file.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_path_constants.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_path_constants.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_timestamp_utilities.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_timestamp_utilities.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_winpaths.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_winpaths.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_internal/_winpaths.pyi` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_internal/_winpaths.pyi`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_jupyter_http_configuration.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_jupyter_http_configuration.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_base_client.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_base_client.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_methods.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_methods.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/_uplink/_with_paging.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/_uplink/_with_paging.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/core/helpers/_iterator_file_like.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/core/helpers/_iterator_file_like.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/_data_frame_client.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/_data_frame_client.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/__init__.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_api_info.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_api_info.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_append_table_data_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_append_table_data_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column_filter.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column_filter.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_column_type.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_column_type.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_create_table_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_create_table_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_data_frame.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_data_frame.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_data_type.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_data_type.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_delete_tables_partial_success.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_delete_tables_partial_success.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_export_table_data_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_export_table_data_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_modify_table_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_modify_table_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_modify_tables_partial_success.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_modify_tables_partial_success.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_modify_tables_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_modify_tables_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_order_by.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_order_by.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_decimated_data_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_decimated_data_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_table_data_base.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_table_data_base.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_table_data_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_table_data_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_query_tables_request.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_query_tables_request.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/dataframe/models/_table_metadata.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/dataframe/models/_table_metadata.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/__init__.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_async_tag_query_result_collection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_async_tag_query_result_collection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_buffered_tag_writer.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_buffered_tag_writer.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_manual_reset_timer.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_manual_reset_timer.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates_reader.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_serialized_tag_with_aggregates_reader.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_core/_system_time_stamper.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_core/_system_time_stamper.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_data_type.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_data_type.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_async_tag_query_result_collection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_async_tag_query_result_collection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_buffered_tag_writer.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_buffered_tag_writer.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_tag_query_result_collection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_tag_query_result_collection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_tag_selection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_tag_selection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_http_tag_subscription.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_http_tag_subscription.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_http/_temporary_tag_selection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_http/_temporary_tag_selection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_itag_reader.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_itag_reader.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_itag_writer.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_itag_writer.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_retention_type.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_retention_type.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_data.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_data.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_data_update.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_data_update.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_manager.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_manager.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_path_utilities.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_path_utilities.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_query_result_collection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_query_result_collection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_selection.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_selection.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_subscription.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_subscription.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_update_fields.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_update_fields.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_value_reader.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_value_reader.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_value_writer.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_value_writer.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/clients/tag/_tag_with_aggregates.py` & `nisystemlink_clients-1.1.2/nisystemlink/clients/tag/_tag_with_aggregates.py`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/nisystemlink/stubs/events.pyi` & `nisystemlink_clients-1.1.2/nisystemlink/stubs/events.pyi`

 * *Files identical despite different names*

### Comparing `nisystemlink_clients-1.1.1/pyproject.toml` & `nisystemlink_clients-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nisystemlink-clients"
-version = "1.1.1"
+version = "1.1.2"
 description = "NI-SystemLink Python API"
 authors = ["National Instruments"]
 maintainers = [
     "Carson Moore <carson.moore@ni.com>",
     "Paul Spangler <paul.spangler@ni.com>",
     "Cameron Waterman <cameron.waterman@ni.com>",
 ]
```

### Comparing `nisystemlink_clients-1.1.1/PKG-INFO` & `nisystemlink_clients-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nisystemlink-clients
-Version: 1.1.1
+Version: 1.1.2
 Summary: NI-SystemLink Python API
 License: MIT
 Keywords: nisystemlink,systemlink
 Author: National Instruments
 Maintainer: Carson Moore
 Maintainer-email: carson.moore@ni.com
 Requires-Python: >=3.8,<4.0
```

