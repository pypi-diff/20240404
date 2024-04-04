# Comparing `tmp/snowflake-connector-python-3.7.1.tar.gz` & `tmp/snowflake-connector-python-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-3.7.1.tar", last modified: Thu Feb 22 22:38:14 2024, max compression
+gzip compressed data, was "snowflake-connector-python-3.8.0.tar", last modified: Thu Apr  4 16:56:15 2024, max compression
```

## Comparing `snowflake-connector-python-3.7.1.tar` & `snowflake-connector-python-3.8.0.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.440243 snowflake-connector-python-3.7.1/
--rw-r--r--   0 user      (1006) user      (1006)     1701 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/CONTRIBUTING.md
--rw-r--r--   0 user      (1006) user      (1006)    56365 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/DESCRIPTION.md
--rw-r--r--   0 user      (1006) user      (1006)    11365 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/LICENSE.txt
--rw-r--r--   0 user      (1006) user      (1006)      926 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/MANIFEST.in
--rw-r--r--   0 user      (1006) user      (1006)      457 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/NOTICE
--rw-r--r--   0 user      (1006) user      (1006)    59869 2024-02-22 22:38:14.440243 snowflake-connector-python-3.7.1/PKG-INFO
--rw-r--r--   0 user      (1006) user      (1006)     3045 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/README.md
--rw-r--r--   0 user      (1006) user      (1006)      308 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/SECURITY.md
--rw-r--r--   0 user      (1006) user      (1006)      593 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/pyproject.toml
--rw-r--r--   0 user      (1006) user      (1006)     3018 2024-02-22 22:38:14.440243 snowflake-connector-python-3.7.1/setup.cfg
--rw-r--r--   0 user      (1006) user      (1006)     6914 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/setup.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.392243 snowflake-connector-python-3.7.1/src/
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.388243 snowflake-connector-python-3.7.1/src/snowflake/
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.404243 snowflake-connector-python-3.7.1/src/snowflake/connector/
--rw-r--r--   0 user      (1006) user      (1006)     1759 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    11339 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 user      (1006) user      (1006)     1521 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 user      (1006) user      (1006)     5381 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/arrow_context.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.408243 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/
--rw-r--r--   0 user      (1006) user      (1006)      991 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    27978 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 user      (1006) user      (1006)     7050 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 user      (1006) user      (1006)     1034 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/default.py
--rw-r--r--   0 user      (1006) user      (1006)     2127 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 user      (1006) user      (1006)     6678 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 user      (1006) user      (1006)     1488 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 user      (1006) user      (1006)    11394 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 user      (1006) user      (1006)     1981 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 user      (1006) user      (1006)    14845 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 user      (1006) user      (1006)     9913 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     4346 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/backoff_policies.py
--rw-r--r--   0 user      (1006) user      (1006)     2355 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 user      (1006) user      (1006)    23454 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/cache.py
--rw-r--r--   0 user      (1006) user      (1006)     2894 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/compat.py
--rw-r--r--   0 user      (1006) user      (1006)    19252 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/config_manager.py
--rw-r--r--   0 user      (1006) user      (1006)    74369 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/connection.py
--rw-r--r--   0 user      (1006) user      (1006)    30807 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 user      (1006) user      (1006)    11638 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/constants.py
--rw-r--r--   0 user      (1006) user      (1006)    27710 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/converter.py
--rw-r--r--   0 user      (1006) user      (1006)     2864 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 user      (1006) user      (1006)      437 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/converter_null.py
--rw-r--r--   0 user      (1006) user      (1006)     7633 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/converter_snowsql.py
--rw-r--r--   0 user      (1006) user      (1006)    66305 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/cursor.py
--rw-r--r--   0 user      (1006) user      (1006)     1268 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/dbapi.py
--rw-r--r--   0 user      (1006) user      (1006)      615 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/description.py
--rw-r--r--   0 user      (1006) user      (1006)     8018 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 user      (1006) user      (1006)     2708 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/errorcode.py
--rw-r--r--   0 user      (1006) user      (1006)    20185 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/errors.py
--rw-r--r--   0 user      (1006) user      (1006)      184 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/feature.py
--rw-r--r--   0 user      (1006) user      (1006)     3246 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 user      (1006) user      (1006)    48252 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 user      (1006) user      (1006)     5011 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/file_util.py
--rw-r--r--   0 user      (1006) user      (1006)    16072 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     2802 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 user      (1006) user      (1006)     2946 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/local_storage_client.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.388243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.416243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
--rw-r--r--   0 user      (1006) user      (1006)     2039 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      765 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      633 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      547 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      499 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      503 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)    19180 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 user      (1006) user      (1006)     2407 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 user      (1006) user      (1006)     4462 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 user      (1006) user      (1006)     4477 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 user      (1006) user      (1006)    42047 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 user      (1006) user      (1006)     4892 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1535 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      994 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     3655 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)     1788 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     2739 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      659 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      991 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      758 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      490 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      750 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)     1011 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)    11583 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
--rw-r--r--   0 user      (1006) user      (1006)     2634 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      811 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1424 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      794 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.416243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
--rw-r--r--   0 user      (1006) user      (1006)      216 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 user      (1006) user      (1006)     2522 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1485 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 user      (1006) user      (1006)      940 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1379 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 user      (1006) user      (1006)      933 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 user      (1006) user      (1006)      631 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      571 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1248 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      708 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)    13329 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)     4114 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.416243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
--rw-r--r--   0 user      (1006) user      (1006)      470 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1963 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 user      (1006) user      (1006)     2262 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.420243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
--rw-r--r--   0 user      (1006) user      (1006)     6007 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
--rw-r--r--   0 user      (1006) user      (1006)     3515 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
--rw-r--r--   0 user      (1006) user      (1006)     1178 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
--rw-r--r--   0 user      (1006) user      (1006)    79675 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
--rw-r--r--   0 user      (1006) user      (1006)     7437 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
--rw-r--r--   0 user      (1006) user      (1006)     3998 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
--rw-r--r--   0 user      (1006) user      (1006)      119 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
--rw-r--r--   0 user      (1006) user      (1006)     1380 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
--rw-r--r--   0 user      (1006) user      (1006)     4778 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
--rw-r--r--   0 user      (1006) user      (1006)      575 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
--rw-r--r--   0 user      (1006) user      (1006)      165 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
--rw-r--r--   0 user      (1006) user      (1006)     4826 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
--rw-r--r--   0 user      (1006) user      (1006)     4917 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
--rw-r--r--   0 user      (1006) user      (1006)     3091 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
--rw-r--r--   0 user      (1006) user      (1006)    10913 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.424243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
--rw-r--r--   0 user      (1006) user      (1006)      198 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
--rw-r--r--   0 user      (1006) user      (1006)     5852 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
--rw-r--r--   0 user      (1006) user      (1006)     2400 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
--rw-r--r--   0 user      (1006) user      (1006)     2613 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
--rw-r--r--   0 user      (1006) user      (1006)      600 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
--rw-r--r--   0 user      (1006) user      (1006)     1179 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
--rw-r--r--   0 user      (1006) user      (1006)     5284 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
--rw-r--r--   0 user      (1006) user      (1006)     3719 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
--rw-r--r--   0 user      (1006) user      (1006)      424 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
--rw-r--r--   0 user      (1006) user      (1006)     1064 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
--rw-r--r--   0 user      (1006) user      (1006)      104 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
--rw-r--r--   0 user      (1006) user      (1006)      677 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
--rw-r--r--   0 user      (1006) user      (1006)     1844 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
--rw-r--r--   0 user      (1006) user      (1006)     4295 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
--rw-r--r--   0 user      (1006) user      (1006)    31201 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
--rw-r--r--   0 user      (1006) user      (1006)     8882 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
--rw-r--r--   0 user      (1006) user      (1006)      190 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
--rw-r--r--   0 user      (1006) user      (1006)     1645 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
--rw-r--r--   0 user      (1006) user      (1006)   102952 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
--rw-r--r--   0 user      (1006) user      (1006)   107680 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
--rw-r--r--   0 user      (1006) user      (1006)   132283 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
--rw-r--r--   0 user      (1006) user      (1006)    12046 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
--rw-r--r--   0 user      (1006) user      (1006)     8404 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
--rw-r--r--   0 user      (1006) user      (1006)    18580 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
--rw-r--r--   0 user      (1006) user      (1006)    14382 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
--rw-r--r--   0 user      (1006) user      (1006)  1616169 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
--rw-r--r--   0 user      (1006) user      (1006)    17533 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.424243 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/Logging/
--rw-r--r--   0 user      (1006) user      (1006)     3113 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
--rw-r--r--   0 user      (1006) user      (1006)     1344 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
--rw-r--r--   0 user      (1006) user      (1006)    42377 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/network.py
--rw-r--r--   0 user      (1006) user      (1006)    16575 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 user      (1006) user      (1006)    69704 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 user      (1006) user      (1006)     4573 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/options.py
--rw-r--r--   0 user      (1006) user      (1006)    22495 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 user      (1006) user      (1006)     1582 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/proxy.py
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/py.typed
--rw-r--r--   0 user      (1006) user      (1006)    26617 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/result_batch.py
--rw-r--r--   0 user      (1006) user      (1006)     9380 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/result_set.py
--rw-r--r--   0 user      (1006) user      (1006)    21870 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     5343 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 user      (1006) user      (1006)     1957 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 user      (1006) user      (1006)     1120 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 user      (1006) user      (1006)    12449 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 user      (1006) user      (1006)     4313 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 user      (1006) user      (1006)      432 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 user      (1006) user      (1006)      813 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 user      (1006) user      (1006)     4563 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 user      (1006) user      (1006)    17583 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     8861 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/telemetry.py
--rw-r--r--   0 user      (1006) user      (1006)    19070 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 user      (1006) user      (1006)      982 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/test_util.py
--rw-r--r--   0 user      (1006) user      (1006)     5073 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.424243 snowflake-connector-python-3.7.1/src/snowflake/connector/tool/
--rw-r--r--   0 user      (1006) user      (1006)       76 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)     1485 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 user      (1006) user      (1006)     4575 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 user      (1006) user      (1006)     6643 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 user      (1006) user      (1006)     2119 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 user      (1006) user      (1006)     1021 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/url_util.py
--rw-r--r--   0 user      (1006) user      (1006)    10405 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.424243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/
--rw-r--r--   0 user      (1006) user      (1006)       76 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.428243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 user      (1006) user      (1006)    10142 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 user      (1006) user      (1006)     4742 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)      435 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 user      (1006) user      (1006)     1495 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 user      (1006) user      (1006)    19577 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 user      (1006) user      (1006)     6449 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 user      (1006) user      (1006)    10187 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 user      (1006) user      (1006)      429 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 user      (1006) user      (1006)     1451 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 user      (1006) user      (1006)    18560 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 user      (1006) user      (1006)     3813 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 user      (1006) user      (1006)     3885 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 user      (1006) user      (1006)      733 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 user      (1006) user      (1006)    35231 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 user      (1006) user      (1006)    30373 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 user      (1006) user      (1006)     4235 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 user      (1006) user      (1006)     2912 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 user      (1006) user      (1006)    33450 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.428243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 user      (1006) user      (1006)     1115 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 user      (1006) user      (1006)     2763 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    11372 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 user      (1006) user      (1006)       64 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 user      (1006) user      (1006)    20300 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 user      (1006) user      (1006)    40285 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.432243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)      957 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.432243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    17632 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 user      (1006) user      (1006)    13922 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 user      (1006) user      (1006)    11012 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 user      (1006) user      (1006)     4528 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 user      (1006) user      (1006)    16772 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 user      (1006) user      (1006)    34431 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 user      (1006) user      (1006)     7097 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 user      (1006) user      (1006)     8217 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 user      (1006) user      (1006)     8579 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 user      (1006) user      (1006)     2440 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.432243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.432243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)     1417 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 user      (1006) user      (1006)     5343 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0 user      (1006) user      (1006)    34665 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 user      (1006) user      (1006)    19990 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 user      (1006) user      (1006)     6691 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 user      (1006) user      (1006)    30760 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.436243 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 user      (1006) user      (1006)     1155 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)     5376 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 user      (1006) user      (1006)     1605 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 user      (1006) user      (1006)      498 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 user      (1006) user      (1006)     4225 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 user      (1006) user      (1006)     3510 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 user      (1006) user      (1006)    22013 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 user      (1006) user      (1006)    17165 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 user      (1006) user      (1006)     5758 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 user      (1006) user      (1006)     6895 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 user      (1006) user      (1006)    10168 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 user      (1006) user      (1006)    14279 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 user      (1006) user      (1006)     5403 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 user      (1006) user      (1006)      107 2024-02-22 22:35:17.000000 snowflake-connector-python-3.7.1/src/snowflake/connector/version.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-02-22 22:38:14.436243 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/
--rw-r--r--   0 user      (1006) user      (1006)    59869 2024-02-22 22:38:14.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/PKG-INFO
--rw-r--r--   0 user      (1006) user      (1006)    13218 2024-02-22 22:38:14.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1006) user      (1006)        1 2024-02-22 22:38:14.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1006) user      (1006)      322 2024-02-22 22:38:14.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/entry_points.txt
--rw-r--r--   0 user      (1006) user      (1006)        1 2024-02-22 22:36:04.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/not-zip-safe
--rw-r--r--   0 user      (1006) user      (1006)      646 2024-02-22 22:38:14.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/requires.txt
--rw-r--r--   0 user      (1006) user      (1006)       10 2024-02-22 22:38:14.000000 snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.404158 snowflake-connector-python-3.8.0/
+-rw-r--r--   0 user      (1006) user      (1006)     1701 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/CONTRIBUTING.md
+-rw-r--r--   0 user      (1006) user      (1006)    58242 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/DESCRIPTION.md
+-rw-r--r--   0 user      (1006) user      (1006)    11365 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/LICENSE.txt
+-rw-r--r--   0 user      (1006) user      (1006)      926 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/MANIFEST.in
+-rw-r--r--   0 user      (1006) user      (1006)      457 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/NOTICE
+-rw-r--r--   0 user      (1006) user      (1006)    61746 2024-04-04 16:56:15.404158 snowflake-connector-python-3.8.0/PKG-INFO
+-rw-r--r--   0 user      (1006) user      (1006)     3045 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/README.md
+-rw-r--r--   0 user      (1006) user      (1006)      308 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/SECURITY.md
+-rw-r--r--   0 user      (1006) user      (1006)      593 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/pyproject.toml
+-rw-r--r--   0 user      (1006) user      (1006)     3018 2024-04-04 16:56:15.408158 snowflake-connector-python-3.8.0/setup.cfg
+-rw-r--r--   0 user      (1006) user      (1006)     6914 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/setup.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.360158 snowflake-connector-python-3.8.0/src/
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.356158 snowflake-connector-python-3.8.0/src/snowflake/
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.372158 snowflake-connector-python-3.8.0/src/snowflake/connector/
+-rw-r--r--   0 user      (1006) user      (1006)     1759 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    11339 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 user      (1006) user      (1006)     1521 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 user      (1006) user      (1006)     5381 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/arrow_context.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.372158 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/
+-rw-r--r--   0 user      (1006) user      (1006)      991 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    27978 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 user      (1006) user      (1006)     7050 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 user      (1006) user      (1006)     1034 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 user      (1006) user      (1006)     2127 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 user      (1006) user      (1006)     6678 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 user      (1006) user      (1006)     1488 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 user      (1006) user      (1006)    11394 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 user      (1006) user      (1006)     1981 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 user      (1006) user      (1006)    17958 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 user      (1006) user      (1006)     9913 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     4346 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/backoff_policies.py
+-rw-r--r--   0 user      (1006) user      (1006)     2355 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 user      (1006) user      (1006)    23454 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/cache.py
+-rw-r--r--   0 user      (1006) user      (1006)     2894 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/compat.py
+-rw-r--r--   0 user      (1006) user      (1006)    19252 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 user      (1006) user      (1006)    75785 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/connection.py
+-rw-r--r--   0 user      (1006) user      (1006)    32728 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 user      (1006) user      (1006)    12971 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/constants.py
+-rw-r--r--   0 user      (1006) user      (1006)    27710 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/converter.py
+-rw-r--r--   0 user      (1006) user      (1006)     2864 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 user      (1006) user      (1006)      437 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 user      (1006) user      (1006)     7633 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/converter_snowsql.py
+-rw-r--r--   0 user      (1006) user      (1006)    64707 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/cursor.py
+-rw-r--r--   0 user      (1006) user      (1006)     1268 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 user      (1006) user      (1006)      615 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/description.py
+-rw-r--r--   0 user      (1006) user      (1006)     8018 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 user      (1006) user      (1006)     2708 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 user      (1006) user      (1006)    20185 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/errors.py
+-rw-r--r--   0 user      (1006) user      (1006)      184 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/feature.py
+-rw-r--r--   0 user      (1006) user      (1006)     3246 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 user      (1006) user      (1006)    48252 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 user      (1006) user      (1006)     5011 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/file_util.py
+-rw-r--r--   0 user      (1006) user      (1006)    16072 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     2802 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 user      (1006) user      (1006)     3162 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/local_storage_client.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.360158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.384158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
+-rw-r--r--   0 user      (1006) user      (1006)     2039 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      765 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      633 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      547 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      499 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      503 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    19180 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     2407 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     4462 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     4477 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    42047 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     4892 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1535 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      994 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     3655 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     1788 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     2739 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      659 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      991 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      758 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      490 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      750 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     1011 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    11583 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
+-rw-r--r--   0 user      (1006) user      (1006)     2634 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      811 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1424 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      794 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.384158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
+-rw-r--r--   0 user      (1006) user      (1006)      216 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     2522 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1485 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      940 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1379 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      933 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      631 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      571 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1248 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      708 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    13329 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     4114 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.384158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
+-rw-r--r--   0 user      (1006) user      (1006)      470 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1963 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     2262 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.388158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
+-rw-r--r--   0 user      (1006) user      (1006)     6007 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
+-rw-r--r--   0 user      (1006) user      (1006)     3515 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
+-rw-r--r--   0 user      (1006) user      (1006)     1178 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
+-rw-r--r--   0 user      (1006) user      (1006)    79675 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
+-rw-r--r--   0 user      (1006) user      (1006)     7437 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
+-rw-r--r--   0 user      (1006) user      (1006)     3998 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
+-rw-r--r--   0 user      (1006) user      (1006)      119 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
+-rw-r--r--   0 user      (1006) user      (1006)     1380 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
+-rw-r--r--   0 user      (1006) user      (1006)     4778 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
+-rw-r--r--   0 user      (1006) user      (1006)      575 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
+-rw-r--r--   0 user      (1006) user      (1006)      165 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
+-rw-r--r--   0 user      (1006) user      (1006)     4826 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
+-rw-r--r--   0 user      (1006) user      (1006)     4917 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
+-rw-r--r--   0 user      (1006) user      (1006)     3091 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
+-rw-r--r--   0 user      (1006) user      (1006)    10913 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.392158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
+-rw-r--r--   0 user      (1006) user      (1006)      198 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
+-rw-r--r--   0 user      (1006) user      (1006)     5852 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
+-rw-r--r--   0 user      (1006) user      (1006)     2400 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
+-rw-r--r--   0 user      (1006) user      (1006)     2613 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
+-rw-r--r--   0 user      (1006) user      (1006)      600 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
+-rw-r--r--   0 user      (1006) user      (1006)     1179 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
+-rw-r--r--   0 user      (1006) user      (1006)     5284 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
+-rw-r--r--   0 user      (1006) user      (1006)     3719 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
+-rw-r--r--   0 user      (1006) user      (1006)      424 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
+-rw-r--r--   0 user      (1006) user      (1006)     1064 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
+-rw-r--r--   0 user      (1006) user      (1006)      104 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
+-rw-r--r--   0 user      (1006) user      (1006)      677 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
+-rw-r--r--   0 user      (1006) user      (1006)     1844 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
+-rw-r--r--   0 user      (1006) user      (1006)     4295 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
+-rw-r--r--   0 user      (1006) user      (1006)    31201 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
+-rw-r--r--   0 user      (1006) user      (1006)     8882 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
+-rw-r--r--   0 user      (1006) user      (1006)      190 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
+-rw-r--r--   0 user      (1006) user      (1006)     1645 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
+-rw-r--r--   0 user      (1006) user      (1006)   102952 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
+-rw-r--r--   0 user      (1006) user      (1006)   107680 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
+-rw-r--r--   0 user      (1006) user      (1006)   132283 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
+-rw-r--r--   0 user      (1006) user      (1006)    12046 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     8404 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
+-rw-r--r--   0 user      (1006) user      (1006)    18580 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
+-rw-r--r--   0 user      (1006) user      (1006)    14382 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
+-rw-r--r--   0 user      (1006) user      (1006)  1616169 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
+-rw-r--r--   0 user      (1006) user      (1006)    17533 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.392158 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/Logging/
+-rw-r--r--   0 user      (1006) user      (1006)     3113 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     1344 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    42377 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/network.py
+-rw-r--r--   0 user      (1006) user      (1006)    16575 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 user      (1006) user      (1006)    69704 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 user      (1006) user      (1006)     4782 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/options.py
+-rw-r--r--   0 user      (1006) user      (1006)    22553 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 user      (1006) user      (1006)     1582 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/proxy.py
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/py.typed
+-rw-r--r--   0 user      (1006) user      (1006)    26617 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 user      (1006) user      (1006)     9380 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/result_set.py
+-rw-r--r--   0 user      (1006) user      (1006)    21870 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     5343 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 user      (1006) user      (1006)     1957 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 user      (1006) user      (1006)     1120 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 user      (1006) user      (1006)    12449 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 user      (1006) user      (1006)     4313 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 user      (1006) user      (1006)      432 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 user      (1006) user      (1006)      813 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 user      (1006) user      (1006)     4563 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 user      (1006) user      (1006)    17583 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     8861 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 user      (1006) user      (1006)    19070 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 user      (1006) user      (1006)      982 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/test_util.py
+-rw-r--r--   0 user      (1006) user      (1006)     5073 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.392158 snowflake-connector-python-3.8.0/src/snowflake/connector/tool/
+-rw-r--r--   0 user      (1006) user      (1006)       76 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)     1485 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 user      (1006) user      (1006)     4575 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 user      (1006) user      (1006)     6643 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 user      (1006) user      (1006)     2119 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 user      (1006) user      (1006)     1021 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/url_util.py
+-rw-r--r--   0 user      (1006) user      (1006)    10405 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.392158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/
+-rw-r--r--   0 user      (1006) user      (1006)       76 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.396158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 user      (1006) user      (1006)    10142 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 user      (1006) user      (1006)     4742 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)      435 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 user      (1006) user      (1006)     1495 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 user      (1006) user      (1006)    19577 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 user      (1006) user      (1006)     6449 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 user      (1006) user      (1006)    10187 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 user      (1006) user      (1006)      429 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 user      (1006) user      (1006)     1451 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 user      (1006) user      (1006)    18560 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 user      (1006) user      (1006)     3813 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 user      (1006) user      (1006)     3885 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 user      (1006) user      (1006)      733 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 user      (1006) user      (1006)    35231 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 user      (1006) user      (1006)    30373 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 user      (1006) user      (1006)     4235 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 user      (1006) user      (1006)     2912 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 user      (1006) user      (1006)    33450 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.396158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 user      (1006) user      (1006)     1115 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 user      (1006) user      (1006)     2763 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    11372 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 user      (1006) user      (1006)       64 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 user      (1006) user      (1006)    20300 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 user      (1006) user      (1006)    40285 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.400158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)      957 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.400158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    17632 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 user      (1006) user      (1006)    13922 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 user      (1006) user      (1006)    11012 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 user      (1006) user      (1006)     4528 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 user      (1006) user      (1006)    16772 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 user      (1006) user      (1006)    34431 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 user      (1006) user      (1006)     7097 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 user      (1006) user      (1006)     8217 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 user      (1006) user      (1006)     8579 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 user      (1006) user      (1006)     2440 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.400158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.400158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)     1417 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 user      (1006) user      (1006)     5343 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0 user      (1006) user      (1006)    34665 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 user      (1006) user      (1006)    19990 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 user      (1006) user      (1006)     6691 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 user      (1006) user      (1006)    30760 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.404158 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 user      (1006) user      (1006)     1155 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)     5376 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 user      (1006) user      (1006)     1605 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 user      (1006) user      (1006)      498 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 user      (1006) user      (1006)     4225 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 user      (1006) user      (1006)     3510 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 user      (1006) user      (1006)    22013 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 user      (1006) user      (1006)    17165 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 user      (1006) user      (1006)     5758 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 user      (1006) user      (1006)     6895 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 user      (1006) user      (1006)    10168 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 user      (1006) user      (1006)    14279 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 user      (1006) user      (1006)     5403 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 user      (1006) user      (1006)      107 2024-04-04 16:53:52.000000 snowflake-connector-python-3.8.0/src/snowflake/connector/version.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-04 16:56:15.404158 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/
+-rw-r--r--   0 user      (1006) user      (1006)    61746 2024-04-04 16:56:15.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1006) user      (1006)    13218 2024-04-04 16:56:15.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1006) user      (1006)        1 2024-04-04 16:56:15.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1006) user      (1006)      322 2024-04-04 16:56:15.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1006) user      (1006)        1 2024-04-04 16:54:36.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1006) user      (1006)      646 2024-04-04 16:56:15.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1006) user      (1006)       10 2024-04-04 16:56:15.000000 snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-3.7.1/CONTRIBUTING.md` & `snowflake-connector-python-3.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/DESCRIPTION.md` & `snowflake-connector-python-3.8.0/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,34 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.8.0(April 04,2024)
+
+  - Improved `externalbrowser` auth in containerized environments
+    - Instruct browser to not fetch `/favicon` on success page
+    - Simple retry strategy on empty socket.recv
+    - Add `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true`) to set the underlying socket's `SO_REUSEPORT` flag (described in the [socket man page](https://man7.org/linux/man-pages/man7/socket.7.html))
+      - Useful when the randomized port used in the localhost callback url is being followed before the container engine completes port forwarding to host
+      - Statically map a port between your host and container and allow that port to be reused in rapid succession with:
+         `SF_AUTH_SOCKET_PORT=3037 SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true poetry run python somescript.py`
+    - Add `SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT=true`) to make a non-blocking socket.recv call and retry on Error
+      - Consider using this if running in a containerized environment and externalbrowser auth frequently hangs while waiting for callback
+      - NOTE: this has not been tested extensively, but has been shown to improve the experience when using WSL
+  - Added support for parsing structured type information in schema queries.
+  - Bumped platformdirs from >=2.6.0,<4.0.0 to >=2.6.0,<5.0.0
+  - Updated diagnostics to use system$allowlist instead of system$whitelist.
+  - Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode.
+  - Improved cleanup logic for connection to rely on interpreter shutdown instead of the `__del__` method.
+  - Updated the logging level from INFO to DEBUG when logging the executed query using `SnowflakeCursor.execute`.
+  - Fixed a bug that the truncated password in log is not masked.
+
 - v3.7.1(February 21, 2024)
 
   - Bumped pandas dependency from >=1.0.0,<2.2.0 to >=1.0.0,<3.0.0.
   - Bumped cryptography dependency from <42.0.0,>=3.1.0 to >=3.1.0,<43.0.0.
   - Bumped pyOpenSSL dependency from >=16.2.0,<24.0.0 to >=16.2.0,<25.0.0.
   - Fixed a memory leak in decimal data conversion.
   - Fixed a bug where `write_pandas` wasn't truncating the target table.
