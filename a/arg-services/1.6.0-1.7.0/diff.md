# Comparing `tmp/arg_services-1.6.0.tar.gz` & `tmp/arg_services-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg_services-1.6.0.tar", max compression
+gzip compressed data, was "arg_services-1.7.0.tar", max compression
```

## Comparing `arg_services-1.6.0.tar` & `arg_services-1.7.0.tar`

### file list

```diff
@@ -1,81 +1,105 @@
--rw-r--r--   0        0        0     1067 2023-11-13 09:03:19.701358 arg_services-1.6.0/LICENSE
--rw-r--r--   0        0        0      657 2023-11-13 09:03:19.701358 arg_services-1.6.0/README.md
--rw-r--r--   0        0        0      666 2023-11-13 09:04:41.590044 arg_services-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     7916 2023-11-13 09:04:41.050040 arg_services-1.6.0/src/arg_services/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.030039 arg_services-1.6.0/src/arg_services/cbr/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.034040 arg_services-1.6.0/src/arg_services/cbr/v1beta/__init__.py
--rw-r--r--   0        0        0     7194 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2.py
--rw-r--r--   0        0        0    12424 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
--rw-r--r--   0        0        0     2783 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
--rw-r--r--   0        0        0     1470 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3487 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2.py
--rw-r--r--   0        0        0     3094 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
--rw-r--r--   0        0        0     1474 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
--rw-r--r--   0        0        0     2566 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/model_pb2.py
--rw-r--r--   0        0        0     2515 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/model_pb2.pyi
--rw-r--r--   0        0        0      159 2023-11-13 09:04:40.986039 arg_services-1.6.0/src/arg_services/cbr/v1beta/model_pb2_grpc.py
--rw-r--r--   0        0        0      400 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     8381 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2.py
--rw-r--r--   0        0        0    15179 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
--rw-r--r--   0        0        0     4628 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
--rw-r--r--   0        0        0     2214 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.022040 arg_services-1.6.0/src/arg_services/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.026039 arg_services-1.6.0/src/arg_services/graph/v1/__init__.py
--rw-r--r--   0        0        0    12004 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/graph/v1/graph_pb2.py
--rw-r--r--   0        0        0    33449 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/graph/v1/graph_pb2.pyi
--rw-r--r--   0        0        0      159 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/graph/v1/graph_pb2_grpc.py
--rw-r--r--   0        0        0      475 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.038040 arg_services-1.6.0/src/arg_services/mining/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.038040 arg_services-1.6.0/src/arg_services/mining/v1beta/__init__.py
--rw-r--r--   0        0        0     5123 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     6692 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     4625 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     2199 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     5853 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     9022 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     2894 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1554 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     4221 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2.py
--rw-r--r--   0        0        0     3932 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
--rw-r--r--   0        0        0     3092 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
--rw-r--r--   0        0        0     1713 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
--rw-r--r--   0        0        0     3883 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     4057 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     2896 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0     1552 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0     2977 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2.py
--rw-r--r--   0        0        0     2419 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2.pyi
--rw-r--r--   0        0        0     2834 2023-11-13 09:04:40.990039 arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py
--rw-r--r--   0        0        0     1502 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.026039 arg_services-1.6.0/src/arg_services/mining_explanation/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.030039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/__init__.py
--rw-r--r--   0        0        0     3418 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     3359 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     3044 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     1644 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     4573 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     5167 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     3110 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1705 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     3928 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     3980 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     3112 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0     1703 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.042039 arg_services-1.6.0/src/arg_services/nlp/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.042039 arg_services-1.6.0/src/arg_services/nlp/v1/__init__.py
--rw-r--r--   0        0        0     9100 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2.py
--rw-r--r--   0        0        0    27846 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2.pyi
--rw-r--r--   0        0        0     6344 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py
--rw-r--r--   0        0        0     4043 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.018039 arg_services-1.6.0/src/google/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 09:04:41.018039 arg_services-1.6.0/src/google/api/__init__.py
--rw-r--r--   0        0        0     1756 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      951 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2654 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/http_pb2.py
--rw-r--r--   0        0        0    18295 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      951 2023-11-13 09:04:40.994039 arg_services-1.6.0/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 arg_services-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-04 09:41:41.288773 arg_services-1.7.0/LICENSE
+-rw-r--r--   0        0        0      657 2024-04-04 09:41:41.288773 arg_services-1.7.0/README.md
+-rw-r--r--   0        0        0      666 2024-04-04 09:42:41.552676 arg_services-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7916 2024-04-04 09:42:41.184677 arg_services-1.7.0/src/arg_services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.160677 arg_services-1.7.0/src/arg_services/cbr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.160677 arg_services-1.7.0/src/arg_services/cbr/v1beta/__init__.py
+-rw-r--r--   0        0        0     7194 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.py
+-rw-r--r--   0        0        0    12424 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
+-rw-r--r--   0        0        0     2783 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
+-rw-r--r--   0        0        0     1470 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3487 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.py
+-rw-r--r--   0        0        0     3094 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi
+-rw-r--r--   0        0        0     2792 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
+-rw-r--r--   0        0        0     1474 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2566 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.py
+-rw-r--r--   0        0        0     2515 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8381 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.py
+-rw-r--r--   0        0        0    15179 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
+-rw-r--r--   0        0        0     4628 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
+-rw-r--r--   0        0        0     2214 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.172677 arg_services-1.7.0/src/arg_services/graph/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.172677 arg_services-1.7.0/src/arg_services/graph/v1/__init__.py
+-rw-r--r--   0        0        0    12004 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.py
+-rw-r--r--   0        0        0    33449 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2_grpc.py
+-rw-r--r--   0        0        0      475 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.152677 arg_services-1.7.0/src/arg_services/mining/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.152677 arg_services-1.7.0/src/arg_services/mining/v1beta/__init__.py
+-rw-r--r--   0        0        0     5123 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     6692 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     4625 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     2199 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5853 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     9022 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     2894 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1554 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4221 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.py
+-rw-r--r--   0        0        0     3932 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
+-rw-r--r--   0        0        0     3092 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
+-rw-r--r--   0        0        0     1713 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3883 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     4057 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     2896 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0     1552 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2977 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.py
+-rw-r--r--   0        0        0     2419 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.pyi
+-rw-r--r--   0        0        0     2834 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py
+-rw-r--r--   0        0        0     1502 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.164677 arg_services-1.7.0/src/arg_services/mining_explanation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.164677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/__init__.py
+-rw-r--r--   0        0        0     3418 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     3359 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     3044 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     1644 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4573 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     5167 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     3110 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1705 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3928 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     3980 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     3112 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0     1703 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.168677 arg_services-1.7.0/src/arg_services/nlp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.168677 arg_services-1.7.0/src/arg_services/nlp/v1/__init__.py
+-rw-r--r--   0        0        0     9100 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.py
+-rw-r--r--   0        0        0    27846 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.pyi
+-rw-r--r--   0        0        0     6344 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py
+-rw-r--r--   0        0        0     4043 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.148677 arg_services-1.7.0/src/arg_services/quality/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.148677 arg_services-1.7.0/src/arg_services/quality/v1beta/__init__.py
+-rw-r--r--   0        0        0     4342 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2.py
+-rw-r--r--   0        0        0     5228 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2.pyi
+-rw-r--r--   0        0        0     2961 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2_grpc.py
+-rw-r--r--   0        0        0     1595 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4494 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2.py
+-rw-r--r--   0        0        0     5884 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2.pyi
+-rw-r--r--   0        0        0     2917 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2_grpc.py
+-rw-r--r--   0        0        0     1570 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4102 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2.py
+-rw-r--r--   0        0        0     5224 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2.pyi
+-rw-r--r--   0        0        0     2923 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2_grpc.py
+-rw-r--r--   0        0        0     1570 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.156677 arg_services-1.7.0/src/arg_services/ranking/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.156677 arg_services-1.7.0/src/arg_services/ranking/v1beta/__init__.py
+-rw-r--r--   0        0        0     3509 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2.py
+-rw-r--r--   0        0        0     3421 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2.pyi
+-rw-r--r--   0        0        0     3063 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2_grpc.py
+-rw-r--r--   0        0        0     1685 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6899 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2.py
+-rw-r--r--   0        0        0     9900 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2.pyi
+-rw-r--r--   0        0        0     4814 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2_grpc.py
+-rw-r--r--   0        0        0     2354 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.176677 arg_services-1.7.0/src/google/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:42:41.176677 arg_services-1.7.0/src/google/api/__init__.py
+-rw-r--r--   0        0        0     1756 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2654 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18295 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 arg_services-1.7.0/PKG-INFO
```

### Comparing `arg_services-1.6.0/LICENSE` & `arg_services-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/README.md` & `arg_services-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/pyproject.toml` & `arg_services-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arg-services"
-version = "1.6.0"
+version = "1.7.0"
 description = "gRPC definitions for microservice-based argumentation machines"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arg-services-python"
 include = ["src/**/*"]
