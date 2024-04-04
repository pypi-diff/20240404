# Comparing `tmp/aserto_directory-0.31.2.tar.gz` & `tmp/aserto_directory-0.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aserto_directory-0.31.2.tar", max compression
+gzip compressed data, was "aserto_directory-0.31.3.tar", max compression
```

## Comparing `aserto_directory-0.31.2.tar` & `aserto_directory-0.31.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    11357 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/LICENSE
--rw-r--r--   0        0        0      952 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/README.md
--rw-r--r--   0        0        0     1372 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/pyproject.toml
--rw-r--r--   0        0        0      753 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/assertion/v3/__init__.py
--rw-r--r--   0        0        0     9277 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2.py
--rw-r--r--   0        0        0     3450 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2.pyi
--rw-r--r--   0        0        0     8581 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2_grpc.py
--rw-r--r--   0        0        0     3897 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2_grpc.pyi
--rw-r--r--   0        0        0      713 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v2/__init__.py
--rw-r--r--   0        0        0     8142 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v2/common_pb2.py
--rw-r--r--   0        0        0     9097 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v2/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v2/common_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v2/common_pb2_grpc.pyi
--rw-r--r--   0        0        0      373 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v3/__init__.py
--rw-r--r--   0        0        0    17456 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v3/common_pb2.py
--rw-r--r--   0        0        0     4262 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v3/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v3/common_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/common/v3/common_pb2_grpc.pyi
--rw-r--r--   0        0        0      383 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v2/__init__.py
--rw-r--r--   0        0        0     3751 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2.py
--rw-r--r--   0        0        0     2704 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2.pyi
--rw-r--r--   0        0        0     2796 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py
--rw-r--r--   0        0        0     1491 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi
--rw-r--r--   0        0        0      383 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v3/__init__.py
--rw-r--r--   0        0        0     3323 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2.py
--rw-r--r--   0        0        0     1803 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2.pyi
--rw-r--r--   0        0        0     2796 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2_grpc.py
--rw-r--r--   0        0        0     1491 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2_grpc.pyi
--rw-r--r--   0        0        0      423 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v2/__init__.py
--rw-r--r--   0        0        0     4009 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2.py
--rw-r--r--   0        0        0     2969 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2.pyi
--rw-r--r--   0        0        0     2826 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2_grpc.py
--rw-r--r--   0        0        0     1523 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi
--rw-r--r--   0        0        0      423 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v3/__init__.py
--rw-r--r--   0        0        0     3394 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2.py
--rw-r--r--   0        0        0     1979 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2.pyi
--rw-r--r--   0        0        0     2826 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2_grpc.py
--rw-r--r--   0        0        0     1523 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2_grpc.pyi
--rw-r--r--   0        0        0      621 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/model/v3/__init__.py
--rw-r--r--   0        0        0     6574 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2.py
--rw-r--r--   0        0        0     2835 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2.pyi
--rw-r--r--   0        0        0     6441 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2_grpc.py
--rw-r--r--   0        0        0     3129 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2_grpc.pyi
--rw-r--r--   0        0        0       68 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/openapi/v3/__init__.py
--rw-r--r--   0        0        0     2927 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/openapi/v3/openapi_pb2.py
--rw-r--r--   0        0        0      212 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/openapi/v3/openapi_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/openapi/v3/openapi_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/openapi/v3/openapi_pb2_grpc.pyi
--rw-r--r--   0        0        0     1815 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v2/__init__.py
--rw-r--r--   0        0        0    13643 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2.py
--rw-r--r--   0        0        0    12578 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2.pyi
--rw-r--r--   0        0        0    26444 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2_grpc.py
--rw-r--r--   0        0        0    11788 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi
--rw-r--r--   0        0        0     1165 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v3/__init__.py
--rw-r--r--   0        0        0    47404 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2.py
--rw-r--r--   0        0        0    12072 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2.pyi
--rw-r--r--   0        0        0    17080 2024-03-05 15:58:15.006631 aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2_grpc.py
--rw-r--r--   0        0        0     7668 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2_grpc.pyi
--rw-r--r--   0        0        0      657 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/__init__.py
--rw-r--r--   0        0        0     1874 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/group_pb2.py
--rw-r--r--   0        0        0      426 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/group_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/group_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/group_pb2_grpc.pyi
--rw-r--r--   0        0        0     2556 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/identity_pb2.py
--rw-r--r--   0        0        0     1512 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/identity_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/identity_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/identity_pb2_grpc.pyi
--rw-r--r--   0        0        0     3237 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/tenant_pb2.py
--rw-r--r--   0        0        0     2124 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/tenant_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/tenant_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/tenant_pb2_grpc.pyi
--rw-r--r--   0        0        0     2628 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/user_pb2.py
--rw-r--r--   0        0        0     1770 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/user_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v2/user_pb2_grpc.pyi
--rw-r--r--   0        0        0      657 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/__init__.py
--rw-r--r--   0        0        0     1874 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/group_pb2.py
--rw-r--r--   0        0        0      426 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/group_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/group_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/group_pb2_grpc.pyi
--rw-r--r--   0        0        0     2556 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/identity_pb2.py
--rw-r--r--   0        0        0     1512 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/identity_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/identity_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/identity_pb2_grpc.pyi
--rw-r--r--   0        0        0     3237 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/tenant_pb2.py
--rw-r--r--   0        0        0     2124 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/tenant_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/tenant_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/tenant_pb2_grpc.pyi
--rw-r--r--   0        0        0     2628 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/user_pb2.py
--rw-r--r--   0        0        0     1770 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/user_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/schema/v3/user_pb2_grpc.pyi
--rw-r--r--   0        0        0     1387 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v2/__init__.py
--rw-r--r--   0        0        0     8466 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2.py
--rw-r--r--   0        0        0     5631 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2.pyi
--rw-r--r--   0        0        0    19345 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2_grpc.py
--rw-r--r--   0        0        0     8700 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi
--rw-r--r--   0        0        0      675 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v3/__init__.py
--rw-r--r--   0        0        0    14090 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2.py
--rw-r--r--   0        0        0     3328 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2.pyi
--rw-r--r--   0        0        0     8204 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2_grpc.py
--rw-r--r--   0        0        0     3794 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2_grpc.pyi
--rw-r--r--   0        0        0     2290 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/expression_pb2.py
--rw-r--r--   0        0        0     1517 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/expression_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0        0        0      964 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/expression_pb2_grpc.pyi
--rw-r--r--   0        0        0     2330 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/priv/private_pb2.py
--rw-r--r--   0        0        0     1113 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/priv/private_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0        0        0      964 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/priv/private_pb2_grpc.pyi
--rw-r--r--   0        0        0   142610 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/validate_pb2.py
--rw-r--r--   0        0        0    23374 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0      964 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/buf/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0     1790 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      310 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      951 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2280 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/field_behavior_pb2.py
--rw-r--r--   0        0        0     1103 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/field_behavior_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0        0        0      951 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/field_behavior_pb2_grpc.pyi
--rw-r--r--   0        0        0     2688 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/http_pb2.py
--rw-r--r--   0        0        0     2272 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      951 2024-03-05 15:58:15.010631 aserto_directory-0.31.2/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 aserto_directory-0.31.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/LICENSE
+-rw-r--r--   0        0        0      952 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/README.md
+-rw-r--r--   0        0        0     1372 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/pyproject.toml
+-rw-r--r--   0        0        0      753 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/assertion/v3/__init__.py
+-rw-r--r--   0        0        0     9277 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2.py
+-rw-r--r--   0        0        0     3450 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2.pyi
+-rw-r--r--   0        0        0     8581 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2_grpc.py
+-rw-r--r--   0        0        0     3897 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2_grpc.pyi
+-rw-r--r--   0        0        0      713 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v2/__init__.py
+-rw-r--r--   0        0        0     8142 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v2/common_pb2.py
+-rw-r--r--   0        0        0     9097 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v2/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v2/common_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v2/common_pb2_grpc.pyi
+-rw-r--r--   0        0        0      373 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v3/__init__.py
+-rw-r--r--   0        0        0    17456 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v3/common_pb2.py
+-rw-r--r--   0        0        0     4262 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v3/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v3/common_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/common/v3/common_pb2_grpc.pyi
+-rw-r--r--   0        0        0      383 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v2/__init__.py
+-rw-r--r--   0        0        0     3751 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2.py
+-rw-r--r--   0        0        0     2704 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2.pyi
+-rw-r--r--   0        0        0     2796 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py
+-rw-r--r--   0        0        0     1491 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi
+-rw-r--r--   0        0        0      383 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v3/__init__.py
+-rw-r--r--   0        0        0     3323 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2.py
+-rw-r--r--   0        0        0     1803 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2.pyi
+-rw-r--r--   0        0        0     2796 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2_grpc.py
+-rw-r--r--   0        0        0     1491 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2_grpc.pyi
+-rw-r--r--   0        0        0      423 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v2/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2.py
+-rw-r--r--   0        0        0     2969 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2.pyi
+-rw-r--r--   0        0        0     2826 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2_grpc.py
+-rw-r--r--   0        0        0     1523 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi
+-rw-r--r--   0        0        0      423 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v3/__init__.py
+-rw-r--r--   0        0        0     3394 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2.py
+-rw-r--r--   0        0        0     1979 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2.pyi
+-rw-r--r--   0        0        0     2826 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2_grpc.py
+-rw-r--r--   0        0        0     1523 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2_grpc.pyi
+-rw-r--r--   0        0        0      621 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/model/v3/__init__.py
+-rw-r--r--   0        0        0     6574 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2.py
+-rw-r--r--   0        0        0     2835 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2.pyi
+-rw-r--r--   0        0        0     6441 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2_grpc.py
+-rw-r--r--   0        0        0     3129 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0       68 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/openapi/v3/__init__.py
+-rw-r--r--   0        0        0     2927 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/openapi/v3/openapi_pb2.py
+-rw-r--r--   0        0        0      212 2024-04-04 19:04:07.946199 aserto_directory-0.31.3/src/aserto/directory/openapi/v3/openapi_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/openapi/v3/openapi_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/openapi/v3/openapi_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1815 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v2/__init__.py
+-rw-r--r--   0        0        0    13643 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2.py
+-rw-r--r--   0        0        0    12578 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2.pyi
+-rw-r--r--   0        0        0    26444 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2_grpc.py
+-rw-r--r--   0        0        0    11788 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1165 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v3/__init__.py
+-rw-r--r--   0        0        0    47404 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2.py
+-rw-r--r--   0        0        0    12072 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2.pyi
+-rw-r--r--   0        0        0    17080 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2_grpc.py
+-rw-r--r--   0        0        0     7668 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2_grpc.pyi
+-rw-r--r--   0        0        0      657 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/group_pb2.py
+-rw-r--r--   0        0        0      426 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/group_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/group_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/group_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2556 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/identity_pb2.py
+-rw-r--r--   0        0        0     1512 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/identity_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/identity_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/identity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3237 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/tenant_pb2.py
+-rw-r--r--   0        0        0     2124 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/tenant_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/tenant_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/tenant_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2628 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/user_pb2.py
+-rw-r--r--   0        0        0     1770 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/user_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v2/user_pb2_grpc.pyi
+-rw-r--r--   0        0        0      657 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/group_pb2.py
+-rw-r--r--   0        0        0      426 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/group_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/group_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/group_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2556 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/identity_pb2.py
+-rw-r--r--   0        0        0     1512 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/identity_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/identity_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/identity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3237 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/tenant_pb2.py
+-rw-r--r--   0        0        0     2124 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/tenant_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/tenant_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/tenant_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2628 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/user_pb2.py
+-rw-r--r--   0        0        0     1770 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/user_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/schema/v3/user_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1387 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v2/__init__.py
+-rw-r--r--   0        0        0     8466 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2.py
+-rw-r--r--   0        0        0     5631 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2.pyi
+-rw-r--r--   0        0        0    19345 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2_grpc.py
+-rw-r--r--   0        0        0     8700 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi
+-rw-r--r--   0        0        0      675 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v3/__init__.py
+-rw-r--r--   0        0        0    14090 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2.py
+-rw-r--r--   0        0        0     3328 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2.pyi
+-rw-r--r--   0        0        0     8204 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2_grpc.py
+-rw-r--r--   0        0        0     3794 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2290 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/expression_pb2.py
+-rw-r--r--   0        0        0     1517 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/expression_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0        0        0      964 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/expression_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2330 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/priv/private_pb2.py
+-rw-r--r--   0        0        0     1113 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/priv/private_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0        0        0      964 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/priv/private_pb2_grpc.pyi
+-rw-r--r--   0        0        0   142610 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/validate_pb2.py
+-rw-r--r--   0        0        0    23374 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0      964 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/buf/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1790 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      310 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2280 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0     1103 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.950199 aserto_directory-0.31.3/src/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-04 19:04:07.954199 aserto_directory-0.31.3/src/google/api/field_behavior_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2688 2024-04-04 19:04:07.954199 aserto_directory-0.31.3/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2024-04-04 19:04:07.954199 aserto_directory-0.31.3/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 19:04:07.954199 aserto_directory-0.31.3/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-04 19:04:07.954199 aserto_directory-0.31.3/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 aserto_directory-0.31.3/PKG-INFO
```

### Comparing `aserto_directory-0.31.2/LICENSE` & `aserto_directory-0.31.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/README.md` & `aserto_directory-0.31.3/README.md`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/pyproject.toml` & `aserto_directory-0.31.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aserto-directory"
-version = "0.31.2"
+version = "0.31.3"
 description = "gRPC client for Aserto Directory service instances"
 readme = "README.md"
 authors = ["Aserto, Inc. <pypi@aserto.com>"]
 homepage = "https://github.com/aserto-dev/python-directory"
 repository = "https://github.com/aserto-dev/python-directory"
 documentation = "https://github.com/aserto-dev/python-directory"
 license = "Apache-2.0"
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/assertion/v3/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/assertion/v3/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # This file is generated by init_gen.py. Do not edit.
 
-from aserto.directory.assertion.v3.assertion_pb2_grpc import (
-    AssertionStub,
-    AssertionServicer,
-)
-
 from aserto.directory.assertion.v3.assertion_pb2 import (
     GetAssertionRequest,
     GetAssertionResponse,
     ListAssertionsRequest,
     ListAssertionsResponse,
     SetAssertionRequest,
     SetAssertionResponse,
     DeleteAssertionRequest,
     DeleteAssertionResponse,
     Assert,
 )
 
+from aserto.directory.assertion.v3.assertion_pb2_grpc import (
+    AssertionStub,
+    AssertionServicer,
+)
+
 __all__ = [
-    "AssertionStub",
-    "AssertionServicer",
     "GetAssertionRequest",
     "GetAssertionResponse",
     "ListAssertionsRequest",
     "ListAssertionsResponse",
     "SetAssertionRequest",
     "SetAssertionResponse",
     "DeleteAssertionRequest",
     "DeleteAssertionResponse",
     "Assert",
+    "AssertionStub",
+    "AssertionServicer",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/assertion/v3/assertion_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/assertion/v3/assertion_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/common/v2/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/common/v2/common_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/common/v2/common_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/common/v2/common_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/common/v2/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/common/v3/common_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/common/v3/common_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/common/v3/common_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/common/v3/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/exporter/v3/exporter_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/exporter/v3/exporter_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/importer/v3/importer_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/importer/v3/importer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/model/v3/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/model/v3/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file is generated by init_gen.py. Do not edit.
 
-from aserto.directory.model.v3.model_pb2_grpc import (
-    ModelStub,
-    ModelServicer,
-)
-
 from aserto.directory.model.v3.model_pb2 import (
     GetManifestRequest,
     GetManifestResponse,
     SetManifestRequest,
     SetManifestResponse,
     DeleteManifestRequest,
     DeleteManifestResponse,
     Metadata,
     Body,
 )
 
+from aserto.directory.model.v3.model_pb2_grpc import (
+    ModelStub,
+    ModelServicer,
+)
+
 __all__ = [
-    "ModelStub",
-    "ModelServicer",
     "GetManifestRequest",
     "GetManifestResponse",
     "SetManifestRequest",
     "SetManifestResponse",
     "DeleteManifestRequest",
     "DeleteManifestResponse",
     "Metadata",
     "Body",
+    "ModelStub",
+    "ModelServicer",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/model/v3/model_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/model/v3/model_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/openapi/v3/openapi_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/openapi/v3/openapi_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)aserto/directory/openapi/v3/openapi.proto\x12\x13\x61serto.directory.v3\x1a.protoc-gen-openapiv2/options/annotations.protoB\xea\x04\n\x17\x63om.aserto.directory.v3B\x0cOpenapiProtoP\x01Z@github.com/aserto-dev/go-directory/aserto/directory/v3;directory\xa2\x02\x03\x41\x44X\xaa\x02\x13\x41serto.Directory.V3\xca\x02\x14\x41serto\\Directory_\\V3\xe2\x02 Aserto\\Directory_\\V3\\GPBMetadata\xea\x02\x15\x41serto::Directory::V3\x92\x41\x8d\x03\x12\xbc\x01\n\x11\x44irectory Service\"N\n\x0c\x41serto, Inc.\x12*https://github.com/aserto-dev/pb-directory\x1a\x12support@aserto.com*R\n\x12\x41pache 2.0 License\x12<https://github.com/aserto-dev/pb-directory/blob/main/LICENSE2\x03\x33.0*\x03\x01\x02\x04\x32\x10\x61pplication/json:\x10\x61pplication/jsonZL\n&\n\x0f\x44irectoryAPIKey\x12\x13\x08\x02\x1a\rauthorization \x02\n\"\n\x08TenantID\x12\x16\x08\x02\x1a\x10\x61serto-tenant-id \x02\x62#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00r0\n\x15\x41serto API Reference.\x12\x17https://docs.aserto.comb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)aserto/directory/openapi/v3/openapi.proto\x12\x13\x61serto.directory.v3\x1a.protoc-gen-openapiv2/options/annotations.protoB\xea\x04\n\x17\x63om.aserto.directory.v3B\x0cOpenapiProtoP\x01Z@github.com/aserto-dev/go-directory/aserto/directory/v3;directory\xa2\x02\x03\x41\x44X\xaa\x02\x13\x41serto.Directory.V3\xca\x02\x14\x41serto\\Directory_\\V3\xe2\x02 Aserto\\Directory_\\V3\\GPBMetadata\xea\x02\x15\x41serto::Directory::V3\x92\x41\x8d\x03\x12\xbc\x01\n\x11\x44irectory Service\"N\n\x0c\x41serto, Inc.\x12*https://github.com/aserto-dev/pb-directory\x1a\x12support@aserto.com*R\n\x12\x41pache 2.0 License\x12<https://github.com/aserto-dev/pb-directory/blob/main/LICENSE2\x03\x33.1*\x03\x01\x02\x04\x32\x10\x61pplication/json:\x10\x61pplication/jsonZL\n&\n\x0f\x44irectoryAPIKey\x12\x13\x08\x02\x1a\rauthorization \x02\n\"\n\x08TenantID\x12\x16\x08\x02\x1a\x10\x61serto-tenant-id \x02\x62#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00r0\n\x15\x41serto API Reference.\x12\x17https://docs.aserto.comb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aserto.directory.openapi.v3.openapi_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n\027com.aserto.directory.v3B\014OpenapiProtoP\001Z@github.com/aserto-dev/go-directory/aserto/directory/v3;directory\242\002\003ADX\252\002\023Aserto.Directory.V3\312\002\024Aserto\\Directory_\\V3\342\002 Aserto\\Directory_\\V3\\GPBMetadata\352\002\025Aserto::Directory::V3\222A\215\003\022\274\001\n\021Directory Service\"N\n\014Aserto, Inc.\022*https://github.com/aserto-dev/pb-directory\032\022support@aserto.com*R\n\022Apache 2.0 License\022<https://github.com/aserto-dev/pb-directory/blob/main/LICENSE2\0033.0*\003\001\002\0042\020application/json:\020application/jsonZL\n&\n\017DirectoryAPIKey\022\023\010\002\032\rauthorization \002\n\"\n\010TenantID\022\026\010\002\032\020aserto-tenant-id \002b#\n\023\n\017DirectoryAPIKey\022\000\n\014\n\010TenantID\022\000r0\n\025Aserto API Reference.\022\027https://docs.aserto.com'
+  _globals['DESCRIPTOR']._serialized_options = b'\n\027com.aserto.directory.v3B\014OpenapiProtoP\001Z@github.com/aserto-dev/go-directory/aserto/directory/v3;directory\242\002\003ADX\252\002\023Aserto.Directory.V3\312\002\024Aserto\\Directory_\\V3\342\002 Aserto\\Directory_\\V3\\GPBMetadata\352\002\025Aserto::Directory::V3\222A\215\003\022\274\001\n\021Directory Service\"N\n\014Aserto, Inc.\022*https://github.com/aserto-dev/pb-directory\032\022support@aserto.com*R\n\022Apache 2.0 License\022<https://github.com/aserto-dev/pb-directory/blob/main/LICENSE2\0033.1*\003\001\002\0042\020application/json:\020application/jsonZL\n&\n\017DirectoryAPIKey\022\023\010\002\032\rauthorization \002\n\"\n\010TenantID\022\026\010\002\032\020aserto-tenant-id \002b#\n\023\n\017DirectoryAPIKey\022\000\n\014\n\010TenantID\022\000r0\n\025Aserto API Reference.\022\027https://docs.aserto.com'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v2/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/reader/v2/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # This file is generated by init_gen.py. Do not edit.
 
+from aserto.directory.reader.v2.reader_pb2_grpc import (
+    ReaderStub,
+    ReaderServicer,
+)
+
 from aserto.directory.reader.v2.reader_pb2 import (
     GetObjectTypeRequest,
     GetObjectTypeResponse,
     GetObjectTypesRequest,
     GetObjectTypesResponse,
     GetRelationTypeRequest,
     GetRelationTypeResponse,
@@ -28,20 +33,17 @@
     CheckRelationRequest,
     CheckRelationResponse,
     CheckResponse,
     GetGraphRequest,
     GetGraphResponse,
 )
 
-from aserto.directory.reader.v2.reader_pb2_grpc import (
-    ReaderStub,
-    ReaderServicer,
-)
-
 __all__ = [
+    "ReaderStub",
+    "ReaderServicer",
     "GetObjectTypeRequest",
     "GetObjectTypeResponse",
     "GetObjectTypesRequest",
     "GetObjectTypesResponse",
     "GetRelationTypeRequest",
     "GetRelationTypeResponse",
     "GetRelationTypesRequest",
@@ -63,10 +65,8 @@
     "CheckPermissionRequest",
     "CheckPermissionResponse",
     "CheckRelationRequest",
     "CheckRelationResponse",
     "CheckResponse",
     "GetGraphRequest",
     "GetGraphResponse",
-    "ReaderStub",
-    "ReaderServicer",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v3/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/reader/v3/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # This file is generated by init_gen.py. Do not edit.
 
+from aserto.directory.reader.v3.reader_pb2_grpc import (
+    ReaderStub,
+    ReaderServicer,
+)
+
 from aserto.directory.reader.v3.reader_pb2 import (
     GetObjectRequest,
     GetObjectResponse,
     GetObjectManyRequest,
     GetObjectManyResponse,
     GetObjectsRequest,
     GetObjectsResponse,
@@ -17,20 +22,17 @@
     CheckPermissionResponse,
     CheckRelationRequest,
     CheckRelationResponse,
     GetGraphRequest,
     GetGraphResponse,
 )
 
-from aserto.directory.reader.v3.reader_pb2_grpc import (
-    ReaderStub,
-    ReaderServicer,
-)
-
 __all__ = [
+    "ReaderStub",
+    "ReaderServicer",
     "GetObjectRequest",
     "GetObjectResponse",
     "GetObjectManyRequest",
     "GetObjectManyResponse",
     "GetObjectsRequest",
     "GetObjectsResponse",
     "GetRelationRequest",
@@ -41,10 +43,8 @@
     "CheckResponse",
     "CheckPermissionRequest",
     "CheckPermissionResponse",
     "CheckRelationRequest",
     "CheckRelationResponse",
     "GetGraphRequest",
     "GetGraphResponse",
-    "ReaderStub",
-    "ReaderServicer",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from aserto.directory.common.v3 import common_pb2 as aserto_dot_directory_dot_common_dot_v3_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/reader/v3/reader.proto\x12\x1a\x61serto.directory.reader.v3\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\'aserto/directory/common/v3/common.proto\"\xaf\x04\n\x10GetObjectRequest\x12\x8e\x02\n\x0bobject_type\x18\x01 \x01(\tB\xec\x01\xe0\x41\x02\xbaH\xe5\x01r\x02\x18@\xba\x01\xda\x01\n\x16get_object.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x95\x01\n\tobject_id\x18\x02 \x01(\tBx\xbaHur\x03\x18\x80\x02\xba\x01j\n\x14get_object.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12*\n\x0ewith_relations\x18\x03 \x01(\x08\x42\x03\xe0\x41\x01R\rwithRelations\x12\x46\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v3.PaginationRequestB\x03\xe0\x41\x01R\x04page\"\xd7\x01\n\x11GetObjectResponse\x12:\n\x06result\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x06result\x12\x42\n\trelations\x18\x04 \x03(\x0b\x32$.aserto.directory.common.v3.RelationR\trelations\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v3.PaginationResponseR\x04page\"_\n\x14GetObjectManyRequest\x12G\n\x05param\x18\x01 \x03(\x0b\x32,.aserto.directory.common.v3.ObjectIdentifierB\x03\xe0\x41\x02R\x05param\"U\n\x15GetObjectManyResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v3.ObjectR\x07results\"\xed\x02\n\x11GetObjectsRequest\x12\x8f\x02\n\x0bobject_type\x18\x01 \x01(\tB\xed\x01\xe0\x41\x01\xbaH\xe6\x01r\x02\x18@\xba\x01\xdb\x01\n\x17get_objects.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x46\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v3.PaginationRequestB\x03\xe0\x41\x01R\x04page\"\x96\x01\n\x12GetObjectsResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v3.ObjectR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v3.PaginationResponseR\x04page\"\xfd\x0f\n\x12GetRelationRequest\x12\x90\x02\n\x0bobject_type\x18\x01 \x01(\tB\xee\x01\xe0\x41\x02\xbaH\xe7\x01r\x02\x18@\xba\x01\xdc\x01\n\x18get_relation.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x9a\x01\n\tobject_id\x18\x02 \x01(\tB}\xe0\x41\x02\xbaHwr\x03\x18\x80\x02\xba\x01l\n\x16get_relation.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\x08objectId\x12\x88\x02\n\x08relation\x18\x03 \x01(\tB\xeb\x01\xe0\x41\x02\xbaH\xe4\x01r\x02\x18@\xba\x01\xd9\x01\n\x15get_relation.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x08relation\x12\x93\x02\n\x0csubject_type\x18\x04 \x01(\tB\xef\x01\xe0\x41\x02\xbaH\xe8\x01r\x02\x18@\xba\x01\xdd\x01\n\x19get_relation.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0bsubjectType\x12\x9d\x01\n\nsubject_id\x18\x05 \x01(\tB~\xe0\x41\x02\xbaHxr\x03\x18\x80\x02\xba\x01m\n\x17get_relation.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\tsubjectId\x12\x9f\x02\n\x10subject_relation\x18\x06 \x01(\tB\xf3\x01\xe0\x41\x01\xbaH\xec\x01r\x02\x18@\xba\x01\xe1\x01\n\x1dget_relation.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\x12&\n\x0cwith_objects\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x0bwithObjects:\xab\x04\xbaH\xa7\x04\x1a\x8c\x02\n get_relation.object_id_with_type\x12Mwhen an object_id is specified, the accompanying object_type must be provided\x1a\x98\x01(this.object_type == \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id != \'\')\x1a\x95\x02\n!get_relation.subject_id_with_type\x12Owhen an subject_id is specified, the accompanying subject_type must be provided\x1a\x9e\x01(this.subject_type == \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id != \'\')\"\x8b\x02\n\x13GetRelationResponse\x12<\n\x06result\x18\x01 \x01(\x0b\x32$.aserto.directory.common.v3.RelationR\x06result\x12V\n\x07objects\x18\x02 \x03(\x0b\x32<.aserto.directory.reader.v3.GetRelationResponse.ObjectsEntryR\x07objects\x1a^\n\x0cObjectsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x05value:\x02\x38\x01\"\x92\x11\n\x13GetRelationsRequest\x12\x91\x02\n\x0bobject_type\x18\x01 \x01(\tB\xef\x01\xe0\x41\x01\xbaH\xe8\x01r\x02\x18@\xba\x01\xdd\x01\n\x19get_relations.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x9b\x01\n\tobject_id\x18\x02 \x01(\tB~\xe0\x41\x01\xbaHxr\x03\x18\x80\x02\xba\x01m\n\x17get_relations.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\x08objectId\x12\x89\x02\n\x08relation\x18\x03 \x01(\tB\xec\x01\xe0\x41\x01\xbaH\xe5\x01r\x02\x18@\xba\x01\xda\x01\n\x16get_relations.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x08relation\x12\x94\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf0\x01\xe0\x41\x01\xbaH\xe9\x01r\x02\x18@\xba\x01\xde\x01\n\x1aget_relations.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0bsubjectType\x12\x9e\x01\n\nsubject_id\x18\x05 \x01(\tB\x7f\xe0\x41\x01\xbaHyr\x03\x18\x80\x02\xba\x01n\n\x18get_relations.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\tsubjectId\x12\xa0\x02\n\x10subject_relation\x18\x06 \x01(\tB\xf4\x01\xe0\x41\x01\xbaH\xed\x01r\x02\x18@\xba\x01\xe2\x01\n\x1eget_relations.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\x12&\n\x0cwith_objects\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x0bwithObjects\x12\x42\n\x1bwith_empty_subject_relation\x18\x08 \x01(\x08\x42\x03\xe0\x41\x01R\x18withEmptySubjectRelation\x12\x46\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v3.PaginationRequestB\x03\xe0\x41\x01R\x04page:\xad\x04\xbaH\xa9\x04\x1a\x8d\x02\n!get_relations.object_id_with_type\x12Mwhen an object_id is specified, the accompanying object_type must be provided\x1a\x98\x01(this.object_type == \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id != \'\')\x1a\x96\x02\n\"get_relations.subject_id_with_type\x12Owhen an subject_id is specified, the accompanying subject_type must be provided\x1a\x9e\x01(this.subject_type == \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id != \'\')\"\xd3\x02\n\x14GetRelationsResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.aserto.directory.common.v3.RelationR\x07results\x12W\n\x07objects\x18\x02 \x03(\x0b\x32=.aserto.directory.reader.v3.GetRelationsResponse.ObjectsEntryR\x07objects\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v3.PaginationResponseR\x04page\x1a^\n\x0cObjectsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x05value:\x02\x38\x01\"\x87\x08\n\x0c\x43heckRequest\x12\x89\x02\n\x0bobject_type\x18\x01 \x01(\tB\xe7\x01\xe0\x41\x02\xbaH\xe0\x01r\x02\x18@\xba\x01\xd5\x01\n\x11\x63heck.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x93\x01\n\tobject_id\x18\x02 \x01(\tBv\xe0\x41\x02\xbaHpr\x03\x18\x80\x02\xba\x01\x65\n\x0f\x63heck.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\x91\x01\n\x08relation\x18\x03 \x01(\tBu\xe0\x41\x02\xbaHor\x03\x18\x80\x02\xba\x01\x64\n\x0e\x63heck.relation\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08relation\x12\x8c\x02\n\x0csubject_type\x18\x04 \x01(\tB\xe8\x01\xe0\x41\x02\xbaH\xe1\x01r\x02\x18@\xba\x01\xd6\x01\n\x12\x63heck.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\x96\x01\n\nsubject_id\x18\x05 \x01(\tBw\xe0\x41\x02\xbaHqr\x03\x18\x80\x02\xba\x01\x66\n\x10\x63heck.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\x19\n\x05trace\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x05trace\";\n\rCheckResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xd1\x08\n\x16\x43heckPermissionRequest\x12\x94\x02\n\x0bobject_type\x18\x01 \x01(\tB\xf2\x01\xe0\x41\x02\xbaH\xeb\x01r\x02\x18@\xba\x01\xe0\x01\n\x1c\x63heck_permission.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x9f\x01\n\tobject_id\x18\x02 \x01(\tB\x81\x01\xe0\x41\x02\xbaH{r\x03\x18\x80\x02\xba\x01p\n\x1a\x63heck_permission.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\xa3\x01\n\npermission\x18\x03 \x01(\tB\x82\x01\xe0\x41\x02\xbaH|r\x03\x18\x80\x02\xba\x01q\n\x1b\x63heck_permission.permission\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\npermission\x12\x97\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf3\x01\xe0\x41\x02\xbaH\xec\x01r\x02\x18@\xba\x01\xe1\x01\n\x1d\x63heck_permission.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\xa2\x01\n\nsubject_id\x18\x05 \x01(\tB\x82\x01\xe0\x41\x02\xbaH|r\x03\x18\x80\x02\xba\x01q\n\x1b\x63heck_permission.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\x19\n\x05trace\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x05trace\"E\n\x17\x43heckPermissionResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xad\t\n\x14\x43heckRelationRequest\x12\x92\x02\n\x0bobject_type\x18\x01 \x01(\tB\xf0\x01\xe0\x41\x02\xbaH\xe9\x01r\x02\x18@\xba\x01\xde\x01\n\x1a\x63heck_relation.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x9c\x01\n\tobject_id\x18\x02 \x01(\tB\x7f\xe0\x41\x02\xbaHyr\x03\x18\x80\x02\xba\x01n\n\x18\x63heck_relation.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\x8a\x02\n\x08relation\x18\x03 \x01(\tB\xed\x01\xe0\x41\x02\xbaH\xe6\x01r\x02\x18@\xba\x01\xdb\x01\n\x17\x63heck_relation.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x08relation\x12\x95\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf1\x01\xe0\x41\x02\xbaH\xea\x01r\x02\x18@\xba\x01\xdf\x01\n\x1b\x63heck_relation.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\xa0\x01\n\nsubject_id\x18\x05 \x01(\tB\x80\x01\xe0\x41\x02\xbaHzr\x03\x18\x80\x02\xba\x01o\n\x19\x63heck_relation.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\x19\n\x05trace\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x05trace\"C\n\x15\x43heckRelationResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xf0\x0b\n\x0fGetGraphRequest\x12\x8d\x02\n\x0bobject_type\x18\x03 \x01(\tB\xeb\x01\xe0\x41\x02\xbaH\xe4\x01r\x02\x18@\xba\x01\xd9\x01\n\x15get_graph.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x97\x01\n\tobject_id\x18\x04 \x01(\tBz\xe0\x41\x01\xbaHtr\x03\x18\x80\x02\xba\x01i\n\x13get_graph.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\x08objectId\x12\x85\x02\n\x08relation\x18\x05 \x01(\tB\xe8\x01\xe0\x41\x02\xbaH\xe1\x01r\x02\x18@\xba\x01\xd6\x01\n\x12get_graph.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x08relation\x12\x90\x02\n\x0csubject_type\x18\x06 \x01(\tB\xec\x01\xe0\x41\x02\xbaH\xe5\x01r\x02\x18@\xba\x01\xda\x01\n\x16get_graph.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0bsubjectType\x12\x9a\x01\n\nsubject_id\x18\x07 \x01(\tB{\xe0\x41\x01\xbaHur\x03\x18\x80\x02\xba\x01j\n\x14get_graph.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\tsubjectId\x12\x9c\x02\n\x10subject_relation\x18\x08 \x01(\tB\xf0\x01\xe0\x41\x01\xbaH\xe9\x01r\x02\x18@\xba\x01\xde\x01\n\x1aget_graph.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\x12\x1d\n\x07\x65xplain\x18\t \x01(\x08\x42\x03\xe0\x41\x01R\x07\x65xplain\x12\x19\n\x05trace\x18\n \x01(\x08\x42\x03\xe0\x41\x01R\x05traceJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03R\x0b\x61nchor_typeR\tanchor_id\"\xb1\x01\n\x10GetGraphResponse\x12\x46\n\x07results\x18\x02 \x03(\x0b\x32,.aserto.directory.common.v3.ObjectIdentifierR\x07results\x12\x39\n\x0b\x65xplanation\x18\x03 \x01(\x0b\x32\x17.google.protobuf.StructR\x0b\x65xplanation\x12\x14\n\x05trace\x18\x04 \x03(\tR\x05traceJ\x04\x08\x01\x10\x02\x32\x85\x14\n\x06Reader\x12\xe2\x02\n\tGetObject\x12,.aserto.directory.reader.v3.GetObjectRequest\x1a-.aserto.directory.reader.v3.GetObjectResponse\"\xf7\x01\x92\x41\xb9\x01\n\tdirectory\x12\x13Get object instance\x1a:Returns single object instance, optionally with relations.*\x17\x64irectory.v3.object.getJ\x1d\n\x03\x33\x30\x34\x12\x16\n\x14Object not modified.b#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v3/directory/object/{object_type}/{object_id}\x12v\n\rGetObjectMany\x12\x30.aserto.directory.reader.v3.GetObjectManyRequest\x1a\x31.aserto.directory.reader.v3.GetObjectManyResponse\"\x00\x12\x98\x02\n\nGetObjects\x12-.aserto.directory.reader.v3.GetObjectsRequest\x1a..aserto.directory.reader.v3.GetObjectsResponse\"\xaa\x01\x92\x41\x85\x01\n\tdirectory\x12\x15List object instances\x1a!Returns list of object instances.*\x19\x64irectory.v3.objects.listb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v3/directory/objects\x12\xd6\x02\n\x0bGetRelation\x12..aserto.directory.reader.v3.GetRelationRequest\x1a/.aserto.directory.reader.v3.GetRelationResponse\"\xe5\x01\x92\x41\xbf\x01\n\tdirectory\x12\x15Get relation instance\x1a:Returns single relation instance, optionally with objects.*\x19\x64irectory.v3.relation.getJ\x1f\n\x03\x33\x30\x34\x12\x18\n\x16Relation not modified.b#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v3/directory/relation\x12\xa7\x02\n\x0cGetRelations\x12/.aserto.directory.reader.v3.GetRelationsRequest\x1a\x30.aserto.directory.reader.v3.GetRelationsResponse\"\xb3\x01\x92\x41\x8c\x01\n\tdirectory\x12\x18List relations instances\x1a#Returns list of relation instances.*\x1b\x64irectory.v3.relations.listb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v3/directory/relations\x12\xe7\x01\n\x05\x43heck\x12(.aserto.directory.reader.v3.CheckRequest\x1a).aserto.directory.reader.v3.CheckResponse\"\x88\x01\x92\x41\x63\n\tdirectory\x12\x05\x43heck\x1a\x16Returns check outcome.*\x12\x64irectory.v3.checkb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v3/directory/check:\x01*\x12\xb2\x02\n\x0f\x43heckPermission\x12\x32.aserto.directory.reader.v3.CheckPermissionRequest\x1a\x33.aserto.directory.reader.v3.CheckPermissionResponse\"\xb5\x01\x92\x41\x84\x01\n\tdirectory\x12\x10\x43heck permission\x1a!Returns check permission outcome.*\x1d\x64irectory.v3.check.permissionb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\'\"\"/api/v3/directory/check/permission:\x01*\x12\xa3\x02\n\rCheckRelation\x12\x30.aserto.directory.reader.v3.CheckRelationRequest\x1a\x31.aserto.directory.reader.v3.CheckRelationResponse\"\xac\x01\x92\x41~\n\tdirectory\x12\x0e\x43heck relation\x1a\x1fReturns check relation outcome.*\x1b\x64irectory.v3.check.relationb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02%\" /api/v3/directory/check/relation:\x01*\x12\xba\x02\n\x08GetGraph\x12+.aserto.directory.reader.v3.GetGraphRequest\x1a,.aserto.directory.reader.v3.GetGraphResponse\"\xd2\x01\x92\x41\x87\x01\n\tdirectory\x12\tGet graph\x1a\x36Returns object graph from anchor to subject or object.*\x12\x64irectory.v3.graphb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x41\x12?/api/v3/directory/graph/{object_type}/{relation}/{subject_type}B\x80\x02\n\x1e\x63om.aserto.directory.reader.v3B\x0bReaderProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/reader/v3;reader\xa2\x02\x03\x41\x44R\xaa\x02\x1a\x41serto.Directory.Reader.V3\xca\x02\x1b\x41serto\\Directory_\\Reader\\V3\xe2\x02\'Aserto\\Directory_\\Reader\\V3\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Reader::V3b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/reader/v3/reader.proto\x12\x1a\x61serto.directory.reader.v3\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\'aserto/directory/common/v3/common.proto\"\xaf\x04\n\x10GetObjectRequest\x12\x8e\x02\n\x0bobject_type\x18\x01 \x01(\tB\xec\x01\xe0\x41\x02\xbaH\xe5\x01r\x02\x18@\xba\x01\xda\x01\n\x16get_object.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x95\x01\n\tobject_id\x18\x02 \x01(\tBx\xbaHur\x03\x18\x80\x02\xba\x01j\n\x14get_object.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12*\n\x0ewith_relations\x18\x03 \x01(\x08\x42\x03\xe0\x41\x01R\rwithRelations\x12\x46\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v3.PaginationRequestB\x03\xe0\x41\x01R\x04page\"\xd7\x01\n\x11GetObjectResponse\x12:\n\x06result\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x06result\x12\x42\n\trelations\x18\x04 \x03(\x0b\x32$.aserto.directory.common.v3.RelationR\trelations\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v3.PaginationResponseR\x04page\"_\n\x14GetObjectManyRequest\x12G\n\x05param\x18\x01 \x03(\x0b\x32,.aserto.directory.common.v3.ObjectIdentifierB\x03\xe0\x41\x02R\x05param\"U\n\x15GetObjectManyResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v3.ObjectR\x07results\"\xed\x02\n\x11GetObjectsRequest\x12\x8f\x02\n\x0bobject_type\x18\x01 \x01(\tB\xed\x01\xe0\x41\x01\xbaH\xe6\x01r\x02\x18@\xba\x01\xdb\x01\n\x17get_objects.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x46\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v3.PaginationRequestB\x03\xe0\x41\x01R\x04page\"\x96\x01\n\x12GetObjectsResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v3.ObjectR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v3.PaginationResponseR\x04page\"\xfd\x0f\n\x12GetRelationRequest\x12\x90\x02\n\x0bobject_type\x18\x01 \x01(\tB\xee\x01\xe0\x41\x02\xbaH\xe7\x01r\x02\x18@\xba\x01\xdc\x01\n\x18get_relation.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x9a\x01\n\tobject_id\x18\x02 \x01(\tB}\xe0\x41\x02\xbaHwr\x03\x18\x80\x02\xba\x01l\n\x16get_relation.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\x08objectId\x12\x88\x02\n\x08relation\x18\x03 \x01(\tB\xeb\x01\xe0\x41\x02\xbaH\xe4\x01r\x02\x18@\xba\x01\xd9\x01\n\x15get_relation.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x08relation\x12\x93\x02\n\x0csubject_type\x18\x04 \x01(\tB\xef\x01\xe0\x41\x02\xbaH\xe8\x01r\x02\x18@\xba\x01\xdd\x01\n\x19get_relation.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0bsubjectType\x12\x9d\x01\n\nsubject_id\x18\x05 \x01(\tB~\xe0\x41\x02\xbaHxr\x03\x18\x80\x02\xba\x01m\n\x17get_relation.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\tsubjectId\x12\x9f\x02\n\x10subject_relation\x18\x06 \x01(\tB\xf3\x01\xe0\x41\x01\xbaH\xec\x01r\x02\x18@\xba\x01\xe1\x01\n\x1dget_relation.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\x12&\n\x0cwith_objects\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x0bwithObjects:\xab\x04\xbaH\xa7\x04\x1a\x8c\x02\n get_relation.object_id_with_type\x12Mwhen an object_id is specified, the accompanying object_type must be provided\x1a\x98\x01(this.object_type == \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id != \'\')\x1a\x95\x02\n!get_relation.subject_id_with_type\x12Owhen an subject_id is specified, the accompanying subject_type must be provided\x1a\x9e\x01(this.subject_type == \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id != \'\')\"\x8b\x02\n\x13GetRelationResponse\x12<\n\x06result\x18\x01 \x01(\x0b\x32$.aserto.directory.common.v3.RelationR\x06result\x12V\n\x07objects\x18\x02 \x03(\x0b\x32<.aserto.directory.reader.v3.GetRelationResponse.ObjectsEntryR\x07objects\x1a^\n\x0cObjectsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x05value:\x02\x38\x01\"\x92\x11\n\x13GetRelationsRequest\x12\x91\x02\n\x0bobject_type\x18\x01 \x01(\tB\xef\x01\xe0\x41\x01\xbaH\xe8\x01r\x02\x18@\xba\x01\xdd\x01\n\x19get_relations.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x9b\x01\n\tobject_id\x18\x02 \x01(\tB~\xe0\x41\x01\xbaHxr\x03\x18\x80\x02\xba\x01m\n\x17get_relations.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\x08objectId\x12\x89\x02\n\x08relation\x18\x03 \x01(\tB\xec\x01\xe0\x41\x01\xbaH\xe5\x01r\x02\x18@\xba\x01\xda\x01\n\x16get_relations.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x08relation\x12\x94\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf0\x01\xe0\x41\x01\xbaH\xe9\x01r\x02\x18@\xba\x01\xde\x01\n\x1aget_relations.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0bsubjectType\x12\x9e\x01\n\nsubject_id\x18\x05 \x01(\tB\x7f\xe0\x41\x01\xbaHyr\x03\x18\x80\x02\xba\x01n\n\x18get_relations.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\tsubjectId\x12\xa0\x02\n\x10subject_relation\x18\x06 \x01(\tB\xf4\x01\xe0\x41\x01\xbaH\xed\x01r\x02\x18@\xba\x01\xe2\x01\n\x1eget_relations.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\x12&\n\x0cwith_objects\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x0bwithObjects\x12\x42\n\x1bwith_empty_subject_relation\x18\x08 \x01(\x08\x42\x03\xe0\x41\x01R\x18withEmptySubjectRelation\x12\x46\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v3.PaginationRequestB\x03\xe0\x41\x01R\x04page:\xad\x04\xbaH\xa9\x04\x1a\x8d\x02\n!get_relations.object_id_with_type\x12Mwhen an object_id is specified, the accompanying object_type must be provided\x1a\x98\x01(this.object_type == \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id == \'\') || (this.object_type != \'\' && this.object_id != \'\')\x1a\x96\x02\n\"get_relations.subject_id_with_type\x12Owhen an subject_id is specified, the accompanying subject_type must be provided\x1a\x9e\x01(this.subject_type == \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id == \'\') || (this.subject_type != \'\' && this.subject_id != \'\')\"\xd3\x02\n\x14GetRelationsResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.aserto.directory.common.v3.RelationR\x07results\x12W\n\x07objects\x18\x02 \x03(\x0b\x32=.aserto.directory.reader.v3.GetRelationsResponse.ObjectsEntryR\x07objects\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v3.PaginationResponseR\x04page\x1a^\n\x0cObjectsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x05value:\x02\x38\x01\"\x87\x08\n\x0c\x43heckRequest\x12\x89\x02\n\x0bobject_type\x18\x01 \x01(\tB\xe7\x01\xe0\x41\x02\xbaH\xe0\x01r\x02\x18@\xba\x01\xd5\x01\n\x11\x63heck.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x93\x01\n\tobject_id\x18\x02 \x01(\tBv\xe0\x41\x02\xbaHpr\x03\x18\x80\x02\xba\x01\x65\n\x0f\x63heck.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\x91\x01\n\x08relation\x18\x03 \x01(\tBu\xe0\x41\x02\xbaHor\x03\x18\x80\x02\xba\x01\x64\n\x0e\x63heck.relation\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08relation\x12\x8c\x02\n\x0csubject_type\x18\x04 \x01(\tB\xe8\x01\xe0\x41\x02\xbaH\xe1\x01r\x02\x18@\xba\x01\xd6\x01\n\x12\x63heck.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\x96\x01\n\nsubject_id\x18\x05 \x01(\tBw\xe0\x41\x02\xbaHqr\x03\x18\x80\x02\xba\x01\x66\n\x10\x63heck.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\x19\n\x05trace\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x05trace\";\n\rCheckResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xd1\x08\n\x16\x43heckPermissionRequest\x12\x94\x02\n\x0bobject_type\x18\x01 \x01(\tB\xf2\x01\xe0\x41\x02\xbaH\xeb\x01r\x02\x18@\xba\x01\xe0\x01\n\x1c\x63heck_permission.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x9f\x01\n\tobject_id\x18\x02 \x01(\tB\x81\x01\xe0\x41\x02\xbaH{r\x03\x18\x80\x02\xba\x01p\n\x1a\x63heck_permission.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\xa3\x01\n\npermission\x18\x03 \x01(\tB\x82\x01\xe0\x41\x02\xbaH|r\x03\x18\x80\x02\xba\x01q\n\x1b\x63heck_permission.permission\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\npermission\x12\x97\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf3\x01\xe0\x41\x02\xbaH\xec\x01r\x02\x18@\xba\x01\xe1\x01\n\x1d\x63heck_permission.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\xa2\x01\n\nsubject_id\x18\x05 \x01(\tB\x82\x01\xe0\x41\x02\xbaH|r\x03\x18\x80\x02\xba\x01q\n\x1b\x63heck_permission.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\x19\n\x05trace\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x05trace\"E\n\x17\x43heckPermissionResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xad\t\n\x14\x43heckRelationRequest\x12\x92\x02\n\x0bobject_type\x18\x01 \x01(\tB\xf0\x01\xe0\x41\x02\xbaH\xe9\x01r\x02\x18@\xba\x01\xde\x01\n\x1a\x63heck_relation.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x9c\x01\n\tobject_id\x18\x02 \x01(\tB\x7f\xe0\x41\x02\xbaHyr\x03\x18\x80\x02\xba\x01n\n\x18\x63heck_relation.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\x8a\x02\n\x08relation\x18\x03 \x01(\tB\xed\x01\xe0\x41\x02\xbaH\xe6\x01r\x02\x18@\xba\x01\xdb\x01\n\x17\x63heck_relation.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x08relation\x12\x95\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf1\x01\xe0\x41\x02\xbaH\xea\x01r\x02\x18@\xba\x01\xdf\x01\n\x1b\x63heck_relation.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\xa0\x01\n\nsubject_id\x18\x05 \x01(\tB\x80\x01\xe0\x41\x02\xbaHzr\x03\x18\x80\x02\xba\x01o\n\x19\x63heck_relation.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\x19\n\x05trace\x18\x07 \x01(\x08\x42\x03\xe0\x41\x01R\x05trace\"C\n\x15\x43heckRelationResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xf0\x0b\n\x0fGetGraphRequest\x12\x8d\x02\n\x0bobject_type\x18\x03 \x01(\tB\xeb\x01\xe0\x41\x02\xbaH\xe4\x01r\x02\x18@\xba\x01\xd9\x01\n\x15get_graph.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\nobjectType\x12\x97\x01\n\tobject_id\x18\x04 \x01(\tBz\xe0\x41\x01\xbaHtr\x03\x18\x80\x02\xba\x01i\n\x13get_graph.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\x08objectId\x12\x85\x02\n\x08relation\x18\x05 \x01(\tB\xe8\x01\xe0\x41\x02\xbaH\xe1\x01r\x02\x18@\xba\x01\xd6\x01\n\x12get_graph.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x08relation\x12\x90\x02\n\x0csubject_type\x18\x06 \x01(\tB\xec\x01\xe0\x41\x02\xbaH\xe5\x01r\x02\x18@\xba\x01\xda\x01\n\x16get_graph.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0bsubjectType\x12\x9a\x01\n\nsubject_id\x18\x07 \x01(\tB{\xe0\x41\x01\xbaHur\x03\x18\x80\x02\xba\x01j\n\x14get_graph.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xd0\x01\x01R\tsubjectId\x12\x9c\x02\n\x10subject_relation\x18\x08 \x01(\tB\xf0\x01\xe0\x41\x01\xbaH\xe9\x01r\x02\x18@\xba\x01\xde\x01\n\x1aget_graph.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\x12\x1d\n\x07\x65xplain\x18\t \x01(\x08\x42\x03\xe0\x41\x01R\x07\x65xplain\x12\x19\n\x05trace\x18\n \x01(\x08\x42\x03\xe0\x41\x01R\x05traceJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03R\x0b\x61nchor_typeR\tanchor_id\"\xb1\x01\n\x10GetGraphResponse\x12\x46\n\x07results\x18\x02 \x03(\x0b\x32,.aserto.directory.common.v3.ObjectIdentifierR\x07results\x12\x39\n\x0b\x65xplanation\x18\x03 \x01(\x0b\x32\x17.google.protobuf.StructR\x0b\x65xplanation\x12\x14\n\x05trace\x18\x04 \x03(\tR\x05traceJ\x04\x08\x01\x10\x02\x32\x85\x14\n\x06Reader\x12\xe2\x02\n\tGetObject\x12,.aserto.directory.reader.v3.GetObjectRequest\x1a-.aserto.directory.reader.v3.GetObjectResponse\"\xf7\x01\x92\x41\xb9\x01\n\tdirectory\x12\x13Get object instance\x1a:Returns single object instance, optionally with relations.*\x17\x64irectory.v3.object.getJ\x1d\n\x03\x33\x30\x34\x12\x16\n\x14Object not modified.b#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v3/directory/object/{object_type}/{object_id}\x12v\n\rGetObjectMany\x12\x30.aserto.directory.reader.v3.GetObjectManyRequest\x1a\x31.aserto.directory.reader.v3.GetObjectManyResponse\"\x00\x12\x98\x02\n\nGetObjects\x12-.aserto.directory.reader.v3.GetObjectsRequest\x1a..aserto.directory.reader.v3.GetObjectsResponse\"\xaa\x01\x92\x41\x85\x01\n\tdirectory\x12\x15List object instances\x1a!Returns list of object instances.*\x19\x64irectory.v3.objects.listb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v3/directory/objects\x12\xd6\x02\n\x0bGetRelation\x12..aserto.directory.reader.v3.GetRelationRequest\x1a/.aserto.directory.reader.v3.GetRelationResponse\"\xe5\x01\x92\x41\xbf\x01\n\tdirectory\x12\x15Get relation instance\x1a:Returns single relation instance, optionally with objects.*\x19\x64irectory.v3.relation.getJ\x1f\n\x03\x33\x30\x34\x12\x18\n\x16Relation not modified.b#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v3/directory/relation\x12\xa7\x02\n\x0cGetRelations\x12/.aserto.directory.reader.v3.GetRelationsRequest\x1a\x30.aserto.directory.reader.v3.GetRelationsResponse\"\xb3\x01\x92\x41\x8c\x01\n\tdirectory\x12\x18List relations instances\x1a#Returns list of relation instances.*\x1b\x64irectory.v3.relations.listb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v3/directory/relations\x12\xe7\x01\n\x05\x43heck\x12(.aserto.directory.reader.v3.CheckRequest\x1a).aserto.directory.reader.v3.CheckResponse\"\x88\x01\x92\x41\x63\n\tdirectory\x12\x05\x43heck\x1a\x16Returns check outcome.*\x12\x64irectory.v3.checkb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v3/directory/check:\x01*\x12\xb2\x02\n\x0f\x43heckPermission\x12\x32.aserto.directory.reader.v3.CheckPermissionRequest\x1a\x33.aserto.directory.reader.v3.CheckPermissionResponse\"\xb5\x01\x92\x41\x84\x01\n\tdirectory\x12\x10\x43heck permission\x1a!Returns check permission outcome.*\x1d\x64irectory.v3.check.permissionb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\'\"\"/api/v3/directory/check/permission:\x01*\x12\xa3\x02\n\rCheckRelation\x12\x30.aserto.directory.reader.v3.CheckRelationRequest\x1a\x31.aserto.directory.reader.v3.CheckRelationResponse\"\xac\x01\x92\x41~\n\tdirectory\x12\x0e\x43heck relation\x1a\x1fReturns check relation outcome.*\x1b\x64irectory.v3.check.relationb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02%\" /api/v3/directory/check/relation:\x01*\x12\xba\x02\n\x08GetGraph\x12+.aserto.directory.reader.v3.GetGraphRequest\x1a,.aserto.directory.reader.v3.GetGraphResponse\"\xd2\x01\x92\x41\x87\x01\n\tdirectory\x12\tGet graph\x1a\x36Returns object graph from anchor to subject or object.*\x12\x64irectory.v3.graphb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x41\x12?/api/v3/directory/graph/{object_type}/{relation}/{subject_type}B\x80\x02\n\x1e\x63om.aserto.directory.reader.v3B\x0bReaderProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/reader/v3;reader\xa2\x02\x03\x41\x44R\xaa\x02\x1a\x41serto.Directory.Reader.V3\xca\x02\x1b\x41serto\\Directory_\\Reader\\V3\xe2\x02\'Aserto\\Directory_\\Reader\\V3\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Reader::V3b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aserto.directory.reader.v3.reader_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\036com.aserto.directory.reader.v3B\013ReaderProtoP\001ZDgithub.com/aserto-dev/go-directory/aserto/directory/reader/v3;reader\242\002\003ADR\252\002\032Aserto.Directory.Reader.V3\312\002\033Aserto\\Directory_\\Reader\\V3\342\002\'Aserto\\Directory_\\Reader\\V3\\GPBMetadata\352\002\035Aserto::Directory::Reader::V3'
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from google.api import annotations_pb2 as _annotations_pb2
+from protoc_gen_openapiv2.options import annotations_pb2 as _annotations_pb2
+from google.api import annotations_pb2 as _annotations_pb2_1
 from google.api import field_behavior_pb2 as _field_behavior_pb2
 from google.protobuf import struct_pb2 as _struct_pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as _annotations_pb2_1
 from buf.validate import validate_pb2 as _validate_pb2
 from aserto.directory.common.v3 import common_pb2 as _common_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/reader/v3/reader_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/reader/v3/reader_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from aserto.directory.schema.v2.tenant_pb2 import (
     TenantKind,
     TenantProperties,
     AccountProperties,
     GuideState,
 )
 
-from aserto.directory.schema.v2.identity_pb2 import (
-    IdentityKind,
-    IdentityProperties,
-)
-
 from aserto.directory.schema.v2.user_pb2 import (
     UserStatus,
     UserProperties,
 )
 
+from aserto.directory.schema.v2.identity_pb2 import (
+    IdentityKind,
+    IdentityProperties,
+)
+
 from aserto.directory.schema.v2.group_pb2 import (
     GroupProperties,
 )
 
 __all__ = [
     "TenantKind",
     "TenantProperties",
     "AccountProperties",
     "GuideState",
-    "IdentityKind",
-    "IdentityProperties",
     "UserStatus",
     "UserProperties",
+    "IdentityKind",
+    "IdentityProperties",
     "GroupProperties",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/group_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/group_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/identity_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/identity_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/identity_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/identity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/tenant_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/tenant_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/tenant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/user_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/user_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v2/user_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/schema/v2/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from aserto.directory.schema.v3.tenant_pb2 import (
     TenantKind,
     TenantProperties,
     AccountProperties,
     GuideState,
 )
 
-from aserto.directory.schema.v3.identity_pb2 import (
-    IdentityKind,
-    IdentityProperties,
-)
-
 from aserto.directory.schema.v3.user_pb2 import (
     UserStatus,
     UserProperties,
 )
 
+from aserto.directory.schema.v3.identity_pb2 import (
+    IdentityKind,
+    IdentityProperties,
+)
+
 from aserto.directory.schema.v3.group_pb2 import (
     GroupProperties,
 )
 
 __all__ = [
     "TenantKind",
     "TenantProperties",
     "AccountProperties",
     "GuideState",
-    "IdentityKind",
-    "IdentityProperties",
     "UserStatus",
     "UserProperties",
+    "IdentityKind",
+    "IdentityProperties",
     "GroupProperties",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/group_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/group_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/identity_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/identity_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/identity_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/identity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/tenant_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/tenant_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/tenant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/user_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/user_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/schema/v3/user_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/schema/v3/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v2/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/writer/v2/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # This file is generated by init_gen.py. Do not edit.
 
+from aserto.directory.writer.v2.writer_pb2_grpc import (
+    WriterStub,
+    WriterServicer,
+)
+
 from aserto.directory.writer.v2.writer_pb2 import (
     SetObjectTypeRequest,
     SetObjectTypeResponse,
     DeleteObjectTypeRequest,
     DeleteObjectTypeResponse,
     SetRelationTypeRequest,
     SetRelationTypeResponse,
@@ -19,20 +24,17 @@
     DeleteObjectResponse,
     SetRelationRequest,
     SetRelationResponse,
     DeleteRelationRequest,
     DeleteRelationResponse,
 )
 
-from aserto.directory.writer.v2.writer_pb2_grpc import (
-    WriterStub,
-    WriterServicer,
-)
-
 __all__ = [
+    "WriterStub",
+    "WriterServicer",
     "SetObjectTypeRequest",
     "SetObjectTypeResponse",
     "DeleteObjectTypeRequest",
     "DeleteObjectTypeResponse",
     "SetRelationTypeRequest",
     "SetRelationTypeResponse",
     "DeleteRelationTypeRequest",
@@ -45,10 +47,8 @@
     "SetObjectResponse",
     "DeleteObjectRequest",
     "DeleteObjectResponse",
     "SetRelationRequest",
     "SetRelationResponse",
     "DeleteRelationRequest",
     "DeleteRelationResponse",
-    "WriterStub",
-    "WriterServicer",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v3/__init__.py` & `aserto_directory-0.31.3/src/aserto/directory/writer/v3/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file is generated by init_gen.py. Do not edit.
 
+from aserto.directory.writer.v3.writer_pb2_grpc import (
+    WriterStub,
+    WriterServicer,
+)
+
 from aserto.directory.writer.v3.writer_pb2 import (
     SetObjectRequest,
     SetObjectResponse,
     DeleteObjectRequest,
     DeleteObjectResponse,
     SetRelationRequest,
     SetRelationResponse,
     DeleteRelationRequest,
     DeleteRelationResponse,
 )
 
-from aserto.directory.writer.v3.writer_pb2_grpc import (
-    WriterStub,
-    WriterServicer,
-)
-
 __all__ = [
+    "WriterStub",
+    "WriterServicer",
     "SetObjectRequest",
     "SetObjectResponse",
     "DeleteObjectRequest",
     "DeleteObjectResponse",
     "SetRelationRequest",
     "SetRelationResponse",
     "DeleteRelationRequest",
     "DeleteRelationResponse",
-    "WriterStub",
-    "WriterServicer",
 ]
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2.py` & `aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from aserto.directory.common.v3 import common_pb2 as aserto_dot_directory_dot_common_dot_v3_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/writer/v3/writer.proto\x12\x1a\x61serto.directory.writer.v3\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\'aserto/directory/common/v3/common.proto\"Y\n\x10SetObjectRequest\x12\x45\n\x06object\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectB\t\xe0\x41\x02\xbaH\x03\xc8\x01\x01R\x06object\"O\n\x11SetObjectResponse\x12:\n\x06result\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x06result\"\xf3\x03\n\x13\x44\x65leteObjectRequest\x12\x91\x02\n\x0bobject_type\x18\x01 \x01(\tB\xef\x01\xe0\x41\x02\xbaH\xe8\x01r\x02\x18@\xba\x01\xdd\x01\n\x19\x64\x65lete_object.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x9b\x01\n\tobject_id\x18\x02 \x01(\tB~\xe0\x41\x02\xbaHxr\x03\x18\x80\x02\xba\x01m\n\x17\x64\x65lete_object.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12*\n\x0ewith_relations\x18\x03 \x01(\x08\x42\x03\xe0\x41\x01R\rwithRelations\"F\n\x14\x44\x65leteObjectResponse\x12.\n\x06result\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyR\x06result\"a\n\x12SetRelationRequest\x12K\n\x08relation\x18\x01 \x01(\x0b\x32$.aserto.directory.common.v3.RelationB\t\xe0\x41\x02\xbaH\x03\xc8\x01\x01R\x08relation\"S\n\x13SetRelationResponse\x12<\n\x06result\x18\x01 \x01(\x0b\x32$.aserto.directory.common.v3.RelationR\x06result\"\xbb\x0b\n\x15\x44\x65leteRelationRequest\x12\x90\x02\n\x0bobject_type\x18\x01 \x01(\tB\xee\x01\xe0\x41\x02\xbaH\xe7\x01r\x02\x18@\xba\x01\xdf\x01\n\x1b\x64\x65lete_relation.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')R\nobjectType\x12\x9e\x01\n\tobject_id\x18\x02 \x01(\tB\x80\x01\xe0\x41\x02\xbaHzr\x03\x18\x80\x02\xba\x01o\n\x19\x64\x65lete_relation.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\x8b\x02\n\x08relation\x18\x03 \x01(\tB\xee\x01\xe0\x41\x02\xbaH\xe7\x01r\x02\x18@\xba\x01\xdc\x01\n\x18\x64\x65lete_relation.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x08relation\x12\x96\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf2\x01\xe0\x41\x02\xbaH\xeb\x01r\x02\x18@\xba\x01\xe0\x01\n\x1c\x64\x65lete_relation.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\xa1\x01\n\nsubject_id\x18\x05 \x01(\tB\x81\x01\xe0\x41\x02\xbaH{r\x03\x18\x80\x02\xba\x01p\n\x1a\x64\x65lete_relation.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\xa2\x02\n\x10subject_relation\x18\x06 \x01(\tB\xf6\x01\xe0\x41\x01\xbaH\xef\x01r\x02\x18@\xba\x01\xe4\x01\n delete_relation.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\"H\n\x16\x44\x65leteRelationResponse\x12.\n\x06result\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyR\x06result2\xb4\x08\n\x06Writer\x12\xf3\x01\n\tSetObject\x12,.aserto.directory.writer.v3.SetObjectRequest\x1a-.aserto.directory.writer.v3.SetObjectResponse\"\x88\x01\x92\x41\x62\n\tdirectory\x12\nSet object\x1a\x0bSet object.*\x17\x64irectory.v3.object.setb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1d\"\x18/api/v3/directory/object:\x01*\x12\x9c\x02\n\x0c\x44\x65leteObject\x12/.aserto.directory.writer.v3.DeleteObjectRequest\x1a\x30.aserto.directory.writer.v3.DeleteObjectResponse\"\xa8\x01\x92\x41k\n\tdirectory\x12\rDelete object\x1a\x0e\x44\x65lete object.*\x1a\x64irectory.v3.object.deleteb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x34*2/api/v3/directory/object/{object_type}/{object_id}\x12\x81\x02\n\x0bSetRelation\x12..aserto.directory.writer.v3.SetRelationRequest\x1a/.aserto.directory.writer.v3.SetRelationResponse\"\x90\x01\x92\x41h\n\tdirectory\x12\x0cSet relation\x1a\rSet relation.*\x19\x64irectory.v3.relation.setb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1f\"\x1a/api/v3/directory/relation:\x01*\x12\x90\x02\n\x0e\x44\x65leteRelation\x12\x31.aserto.directory.writer.v3.DeleteRelationRequest\x1a\x32.aserto.directory.writer.v3.DeleteRelationResponse\"\x96\x01\x92\x41q\n\tdirectory\x12\x0f\x44\x65lete relation\x1a\x10\x44\x65lete relation.*\x1c\x64irectory.v3.relation.deleteb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1c*\x1a/api/v3/directory/relationB\x80\x02\n\x1e\x63om.aserto.directory.writer.v3B\x0bWriterProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/writer/v3;writer\xa2\x02\x03\x41\x44W\xaa\x02\x1a\x41serto.Directory.Writer.V3\xca\x02\x1b\x41serto\\Directory_\\Writer\\V3\xe2\x02\'Aserto\\Directory_\\Writer\\V3\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Writer::V3b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/writer/v3/writer.proto\x12\x1a\x61serto.directory.writer.v3\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\'aserto/directory/common/v3/common.proto\"Y\n\x10SetObjectRequest\x12\x45\n\x06object\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectB\t\xe0\x41\x02\xbaH\x03\xc8\x01\x01R\x06object\"O\n\x11SetObjectResponse\x12:\n\x06result\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v3.ObjectR\x06result\"\xf3\x03\n\x13\x44\x65leteObjectRequest\x12\x91\x02\n\x0bobject_type\x18\x01 \x01(\tB\xef\x01\xe0\x41\x02\xbaH\xe8\x01r\x02\x18@\xba\x01\xdd\x01\n\x19\x64\x65lete_object.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\nobjectType\x12\x9b\x01\n\tobject_id\x18\x02 \x01(\tB~\xe0\x41\x02\xbaHxr\x03\x18\x80\x02\xba\x01m\n\x17\x64\x65lete_object.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12*\n\x0ewith_relations\x18\x03 \x01(\x08\x42\x03\xe0\x41\x01R\rwithRelations\"F\n\x14\x44\x65leteObjectResponse\x12.\n\x06result\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyR\x06result\"a\n\x12SetRelationRequest\x12K\n\x08relation\x18\x01 \x01(\x0b\x32$.aserto.directory.common.v3.RelationB\t\xe0\x41\x02\xbaH\x03\xc8\x01\x01R\x08relation\"S\n\x13SetRelationResponse\x12<\n\x06result\x18\x01 \x01(\x0b\x32$.aserto.directory.common.v3.RelationR\x06result\"\xbb\x0b\n\x15\x44\x65leteRelationRequest\x12\x90\x02\n\x0bobject_type\x18\x01 \x01(\tB\xee\x01\xe0\x41\x02\xbaH\xe7\x01r\x02\x18@\xba\x01\xdf\x01\n\x1b\x64\x65lete_relation.object_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')R\nobjectType\x12\x9e\x01\n\tobject_id\x18\x02 \x01(\tB\x80\x01\xe0\x41\x02\xbaHzr\x03\x18\x80\x02\xba\x01o\n\x19\x64\x65lete_relation.object_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\x08objectId\x12\x8b\x02\n\x08relation\x18\x03 \x01(\tB\xee\x01\xe0\x41\x02\xbaH\xe7\x01r\x02\x18@\xba\x01\xdc\x01\n\x18\x64\x65lete_relation.relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x08relation\x12\x96\x02\n\x0csubject_type\x18\x04 \x01(\tB\xf2\x01\xe0\x41\x02\xbaH\xeb\x01r\x02\x18@\xba\x01\xe0\x01\n\x1c\x64\x65lete_relation.subject_type\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xc8\x01\x01R\x0bsubjectType\x12\xa1\x01\n\nsubject_id\x18\x05 \x01(\tB\x81\x01\xe0\x41\x02\xbaH{r\x03\x18\x80\x02\xba\x01p\n\x1a\x64\x65lete_relation.subject_id\x12\x38\x63\x61nnot contain any spaces or other whitespace characters\x1a\x18this.matches(\'^[\\\\S]+$\')\xc8\x01\x01R\tsubjectId\x12\xa2\x02\n\x10subject_relation\x18\x06 \x01(\tB\xf6\x01\xe0\x41\x01\xbaH\xef\x01r\x02\x18@\xba\x01\xe4\x01\n delete_relation.subject_relation\x12\x8b\x01must be all lowercase, start with a letter, can contain letters, digits, dots, underscores, and dashes, and must end with a letter or digit\x1a\x32this.matches(\'^[a-z][a-z0-9\\\\._-]{1,62}[a-z0-9]$\')\xd0\x01\x01R\x0fsubjectRelation\"H\n\x16\x44\x65leteRelationResponse\x12.\n\x06result\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyR\x06result2\xb4\x08\n\x06Writer\x12\xf3\x01\n\tSetObject\x12,.aserto.directory.writer.v3.SetObjectRequest\x1a-.aserto.directory.writer.v3.SetObjectResponse\"\x88\x01\x92\x41\x62\n\tdirectory\x12\nSet object\x1a\x0bSet object.*\x17\x64irectory.v3.object.setb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1d\"\x18/api/v3/directory/object:\x01*\x12\x9c\x02\n\x0c\x44\x65leteObject\x12/.aserto.directory.writer.v3.DeleteObjectRequest\x1a\x30.aserto.directory.writer.v3.DeleteObjectResponse\"\xa8\x01\x92\x41k\n\tdirectory\x12\rDelete object\x1a\x0e\x44\x65lete object.*\x1a\x64irectory.v3.object.deleteb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x34*2/api/v3/directory/object/{object_type}/{object_id}\x12\x81\x02\n\x0bSetRelation\x12..aserto.directory.writer.v3.SetRelationRequest\x1a/.aserto.directory.writer.v3.SetRelationResponse\"\x90\x01\x92\x41h\n\tdirectory\x12\x0cSet relation\x1a\rSet relation.*\x19\x64irectory.v3.relation.setb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1f\"\x1a/api/v3/directory/relation:\x01*\x12\x90\x02\n\x0e\x44\x65leteRelation\x12\x31.aserto.directory.writer.v3.DeleteRelationRequest\x1a\x32.aserto.directory.writer.v3.DeleteRelationResponse\"\x96\x01\x92\x41q\n\tdirectory\x12\x0f\x44\x65lete relation\x1a\x10\x44\x65lete relation.*\x1c\x64irectory.v3.relation.deleteb#\n\x13\n\x0f\x44irectoryAPIKey\x12\x00\n\x0c\n\x08TenantID\x12\x00\x82\xd3\xe4\x93\x02\x1c*\x1a/api/v3/directory/relationB\x80\x02\n\x1e\x63om.aserto.directory.writer.v3B\x0bWriterProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/writer/v3;writer\xa2\x02\x03\x41\x44W\xaa\x02\x1a\x41serto.Directory.Writer.V3\xca\x02\x1b\x41serto\\Directory_\\Writer\\V3\xe2\x02\'Aserto\\Directory_\\Writer\\V3\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Writer::V3b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aserto.directory.writer.v3.writer_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\036com.aserto.directory.writer.v3B\013WriterProtoP\001ZDgithub.com/aserto-dev/go-directory/aserto/directory/writer/v3;writer\242\002\003ADW\252\002\032Aserto.Directory.Writer.V3\312\002\033Aserto\\Directory_\\Writer\\V3\342\002\'Aserto\\Directory_\\Writer\\V3\\GPBMetadata\352\002\035Aserto::Directory::Writer::V3'
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2.pyi` & `aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from protoc_gen_openapiv2.options import annotations_pb2 as _annotations_pb2
 from google.protobuf import empty_pb2 as _empty_pb2
-from google.api import annotations_pb2 as _annotations_pb2
+from google.api import annotations_pb2 as _annotations_pb2_1
 from google.api import field_behavior_pb2 as _field_behavior_pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as _annotations_pb2_1
 from buf.validate import validate_pb2 as _validate_pb2
 from aserto.directory.common.v3 import common_pb2 as _common_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2_grpc.py` & `aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/aserto/directory/writer/v3/writer_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/aserto/directory/writer/v3/writer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/expression_pb2.py` & `aserto_directory-0.31.3/src/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/expression_pb2.pyi` & `aserto_directory-0.31.3/src/buf/validate/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/expression_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/buf/validate/expression_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/priv/private_pb2.py` & `aserto_directory-0.31.3/src/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/priv/private_pb2.pyi` & `aserto_directory-0.31.3/src/buf/validate/priv/private_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/priv/private_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/buf/validate/priv/private_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/validate_pb2.py` & `aserto_directory-0.31.3/src/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/validate_pb2.pyi` & `aserto_directory-0.31.3/src/buf/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/buf/validate/validate_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/buf/validate/validate_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/annotations_pb2.py` & `aserto_directory-0.31.3/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/annotations_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/field_behavior_pb2.py` & `aserto_directory-0.31.3/src/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/field_behavior_pb2.pyi` & `aserto_directory-0.31.3/src/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/field_behavior_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/http_pb2.py` & `aserto_directory-0.31.3/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/http_pb2.pyi` & `aserto_directory-0.31.3/src/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/src/google/api/http_pb2_grpc.pyi` & `aserto_directory-0.31.3/src/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto_directory-0.31.2/PKG-INFO` & `aserto_directory-0.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aserto-directory
-Version: 0.31.2
+Version: 0.31.3
 Summary: gRPC client for Aserto Directory service instances
 Home-page: https://github.com/aserto-dev/python-directory
 License: Apache-2.0
 Author: Aserto, Inc.
 Author-email: pypi@aserto.com
 Requires-Python: >=3.8,<4
 Classifier: Intended Audience :: Developers
```