@@ -58,14 +78,15 @@
   - Added support for `use_logical_type` in `write_pandas`.
   - Removed dependencies on pycryptodomex and oscrypto. All connections now go through OpenSSL via the cryptography library, which was already a dependency.
   - Fixed issue with ingesting files over 80 GB to S3.
   - Added the `backoff_policy` argument to `snowflake.connector.connect` allowing for configurable backoff policy between retries of failed requests. See available implementations in the `backoff_policies` module.
   - Added the `socket_timeout` argument to `snowflake.connector.connect` specifying socket read and connect timeout.
   - Fixed `login_timeout` and `network_timeout` behaviour. Retries of login and network requests are now properly halted after these timeouts expire.
   - Fixed bug for issue https://github.com/urllib3/urllib3/issues/1878 in vendored `urllib`.
+  - Add User-Agent header for diagnostic report for tracking.
 
 - v3.3.1(October 16,2023)
 
   - Added for non-Windows platforms command suggestions (chown/chmod) for insufficient file permissions of config files.
   - Fixed issue with connection diagnostics failing to complete certificate checks.
   - Fixed issue that arrow iterator causes `ImportError` when the c extensions are not compiled.
```

### Comparing `snowflake-connector-python-3.7.1/LICENSE.txt` & `snowflake-connector-python-3.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/MANIFEST.in` & `snowflake-connector-python-3.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/PKG-INFO` & `snowflake-connector-python-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.7.1
+Version: 3.8.0
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
@@ -50,15 +50,15 @@
 Requires-Dist: charset_normalizer<4,>=2
 Requires-Dist: idna<4,>=2.5
 Requires-Dist: urllib3<2.0.0,>=1.21.1; python_version < "3.10"
 Requires-Dist: certifi>=2017.4.17
 Requires-Dist: typing_extensions<5,>=4.3
 Requires-Dist: filelock<4,>=3.5
 Requires-Dist: sortedcontainers>=2.4.0