```

### Comparing `arg_services-1.6.0/src/arg_services/__init__.py` & `arg_services-1.7.0/src/arg_services/__init__.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/model_pb2.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/model_pb2.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/graph/v1/graph_pb2.py` & `arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/graph/v1/graph_pb2.pyi` & `arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2.py` & `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2.pyi` & `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py` & `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi` & `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/google/api/annotations_pb2.py` & `arg_services-1.7.0/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/google/api/annotations_pb2.pyi` & `arg_services-1.7.0/src/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/google/api/annotations_pb2_grpc.pyi` & `arg_services-1.7.0/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/google/api/http_pb2.py` & `arg_services-1.7.0/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/google/api/http_pb2.pyi` & `arg_services-1.7.0/src/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/src/google/api/http_pb2_grpc.pyi` & `arg_services-1.7.0/src/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.6.0/PKG-INFO` & `arg_services-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: arg-services
-Version: 1.6.0
+Version: 1.7.0
 Summary: gRPC definitions for microservice-based argumentation machines
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpc-stubs (>=1.53,<2.0)
 Requires-Dist: grpcio (>=1.53,<2.0)
 Requires-Dist: grpcio-reflection (>=1.53,<2.0)
 Requires-Dist: protobuf (>=4.22,<5.0)
 Project-URL: Repository, https://github.com/recap-utr/arg-services-python
 Description-Content-Type: text/markdown
```