-Requires-Dist: platformdirs<4.0.0,>=2.6.0
+Requires-Dist: platformdirs<5.0.0,>=2.6.0
 Requires-Dist: tomlkit
 Provides-Extra: development
 Requires-Dist: Cython; extra == "development"
 Requires-Dist: coverage; extra == "development"
 Requires-Dist: more-itertools; extra == "development"
 Requires-Dist: numpy<1.27.0; extra == "development"
 Requires-Dist: pendulum!=2.1.1; extra == "development"
@@ -81,14 +81,34 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.8.0(April 04,2024)
+
+  - Improved `externalbrowser` auth in containerized environments
+    - Instruct browser to not fetch `/favicon` on success page
+    - Simple retry strategy on empty socket.recv
+    - Add `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true`) to set the underlying socket's `SO_REUSEPORT` flag (described in the [socket man page](https://man7.org/linux/man-pages/man7/socket.7.html))
+      - Useful when the randomized port used in the localhost callback url is being followed before the container engine completes port forwarding to host
+      - Statically map a port between your host and container and allow that port to be reused in rapid succession with:
+         `SF_AUTH_SOCKET_PORT=3037 SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true poetry run python somescript.py`
+    - Add `SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT=true`) to make a non-blocking socket.recv call and retry on Error
+      - Consider using this if running in a containerized environment and externalbrowser auth frequently hangs while waiting for callback
+      - NOTE: this has not been tested extensively, but has been shown to improve the experience when using WSL
+  - Added support for parsing structured type information in schema queries.
+  - Bumped platformdirs from >=2.6.0,<4.0.0 to >=2.6.0,<5.0.0
+  - Updated diagnostics to use system$allowlist instead of system$whitelist.
+  - Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode.
+  - Improved cleanup logic for connection to rely on interpreter shutdown instead of the `__del__` method.
+  - Updated the logging level from INFO to DEBUG when logging the executed query using `SnowflakeCursor.execute`.
+  - Fixed a bug that the truncated password in log is not masked.
+
 - v3.7.1(February 21, 2024)
 
   - Bumped pandas dependency from >=1.0.0,<2.2.0 to >=1.0.0,<3.0.0.
   - Bumped cryptography dependency from <42.0.0,>=3.1.0 to >=3.1.0,<43.0.0.
   - Bumped pyOpenSSL dependency from >=16.2.0,<24.0.0 to >=16.2.0,<25.0.0.
   - Fixed a memory leak in decimal data conversion.
   - Fixed a bug where `write_pandas` wasn't truncating the target table.
@@ -135,14 +155,15 @@
   - Added support for `use_logical_type` in `write_pandas`.
   - Removed dependencies on pycryptodomex and oscrypto. All connections now go through OpenSSL via the cryptography library, which was already a dependency.
   - Fixed issue with ingesting files over 80 GB to S3.
   - Added the `backoff_policy` argument to `snowflake.connector.connect` allowing for configurable backoff policy between retries of failed requests. See available implementations in the `backoff_policies` module.
   - Added the `socket_timeout` argument to `snowflake.connector.connect` specifying socket read and connect timeout.
   - Fixed `login_timeout` and `network_timeout` behaviour. Retries of login and network requests are now properly halted after these timeouts expire.
   - Fixed bug for issue https://github.com/urllib3/urllib3/issues/1878 in vendored `urllib`.
+  - Add User-Agent header for diagnostic report for tracking.
 
 - v3.3.1(October 16,2023)
 
   - Added for non-Windows platforms command suggestions (chown/chmod) for insufficient file permissions of config files.
   - Fixed issue with connection diagnostics failing to complete certificate checks.
   - Fixed issue that arrow iterator causes `ImportError` when the c extensions are not compiled.
```

### Comparing `snowflake-connector-python-3.7.1/README.md` & `snowflake-connector-python-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/pyproject.toml` & `snowflake-connector-python-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/setup.cfg` & `snowflake-connector-python-3.8.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 	charset_normalizer>=2,<4
 	idna>=2.5,<4
 	urllib3>=1.21.1,<2.0.0; python_version < '3.10'
 	certifi>=2017.4.17
 	typing_extensions>=4.3,<5
 	filelock>=3.5,<4
 	sortedcontainers>=2.4.0
-	platformdirs>=2.6.0,<4.0.0
+	platformdirs>=2.6.0,<5.0.0
 	tomlkit
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
```

### Comparing `snowflake-connector-python-3.7.1/setup.py` & `snowflake-connector-python-3.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/__init__.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/auth/webbrowser.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from __future__ import annotations
 
 import base64
 import json
 import logging
 import os
 import secrets
+import select
 import socket
 import time
 import webbrowser
 from types import ModuleType
 from typing import TYPE_CHECKING, Any
 
-from ..compat import parse_qs, urlencode, urlparse, urlsplit
+from ..compat import IS_WINDOWS, parse_qs, urlencode, urlparse, urlsplit
 from ..constants import (
     HTTP_HEADER_ACCEPT,
     HTTP_HEADER_CONTENT_TYPE,
     HTTP_HEADER_SERVICE_NAME,
     HTTP_HEADER_USER_AGENT,
 )
 from ..errorcode import (
@@ -112,14 +113,23 @@
         user: str,
         **kwargs: Any,
     ) -> None:
         """Web Browser based Authentication."""
         logger.debug("authenticating by Web Browser")
 
         socket_connection = self._socket(socket.AF_INET, socket.SOCK_STREAM)
+
+        if os.getenv("SNOWFLAKE_AUTH_SOCKET_REUSE_PORT", "False").lower() == "true":
+            if IS_WINDOWS:
+                logger.warning(
+                    "Configuration SNOWFLAKE_AUTH_SOCKET_REUSE_PORT is not available in Windows. Ignoring."
+                )
+            else:
+                socket_connection.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+
         try:
             try:
                 socket_connection.bind(
                     (
                         os.getenv("SF_AUTH_SOCKET_ADDR", "localhost"),
                         int(os.getenv("SF_AUTH_SOCKET_PORT", 0)),
                     )
@@ -201,22 +211,76 @@
     ) -> dict[str, bool]:
         conn.authenticate_with_retry(self)
         return {"success": True}
 
     def _receive_saml_token(self, conn: SnowflakeConnection, socket_connection) -> None:
         """Receives SAML token from web browser."""
         while True:
-            socket_client, _ = socket_connection.accept()
             try:
-                # Receive the data in small chunks and retransmit it
-                data = socket_client.recv(BUF_SIZE).decode("utf-8").split("\r\n")
+                attempts = 0
+                raw_data = bytearray()
+                socket_client = None
+                max_attempts = 15
+
+                msg_dont_wait = (
+                    os.getenv("SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT", "false").lower()
+                    == "true"
+                )
+                if IS_WINDOWS:
+                    if msg_dont_wait:
+                        logger.warning(
+                            "Configuration SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT is not available in Windows. Ignoring."
+                        )
+                    msg_dont_wait = False
+
+                # when running in a containerized environment, socket_client.recv ocassionally returns an empty byte array
+                #   an immediate successive call to socket_client.recv gets the actual data
+                while len(raw_data) == 0 and attempts < max_attempts:
+                    attempts += 1
+                    read_sockets, _write_sockets, _exception_sockets = select.select(
+                        [socket_connection], [], []
+                    )
+
+                    if read_sockets[0] is not None:
+                        # Receive the data in small chunks and retransmit it
+                        socket_client, _ = socket_connection.accept()
+
+                        try:
+                            if msg_dont_wait:
+                                # WSL containerized environment sometimes causes socket_client.recv to hang indefinetly
+                                #   To avoid this, passing the socket.MSG_DONTWAIT flag which raises BlockingIOError if
+                                #   operation would block
+                                logger.debug(
+                                    "Calling socket_client.recv with MSG_DONTWAIT flag due to SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT env var"
+                                )
+                                raw_data = socket_client.recv(
+                                    BUF_SIZE, socket.MSG_DONTWAIT
+                                )
+                            else:
+                                raw_data = socket_client.recv(BUF_SIZE)
+
+                        except BlockingIOError:
+                            logger.debug(
+                                "BlockingIOError raised from socket.recv while attempting to retrieve callback token request"
+                            )
+                            if attempts < max_attempts:
+                                sleep_time = 0.25
+                                logger.debug(
+                                    f"Waiting {sleep_time} seconds before trying again"
+                                )
+                                time.sleep(sleep_time)
+                            else:
+                                logger.debug("Exceeded retry count")
+
+                data = raw_data.decode("utf-8").split("\r\n")
 
                 if not self._process_options(data, socket_client):
                     self._process_receive_saml_token(conn, data, socket_client)
                     break
+
             finally:
                 socket_client.shutdown(socket.SHUT_RDWR)
                 socket_client.close()
 
     def _process_options(self, data: list[str], socket_client: socket.socket) -> bool:
         """Allows JS Ajax access to this endpoint."""
         for line in data:
@@ -278,14 +342,15 @@
             data = {"consent": self.consent_cache_id_token}
             msg = json.dumps(data)
             content.append(f"Access-Control-Allow-Origin: {self._origin}")
             content.append("Vary: Accept-Encoding, Origin")
         else:
             msg = f"""
 <!DOCTYPE html><html><head><meta charset="UTF-8"/>
+<link rel="icon" href="data:,">
 <title>SAML Response for Snowflake</title></head>
 <body>
 Your identity was confirmed and propagated to Snowflake {self._application}.
 You can close this window now and go back where you started from.
 </body></html>"""
         content.append(f"Content-Length: {len(msg)}")
         content.append("")
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/backoff_policies.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/backoff_policies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/cache.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/compat.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/config_manager.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/config_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/connection.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
+import atexit
 import logging
 import os
 import pathlib
 import re
 import sys
 import traceback
 import uuid
 import warnings
 import weakref
 from concurrent.futures import as_completed
 from concurrent.futures.thread import ThreadPoolExecutor
+from contextlib import suppress
 from difflib import get_close_matches
 from functools import partial
 from io import StringIO
 from logging import getLogger
 from threading import Lock
 from time import strptime
 from types import TracebackType
@@ -120,16 +122,18 @@
         from .converter import SnowflakeConverter
 
         return SnowflakeConverter
 
 
 def _get_private_bytes_from_file(
     private_key_file: str | bytes | os.PathLike[str] | os.PathLike[bytes],
-    private_key_file_pwd: bytes | None = None,
+    private_key_file_pwd: bytes | str | None = None,
 ) -> bytes:
+    if private_key_file_pwd is not None and isinstance(private_key_file_pwd, str):
+        private_key_file_pwd = private_key_file_pwd.encode("utf-8")
     with open(private_key_file, "rb") as key:
         private_key = serialization.load_pem_private_key(
             key.read(),
             password=private_key_file_pwd,
             backend=default_backend(),
         )
 
@@ -174,15 +178,15 @@
     ),  # network timeout (infinite by default)
     "socket_timeout": (None, (type(None), int)),
     "backoff_policy": (DEFAULT_BACKOFF_POLICY, Callable),
     "passcode_in_password": (False, bool),  # Snowflake MFA
     "passcode": (None, (type(None), str)),  # Snowflake MFA
     "private_key": (None, (type(None), str, RSAPrivateKey)),
     "private_key_file": (None, (type(None), str)),
-    "private_key_file_pwd": (None, (type(None), str)),
+    "private_key_file_pwd": (None, (type(None), str, bytes)),
     "token": (None, (type(None), str)),  # OAuth or JWT Token
     "authenticator": (DEFAULT_AUTHENTICATOR, (type(None), str)),
     "mfa_callback": (None, (type(None), Callable)),
     "password_callback": (None, (type(None), Callable)),
     "auth_class": (None, (type(None), AuthByPlugin)),
     "application": (CLIENT_NAME, (type(None), str)),
     "internal_application_name": (CLIENT_NAME, (type(None), str)),
@@ -231,15 +235,19 @@
     "connection_diag_log_path": (
         None,
         (type(None), str),
     ),  # Path to connection diag report
     "connection_diag_whitelist_path": (
         None,
         (type(None), str),
-    ),  # Path to connection diag whitelist json
+    ),  # Path to connection diag whitelist json - Deprecated remove in future
+    "connection_diag_allowlist_path": (
+        None,
+        (type(None), str),
+    ),  # Path to connection diag allowlist json
     "log_imported_packages_in_telemetry": (
         True,
         bool,
     ),  # Whether to log imported packages in telemetry
     "disable_query_context_cache": (
         False,
         bool,
@@ -339,15 +347,16 @@
         converter_class: Handler used to convert data to Python native objects.
         validate_default_parameters: Validate database, schema, role and warehouse used on Snowflake.
         is_pyformat: Whether the current argument binding is pyformat or format.
         consent_cache_id_token: Consented cache ID token.
         enable_stage_s3_privatelink_for_us_east_1: when true, clients use regional s3 url to upload files.
         enable_connection_diag: when true, clients will generate a connectivity diagnostic report.
         connection_diag_log_path: path to location to create diag report with enable_connection_diag.
-        connection_diag_whitelist_path: path to a whitelist.json file to test with enable_connection_diag.
+        connection_diag_whitelist_path: path to a whitelist.json file to test with enable_connection_diag - deprecated remove in future
+        connection_diag_allowlist_path: path to a allowlist.json file to test with enable_connection_diag.
         json_result_force_utf8_decoding: When true, json result will be decoded in utf-8,
           when false, the encoding of the content is auto-detected. Default value is false.
           This parameter is only effective when the result format is JSON.
         server_session_keep_alive: When true, the connector does not destroy the session on the Snowflake server side
           before the connector shuts down. Default value is false.
     """
 
@@ -428,20 +437,16 @@
         self.__set_error_attributes()
         self.connect(**kwargs)
         self._telemetry = TelemetryClient(self._rest)
         self.expired = False
 
         # get the imported modules from sys.modules
         self._log_telemetry_imported_packages()
-
-    def __del__(self) -> None:  # pragma: no cover
-        try:
-            self.close(retry=False)
-        except Exception:
-            pass
+        # check SNOW-1218851 for long term improvement plan to refactor ocsp code
+        atexit.register(self._close_at_exit)
 
     @property
     def insecure_mode(self) -> bool:
         return self._insecure_mode
 
     @property
     def ocsp_fail_open(self) -> bool:
@@ -651,16 +656,31 @@
 
     @property
     def connection_diag_log_path(self):
         return self._connection_diag_log_path
 
     @property
     def connection_diag_whitelist_path(self):
+        """
+        Old version of ``connection_diag_allowlist_path``.
+        This used to be the original name, but snowflake backend
+        deprecated whitelist for allowlist. This name will be
+        deprecated in the future.
+        """
+        warnings.warn(
+            "connection_diag_whitelist_path has been deprecated, use connection_diag_allowlist_path instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._connection_diag_whitelist_path
 
+    @property
+    def connection_diag_allowlist_path(self):
+        return self._connection_diag_allowlist_path
+
     @arrow_number_to_decimal.setter
     def arrow_number_to_decimal_setter(self, value: bool) -> None:
         self._arrow_number_to_decimal = value
 
     @property
     def auth_class(self) -> AuthByPlugin | None:
         return self._auth_class
@@ -685,15 +705,17 @@
 
         if self.enable_connection_diag:
             exceptions_dict = {}
             connection_diag = ConnectionDiagnostic(
                 account=self.account,
                 host=self.host,
                 connection_diag_log_path=self.connection_diag_log_path,
-                connection_diag_whitelist_path=self.connection_diag_whitelist_path,
+                connection_diag_allowlist_path=self.connection_diag_allowlist_path
+                if self.connection_diag_allowlist_path is not None
+                else self.connection_diag_whitelist_path,
                 proxy_host=self.proxy_host,
                 proxy_port=self.proxy_port,
                 proxy_user=self.proxy_user,
                 proxy_password=self.proxy_password,
             )
             try:
                 connection_diag.run_test()
@@ -716,14 +738,16 @@
                 if exceptions_dict:
                     raise Exception(str(exceptions_dict))
         else:
             self.__open_connection()
 
     def close(self, retry: bool = True) -> None:
         """Closes the connection."""
+        # unregister to dereference connection object as it's already closed after the execution
+        atexit.unregister(self._close_at_exit)
         try:
             if not self.rest:
                 logger.debug("Rest object has been destroyed, cannot close session")
                 return
 
             # will hang if the application doesn't close the connection and
             # CLIENT_SESSION_KEEP_ALIVE is set, because the heartbeat runs on
@@ -1743,14 +1767,18 @@
         # If query was started by us and it has finished let's cache this info
         if sf_qid in self._async_sfqids and not self.is_still_running(status_ret):
             self._async_sfqids.pop(
                 sf_qid, None
             )  # Prevent KeyError when multiple threads try to remove the same query id
             self._done_async_sfqids[sf_qid] = None
 
+    def _close_at_exit(self):
+        with suppress(Exception):
+            self.close(retry=False)
+
     def get_query_status(self, sf_qid: str) -> QueryStatus:
         """Retrieves the status of query with sf_qid.
 
         Query status is returned as a QueryStatus.
 
         Args:
             sf_qid: Snowflake query id of interest.
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/connection_diagnostic.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,51 +14,64 @@
 import tempfile
 from datetime import datetime
 from logging import getLogger
 from pathlib import Path
 from typing import Any, AnyStr
 from urllib.request import getproxies
 
+import certifi
 import OpenSSL
 
 from .compat import IS_WINDOWS, urlparse
 from .cursor import SnowflakeCursor
 from .vendored import urllib3
 
 logger = getLogger(__name__)
 
 if IS_WINDOWS:
     import winreg
 
 
-def _decode_dict(d):
-    result = {}
+def _decode_dict(d: dict[str, dict[str, Any]]):
+    result: dict[str, dict[str, Any]] = {}
     for key, value in d.items():
         if isinstance(key, bytes):
             key = key.decode()
         if isinstance(value, bytes):
             value = value.decode()
         elif isinstance(value, dict):
             value = _decode_dict(value)
         result.update({key: value})
     return result
 
 
+def _is_list_of_json_objects(allowlist: List[Dict[str, Any]]):
+    if isinstance(allowlist, list) and all(
+        isinstance(item, dict) for item in allowlist
+    ):
+        try:
+            json.dumps(allowlist)
+            return True
+        except TypeError:
+            return False
+    return False
+
+
 class ConnectionDiagnostic:
     """Implementation of a connection test utility for Snowflake connector
 
     Use new ConnectionTest() to get the object.
     """
 
     def __init__(
         self,
         account: str,
         host: str,
         connection_diag_log_path: str | None = None,
-        connection_diag_whitelist_path: str | None = None,
+        connection_diag_allowlist_path: str | None = None,
         proxy_host: str | None = None,
         proxy_port: str | None = None,
         proxy_user: str | None = None,
         proxy_password: str | None = None,
     ) -> None:
         self.account = account
         self.host = host
@@ -113,17 +126,17 @@
         ) = self.__parse_proxy(proxy_url)
         self.__https_host_report(self.host)
         self.full_connection_diag_log_path: Path | None = (
             Path(connection_diag_log_path)
             if connection_diag_log_path is not None
             else None
         )
-        self.full_connection_diag_whitelist_path: Path | None = (
-            Path(connection_diag_whitelist_path)
-            if connection_diag_whitelist_path is not None
+        self.full_connection_diag_allowlist_path: Path | None = (
+            Path(connection_diag_allowlist_path)
+            if connection_diag_allowlist_path is not None
             else None
         )
         self.tmpdir: str = tempfile.gettempdir()
         if self.full_connection_diag_log_path is None:
             self.full_connection_diag_log_path = Path(self.tmpdir)
         else:
             if not self.full_connection_diag_log_path.is_absolute():
@@ -138,43 +151,43 @@
                 self.full_connection_diag_log_path = Path(self.tmpdir)
 
         self.report_file: Path = (
             self.full_connection_diag_log_path / "SnowflakeConnectionTestReport.txt"
         )
         logger.info(f"Reporting to file {self.report_file}")
 
-        if self.full_connection_diag_whitelist_path is not None:
-            if not self.full_connection_diag_whitelist_path.is_absolute():
+        if self.full_connection_diag_allowlist_path is not None:
+            if not self.full_connection_diag_allowlist_path.is_absolute():
                 logger.warning(
-                    f"Path '{self.full_connection_diag_whitelist_path}' for connection test whitelist is not absolute."
+                    f"Path '{self.full_connection_diag_allowlist_path}' for connection test allowlist is not absolute."
                 )
                 logger.warning(
-                    "Will connect to Snowflake for whitelist json instead.  If you did not provide a valid "
+                    "Will connect to Snowflake for allowlist json instead.  If you did not provide a valid "
                     "password, please make sure to update and run again."
                 )
-                self.full_connection_diag_whitelist_path = None
-            elif not self.full_connection_diag_whitelist_path.exists():
+                self.full_connection_diag_allowlist_path = None
+            elif not self.full_connection_diag_allowlist_path.exists():
                 logger.warning(
-                    f"File '{self.full_connection_diag_whitelist_path}' for connection test whitelist does not exist."
+                    f"File '{self.full_connection_diag_allowlist_path}' for connection test allowlist does not exist."
                 )
                 logger.warning(
-                    "Will connect to Snowflake for whitelist json instead.  If you did not provide a valid "
+                    "Will connect to Snowflake for allowlist json instead.  If you did not provide a valid "
                     "password, please make sure to update and run again."
                 )
-                self.full_connection_diag_whitelist_path = None
+                self.full_connection_diag_allowlist_path = None
 
-        self.whitelist_sql: str = "select /* snowflake-connector-python:connection_diagnostics */ system$whitelist();"
+        self.allowlist_sql: str = "select /* snowflake-connector-python:connection_diagnostics */ system$allowlist();"
 
         if self.__is_privatelink():
             self.ocsp_urls.append(f"ocsp.{self.host}")
-            self.whitelist_sql = "select system$whitelist_privatelink();"
+            self.allowlist_sql = "select system$allowlist_privatelink();"
         else:
             self.ocsp_urls.append("ocsp.snowflakecomputing.com")
 
-        self.whitelist_retrieval_success: bool = False
+        self.allowlist_retrieval_success: bool = False
         self.cursor: SnowflakeCursor | None = None
 
     def __parse_proxy(self, proxy_url: str) -> tuple[str, str, str, str]:
         parsed = urlparse(proxy_url)
         proxy_host = parsed.hostname
         proxy_port = parsed.port
         proxy_user = parsed.username
@@ -208,16 +221,28 @@
                 if self.proxy_host is not None:
                     connect = f"CONNECT {host}:{port} HTTP/1.1\r\n{connect_creds}"
                     connect = f"{connect}Host: {host}\r\n\r\n"
                     conn.send(str.encode(connect))
                     conn.recv(4096).decode("utf-8")
 
                 context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+                context.load_verify_locations(certifi.where())
                 sock = context.wrap_socket(conn, server_hostname=host)
                 certificate = ssl.DER_cert_to_PEM_cert(sock.getpeercert(True))
+                http_request = f"""GET / {host}:{port} HTTP/1.1\r\n
+                                   Host: {host}\r\n
+                                   User-Agent: snowflake-connector-python-diagnostic
+                                   \r\n\r\n"""
+                try:
+                    sock.send(str.encode(http_request))
+                except Exception as e:
+                    self.__append_message(
+                        host_type,
+                        f"{host}:{port}: URL Check: Failed: Unknown Exception: {e}",
+                    )
                 conn.close()
                 return certificate
             else:
                 if self.proxy_host is not None:
                     connect = (
                         f"CONNECT {host}:{port} HTTP/1.1\r\n{connect_creds}\r\n\r\n"
                     )
@@ -256,45 +281,60 @@
 
         self.__append_message(
             host_type, f"{host}:{port}: URL Check: Connected Successfully"
         )
         return "SUCCESS"
 
     def run_post_test(self) -> None:
-        results: list[str] = []
-        if self.full_connection_diag_whitelist_path is None:
+        results: list[str] = None
+        if self.full_connection_diag_allowlist_path is None:
             if self.cursor is not None:
                 try:
                     results = self.cursor.execute(
-                        self.whitelist_sql, _is_internal=True
+                        self.allowlist_sql, _is_internal=True
                     ).fetchall()[0][0]
                     results = json.loads(str(results))
-                    self.whitelist_retrieval_success = True
+                    self.allowlist_retrieval_success = True
                 except Exception as e:
-                    logger.warning(f"Unable to do whitelist checks: exception: {e}")
+                    logger.warning(f"Unable to do allowlist checks: exception: {e}")
         else:
-            results_file = open(self.full_connection_diag_whitelist_path)
-            results = json.load(results_file)
-            self.whitelist_retrieval_success = True
-
-        for result in results:
-            host_type = result["type"]
-            host = result["host"]
-            host_port = result["port"]
-
-            if host_type in ("OCSP_RESPONDER"):
-                if host not in self.ocsp_urls:
-                    self.__test_socket_get_cert(
-                        host, port=host_port, host_type=host_type
-                    )
-            elif host_type in ("STAGE", "OUT_OF_BAND_TELEMETRY"):
-                try:
-                    self.__https_host_report(host, port=host_port, host_type=host_type)
-                except Exception:
-                    pass
+            results_file = open(self.full_connection_diag_allowlist_path)
+            try:
+                results = json.load(results_file)
+                self.allowlist_retrieval_success = True
+            except Exception as e:
+                self.__append_message(
+                    "INITIAL",
+                    f"Allowlist was not valid json: '{e}'.  Please run 'select system$allowlist();' and validate the file {self.full_connection_diag_allowlist_path} is correct.",
+                )
+                pass
+
+        if _is_list_of_json_objects(results):
+            for result in results:
+                host_type = result["type"]
+                host = result["host"]
+                host_port = result["port"]
+
+                if host_type in ("OCSP_RESPONDER"):
+                    if host not in self.ocsp_urls:
+                        self.__test_socket_get_cert(
+                            host, port=host_port, host_type=host_type
+                        )
+                elif host_type in ("STAGE", "OUT_OF_BAND_TELEMETRY"):
+                    try:
+                        self.__https_host_report(
+                            host, port=host_port, host_type=host_type
+                        )
+                    except Exception:
+                        pass
+        else:
+            self.__append_message(
+                "INITIAL",
+                "Allowlist is not a valid list of json objects. Please run 'select system$allowlist();' and provide as a json file using the connection_diag_allowlist_path option.",
+            )
 
     def __is_privatelink(self) -> bool:
         return "privatelink" in self.host
 
     def __list_ips(self, host: str, host_type: str = "SNOWFLAKE_URL") -> None:
         try:
             ips = socket.gethostbyname_ex(host)[2]
@@ -486,31 +526,33 @@
         cert_authorities = (
             "C=US; O=Google Trust Services LLC",
             "C=US; O=Amazon",
             "C=US; O=DigiCert Inc",
         )
 
         check_pattern = f"(^{'|^'.join(cert_authorities)})"
-        issuer = self.__get_issuer_string(self.cert_info[self.host]["issuer"])
-        if not re.search(check_pattern, issuer):
-            self.__append_message(
-                host_type,
-                f"There is likely a proxy because the issuer for {self.host} is "
-                f"not correct. Got {issuer} and expected one of {cert_authorities}",
-            )
+        if self.host in self.cert_info.keys():
+            issuer = self.__get_issuer_string(self.cert_info[self.host]["issuer"])
+            if not re.search(check_pattern, issuer):
+                self.__append_message(
+                    host_type,
+                    f"There is likely a proxy because the issuer for {self.host} is "
+                    f"not correct. Got {issuer} and expected one of {cert_authorities}",
+                )
 
         test_host = "www.google.com"
         self.__https_host_report(test_host, port=443, host_type="IGNORE")
-        issuer = self.__get_issuer_string(self.cert_info[test_host]["issuer"])
-        if not re.search(check_pattern, issuer):
-            self.__append_message(
-                host_type,
-                f"There is likely a proxy because the issuer for {test_host} is "
-                f"not correct. Got {issuer} and expected one of {cert_authorities}",
-            )
+        if test_host in self.cert_info.keys():
+            issuer = self.__get_issuer_string(self.cert_info[test_host]["issuer"])
+            if not re.search(check_pattern, issuer):
+                self.__append_message(
+                    host_type,
+                    f"There is likely a proxy because the issuer for {test_host} is "
+                    f"not correct. Got {issuer} and expected one of {cert_authorities}",
+                )
 
         # Get Windows proxy info from Registry just in case:
         if IS_WINDOWS:
             registry_start_key = "Software\\Microsoft\\Windows\\CurrentVersion"
             hkey_strings = ["HKEY_CURRENT_USER", "HKEY_LOCAL_MACHINE"]
             for hkey_str in hkey_strings:
                 self.__walk_win_registry(host_type, hkey_str, registry_start_key)
@@ -580,50 +622,50 @@
         snowflake_url_joined_results = "\n".join(self.test_results["SNOWFLAKE_URL"])
         message = (
             f"{message}\n"
             "=========Snowflake URL information=====================================\n"
             f"{snowflake_url_joined_results}\n"
         )
 
-        if self.whitelist_retrieval_success:
+        if self.allowlist_retrieval_success:
             snowflake_stage_joined_results = "\n".join(self.test_results["STAGE"])
             message = (
                 f"{message}\n"
                 "=========Snowflake Stage information===================================\n"
-                "We retrieved stage info from the whitelist\n"
+                "We retrieved stage info from the allowlist\n"
                 f"{snowflake_stage_joined_results}\n"
             )
         else:
             message = (
                 f"{message}\n"
                 "=========Snowflake Stage information - Unavailable=====================\n"
-                "We could not connect to Snowflake to get whitelist, so we do not have stage\n"
+                "We could not connect to Snowflake to get allowlist, so we do not have stage\n"
                 f"diagnostic info\n"
             )
 
         message = (
             f"{message}\n"
             "=========Snowflake OCSP information===================================="
         )
         snowflake_ocsp_joined_results = "\n".join(self.test_results["OCSP_RESPONDER"])
-        if self.whitelist_retrieval_success:
+        if self.allowlist_retrieval_success:
             message = (
                 f"{message}\n"
-                "We were able to retrieve system whitelist.\n"
-                "These OCSP hosts came from the certificate and the whitelist."
+                "We were able to retrieve system allowlist.\n"
+                "These OCSP hosts came from the certificate and the allowlist."
             )
         else:
             message = (
                 f"{message}\n"
-                "We were unable to retrieve system whitelist.\n"
+                "We were unable to retrieve system allowlist.\n"
                 "These OCSP hosts only came from the certificate."
             )
         message = f"{message}\n" f"{snowflake_ocsp_joined_results}\n"
 
-        if self.whitelist_retrieval_success:
+        if self.allowlist_retrieval_success:
             snowflake_telemetry_joined_results = "\n".join(
                 self.test_results["OUT_OF_BAND_TELEMETRY"]
             )
             message = (
                 f"{message}\n"
                 "=========Snowflake Out of bound telemetry check========================\n"
                 f"{snowflake_telemetry_joined_results}\n"
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/constants.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,46 +40,83 @@
 class FieldType(NamedTuple):
     name: str
     dbapi_type: list[int]
     pa_type: Callable[[ResultMetadataV2], DataType]
 
 
 def vector_pa_type(metadata: ResultMetadataV2) -> DataType:
-    """Generate the Arrow type represented by the given vector column metadata.
-
+    """
+    Generate the Arrow type represented by the given vector column metadata.
     Vectors are represented as Arrow fixed-size lists.
     """
+    assert (
+        metadata.fields is not None and len(metadata.fields) == 1
+    ), "Invalid result metadata for vector type: expected a single field to be defined"
+    assert (
+        metadata.vector_dimension or 0
+    ) > 0, "Invalid result metadata for vector type: expected a positive dimension"
+
+    field_type = FIELD_TYPES[metadata.fields[0].type_code]
+    return pa.list_(field_type.pa_type(metadata.fields[0]), metadata.vector_dimension)
+
+
+def array_pa_type(metadata: ResultMetadataV2) -> DataType:
+    """
+    Generate the Arrow type represented by the given array column metadata.
+    """
+    # If fields is missing then structured types are not enabled.
+    # Fallback to json encoded string
+    if metadata.fields is None:
+        return pa.string()
+
+    assert (
+        len(metadata.fields) == 1
+    ), "Invalid result metadata for array type: expected a single field to be defined"
+
+    field_type = FIELD_TYPES[metadata.fields[0].type_code]
+    return pa.list_(field_type.pa_type(metadata.fields[0]))
+
+
+def map_pa_type(metadata: ResultMetadataV2) -> DataType:
+    """
+    Generate the Arrow type represented by the given map column metadata.
+    """
+    # If fields is missing then structured types are not enabled.
+    # Fallback to json encoded string
+    if metadata.fields is None:
+        return pa.string()
 
+    assert (
+        len(metadata.fields or []) == 2
+    ), "Invalid result metadata for map type: expected a field for key and a field for value"
+    key_type = FIELD_TYPES[metadata.fields[0].type_code]
+    value_type = FIELD_TYPES[metadata.fields[1].type_code]
+    return pa.map_(
+        key_type.pa_type(metadata.fields[0]), value_type.pa_type(metadata.fields[1])
+    )
+
+
+def struct_pa_type(metadata: ResultMetadataV2) -> DataType:
+    """
+    Generate the Arrow type represented by the given struct column metadata.
+    """
+    # If fields is missing then structured types are not enabled.
+    # Fallback to json encoded string
     if metadata.fields is None:
-        raise ValueError(
-            "Invalid result metadata for vector type: expected sub-field metadata"
-        )
-    if len(metadata.fields) != 1:
-        raise ValueError(
-            "Invalid result metadata for vector type: expected a single sub-field metadata"
-        )
-    field_type = FIELD_ID_TO_NAME[metadata.fields[0].type_code]
-
-    if metadata.vector_dimension is None:
-        raise ValueError(
-            "Invalid result metadata for vector type: expected a dimension"
-        )
-    elif metadata.vector_dimension <= 0:
-        raise ValueError(
-            "Invalid result metadata for vector type: expected a positive dimension"
-        )
-
-    if field_type == "FIXED":
-        return pa.list_(pa.int32(), metadata.vector_dimension)
-    elif field_type == "REAL":
-        return pa.list_(pa.float32(), metadata.vector_dimension)
-    else:
-        raise ValueError(
-            f"Invalid result metadata for vector type: invalid element type: {field_type}"
-        )
+        return pa.string()
+
+    assert all(
+        field.name is not None for field in metadata.fields
+    ), "All fields of a stuct type must have a name."
+    return pa.struct(
+        {
+            field.name: FIELD_TYPES[field.type_code].pa_type(field)
+            for field in metadata.fields
+        }
+    )
 
 
 # This type mapping holds column type definitions.
 #  Be careful to not change the ordering as the index is what Snowflake
 #  gives to as schema
 #
 # `name` is the SQL name of the type, `dbapi_type` is the set of corresponding
@@ -117,20 +154,16 @@
         pa_type=lambda _: pa.timestamp("ns"),
     ),
     FieldType(
         name="TIMESTAMP_NTZ",
         dbapi_type=[DBAPI_TYPE_TIMESTAMP],
         pa_type=lambda _: pa.timestamp("ns"),
     ),
-    FieldType(
-        name="OBJECT", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=lambda _: pa.string()
-    ),
-    FieldType(
-        name="ARRAY", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=lambda _: pa.string()
-    ),
+    FieldType(name="OBJECT", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=struct_pa_type),
+    FieldType(name="ARRAY", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=array_pa_type),
     FieldType(
         name="BINARY", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=lambda _: pa.binary()
     ),
     FieldType(
         name="TIME",
         dbapi_type=[DBAPI_TYPE_TIMESTAMP],
         pa_type=lambda _: pa.time64("ns"),
@@ -139,14 +172,15 @@
     FieldType(
         name="GEOGRAPHY", dbapi_type=[DBAPI_TYPE_STRING], pa_type=lambda _: pa.string()
     ),
     FieldType(
         name="GEOMETRY", dbapi_type=[DBAPI_TYPE_STRING], pa_type=lambda _: pa.string()
     ),
     FieldType(name="VECTOR", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=vector_pa_type),
+    FieldType(name="MAP", dbapi_type=[DBAPI_TYPE_BINARY], pa_type=map_pa_type),
 )
 
 FIELD_NAME_TO_ID: DefaultDict[Any, int] = defaultdict(int)
 FIELD_ID_TO_NAME: DefaultDict[int, str] = defaultdict(str)
 
 __binary_types: list[int] = []
 __binary_type_names: list[str] = []
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/converter.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/cursor.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,79 +161,16 @@
             col["length"],
             col["precision"],
             col["scale"],
             col["nullable"],
         )
 
 
-class ResultMetadataV2Field:
-    """ResultMetadataV2Field represents the type information of one sub-type in a nested type."""
-
-    def __init__(
-        self,
-        type_code: int,
-        is_nullable: bool,
-        internal_size: int | None = None,
-        precision: int | None = None,
-        scale: int | None = None,
-        fields: list[ResultMetadataV2] | None = None,
-    ):
-        self._type_code = type_code
-        self._is_nullable = is_nullable
-        self._internal_size = internal_size
-        self._precision = precision
-        self._scale = scale
-        self._fields = fields
-
-    @classmethod
-    def from_column(cls, col: dict[str, Any]) -> ResultMetadataV2Field:
-        """Initializes a ResultMetadataV2Field object from a child of the column description in the query response."""
-        fields = None
-        if col.get("fields") is not None:
-            fields = [cls.from_column(f) for f in col["fields"]]
-        return cls(
-            FIELD_NAME_TO_ID[
-                col["extTypeName"].upper()
-                if col.get("extTypeName")
-                else col["type"].upper()
-            ],
-            col["nullable"],
-            col["length"],
-            col["precision"],
-            col["scale"],
-            fields,
-        )
-
-    @property
-    def type_code(self) -> int:
-        return self._type_code
-
-    @property
-    def is_nullable(self) -> bool:
-        return self._is_nullable
-
-    @property
-    def internal_size(self) -> int | None:
-        return self._internal_size
-
-    @property
-    def precision(self) -> int | None:
-        return self._precision
-
-    @property
-    def scale(self) -> int | None:
-        return self._scale
-
-    @property
-    def fields(self) -> list[ResultMetadataV2Field] | None:
-        return self._fields
-
-
 class ResultMetadataV2:
-    """ResultMetadataV2Field represents the type information of a single column.
+    """ResultMetadataV2 represents the type information of a single column.
 
     It is a replacement for ResultMetadata that contains additional attributes, currently
     `vector_dimension` and `fields`. This class will be unified with ResultMetadata in the
     near future.
     """
 
     def __init__(
@@ -260,34 +197,43 @@
 
     @classmethod
     def from_column(cls, col: dict[str, Any]) -> ResultMetadataV2:
         """Initializes a ResultMetadataV2 object from the column description in the query response.
         This differs from ResultMetadata in that it has newly-added fields which cannot be added to
         ResultMetadata since it is a named tuple.
         """
-        type_code = FIELD_NAME_TO_ID[
+        col_type = (
             col["extTypeName"].upper()
             if col.get("extTypeName")
             else col["type"].upper()
-        ]
+        )
 
-        fields = None
-        if type_code == FIELD_NAME_TO_ID["VECTOR"] and col.get("fields") is not None:
-            fields = [ResultMetadataV2Field.from_column(f) for f in col["fields"]]
+        fields = col.get("fields")
+        processed_fields: Optional[List[ResultMetadataV2]] = None
+        if fields is not None:
+            if col_type in {"VECTOR", "ARRAY", "OBJECT", "MAP"}:
+                processed_fields = [
+                    ResultMetadataV2.from_column({"name": None, **f})
+                    for f in col["fields"]
+                ]
+            else:
+                raise ValueError(
+                    f"Field parsing is not supported for columns of type {col_type}."
+                )
 
         return cls(
             col["name"],
-            type_code,
+            FIELD_NAME_TO_ID[col_type],
             col["nullable"],
             None,
             col["length"],
             col["precision"],
             col["scale"],
             col.get("vectorDimension"),
-            fields,
+            processed_fields,
         )
 
     def _to_result_metadata_v1(self):
         """Initializes a ResultMetadata object from a ResultMetadataV2 object.
 
         This method is for internal use only.
         """
@@ -356,15 +302,15 @@
         return self._scale
 
     @property
     def vector_dimension(self) -> int | None:
         return self._vector_dimension
 
     @property
-    def fields(self) -> list[ResultMetadataV2Field] | None:
+    def fields(self) -> list[ResultMetadataV2] | None:
         return self._fields
 
 
 def exit_handler(*_) -> NoReturn:
     """Handler for signal. When called, it will raise SystemExit with exit code FORCE_EXIT."""
     print("\nForce exit")
     logger.info("Force exit")
@@ -972,14 +918,15 @@
 
         if _do_reset:
             self.reset()
         command = command.strip(" \t\n\r") if command else None
         if not command:
             logger.warning("execute: no query is given to execute")
             return None
+        logger.debug("query: [%s]", self._format_query_for_log(command))
 
         _statement_params = _statement_params or dict()
         # If we need to add another parameter, please consider introducing a dict for all extra params
         # See discussion in https://github.com/snowflakedb/snowflake-connector-python/pull/1524#discussion_r1174061775
         if num_statements is not None:
             _statement_params = {
                 **_statement_params,
@@ -1016,37 +963,34 @@
                 kwargs["binding_params"] = self._connection._process_params_qmarks(
                     params, self
                 )
 
         m = DESC_TABLE_RE.match(query)
         if m:
             query1 = f"describe table {m.group(1)}"
-            if logger.getEffectiveLevel() <= logging.WARNING:
-                logger.info(
-                    "query was rewritten: org=%s, new=%s",
-                    " ".join(line.strip() for line in query.split("\n")),
-                    query1,
-                )
+            logger.debug(
+                "query was rewritten: org=%s, new=%s",
+                " ".join(line.strip() for line in query.split("\n")),
+                query1,
+            )
             query = query1
 
-        if logger.getEffectiveLevel() <= logging.INFO:
-            logger.info("query: [%s]", self._format_query_for_log(query))
         ret = self._execute_helper(query, **kwargs)
         self._sfqid = (
             ret["data"]["queryId"]
             if "data" in ret and "queryId" in ret["data"]
             else None
         )
         logger.debug(f"sfqid: {self.sfqid}")
         self._sqlstate = (
             ret["data"]["sqlState"]
             if "data" in ret and "sqlState" in ret["data"]
             else None
         )
-        logger.info("query execution done")
+        logger.debug("query execution done")
 
         self._first_chunk_time = get_time_millis()
 
         # if server gives a send time, log the time it took to arrive
         if "data" in ret and "sendResultTime" in ret["data"]:
             time_consume_first_result = (
                 self._first_chunk_time - ret["data"]["sendResultTime"]
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/description.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/errors.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/file_util.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/local_storage_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,22 @@
     ) -> None:
         super().__init__(meta, stage_info, chunk_size)
         self.data_file = meta.src_file_name
         self.full_dst_file_name: str = os.path.join(
             stage_info["location"], os.path.basename(meta.dst_file_name)
         )
         if meta.local_location:
-            self.stage_file_name = self.full_dst_file_name
+            src_file_name = self.data_file
+            if src_file_name.startswith("/"):
+                src_file_name = src_file_name[1:]
+            self.stage_file_name: str = os.path.join(
+                stage_info["location"], src_file_name
+            )
             self.full_dst_file_name = os.path.join(
-                meta.local_location, meta.dst_file_name
+                meta.local_location, os.path.basename(meta.dst_file_name)
             )
 
     def get_file_header(self, filename: str) -> FileHeader | None:
         """
         Notes:
             Checks whether the file exits in specified directory, does not return FileHeader
         """
@@ -60,15 +65,15 @@
                     tfd.write(sfd.read())
                 else:
                     tfd.seek(chunk_id * self.chunk_size)
                     sfd.seek(chunk_id * self.chunk_size)
                     tfd.write(sfd.read(self.chunk_size))
 
     def finish_download(self) -> None:
-        shutil.copyfile(self.intermediate_dst_path, self.full_dst_file_name)
+        shutil.move(self.intermediate_dst_path, self.full_dst_file_name)
         self.meta.dst_file_size = os.stat(self.full_dst_file_name).st_size
         self.meta.result_status = ResultStatus.DOWNLOADED
 
     def _has_expired_token(self, response: requests.Response) -> bool:
         return False
 
     def prepare_upload(self) -> None:
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp` & `snowflake-connector-python-3.8.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/network.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/network.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/options.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import importlib
+import os
 import warnings
 from importlib.metadata import distributions
 from logging import getLogger
 from types import ModuleType
 from typing import Union
 
 from packaging.requirements import Requirement
@@ -75,14 +76,18 @@
     try:
         pandas = importlib.import_module("pandas")
         # since we enable relative imports without dots this import gives us an issues when ran from test directory
         from pandas import DataFrame  # NOQA
 
         pyarrow = importlib.import_module("pyarrow")
 
+        # set default memory pool to system for pyarrow to_pandas conversion
+        if "ARROW_DEFAULT_MEMORY_POOL" not in os.environ:
+            os.environ["ARROW_DEFAULT_MEMORY_POOL"] = "system"
+
         # Check whether we have the currently supported pyarrow installed
         installed_packages = {
             package.metadata["Name"]: package for package in distributions()
         }
         if {"pyarrow", "snowflake-connector-python"} <= installed_packages.keys():
             dependencies = installed_packages[
                 "snowflake-connector-python"
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/pandas_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,21 +389,22 @@
         target_table_location = build_location_helper(
             database,
             schema,
             random_string() if (overwrite and auto_create_table) else table_name,
             quote_identifiers,
         )
 
-        create_table_sql = (
-            f"CREATE {table_type.upper()} TABLE IF NOT EXISTS {target_table_location} "
-            f"({create_table_columns})"
-            f" /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
-        )
-        logger.debug(f"auto creating table with '{create_table_sql}'")
-        cursor.execute(create_table_sql, _is_internal=True)
+        if auto_create_table:
+            create_table_sql = (
+                f"CREATE {table_type.upper()} TABLE IF NOT EXISTS {target_table_location} "
+                f"({create_table_columns})"
+                f" /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
+            )
+            logger.debug(f"auto creating table with '{create_table_sql}'")
+            cursor.execute(create_table_sql, _is_internal=True)
         # need explicit casting when the underlying table schema is inferred
         parquet_columns = "$1:" + ",$1:".join(
             f"{quote}{snowflake_col}{quote}::{column_type_mapping[col]}"
             for snowflake_col, col in zip(snowflake_column_names, df.columns)
         )
     else:
         target_table_location = build_location_helper(
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/proxy.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/result_set.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/secret_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         flags=re.IGNORECASE,
     )
 
     PASSWORD_PATTERN = re.compile(
         r"(password"
         r"|pwd)"
         r"([\'\"\s:=]+)"
-        r"([a-z0-9!\"#\$%&\\\'\(\)\*\+\,-\./:;<=>\?\@\[\]\^_`\{\|\}~]{8,})",
+        r"([a-z0-9!\"#\$%&\\\'\(\)\*\+\,-\./:;<=>\?\@\[\]\^_`\{\|\}~]{1,})",
         flags=re.IGNORECASE,
     )
 
     @staticmethod
     def mask_connection_token(text: str) -> str:
         return SecretDetector.CONNECTION_TOKEN_PATTERN.sub(r"\1\2****", text)
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/sf_dirs.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/sf_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/test_util.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/time_util.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/url_util.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/util_text.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-3.8.0/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/PKG-INFO` & `snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.7.1
+Version: 3.8.0
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
@@ -50,15 +50,15 @@
 Requires-Dist: charset_normalizer<4,>=2
 Requires-Dist: idna<4,>=2.5
 Requires-Dist: urllib3<2.0.0,>=1.21.1; python_version < "3.10"
 Requires-Dist: certifi>=2017.4.17
 Requires-Dist: typing_extensions<5,>=4.3
 Requires-Dist: filelock<4,>=3.5
 Requires-Dist: sortedcontainers>=2.4.0
-Requires-Dist: platformdirs<4.0.0,>=2.6.0
+Requires-Dist: platformdirs<5.0.0,>=2.6.0
 Requires-Dist: tomlkit
 Provides-Extra: development
 Requires-Dist: Cython; extra == "development"
 Requires-Dist: coverage; extra == "development"
 Requires-Dist: more-itertools; extra == "development"
 Requires-Dist: numpy<1.27.0; extra == "development"
 Requires-Dist: pendulum!=2.1.1; extra == "development"
@@ -81,14 +81,34 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.8.0(April 04,2024)
+
+  - Improved `externalbrowser` auth in containerized environments
+    - Instruct browser to not fetch `/favicon` on success page
+    - Simple retry strategy on empty socket.recv
+    - Add `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true`) to set the underlying socket's `SO_REUSEPORT` flag (described in the [socket man page](https://man7.org/linux/man-pages/man7/socket.7.html))
+      - Useful when the randomized port used in the localhost callback url is being followed before the container engine completes port forwarding to host
+      - Statically map a port between your host and container and allow that port to be reused in rapid succession with:
+         `SF_AUTH_SOCKET_PORT=3037 SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true poetry run python somescript.py`
+    - Add `SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_MSG_DONTWAIT=true`) to make a non-blocking socket.recv call and retry on Error
+      - Consider using this if running in a containerized environment and externalbrowser auth frequently hangs while waiting for callback
+      - NOTE: this has not been tested extensively, but has been shown to improve the experience when using WSL
+  - Added support for parsing structured type information in schema queries.
+  - Bumped platformdirs from >=2.6.0,<4.0.0 to >=2.6.0,<5.0.0
+  - Updated diagnostics to use system$allowlist instead of system$whitelist.
+  - Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode.
+  - Improved cleanup logic for connection to rely on interpreter shutdown instead of the `__del__` method.
+  - Updated the logging level from INFO to DEBUG when logging the executed query using `SnowflakeCursor.execute`.
+  - Fixed a bug that the truncated password in log is not masked.
+
 - v3.7.1(February 21, 2024)
 
   - Bumped pandas dependency from >=1.0.0,<2.2.0 to >=1.0.0,<3.0.0.
   - Bumped cryptography dependency from <42.0.0,>=3.1.0 to >=3.1.0,<43.0.0.
   - Bumped pyOpenSSL dependency from >=16.2.0,<24.0.0 to >=16.2.0,<25.0.0.
   - Fixed a memory leak in decimal data conversion.
   - Fixed a bug where `write_pandas` wasn't truncating the target table.
@@ -135,14 +155,15 @@
   - Added support for `use_logical_type` in `write_pandas`.
   - Removed dependencies on pycryptodomex and oscrypto. All connections now go through OpenSSL via the cryptography library, which was already a dependency.
   - Fixed issue with ingesting files over 80 GB to S3.
   - Added the `backoff_policy` argument to `snowflake.connector.connect` allowing for configurable backoff policy between retries of failed requests. See available implementations in the `backoff_policies` module.
   - Added the `socket_timeout` argument to `snowflake.connector.connect` specifying socket read and connect timeout.
   - Fixed `login_timeout` and `network_timeout` behaviour. Retries of login and network requests are now properly halted after these timeouts expire.
   - Fixed bug for issue https://github.com/urllib3/urllib3/issues/1878 in vendored `urllib`.
+  - Add User-Agent header for diagnostic report for tracking.
 
 - v3.3.1(October 16,2023)
 
   - Added for non-Windows platforms command suggestions (chown/chmod) for insufficient file permissions of config files.
   - Fixed issue with connection diagnostics failing to complete certificate checks.
   - Fixed issue that arrow iterator causes `ImportError` when the c extensions are not compiled.
```

### Comparing `snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/SOURCES.txt` & `snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.7.1/src/snowflake_connector_python.egg-info/requires.txt` & `snowflake-connector-python-3.8.0/src/snowflake_connector_python.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 packaging
 charset_normalizer<4,>=2
 idna<4,>=2.5
 certifi>=2017.4.17
 typing_extensions<5,>=4.3
 filelock<4,>=3.5
 sortedcontainers>=2.4.0
-platformdirs<4.0.0,>=2.6.0
+platformdirs<5.0.0,>=2.6.0
 tomlkit
 
 [:python_version < "3.10"]
 urllib3<2.0.0,>=1.21.1
 
 [:python_version < "3.8"]
 importlib-metadata
```

