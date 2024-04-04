# Comparing `tmp/pycspr-1.1.3.tar.gz` & `tmp/pycspr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycspr-1.1.3.tar", max compression
+gzip compressed data, was "pycspr-1.2.0.tar", max compression
```

## Comparing `pycspr-1.1.3.tar` & `pycspr-1.2.0.tar`

### file list

```diff
@@ -1,77 +1,80 @@
--rw-r--r--   0        0        0    11357 2023-05-15 10:59:30.289726 pycspr-1.1.3/LICENSE
--rw-r--r--   0        0        0     2517 2024-03-03 21:45:57.409847 pycspr-1.1.3/README.md
--rw-r--r--   0        0        0     2747 2024-03-19 20:37:54.719931 pycspr-1.1.3/pycspr/__init__.py
--rw-r--r--   0        0        0      460 2024-03-03 21:45:57.413347 pycspr-1.1.3/pycspr/api/__init__.py
--rw-r--r--   0        0        0      602 2024-03-05 10:29:32.580956 pycspr-1.1.3/pycspr/api/connection.py
--rw-r--r--   0        0        0     1963 2024-03-15 18:54:27.914869 pycspr-1.1.3/pycspr/api/constants.py
--rw-r--r--   0        0        0       42 2024-02-28 10:36:33.382052 pycspr-1.1.3/pycspr/api/rest/__init__.py
--rw-r--r--   0        0        0     2146 2024-03-05 10:29:32.581142 pycspr-1.1.3/pycspr/api/rest/client.py
--rw-r--r--   0        0        0     2127 2024-03-05 10:29:32.581328 pycspr-1.1.3/pycspr/api/rest/proxy.py
--rw-r--r--   0        0        0       41 2024-02-28 10:36:33.383627 pycspr-1.1.3/pycspr/api/rpc/__init__.py
--rw-r--r--   0        0        0    13234 2024-03-19 20:49:45.550545 pycspr-1.1.3/pycspr/api/rpc/client.py
--rw-r--r--   0        0        0    19655 2024-03-19 20:26:50.713953 pycspr-1.1.3/pycspr/api/rpc/decoder.py
--rw-r--r--   0        0        0     5773 2024-03-19 20:26:50.714373 pycspr-1.1.3/pycspr/api/rpc/params.py
--rw-r--r--   0        0        0    11135 2024-03-19 20:26:50.714875 pycspr-1.1.3/pycspr/api/rpc/proxy.py
--rw-r--r--   0        0        0     6671 2024-03-19 20:26:50.715290 pycspr-1.1.3/pycspr/api/rpc/types.py
--rw-r--r--   0        0        0       53 2024-02-28 10:36:33.387538 pycspr-1.1.3/pycspr/api/rpc_speculative/__init__.py
--rw-r--r--   0        0        0      926 2024-03-05 10:29:32.582633 pycspr-1.1.3/pycspr/api/rpc_speculative/client.py
--rw-r--r--   0        0        0     1377 2024-03-19 20:26:50.716155 pycspr-1.1.3/pycspr/api/rpc_speculative/proxy.py
--rw-r--r--   0        0        0      243 2024-03-05 10:29:32.583007 pycspr-1.1.3/pycspr/api/sse/__init__.py
--rw-r--r--   0        0        0     5239 2024-03-03 21:45:57.416248 pycspr-1.1.3/pycspr/api/sse/client.py
--rw-r--r--   0        0        0     2653 2024-03-19 20:26:50.716398 pycspr-1.1.3/pycspr/api/sse/proxy.py
--rw-r--r--   0        0        0     1541 2024-03-02 21:52:48.787077 pycspr-1.1.3/pycspr/api/sse/types.py
--rw-r--r--   0        0        0     1183 2023-05-15 10:59:30.291740 pycspr-1.1.3/pycspr/crypto/__init__.py
--rw-r--r--   0        0        0     4802 2023-05-15 10:59:30.291792 pycspr-1.1.3/pycspr/crypto/cl_checksum.py
--rw-r--r--   0        0        0     3187 2024-03-15 20:06:52.108662 pycspr-1.1.3/pycspr/crypto/cl_operations.py
--rw-r--r--   0        0        0      174 2024-02-11 20:41:49.550992 pycspr-1.1.3/pycspr/crypto/defaults.py
--rw-r--r--   0        0        0     5427 2024-03-15 20:54:21.551040 pycspr-1.1.3/pycspr/crypto/ecc.py
--rw-r--r--   0        0        0     3840 2023-05-15 10:59:30.291984 pycspr-1.1.3/pycspr/crypto/ecc_ed25519.py
--rw-r--r--   0        0        0     3090 2023-05-15 10:59:30.292031 pycspr-1.1.3/pycspr/crypto/ecc_secp256k1.py
--rw-r--r--   0        0        0      297 2024-02-11 20:50:27.642942 pycspr-1.1.3/pycspr/crypto/enums.py
--rw-r--r--   0        0        0      791 2024-02-11 20:50:27.643103 pycspr-1.1.3/pycspr/crypto/hashifier.py
--rw-r--r--   0        0        0      322 2024-02-11 20:37:22.630050 pycspr-1.1.3/pycspr/crypto/hashifier_blake2b.py
--rw-r--r--   0        0        0      302 2024-02-11 20:50:27.643216 pycspr-1.1.3/pycspr/crypto/hashifier_blake3.py
--rw-r--r--   0        0        0     1363 2023-05-15 10:59:30.292257 pycspr-1.1.3/pycspr/factory/__init__.py
--rw-r--r--   0        0        0     2957 2023-05-15 10:59:30.292315 pycspr-1.1.3/pycspr/factory/accounts.py
--rw-r--r--   0        0        0    12129 2024-03-15 20:44:25.575732 pycspr-1.1.3/pycspr/factory/deploys.py
--rw-r--r--   0        0        0     1626 2024-03-19 20:26:50.716628 pycspr-1.1.3/pycspr/factory/digests.py
--rw-r--r--   0        0        0      505 2024-03-19 20:32:14.668303 pycspr-1.1.3/pycspr/serialisation/__init__.py
--rw-r--r--   0        0        0      930 2024-03-19 20:26:50.717015 pycspr-1.1.3/pycspr/serialisation/binary/__init__.py
--rw-r--r--   0        0        0      126 2023-05-15 10:59:30.292713 pycspr-1.1.3/pycspr/serialisation/binary/cl_type/__init__.py
--rw-r--r--   0        0        0     2971 2024-03-19 20:26:50.717205 pycspr-1.1.3/pycspr/serialisation/binary/cl_type/decoder.py
--rw-r--r--   0        0        0     2204 2024-03-19 20:26:50.717397 pycspr-1.1.3/pycspr/serialisation/binary/cl_type/encoder.py
--rw-r--r--   0        0        0      128 2023-05-15 10:59:30.292894 pycspr-1.1.3/pycspr/serialisation/binary/cl_value/__init__.py
--rw-r--r--   0        0        0     7866 2024-03-19 20:26:50.717595 pycspr-1.1.3/pycspr/serialisation/binary/cl_value/decoder.py
--rw-r--r--   0        0        0     3237 2024-03-19 20:26:50.717788 pycspr-1.1.3/pycspr/serialisation/binary/cl_value/encoder.py
--rw-r--r--   0        0        0      124 2024-03-19 20:26:50.717944 pycspr-1.1.3/pycspr/serialisation/binary/entity/__init__.py
--rw-r--r--   0        0        0     9193 2024-03-19 20:26:50.718158 pycspr-1.1.3/pycspr/serialisation/binary/entity/decoder.py
--rw-r--r--   0        0        0     5645 2024-03-19 20:26:50.718282 pycspr-1.1.3/pycspr/serialisation/binary/entity/encoder.py
--rw-r--r--   0        0        0      933 2024-03-19 20:26:50.718498 pycspr-1.1.3/pycspr/serialisation/json/__init__.py
--rw-r--r--   0        0        0      122 2023-05-15 10:59:30.293329 pycspr-1.1.3/pycspr/serialisation/json/cl_type/__init__.py
--rw-r--r--   0        0        0     2340 2024-03-19 20:26:50.718695 pycspr-1.1.3/pycspr/serialisation/json/cl_type/decoder.py
--rw-r--r--   0        0        0     2402 2024-03-19 20:26:50.718924 pycspr-1.1.3/pycspr/serialisation/json/cl_type/encoder.py
--rw-r--r--   0        0        0      124 2023-05-15 10:59:30.293485 pycspr-1.1.3/pycspr/serialisation/json/cl_value/__init__.py
--rw-r--r--   0        0        0      616 2024-03-19 20:26:50.719133 pycspr-1.1.3/pycspr/serialisation/json/cl_value/decoder.py
--rw-r--r--   0        0        0      714 2024-03-19 20:26:50.719319 pycspr-1.1.3/pycspr/serialisation/json/cl_value/encoder.py
--rw-r--r--   0        0        0      120 2024-03-19 20:26:50.719448 pycspr-1.1.3/pycspr/serialisation/json/entity/__init__.py
--rw-r--r--   0        0        0     5816 2024-03-19 20:26:50.719577 pycspr-1.1.3/pycspr/serialisation/json/entity/decoder.py
--rw-r--r--   0        0        0     4385 2024-03-19 20:26:50.719700 pycspr-1.1.3/pycspr/serialisation/json/entity/encoder.py
--rw-r--r--   0        0        0      176 2023-05-15 10:59:30.293843 pycspr-1.1.3/pycspr/serialisation/utils/__init__.py
--rw-r--r--   0        0        0     2975 2024-02-11 20:50:27.643388 pycspr-1.1.3/pycspr/serialisation/utils/cl_value_to_cl_type.py
--rw-r--r--   0        0        0     2652 2024-03-19 20:26:50.719899 pycspr-1.1.3/pycspr/serialisation/utils/cl_value_to_parsed.py
--rw-r--r--   0        0        0     5965 2024-02-28 10:36:33.388518 pycspr-1.1.3/pycspr/types/__init__.py
--rw-r--r--   0        0        0     7075 2023-05-15 10:59:30.294123 pycspr-1.1.3/pycspr/types/cl_types.py
--rw-r--r--   0        0        0     7404 2024-03-05 23:01:01.006318 pycspr-1.1.3/pycspr/types/cl_values.py
--rw-r--r--   0        0        0     1549 2024-03-19 20:26:50.720158 pycspr-1.1.3/pycspr/types/deploy_execution.py
--rw-r--r--   0        0        0     1352 2024-03-05 10:29:32.583802 pycspr-1.1.3/pycspr/types/deploy_transform.py
--rw-r--r--   0        0        0    10750 2024-03-13 20:07:26.473948 pycspr-1.1.3/pycspr/types/deploys.py
--rw-r--r--   0        0        0     4142 2024-03-15 20:18:03.366634 pycspr-1.1.3/pycspr/types/identifiers.py
--rw-r--r--   0        0        0     2480 2024-03-15 20:44:23.925060 pycspr-1.1.3/pycspr/types/keys.py
--rw-r--r--   0        0        0      850 2024-03-16 22:30:05.847176 pycspr-1.1.3/pycspr/types/timestamp.py
--rw-r--r--   0        0        0        0 2023-05-15 10:59:30.294503 pycspr-1.1.3/pycspr/utils/__init__.py
--rw-r--r--   0        0        0      911 2024-02-15 10:23:41.848783 pycspr-1.1.3/pycspr/utils/constants.py
--rw-r--r--   0        0        0     2978 2024-03-19 20:26:50.720374 pycspr-1.1.3/pycspr/utils/conversion.py
--rw-r--r--   0        0        0     2113 2023-05-15 10:59:30.294683 pycspr-1.1.3/pycspr/utils/io.py
--rw-r--r--   0        0        0     1241 2024-03-03 22:04:34.295970 pycspr-1.1.3/pycspr/utils/validation.py
--rw-r--r--   0        0        0     1396 2024-03-19 20:37:53.769021 pycspr-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 pycspr-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 10:59:30.289726 pycspr-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2560 2024-04-04 10:16:08.307672 pycspr-1.2.0/README.md
+-rw-r--r--   0        0        0     3461 2024-04-04 10:16:08.312140 pycspr-1.2.0/pycspr/__init__.py
+-rw-r--r--   0        0        0      728 2024-04-04 10:16:08.312464 pycspr-1.2.0/pycspr/api/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-04 10:16:08.312607 pycspr-1.2.0/pycspr/api/constants.py
+-rw-r--r--   0        0        0       96 2024-04-04 10:16:08.312913 pycspr-1.2.0/pycspr/api/rest/__init__.py
+-rw-r--r--   0        0        0     2746 2024-04-04 10:16:08.313051 pycspr-1.2.0/pycspr/api/rest/client.py
+-rw-r--r--   0        0        0      322 2024-04-04 10:16:08.313303 pycspr-1.2.0/pycspr/api/rest/connection.py
+-rw-r--r--   0        0        0     2330 2024-04-04 10:16:08.313429 pycspr-1.2.0/pycspr/api/rest/proxy.py
+-rw-r--r--   0        0        0       94 2024-04-04 10:16:08.313691 pycspr-1.2.0/pycspr/api/rpc/__init__.py
+-rw-r--r--   0        0        0    15022 2024-04-04 10:16:08.313870 pycspr-1.2.0/pycspr/api/rpc/client.py
+-rw-r--r--   0        0        0      324 2024-04-04 10:16:08.314062 pycspr-1.2.0/pycspr/api/rpc/connection.py
+-rw-r--r--   0        0        0     5353 2024-04-04 10:16:08.314285 pycspr-1.2.0/pycspr/api/rpc/params.py
+-rw-r--r--   0        0        0    12374 2024-04-04 10:16:08.314492 pycspr-1.2.0/pycspr/api/rpc/proxy.py
+-rw-r--r--   0        0        0      118 2024-04-04 10:16:08.314678 pycspr-1.2.0/pycspr/api/rpc_speculative/__init__.py
+-rw-r--r--   0        0        0      952 2024-04-04 10:16:08.315137 pycspr-1.2.0/pycspr/api/rpc_speculative/client.py
+-rw-r--r--   0        0        0      360 2024-04-04 10:16:08.315257 pycspr-1.2.0/pycspr/api/rpc_speculative/connection.py
+-rw-r--r--   0        0        0     1540 2024-04-04 10:16:08.315421 pycspr-1.2.0/pycspr/api/rpc_speculative/proxy.py
+-rw-r--r--   0        0        0       94 2024-04-04 10:16:08.315757 pycspr-1.2.0/pycspr/api/sse/__init__.py
+-rw-r--r--   0        0        0     5318 2024-04-04 10:16:08.316419 pycspr-1.2.0/pycspr/api/sse/client.py
+-rw-r--r--   0        0        0      418 2024-04-04 10:16:08.316622 pycspr-1.2.0/pycspr/api/sse/connection.py
+-rw-r--r--   0        0        0     2756 2024-04-04 10:16:08.316995 pycspr-1.2.0/pycspr/api/sse/proxy.py
+-rw-r--r--   0        0        0     1027 2024-04-04 10:16:08.317154 pycspr-1.2.0/pycspr/crypto/__init__.py
+-rw-r--r--   0        0        0     4858 2024-04-04 10:16:08.317523 pycspr-1.2.0/pycspr/crypto/checksummer.py
+-rw-r--r--   0        0        0     2963 2024-04-04 10:16:08.317768 pycspr-1.2.0/pycspr/crypto/cl_operations.py
+-rw-r--r--   0        0        0     5448 2024-04-04 10:16:08.318163 pycspr-1.2.0/pycspr/crypto/ecc.py
+-rw-r--r--   0        0        0     3840 2024-03-24 21:01:15.015766 pycspr-1.2.0/pycspr/crypto/ecc_ed25519.py
+-rw-r--r--   0        0        0     3090 2023-05-15 10:59:30.292031 pycspr-1.2.0/pycspr/crypto/ecc_secp256k1.py
+-rw-r--r--   0        0        0      874 2024-04-04 10:16:08.318398 pycspr-1.2.0/pycspr/crypto/hashifier.py
+-rw-r--r--   0        0        0      322 2024-02-11 20:37:22.630050 pycspr-1.2.0/pycspr/crypto/hashifier_blake2b.py
+-rw-r--r--   0        0        0      302 2024-03-21 17:38:07.874734 pycspr-1.2.0/pycspr/crypto/hashifier_blake3.py
+-rw-r--r--   0        0        0     1363 2023-05-15 10:59:30.292257 pycspr-1.2.0/pycspr/factory/__init__.py
+-rw-r--r--   0        0        0     2995 2024-04-04 10:16:08.318733 pycspr-1.2.0/pycspr/factory/accounts.py
+-rw-r--r--   0        0        0    12413 2024-04-04 10:16:08.318997 pycspr-1.2.0/pycspr/factory/deploys.py
+-rw-r--r--   0        0        0     1634 2024-04-04 10:16:08.319238 pycspr-1.2.0/pycspr/factory/digests.py
+-rw-r--r--   0        0        0      487 2024-04-04 10:16:08.319420 pycspr-1.2.0/pycspr/serializer/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-04 10:16:08.319630 pycspr-1.2.0/pycspr/serializer/binary/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-04 10:16:08.320218 pycspr-1.2.0/pycspr/serializer/binary/cl_type/__init__.py
+-rw-r--r--   0        0        0     3770 2024-04-04 10:16:08.320336 pycspr-1.2.0/pycspr/serializer/binary/cl_type/decoder.py
+-rw-r--r--   0        0        0     1661 2024-04-04 10:16:08.320447 pycspr-1.2.0/pycspr/serializer/binary/cl_type/encoder.py
+-rw-r--r--   0        0        0      122 2024-04-04 10:16:08.320566 pycspr-1.2.0/pycspr/serializer/binary/cl_value/__init__.py
+-rw-r--r--   0        0        0     9196 2024-04-04 10:16:08.320801 pycspr-1.2.0/pycspr/serializer/binary/cl_value/decoder.py
+-rw-r--r--   0        0        0     3816 2024-04-04 10:16:08.321005 pycspr-1.2.0/pycspr/serializer/binary/cl_value/encoder.py
+-rw-r--r--   0        0        0      122 2024-04-04 10:16:08.321128 pycspr-1.2.0/pycspr/serializer/binary/node_rpc/__init__.py
+-rw-r--r--   0        0        0    10091 2024-04-04 10:16:08.321299 pycspr-1.2.0/pycspr/serializer/binary/node_rpc/decoder.py
+-rw-r--r--   0        0        0     5804 2024-04-04 10:16:08.321441 pycspr-1.2.0/pycspr/serializer/binary/node_rpc/encoder.py
+-rw-r--r--   0        0        0      918 2024-04-04 10:16:08.321555 pycspr-1.2.0/pycspr/serializer/json/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-04 10:16:08.321668 pycspr-1.2.0/pycspr/serializer/json/cl_type/__init__.py
+-rw-r--r--   0        0        0     3274 2024-04-04 10:16:08.322076 pycspr-1.2.0/pycspr/serializer/json/cl_type/decoder.py
+-rw-r--r--   0        0        0     2729 2024-04-04 10:16:08.322441 pycspr-1.2.0/pycspr/serializer/json/cl_type/encoder.py
+-rw-r--r--   0        0        0      118 2024-04-04 10:16:08.322556 pycspr-1.2.0/pycspr/serializer/json/cl_value/__init__.py
+-rw-r--r--   0        0        0      783 2024-04-04 10:16:08.322836 pycspr-1.2.0/pycspr/serializer/json/cl_value/decoder.py
+-rw-r--r--   0        0        0      702 2024-04-04 10:16:08.322929 pycspr-1.2.0/pycspr/serializer/json/cl_value/encoder.py
+-rw-r--r--   0        0        0      118 2024-04-04 10:16:08.323138 pycspr-1.2.0/pycspr/serializer/json/node_rpc/__init__.py
+-rw-r--r--   0        0        0    23483 2024-04-04 10:16:08.323264 pycspr-1.2.0/pycspr/serializer/json/node_rpc/decoder.py
+-rw-r--r--   0        0        0     4616 2024-04-04 10:16:08.323588 pycspr-1.2.0/pycspr/serializer/json/node_rpc/encoder.py
+-rw-r--r--   0        0        0      170 2024-04-04 10:16:08.323695 pycspr-1.2.0/pycspr/serializer/utils/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-04 10:16:08.323861 pycspr-1.2.0/pycspr/serializer/utils/cl_value_to_cl_type.py
+-rw-r--r--   0        0        0     3326 2024-04-04 10:16:08.323946 pycspr-1.2.0/pycspr/serializer/utils/cl_value_to_parsed.py
+-rw-r--r--   0        0        0       90 2024-04-04 10:16:08.324204 pycspr-1.2.0/pycspr/types/__init__.py
+-rw-r--r--   0        0        0     2380 2024-04-04 10:16:08.324406 pycspr-1.2.0/pycspr/types/cl/__init__.py
+-rw-r--r--   0        0        0     7179 2024-04-04 10:16:08.324643 pycspr-1.2.0/pycspr/types/cl/types.py
+-rw-r--r--   0        0        0     6427 2024-04-04 10:16:08.324756 pycspr-1.2.0/pycspr/types/cl/values.py
+-rw-r--r--   0        0        0      471 2024-04-04 10:16:08.325093 pycspr-1.2.0/pycspr/types/crypto/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-04 10:16:08.325425 pycspr-1.2.0/pycspr/types/crypto/complex.py
+-rw-r--r--   0        0        0      989 2024-04-04 10:16:08.325610 pycspr-1.2.0/pycspr/types/crypto/simple.py
+-rw-r--r--   0        0        0       68 2024-04-04 10:16:08.325859 pycspr-1.2.0/pycspr/types/node/__init__.py
+-rw-r--r--   0        0        0     4446 2024-04-04 10:16:08.325967 pycspr-1.2.0/pycspr/types/node/rpc/__init__.py
+-rw-r--r--   0        0        0    13097 2024-04-04 10:16:08.326084 pycspr-1.2.0/pycspr/types/node/rpc/complex.py
+-rw-r--r--   0        0        0     2384 2024-04-04 10:16:08.326261 pycspr-1.2.0/pycspr/types/node/rpc/simple.py
+-rw-r--r--   0        0        0      235 2024-04-04 10:16:08.326445 pycspr-1.2.0/pycspr/types/node/sse/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-04 10:16:08.326717 pycspr-1.2.0/pycspr/types/node/sse/complex.py
+-rw-r--r--   0        0        0     1156 2024-04-04 10:16:08.326973 pycspr-1.2.0/pycspr/types/node/sse/simple.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:59:30.294503 pycspr-1.2.0/pycspr/utils/__init__.py
+-rw-r--r--   0        0        0     1044 2024-04-04 10:16:08.327211 pycspr-1.2.0/pycspr/utils/constants.py
+-rw-r--r--   0        0        0     3960 2024-04-04 10:16:08.327296 pycspr-1.2.0/pycspr/utils/convertor.py
+-rw-r--r--   0        0        0     2107 2024-04-04 10:16:08.327504 pycspr-1.2.0/pycspr/utils/io.py
+-rw-r--r--   0        0        0     1260 2024-04-04 10:16:08.327754 pycspr-1.2.0/pycspr/utils/validation.py
+-rw-r--r--   0        0        0     1396 2024-04-04 10:16:08.327895 pycspr-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 pycspr-1.2.0/PKG-INFO
```

### Comparing `pycspr-1.1.3/LICENSE` & `pycspr-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycspr-1.1.3/README.md` & `pycspr-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 pip3 install pycspr
 ```
 
 ##  Usage
 
 ### Cryptography
 
-* [How To: Hash data ?](how_tos/cryptography/how_to_hash_data.py)
+* [How To: Apply a checksum ?](how_tos/crypto/how_to_apply_a_checksum.py)
 
-* [How To: Create Key Pairs ?](how_tos/cryptography/how_to_create_key_pairs.py)
+* [How To: Create Key Pairs ?](how_tos/crypto/how_to_create_key_pairs.py)
 
-* [How To: Apply a checksum ?](how_tos/cryptography/how_to_apply_a_checksum.py)
+* [How To: Hash data ?](how_tos/crypto/how_to_hash_data.py)
+
+* [How To: Sign data ?](how_tos/crypto/how_to_sign_data.py)
 
 ### Deploys
 
 * [How To: Transfer funds between 2 accounts ?](how_tos/deploys/how_to_transfer.py)
 
 * [How To: Delegate funds to a validator ?](how_tos/deploys/how_to_delegate.py)
```

### Comparing `pycspr-1.1.3/pycspr/__init__.py` & `pycspr-1.2.0/pycspr/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,42 +3,54 @@
 #  88       d8   `8b   d8'   8b           `"Y8ba,   88       d8  88
 #  88b,   ,a8"    `8b,d8'    "8a,   ,aa  aa    ]8I  88b,   ,a8"  88
 #  88`YbbdP"'       Y88'      `"Ybbd8"'  `"YbbdP"'  88`YbbdP"'   88
 #  88               d8'                             88
 #  88              d8'                              88
 
 __title__ = "pycspr"
-__version__ = "1.1.3"
+__version__ = "1.2.0"
 __author__ = "Mark A. Greenslade et al"
 __license__ = "Apache 2.0"
 
+from pycspr import types
 from pycspr import crypto
 from pycspr import factory
-from pycspr import serialisation
-from pycspr import types
 
-from pycspr.api import NodeConnectionInfo
 from pycspr.api import NodeRestClient
+from pycspr.api import NodeRestConnectionInfo
 from pycspr.api import NodeRpcClient
+from pycspr.api import NodeRpcConnectionInfo
 from pycspr.api import NodeSpeculativeRpcClient
+from pycspr.api import NodeSpeculativeRpcConnectionInfo
 from pycspr.api import NodeSseClient
+from pycspr.api import NodeSseConnectionInfo
 from pycspr.api import NodeEventChannel
 from pycspr.api import NodeEventInfo
 from pycspr.api import NodeEventType
 from pycspr.api import SSE_CHANNEL_TO_SSE_EVENT
 
 from pycspr.crypto import DEFAULT_HASH_ALGO
 from pycspr.crypto import DEFAULT_KEY_ALGO
+from pycspr.crypto import checksummer
 from pycspr.crypto import get_account_hash
-from pycspr.crypto import get_account_hash as get_account_address
 from pycspr.crypto import get_account_key
-from pycspr.crypto import get_account_key_algo
 from pycspr.crypto import get_hash
-from pycspr.crypto import HashAlgorithm
-from pycspr.crypto import KeyAlgorithm
+from pycspr.crypto import get_key_pair
+from pycspr.crypto import get_key_pair_from_base64
+from pycspr.crypto import get_key_pair_from_bytes
+from pycspr.crypto import get_key_pair_from_hex_string
+from pycspr.crypto import get_key_pair_from_pem_file
+from pycspr.crypto import get_key_pair_from_seed
+from pycspr.crypto import get_pvk_pem_file_from_bytes
+from pycspr.crypto import get_pvk_pem_from_bytes
+from pycspr.crypto import get_signature
+from pycspr.crypto import get_signature_for_deploy_approval
+from pycspr.crypto import get_signature_from_pem_file
+from pycspr.crypto import is_signature_valid
+from pycspr.crypto import verify_deploy_approval_signature
 
 from pycspr.factory import create_deploy
 from pycspr.factory import create_deploy_approval
 from pycspr.factory import create_deploy_arguments
 from pycspr.factory import create_deploy_parameters
 from pycspr.factory import create_deploy_ttl
 from pycspr.factory import create_transfer
@@ -48,21 +60,23 @@
 from pycspr.factory import create_validator_delegation
 from pycspr.factory import create_validator_delegation_withdrawal
 from pycspr.factory import parse_private_key
 from pycspr.factory import parse_private_key_bytes
 from pycspr.factory import parse_public_key
 from pycspr.factory import parse_public_key_bytes
 
-from pycspr.serialisation import to_bytes
-from pycspr.serialisation import to_json
-from pycspr.serialisation import from_bytes
-from pycspr.serialisation import from_json
-
-from pycspr.types import PublicKey
-from pycspr.types import PrivateKey
+from pycspr.serializer import to_bytes
+from pycspr.serializer import to_json
+from pycspr.serializer import from_bytes
+from pycspr.serializer import from_json
+
+from pycspr.types.crypto import HashAlgorithm
+from pycspr.types.crypto import KeyAlgorithm
+from pycspr.types.crypto import PublicKey
+from pycspr.types.crypto import PrivateKey
 
 from pycspr.utils.io import get_deploy_size_bytes
 from pycspr.utils.io import read_deploy
 from pycspr.utils.io import read_wasm
 from pycspr.utils.io import write_deploy
 
 from pycspr.utils.validation import validate_deploy
```

### Comparing `pycspr-1.1.3/pycspr/api/constants.py` & `pycspr-1.2.0/pycspr/api/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 RPC_QUERY_BALANCE = "query_balance"
 RPC_QUERY_GLOBAL_STATE = "query_global_state"
 RPC_STATE_GET_ACCOUNT_INFO = "state_get_account_info"
 RPC_STATE_GET_AUCTION_INFO = "state_get_auction_info"
 RPC_STATE_GET_BALANCE = "state_get_balance"
 RPC_STATE_GET_DICTIONARY_ITEM = "state_get_dictionary_item"
 RPC_STATE_GET_ITEM = "state_get_item"
+RPC_STATE_GET_TRIE = "state_get_trie"
 
 RPC_ENDPOINTS: set = {
     RPC_ACCOUNT_PUT_DEPLOY,
     RPC_CHAIN_GET_BLOCK,
     RPC_CHAIN_GET_BLOCK_TRANSFERS,
     RPC_CHAIN_GET_ERA_INFO_BY_SWITCH_BLOCK,
     RPC_CHAIN_GET_ERA_SUMMARY,
```

### Comparing `pycspr-1.1.3/pycspr/api/rest/client.py` & `pycspr-1.2.0/pycspr/api/rest/proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,85 @@
-from pycspr.api.connection import NodeConnectionInfo
-from pycspr.api.rest.proxy import Proxy
+import json
 
+import requests
 
-class Client():
-    """Node REST server client.
+from pycspr.api import constants
+from pycspr.api.rest.connection import ConnectionInfo
+
+
+class Proxy:
+    """Node REST server proxy.
 
     """
-    def __init__(self, connection_info: NodeConnectionInfo):
+    def __init__(self, connection_info: ConnectionInfo):
         """Instance constructor.
 
-        :param connection: Information required to connect to a node.
+        :param connection_info: Information required to connect to a node.
 
         """
-        self.proxy = Proxy(connection_info.host, connection_info.port_rest)
+        self.connection_info = connection_info
+
+    @property
+    def address(self) -> str:
+        """A node's REST server base address."""
+        return f"http://{self.connection_info.host}:{self.connection_info.port}"
 
-        # Extension methods -> 2nd order functions.
-        ext = ClientExtensions(self)
-        self.get_node_metric = ext.get_node_metric
+    def __str__(self):
+        """Instance string representation."""
+        return self.address
 
-    def get_chainspec(self) -> dict:
+    async def get_chainspec(self) -> dict:
         """Returns network chainspec.
 
         :returns: Network chainspec.
 
         """
-        return self.proxy.get_chainspec()
+        response: str = await self._get_response(constants.REST_GET_CHAINSPEC)
 
-    def get_node_metrics(self) -> list:
+        return json.loads(response)["chainspec_bytes"]
+
+    async def get_node_metrics(self) -> list:
         """Returns set of node metrics.
 
         :returns: Node metrics information.
 
         """
-        return self.proxy.get_node_metrics()
+        response = await self._get_response(constants.REST_GET_METRICS)
 
-    def get_node_status(self) -> dict:
-        """Returns node status information.
+        return sorted([i.strip() for i in response.split("\n") if not i.startswith("#")])
 
-        :returns: Node status information.
-
-        """
-        return self.proxy.get_node_status()
-
-    def get_node_rpc_schema(self) -> dict:
+    async def get_rpc_schema(self) -> dict:
         """Returns node RPC API schema.
 
         :returns: Node RPC API schema.
 
         """
-        return self.proxy.get_rpc_schema()
-
-    def get_validator_changes(self) -> list:
-        """Returns validator change information.
+        response: str = await self._get_response(constants.REST_GET_RPC_SCHEMA)
 
-        :returns: Validator change information.
+        return json.loads(response)
 
-        """
-        return self.proxy.get_validator_changes()
+    async def get_node_status(self) -> dict:
+        """Returns node status information.
 
+        :returns: Node status information.
 
-class ClientExtensions():
-    """Node REST server client extensions, i.e. 2nd order functions.
+        """
+        return json.loads(await self._get_response(constants.REST_GET_STATUS))
 
-    """
-    def __init__(self, client: Client):
-        """Instance constructor.
+    async def get_validator_changes(self) -> list:
+        """Returns validator change information.
 
-        :param client: Node REST client.
+        :returns: Validator change information.
 
         """
-        self.client = client
+        response = await self._get_response(constants.REST_GET_VALIDATOR_CHANGES)
 
-    def get_node_metric(self, metric_id: str) -> list:
-        """Returns node metrics information filtered by a particular metric.
+        return json.loads(response)["changes"]
 
-        :param metric_id: Identifier of node metric.
-        :returns: Node metrics information filtered by a particular metric.
+    async def _get_response(self, endpoint: str) -> dict:
+        """Invokes remote REST API and returns parsed response.
 
-        """
-        metrics: list = self.client.get_node_metrics()
+        :endpoint: Target endpoint to invoke.
+        :returns: Parsed REST API response.
 
-        return [i for i in metrics if i.lower().startswith(metric_id.lower())]
+        """
+        return requests.get(f"{self.address}/{endpoint}").content.decode("utf-8")
```

### Comparing `pycspr-1.1.3/pycspr/api/rpc/client.py` & `pycspr-1.2.0/pycspr/api/rpc/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,410 +1,439 @@
 import time
 import typing
 
-from pycspr.api.connection import NodeConnectionInfo
-from pycspr.api.rpc import decoder
+from pycspr.api.rpc.connection import ConnectionInfo
 from pycspr.api.rpc.proxy import Proxy
-from pycspr.api.rpc import types as rpc_types
-from pycspr.types import AccountID
-from pycspr.types import BlockID
-from pycspr.types import CL_Key
-from pycspr.types import CL_URef
-from pycspr.types import DeployID
-from pycspr.types import Deploy
-from pycspr.types import DictionaryID
-from pycspr.types import GlobalStateID
-from pycspr.types import PurseID
-from pycspr.types import StateRootID
+from pycspr.serializer.json.node_rpc import decoder
+from pycspr.types.cl import CLV_Key
+from pycspr.types.crypto import Digest
+from pycspr.types.node.rpc import Address
+from pycspr.types.node.rpc import AccountInfo
+from pycspr.types.node.rpc import AuctionState
+from pycspr.types.node.rpc import Block
+from pycspr.types.node.rpc import BlockID
+from pycspr.types.node.rpc import BlockTransfers
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import DeployHash
+from pycspr.types.node.rpc import DictionaryID
+from pycspr.types.node.rpc import EraSummary
+from pycspr.types.node.rpc import GlobalStateID
+from pycspr.types.node.rpc import NodePeer
+from pycspr.types.node.rpc import NodeStatus
+from pycspr.types.node.rpc import PurseID
+from pycspr.types.node.rpc import StateRootHash
+from pycspr.types.node.rpc import ValidatorChanges
+from pycspr.types.node.rpc import URef
+from pycspr.utils import convertor
 
 
 class Client():
     """Node RPC server client.
 
     """
-    def __init__(self, connection_info: NodeConnectionInfo):
+    def __init__(self, connection_info: ConnectionInfo):
         """Instance constructor.
 
-        :param connection: Information required to connect to a node.
+        :param connection_info: Information required to connect to a node.
 
         """
-        self.proxy = Proxy(
-            host=connection_info.host,
-            port=connection_info.port_rpc,
-        )
+        self.proxy = Proxy(connection_info)
 
         # Alias methods.
         self.get_auction_state = self.get_auction_info
         self.get_era_info = self.get_era_info_by_switch_block
-        self.get_state_root_hash = self.get_state_root
+        self.get_state_root_hash = self.get_state_root_hash
         self.send_deploy = self.account_put_deploy
 
         # Extension methods -> 2nd order functions.
         ext = ClientExtensions(self)
         self.get_account_main_purse_uref = ext.get_account_main_purse_uref
         self.get_account_named_key = ext.get_account_named_key
         self.get_block_at_era_switch = ext.get_block_at_era_switch
         self.get_block_height = ext.get_block_height
         self.get_chain_heights = ext.get_chain_heights
         self.get_era_height = ext.get_era_height
         self.get_rpc_endpoint = ext.get_rpc_endpoint
         self.get_rpc_endpoints = ext.get_rpc_endpoints
 
-    def account_put_deploy(self, deploy: Deploy) -> DeployID:
+    async def account_put_deploy(self, deploy: Deploy) -> DeployHash:
         """Dispatches a deploy to a node for processing.
 
         :param deploy: A deploy to be processed at a node.
-        :returns: Deploy identifier.
+        :returns: Deploy hash.
 
         """
-        return self.proxy.account_put_deploy(deploy)
+        return await self.proxy.account_put_deploy(deploy)
 
-    def get_account_balance(
+    async def get_account_balance(
         self,
         purse_id: PurseID,
         global_state_id: GlobalStateID = None
     ) -> int:
         """Returns account balance at a certain point in global state history.
 
         :param purse_id: Identifier of purse being queried.
         :param global_state_id: Identifier of global state root at some point in time.
         :returns: Account balance in motes (if purse exists).
 
         """
-        return self.proxy.query_balance(purse_id, global_state_id)
+        return await self.proxy.query_balance(purse_id, global_state_id)
 
-    def get_account_info(
+    async def get_account_info(
         self,
-        account_id: AccountID,
+        account_id: Address,
         block_id: BlockID = None,
-        decode=False
-    ) -> typing.Union[dict, rpc_types.AccountInfo]:
+        decode: bool = True
+    ) -> typing.Union[dict, AccountInfo]:
         """Returns account information at a certain global state root hash.
 
         :param account_id: An account holder's public key prefixed with a key type identifier.
         :param block_id: Identifier of a finalised block.
         :returns: Account information in JSON format.
 
         """
-        obj: dict = self.proxy.state_get_account_info(account_id, block_id)
+        encoded: dict = await self.proxy.state_get_account_info(account_id, block_id)
 
-        return obj if decode is False else decoder.decode(obj, rpc_types.AccountInfo)
+        return encoded if decode is False else decoder.decode(encoded, AccountInfo)
 
-    def get_auction_info(
+    async def get_auction_info(
         self,
         block_id: BlockID = None,
         decode: bool = True
-    ) -> typing.Union[dict, rpc_types.AuctionState]:
+    ) -> typing.Union[dict, AuctionState]:
         """Returns current auction system contract information.
 
         :param block_id: Identifier of a finalised block.
         :returns: Current auction system contract information.
 
         """
-        obj: dict = self.proxy.state_get_auction_info(block_id)
+        encoded: dict = await self.proxy.state_get_auction_info(block_id)
 
-        return obj if decode is False else decoder.decode(obj, rpc_types.AuctionState)
+        return encoded if decode is False else decoder.decode(encoded, AuctionState)
 
-    def get_block(
+    async def get_block(
         self,
         block_id: BlockID = None,
-        decode=False
-    ) -> typing.Union[dict, rpc_types.Block]:
+        decode: bool = True
+    ) -> typing.Union[dict, Block]:
         """Returns on-chain block information.
 
         :param block_id: Identifier of a finalised block.
         :param decode: Flag indicating whether to decode API response.
         :returns: On-chain block information.
 
         """
-        obj: dict = self.proxy.chain_get_block(block_id)
+        encoded: dict = await self.proxy.chain_get_block(block_id)
 
-        return obj if decode is False else decoder.decode(obj, rpc_types.Block)
+        return encoded if decode is False else decoder.decode(encoded, Block)
 
-    def get_block_transfers(
+    async def get_block_transfers(
         self,
         block_id: BlockID = None,
         decode: bool = True
-    ) -> typing.Union[dict, rpc_types.BlockTransfers]:
+    ) -> typing.Union[dict, BlockTransfers]:
         """Returns on-chain block transfers information.
 
         :param block_id: Identifier of a finalised block.
         :param decode: Flag indicating whether to decode API response.
         :returns: On-chain block transfers information.
 
         """
-        obj: dict = self.proxy.chain_get_block_transfers(block_id)
+        encoded: dict = await self.proxy.chain_get_block_transfers(block_id)
 
-        return obj if decode is False else decoder.decode(obj, rpc_types.BlockTransfers)
+        return encoded if decode is False else decoder.decode(encoded, BlockTransfers)
 
-    def get_chainspec(self) -> dict:
+    async def get_chainspec(self) -> dict:
         """Returns canonical network state information.
 
         :returns: Chain spec, genesis accounts and global state information.
 
         """
-        # TODO: decode
-        return self.proxy.info_get_chainspec()
+        return await self.proxy.info_get_chainspec()
 
-    def get_deploy(
+    async def get_deploy(
         self,
-        deploy_id: DeployID,
+        deploy_hash: DeployHash,
         decode: bool = True
-    ) -> typing.Union[dict, rpc_types.Deploy]:
+    ) -> typing.Union[dict, Deploy]:
         """Returns on-chain deploy information.
 
-        :param deploy_id: Identifier of a deploy processed by network.
+        :param deploy_id: Hash of a deploy processed by network.
         :param decode: Flag indicating whether to decode API response.
         :returns: On-chain deploy information.
 
         """
-        obj: dict = self.proxy.info_get_deploy(deploy_id)
-        obj["deploy"]["execution_info"] = obj.get("execution_results", None)
+        encoded: dict = await self.proxy.info_get_deploy(deploy_hash)
+        encoded["deploy"]["execution_info"] = encoded.get("execution_results", None)
 
-        return obj["deploy"] if decode is False else decoder.decode(obj["deploy"], rpc_types.Deploy)
+        return \
+            encoded["deploy"] if decode is False else \
+            decoder.decode(encoded["deploy"], Deploy)
 
-    def get_dictionary_item(
+    async def get_dictionary_item(
         self,
         identifier: DictionaryID,
-        state_root_hash: StateRootID = None
+        state_root_hash: StateRootHash = None
     ) -> dict:
         """Returns current auction system contract information.
 
         :param identifier: Identifier required to query a dictionary item.
         :param state_root_hash: A node's root state hash at some point in chain time.
         :returns: On-chain data stored under a dictionary item.
 
         """
         # TODO: decode
-        return self.proxy.state_get_dictionary_item(identifier, state_root_hash)
+        return await self.proxy.state_get_dictionary_item(identifier, state_root_hash)
 
-    def get_era_summary(
+    async def get_era_summary(
         self,
         block_id: BlockID = None,
         decode: bool = True
-    ) -> typing.Union[dict, rpc_types.EraSummary]:
+    ) -> typing.Union[dict, EraSummary]:
         """Returns consensus era summary information.
 
         :param block_id: Identifier of a block.
+        :param decode: Flag indicating whether to decode API response.
         :returns: Era summary information.
 
         """
-        obj: dict = self.proxy.chain_get_era_summary(block_id)
+        encoded: dict = await self.proxy.chain_get_era_summary(block_id)
 
-        return obj if decode is False else decoder.decode(obj, rpc_types.EraSummary)
+        return encoded if decode is False else decoder.decode(encoded, EraSummary)
 
-    def get_era_info_by_switch_block(self, block_id: BlockID = None) -> dict:
+    async def get_era_info_by_switch_block(
+        self,
+        block_id: BlockID = None,
+        decode: bool = True
+    ) -> typing.Union[dict, EraSummary]:
         """Returns consensus era information scoped by block id.
 
         :param block_id: Identifier of a block.
+        :param decode: Flag indicating whether to decode API response.
         :returns: Era information.
 
         """
-        # TODO: decode
-        return self.proxy.chain_get_era_info_by_switch_block(block_id)
+        encoded: dict = await self.proxy.chain_get_era_info_by_switch_block(block_id)
 
-    def get_node_peers(self) -> dict:
+        return encoded if decode is False else decoder.decode(encoded, EraSummary)
+
+    async def get_node_peers(
+        self,
+        decode: bool = True
+    ) -> typing.Union[typing.List[dict], typing.List[NodePeer]]:
         """Returns node peer information.
 
+        :param decode: Flag indicating whether to decode API response.
         :returns: Node peer information.
 
         """
-        # TODO: decode
-        return self.proxy.info_get_peers()
+        encoded: list = await self.proxy.info_get_peers()
+
+        return encoded if decode is False else [decoder.decode(i, NodePeer) for i in encoded]
 
-    def get_node_status(self) -> dict:
+    async def get_node_status(self, decode: bool = True) -> typing.Union[dict, NodeStatus]:
         """Returns node status information.
 
+        :param decode: Flag indicating whether to decode API response.
         :returns: Node status information.
 
         """
-        # TODO: decode
-        return self.proxy.info_get_status()
+        encoded: dict = await self.proxy.info_get_status()
+
+        return encoded if decode is False else decoder.decode(encoded, NodeStatus)
 
-    def get_rpc_schema(self) -> dict:
+    async def get_rpc_schema(self) -> dict:
         """Returns RPC schema.
 
         :returns: Node JSON-RPC API schema.
 
         """
-        # TODO: decode
-        return self.proxy.discover()
+        return await self.proxy.discover()
 
-    def get_state_item(
+    async def get_state_item(
         self,
         key: str,
         path: typing.Union[str, typing.List[str]] = [],
-        state_root_hash: StateRootID = None
+        state_root_hash: StateRootHash = None
     ) -> bytes:
         """Returns a representation of an item stored under a key in global state.
 
         :param key: Storage item key.
         :param path: Storage item path.
         :param state_root_hash: A node's root state hash at some point in chain time.
         :returns: Item stored under passed key/path.
 
         """
         # TODO: decode
-        return self.proxy.state_get_item(key, path, state_root_hash)
+        return await self.proxy.state_get_item(key, path, state_root_hash)
 
-    def get_state_key_value(
+    async def get_state_key_value(
         self,
         key: str,
         path: typing.List[str],
         state_id: GlobalStateID = None
     ) -> bytes:
         """Returns results of a query to global state at a specified block or state root hash.
 
         :param key: Key of an item stored within global state.
         :param path: Identifier of a path within item.
         :param state_id: Identifier of global state leaf.
         :returns: Results of a global state query.
 
         """
         # TODO: decode
-        return self.proxy.query_global_state(key, path, state_id)
+        return await self.proxy.query_global_state(key, path, state_id)
 
-    def get_state_root(self, block_id: BlockID = None) -> StateRootID:
+    async def get_state_root_hash(self, block_id: BlockID = None) -> StateRootHash:
         """Returns an root hash of global state at a specified block.
 
         :param block_id: Identifier of a finalised block.
         :returns: State root hash at specified block.
 
         """
-        return self.proxy.chain_get_state_root_hash(block_id)
+        return await self.proxy.chain_get_state_root_hash(block_id)
+
+    async def get_state_trie(self, trie_key: Digest) -> typing.Optional[bytes]:
+        """Returns results of a query to global state trie store at a specified key.
+
+        :param trie_key: Key of an item stored within global state.
+        :returns:  A list of keys read under the specified prefix.
+
+        """
+        return await self.proxy.state_get_trie(trie_key)
 
-    def get_validator_changes(
+    async def get_validator_changes(
         self,
         decode: bool = True
-    ) -> typing.List[typing.Union[dict, rpc_types.ValidatorChanges]]:
+    ) -> typing.List[typing.Union[dict, ValidatorChanges]]:
         """Returns status changes of active validators.
 
         :param node: Information required to connect to a node.
         :returns: Status changes of active validators.
 
         """
-        obj = self.proxy.info_get_validator_changes()
+        obj = await self.proxy.info_get_validator_changes()
 
-        return obj if decode is False else [decoder.decode(i, rpc_types.ValidatorChanges) for i in obj]
+        return obj if decode is False else [decoder.decode(i, ValidatorChanges) for i in obj]
 
 
 class ClientExtensions():
     """Node RPC server client extensions, i.e. 2nd order functions.
 
     """
     def __init__(self, client: Client):
         """Instance constructor.
 
         :param client: Node RPC client.
 
         """
         self.client = client
 
-    def get_account_main_purse_uref(
+    async def get_account_main_purse_uref(
         self,
-        account_id: AccountID,
+        account_id: Address,
         block_id: BlockID = None
-    ) -> CL_URef:
+    ) -> URef:
         """Returns an on-chain account's main purse unforgeable reference.
 
         :param account_id: An account holder's public key prefixed with a key type identifier.
         :param block_id: Identifier of a finalised block.
         :returns: Account main purse unforgeable reference.
 
         """
-        account_info = self.client.get_account_info(account_id, block_id)
+        account_info: AccountInfo = await self.client.get_account_info(account_id, block_id)
 
-        return CL_URef.from_string(account_info["main_purse"])
+        return account_info.main_purse
 
-    def get_account_named_key(
+    async def get_account_named_key(
         self,
-        account_id: AccountID,
+        account_id: Address,
         key_name: str,
         block_id: BlockID = None
-    ) -> CL_Key:
+    ) -> CLV_Key:
         """Returns a key stored under an account's storage under a specific name.
 
         :param account_id: An account holder's public key prefixed with a key type identifier.
         :param key_name: Name of key under which account data is stored.
         :param block_id: Identifier of a finalised block.
         :returns: A CL key if found.
 
         """
-        account_info = self.client.get_account_info(account_id, block_id)
-        for named_key in account_info["named_keys"]:
-            if named_key["name"] == key_name:
-                return CL_Key.from_string(named_key["key"])
+        account_info: AccountInfo = await self.client.get_account_info(account_id, block_id)
+        for named_key in account_info.named_keys:
+            if named_key.name == key_name:
+                return convertor.clv_key_from_str(named_key.key)
 
-    def get_block_at_era_switch(
+    async def get_block_at_era_switch(
         self,
         polling_interval_seconds: float = 1.0,
         max_polling_time_seconds: float = 120.0
-    ) -> dict:
+    ) -> Block:
         """Returns next switch block.
 
         :param polling_interval_seconds: Time interval time before polling for next switch block.
         :param max_polling_time_seconds: Maximum time in seconds to poll.
         :returns: On-chain block information.
 
         """
         elapsed = 0.0
         while True:
-            block = self.client.get_block()
-            if block["header"]["era_end"] is not None:
+            block: Block = await self.client.get_block()
+            if block.header.era_end is not None:
                 return block
 
             elapsed += polling_interval_seconds
             if elapsed > max_polling_time_seconds:
                 break
             time.sleep(polling_interval_seconds)
 
-    def get_block_height(self) -> int:
+    async def get_block_height(self) -> int:
         """Returns height of current block.
 
         :returns: Hieght of current block.
 
         """
-        _, block_height = self.get_chain_heights()
+        _, block_height = await self.get_chain_heights()
 
         return block_height
 
-    def get_chain_heights(self) -> int:
+    async def get_chain_heights(self) -> typing.Tuple[int, int]:
         """Returns height of current era & block.
 
         :returns: 2-ary tuple: (era height, block height).
 
         """
-        block: dict = self.client.get_block()
+        block: Block = await self.client.get_block(decode=True)
 
-        return block["header"]["era_id"], block["header"]["height"]
+        return block.header.era_id, block.header.height
 
-    def get_era_height(self) -> int:
+    async def get_era_height(self) -> int:
         """Returns height of current era.
 
         :returns: Hieght of current era.
 
         """
-        era_height, _ = self.get_chain_heights()
+        era_height, _ = await self.get_chain_heights()
 
         return era_height
 
-    def get_rpc_endpoint(self, endpoint: str) -> dict:
+    async def get_rpc_endpoint(self, endpoint: str) -> dict:
         """Returns RPC schema.
 
         :param endpoint: A specific endpoint of interest.
         :returns: A JSON-RPC schema endpoint fragment.
 
         """
-        schema = self.client.get_rpc_schema()
+        schema = await self.client.get_rpc_schema()
         for obj in schema["methods"]:
             if obj["name"].lower() == endpoint.lower():
                 return obj
 
-    def get_rpc_endpoints(self) -> typing.Union[dict, list]:
+    async def get_rpc_endpoints(self) -> typing.Union[dict, list]:
         """Returns RPC schema.
 
         :returns: A list of all supported JSON-RPC endpoints.
 
         """
-        schema = self.client.get_rpc_schema()
+        schema = await self.client.get_rpc_schema()
 
         return sorted([i["name"] for i in schema["methods"]])
```

### Comparing `pycspr-1.1.3/pycspr/api/rpc/params.py` & `pycspr-1.2.0/pycspr/api/rpc/params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,180 +1,171 @@
 import typing
 
-from pycspr import serialisation
-from pycspr.crypto import cl_checksum
-from pycspr.types import AccountID
-from pycspr.types import BlockID
-from pycspr.types import CL_Key
-from pycspr.types import DeployID
-from pycspr.types import DICTIONARY_ID_VARIANTS
-from pycspr.types import DictionaryID
-from pycspr.types import DictionaryID_AccountNamedKey
-from pycspr.types import DictionaryID_ContractNamedKey
-from pycspr.types import DictionaryID_SeedURef
-from pycspr.types import DictionaryID_UniqueKey
-from pycspr.types import GlobalStateID
-from pycspr.types import GlobalStateIDType
-from pycspr.types import PurseID
-from pycspr.types import PurseIDType
-from pycspr.types import StateRootID
+from pycspr import serializer
+from pycspr.crypto import checksummer
+from pycspr.types.cl import CLV_Key
+from pycspr.types.node.rpc import Address
+from pycspr.types.node.rpc import BlockID
+from pycspr.types.node.rpc import DeployHash
+from pycspr.types.node.rpc import DictionaryID
+from pycspr.types.node.rpc import DictionaryID_AccountNamedKey
+from pycspr.types.node.rpc import DictionaryID_ContractNamedKey
+from pycspr.types.node.rpc import DictionaryID_SeedURef
+from pycspr.types.node.rpc import DictionaryID_UniqueKey
+from pycspr.types.node.rpc import GlobalStateID
+from pycspr.types.node.rpc import GlobalStateIDType
+from pycspr.types.node.rpc import PurseID
+from pycspr.types.node.rpc import PurseIDType
+from pycspr.types.node.rpc import StateRootHash
+from pycspr.utils import convertor
 
 
 # Map: global state identifier type to JSON-RPC paramater name.
 _GLOBAL_STATE_ID_PARAM_NAME: typing.Dict[GlobalStateIDType, str] = {
     GlobalStateIDType.BLOCK_HASH: "BlockHash",
     GlobalStateIDType.BLOCK_HEIGHT: "BlockHeight",
     GlobalStateIDType.STATE_ROOT_HASH: "StateRootHash",
 }
 
 
-def get_block_id(block_id: BlockID, allow_none=True) -> dict:
-    if block_id is not None:
+def account_key(account_id: Address) -> dict:
+    return {
+        "public_key": checksummer.encode_account_key(account_id)
+    }
+
+
+def block_id(block_id: BlockID, allow_none=True) -> dict:
+    if block_id is None:
+        return dict()
+    else:
         if isinstance(block_id, (bytes, str)):
             return {
                 "block_identifier": {
-                    "Hash": cl_checksum.encode_block_id(block_id)
+                    "Hash": checksummer.encode_block_id(block_id)
                 }
             }
         elif isinstance(block_id, int):
             return {
                 "block_identifier": {
                     "Height": block_id
                 }
             }
         elif allow_none is True:
             return {
                 "block_identifier": None
             }
-    else:
-        return dict()
-
-
-def get_account_key(account_id: AccountID) -> dict:
-    return {
-        "public_key": cl_checksum.encode_account_key(account_id)
-    }
 
 
-def get_deploy_id(deploy_id: DeployID) -> dict:
+def deploy_hash(deploy_hash: DeployHash) -> dict:
     return {
-        "deploy_hash": cl_checksum.encode_deploy_id(deploy_id)
+        "deploy_hash": checksummer.encode_deploy_hash(deploy_hash)
     }
 
 
-def get_purse_id(purse_id: PurseID) -> dict:
-    id = \
-        purse_id.identifier.hex() if isinstance(purse_id.identifier, bytes) else \
-        purse_id.identifier
-
-    if purse_id.id_type == PurseIDType.ACCOUNT_HASH:
-        id = f"account-hash-{id}"
-        id_type = "main_purse_under_account_hash"
-    elif purse_id.id_type == PurseIDType.PUBLIC_KEY:
-        id_type = "main_purse_under_public_key"
-    elif purse_id.id_type == PurseIDType.UREF:
-        id = serialisation.cl_value_to_parsed(purse_id.identifier)
-        id_type = "purse_uref"
-    else:
-        raise ValueError(f"Invalid purse identifier type: {purse_id.id_type}")
-
-    return {
-        "purse_identifier": {
-            id_type: id
-        }
-    }
-
-
-def get_global_state_id(global_state_id: GlobalStateID) -> dict:
+def global_state_id(global_state_id: GlobalStateID) -> dict:
     id = \
         global_state_id.identifier.hex() if isinstance(global_state_id.identifier, bytes) else \
         global_state_id.identifier
 
-    if global_state_id.id_type == GlobalStateIDType.BLOCK_HASH:
-        id_type = "BlockHash"
-    elif global_state_id.id_type == GlobalStateIDType.BLOCK_HEIGHT:
-        id_type = "BlockHash"
-    elif global_state_id.id_type == GlobalStateIDType.STATE_ROOT_HASH:
-        id_type = "StateRootHash"
-    else:
-        raise ValueError(f"Invalid global state identifier type: {global_state_id.id_type}")
-
     return {
-        id_type: id
+        global_state_id.id_type.value: id
     }
 
 
-def get_params_for_query_global_state(
-    key: CL_Key,
+def for_query_global_state(
+    key: CLV_Key,
     path: typing.List[str],
     state_id: GlobalStateID
 ) -> dict:
-    try:
-        state_id_type = _GLOBAL_STATE_ID_PARAM_NAME[state_id.id_type]
-    except KeyError:
-        raise ValueError(f"Invalid global state identifier type: {state_id.id_type}")
-
     if isinstance(state_id.identifier, bytes):
         state_id = state_id.identifier.hex()
     else:
         state_id = state_id.identifier
 
     return {
-        "key": serialisation.cl_value_to_parsed(key),
+        "key": serializer.cl_value_to_parsed(key),
         "path": path,
         "state_identifier": {
-            state_id_type: state_id
+            state_id.id_type.value: state_id
         }
     }
 
 
-def get_params_for_state_get_dictionary_item(
+def for_state_get_dictionary_item(
     identifier: DictionaryID,
-    state_root_hash: StateRootID
+    state_root_hash: StateRootHash
 ) -> dict:
     def get_dictionary_param():
-        if not isinstance(identifier, DICTIONARY_ID_VARIANTS):
-            raise ValueError("Unrecognized dictionary item type.")
-        elif isinstance(identifier, DictionaryID_AccountNamedKey):
+        if isinstance(identifier, DictionaryID_AccountNamedKey):
             return {
                 "AccountNamedKey": {
                     "dictionary_item_key": identifier.dictionary_item_key,
                     "dictionary_name": identifier.dictionary_name,
-                    "key": f"hash-{cl_checksum.encode_account_id(identifier.account_key)}"
+                    "key": f"hash-{checksummer.encode_account_id(identifier.account_key)}"
                 }
             }
         elif isinstance(identifier, DictionaryID_ContractNamedKey):
             return {
                 "ContractNamedKey": {
                     "dictionary_item_key": identifier.dictionary_item_key,
                     "dictionary_name": identifier.dictionary_name,
-                    "key": f"hash-{cl_checksum.encode_contract_id(identifier.contract_key)}"
+                    "key": f"hash-{checksummer.encode_contract_id(identifier.contract_key)}"
                 }
             }
         elif isinstance(identifier, DictionaryID_SeedURef):
             return {
                 "URef": {
                     "dictionary_item_key": identifier.dictionary_item_key,
                     "seed_uref": identifier.dictionary_name
                 }
             }
         elif isinstance(identifier, DictionaryID_UniqueKey):
             return {
                 "Dictionary": identifier.seed_uref.as_string()
             }
+        else:
+            raise ValueError("Unrecognized dictionary item type.")
 
     return {
         "dictionary_identifier": get_dictionary_param(),
         "state_root_hash": state_root_hash.hex(),
     }
 
 
-def get_params_for_state_get_item(
+def for_state_get_item(
     key: str,
     path: typing.Union[str, typing.List[str]],
     state_root_hash: bytes
 ) -> dict:
     return {
         "key": key,
         "path": path,
         "state_root_hash": state_root_hash.hex() if state_root_hash else None
     }
+
+
+def purse_id(purse_id: PurseID) -> dict:
+    id = \
+        purse_id.identifier.hex() if isinstance(purse_id.identifier, bytes) else \
+        purse_id.identifier
+    
+
+    if purse_id.id_type == PurseIDType.ACCOUNT_HASH:
+        return {
+            "purse_identifier": {
+                "main_purse_under_account_hash": f"{convertor.str_from_account_key(id)}"
+            }
+        }
+    elif purse_id.id_type == PurseIDType.PUBLIC_KEY:
+        return {
+            "purse_identifier": {
+                "main_purse_under_public_key": id
+            }
+        }
+    elif purse_id.id_type == PurseIDType.UREF:
+        return {
+            "purse_identifier": {
+                "purse_uref": convertor.str_from_uref(purse_id.identifier)
+            }
+        }
+    else:
+        raise ValueError(f"Invalid purse identifier type: {purse_id.id_type}")
```

### Comparing `pycspr-1.1.3/pycspr/api/rpc/proxy.py` & `pycspr-1.2.0/pycspr/api/rpc/proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,220 +1,235 @@
-import dataclasses
 import typing
 
 import jsonrpcclient
 import requests
 
-from pycspr import serialisation
+from pycspr import serializer
 from pycspr.api import constants
 from pycspr.api.rpc import params as param_utils
-from pycspr.types import AccountID
-from pycspr.types import BlockID
-from pycspr.types import Deploy
-from pycspr.types import DeployID
-from pycspr.types import DictionaryID
-from pycspr.types import GlobalStateID
-from pycspr.types import GlobalStateIDType
-from pycspr.types import PurseID
-from pycspr.types import StateRootID
+from pycspr.api.rpc.connection import ConnectionInfo
+from pycspr.types.crypto import Digest
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import Address
+from pycspr.types.node.rpc import BlockID
+from pycspr.types.node.rpc import DeployHash
+from pycspr.types.node.rpc import DictionaryID
+from pycspr.types.node.rpc import GlobalStateID
+from pycspr.types.node.rpc import GlobalStateIDType
+from pycspr.types.node.rpc import PurseID
+from pycspr.types.node.rpc import StateRootHash
 
 
-@dataclasses.dataclass
 class Proxy:
     """Node JSON-RPC server proxy.
 
     """
-    # Host address.
-    host: str = constants.DEFAULT_HOST
+    def __init__(self, connection_info: ConnectionInfo):
+        """Instance constructor.
+
+        :param connection_info: Information required to connect to a node.
 
-    # Number of exposed REST port.
-    port: int = constants.DEFAULT_PORT_RPC
+        """
+        self.connection_info = connection_info
 
     @property
     def address(self) -> str:
         """A node's RPC server base address."""
-        return f"http://{self.host}:{self.port}/rpc"
+        return f"http://{self.connection_info.host}:{self.connection_info.port}/rpc"
 
     def __str__(self):
         """Instance string representation."""
         return self.address
 
-    def account_put_deploy(self, deploy: Deploy) -> DeployID:
+    async def account_put_deploy(self, deploy: Deploy) -> DeployHash:
         """Dispatches a deploy to a node for processing.
 
         :param deploy: A deploy to be processed at a node.
-        :returns: Deploy identifier.
+        :returns: Deploy hash.
 
         """
         params: dict = {
-            "deploy": serialisation.to_json(deploy),
+            "deploy": serializer.to_json(deploy),
         }
 
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_ACCOUNT_PUT_DEPLOY,
             params,
             "deploy_hash"
             )
 
-    def chain_get_block(self, block_id: BlockID = None) -> dict:
+    async def chain_get_block(self, block_id: BlockID = None) -> dict:
         """Returns on-chain block information.
 
         :param block_id: Identifier of a finalised block.
         :returns: On-chain block information.
 
         """
-        params: dict = param_utils.get_block_id(block_id, False)
+        params: dict = param_utils.block_id(block_id, False)
 
-        return get_response(self.address, constants.RPC_CHAIN_GET_BLOCK, params, "block")
+        return await get_response(self.address, constants.RPC_CHAIN_GET_BLOCK, params, "block")
 
-    def chain_get_block_transfers(self, block_id: BlockID = None) -> dict:
+    async def chain_get_block_transfers(self, block_id: BlockID = None) -> dict:
         """Returns on-chain block transfers information.
 
         :param block_id: Identifier of a finalised block.
         :param decode: Flag indicating whether to decode API response.
         :returns: On-chain block transfers information.
 
         """
-        params: dict = param_utils.get_block_id(block_id, False)
+        params: dict = param_utils.block_id(block_id, False)
 
-        return get_response(self.address, constants.RPC_CHAIN_GET_BLOCK_TRANSFERS, params)
+        return await get_response(self.address, constants.RPC_CHAIN_GET_BLOCK_TRANSFERS, params)
 
-    def chain_get_era_info_by_switch_block(self, block_id: BlockID = None) -> dict:
+    async def chain_get_era_info_by_switch_block(self, block_id: BlockID = None) -> dict:
         """Returns consensus era information scoped by block id.
 
         :param block_id: Identifier of a block.
         :returns: Era information.
 
         """
-        params: dict = param_utils.get_block_id(block_id, False)
+        params: dict = param_utils.block_id(block_id, False)
 
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_CHAIN_GET_ERA_INFO_BY_SWITCH_BLOCK,
-            params
+            params,
+            "era_summary"
             )
 
-    def chain_get_era_summary(self, block_id: BlockID = None) -> dict:
+    async def chain_get_era_summary(self, block_id: BlockID = None) -> dict:
         """Returns consensus era summary information.
 
         :param block_id: Identifier of a block.
         :returns: Era summary information.
 
         """
-        params: dict = param_utils.get_block_id(block_id, False)
+        params: dict = param_utils.block_id(block_id, False)
 
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_CHAIN_GET_ERA_SUMMARY,
             params,
             "era_summary"
             )
 
-    def chain_get_state_root_hash(self, block_id: BlockID = None) -> StateRootID:
+    async def chain_get_state_root_hash(self, block_id: BlockID = None) -> StateRootHash:
         """Returns root hash of global state at a finalised block.
 
         :param block_id: Identifier of a finalised block.
         :returns: State root hash at finalised block.
 
         """
-        params: dict = param_utils.get_block_id(block_id, False)
+        params: dict = param_utils.block_id(block_id, False)
         response: str = \
-            get_response(
+            await get_response(
                 self.address,
                 constants.RPC_CHAIN_GET_STATE_ROOT_HASH,
                 params,
                 "state_root_hash"
                 )
 
         return bytes.fromhex(response)
 
-    def discover(self) -> dict:
+    async def discover(self) -> dict:
         """Returns RPC schema.
 
         :returns: Node JSON-RPC API schema.
 
         """
-        return get_response(self.address, constants.RPC_DISCOVER, field="schema")
+        return await get_response(self.address, constants.RPC_DISCOVER, field="schema")
 
-    def info_get_chainspec(self) -> dict:
+    async def info_get_chainspec(self) -> dict:
         """Returns canonical network state information.
 
         :returns: Chain spec, genesis accounts and global state information.
 
         """
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_INFO_GET_CHAINSPEC,
             field="chainspec_bytes"
             )
 
-    def info_get_deploy(self, deploy_id: DeployID) -> dict:
+    async def info_get_deploy(
+        self,
+        deploy_hash: DeployHash,
+        finalized_approvals: bool = False
+    ) -> dict:
         """Returns on-chain deploy information.
 
-        :param deploy_id: Identifier of a deploy processed by network.
+        :param deploy_hash: Hash of a deploy processed by network.
         :returns: On-chain deploy information.
 
         """
-        params: dict = param_utils.get_deploy_id(deploy_id)
+        params: dict = param_utils.deploy_hash(deploy_hash) | {
+            "finalized_approvals": finalized_approvals
+        }
 
-        return get_response(self.address, constants.RPC_INFO_GET_DEPLOY, params)
+        return await get_response(self.address, constants.RPC_INFO_GET_DEPLOY, params)
 
-    def info_get_peers(self) -> typing.List[dict]:
+    async def info_get_peers(self) -> typing.List[dict]:
         """Returns node peer information.
 
         :returns: Node peer information.
 
         """
-        return get_response(self.address, constants.RPC_INFO_GET_PEERS, field="peers")
+        return await get_response(self.address, constants.RPC_INFO_GET_PEERS, field="peers")
 
-    def info_get_status(self) -> dict:
+    async def info_get_status(self) -> dict:
         """Returns node status information.
 
         :returns: Node status information.
 
         """
-        return get_response(self.address, constants.RPC_INFO_GET_STATUS)
+        return await get_response(self.address, constants.RPC_INFO_GET_STATUS)
 
-    def info_get_validator_changes(self) -> typing.List[dict]:
+    async def info_get_validator_changes(self) -> typing.List[dict]:
         """Returns validator change set.
 
         :returns: Validator change set.
 
         """
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_INFO_GET_VALIDATOR_CHANGES,
             field="changes"
             )
 
-    def query_balance(self, purse_id: PurseID, global_state_id: GlobalStateID = None) -> int:
+    async def query_balance(
+        self,
+        purse_id: PurseID,
+        global_state_id: GlobalStateID = None
+    ) -> int:
         """Returns account balance at a certain point in global state history.
 
         :param proxy: Remote RPC server proxy.
         :param purse_id: Identifier of purse being queried.
         :param global_state_id: Identifier of global state root at some point in time.
         :returns: Account balance in motes (if purse exists).
 
         """
         if global_state_id is None:
             global_state_id = GlobalStateID(
-                self.chain_get_state_root_hash(),
+                await self.chain_get_state_root_hash(),
                 GlobalStateIDType.STATE_ROOT_HASH
             )
 
         params: dict = \
-            param_utils.get_global_state_id(global_state_id) | \
-            param_utils.get_purse_id(purse_id)
+            param_utils.global_state_id(global_state_id) | \
+            param_utils.purse_id(purse_id)
         
+        print(params)
+
         return int(
-            get_response(self.address, constants.RPC_QUERY_BALANCE, params, "balance")
+            await get_response(self.address, constants.RPC_QUERY_BALANCE, params, "balance")
         )
 
-    def query_global_state(
+    async def query_global_state(
         self,
         key: str,
         path: typing.List[str],
         state_id: GlobalStateID = None
     ) -> bytes:
         """Returns results of a query to global state at a specified block or state root hash.
 
@@ -222,114 +237,138 @@
         :param path: Identifier of a path within item.
         :param state_id: Identifier of global state leaf.
         :returns: Results of a global state query.
 
         """
         if state_id is None:
             state_id: GlobalStateID = GlobalStateID(
-                self.chain_get_state_root_hash(),
+                await self.chain_get_state_root_hash(),
                 GlobalStateIDType.STATE_ROOT_HASH
                 )
 
-        params: dict = param_utils.get_params_for_query_global_state(key, path, state_id)
+        params: dict = param_utils.for_query_global_state(key, path, state_id)
 
-        return get_response(self.address, constants.RPC_QUERY_GLOBAL_STATE, params)
+        return await get_response(self.address, constants.RPC_QUERY_GLOBAL_STATE, params)
 
-    def state_get_account_info(self, account_id: AccountID, block_id: BlockID = None) -> dict:
+    async def state_get_account_info(
+        self,
+        account_id: Address,
+        block_id: BlockID = None
+    ) -> dict:
         """Returns account information at a certain global state root hash.
 
         :param account_id: An account holder's public key prefixed with a key type identifier.
         :param block_id: Identifier of a finalised block.
         :returns: Account information in JSON format.
 
         """
         params: dict = \
-            param_utils.get_account_key(account_id) | \
-            param_utils.get_block_id(block_id)
-        
-        print(block_id)
+            param_utils.account_key(account_id) | \
+            param_utils.block_id(block_id)
 
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_STATE_GET_ACCOUNT_INFO,
             params,
             "account"
             )
 
-    def state_get_auction_info(self, block_id: BlockID = None) -> dict:
+    async def state_get_auction_info(self, block_id: BlockID = None) -> dict:
         """Returns current auction system contract information.
 
         :param block_id: Identifier of a finalised block.
         :returns: Current auction system contract information.
 
         """
-        params: dict = param_utils.get_block_id(block_id, False)
+        params: dict = param_utils.block_id(block_id, False)
 
-        return get_response(
+        return await get_response(
             self.address,
             constants.RPC_STATE_GET_AUCTION_INFO,
             params,
             "auction_state"
             )
 
-    def state_get_dictionary_item(
+    async def state_get_dictionary_item(
         self,
         identifier: DictionaryID,
-        state_root_hash: StateRootID = None
+        state_root_hash: StateRootHash = None
     ) -> dict:
         """Returns on-chain data stored under a dictionary item.
 
         :param identifier: Identifier required to query a dictionary item.
         :param state_root_hash: A node's root state hash at some point in chain time.
         :returns: On-chain data stored under a dictionary item.
 
         """
         if state_root_hash is None:
-            state_root_hash = self.chain_get_state_root_hash()
+            state_root_hash = await self.chain_get_state_root_hash()
 
         params: dict = \
-            param_utils.get_params_for_state_get_dictionary_item(identifier, state_root_hash)
+            param_utils.for_state_get_dictionary_item(identifier, state_root_hash)
 
-        return get_response(self.address, constants.RPC_STATE_GET_DICTIONARY_ITEM, params)
+        return await get_response(self.address, constants.RPC_STATE_GET_DICTIONARY_ITEM, params)
 
-    def state_get_item(
+    async def state_get_item(
         self,
         key: str,
         path: typing.Union[str, typing.List[str]] = [],
-        state_root_hash: StateRootID = None
+        state_root_hash: StateRootHash = None
     ) -> bytes:
         """Returns results of a query to global state at a specified block or state root hash.
 
         :param proxy: Remote RPC server proxy.
         :param key: Key of an item stored within global state.
         :param path: Identifier of a path within item.
         :param state_root_hash: A node's root state hash at some point in chain time.
         :returns: Results of a global state query.
 
         """
         path = path if isinstance(path, list) else [path]
-        state_root_hash = state_root_hash or self.chain_get_state_root_hash()
+        state_root_hash = state_root_hash or await self.chain_get_state_root_hash()
 
-        params: dict = param_utils.get_params_for_state_get_item(key, path, state_root_hash)
+        params: dict = param_utils.for_state_get_item(key, path, state_root_hash)
 
-        return get_response(self.address, constants.RPC_STATE_GET_ITEM, params, "stored_value")
+        return await get_response(
+            self.address,
+            constants.RPC_STATE_GET_ITEM,
+            params,
+            "stored_value"
+            )
+
+    async def state_get_trie(self, trie_key: Digest) -> typing.Optional[bytes]:
+        """Returns results of a query to global state trie store at a specified key.
+
+        :param trie_key: Key of an item stored within global state.
+        :returns:  A list of keys read under the specified prefix.
+
+        """
+        params: dict = {
+            "trie_key": trie_key.hex()
+        }
+
+        return await get_response(
+            self.address,
+            constants.RPC_STATE_GET_TRIE, params,
+            "maybe_trie_bytes"
+            )
 
 
 class ProxyError(Exception):
     """Node API error wrapper.
 
     """
     def __init__(self, msg):
         """Instance constructor.
 
         """
         super(ProxyError, self).__init__(msg)
 
 
-def get_response(
+async def get_response(
     address: str,
     endpoint: str,
     params: dict = None,
     field: str = None,
 ) -> dict:
     """Invokes JSON-RPC API & returns parsed response.
```

### Comparing `pycspr-1.1.3/pycspr/api/rpc_speculative/client.py` & `pycspr-1.2.0/pycspr/api/rpc_speculative/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from pycspr.api.connection import NodeConnectionInfo
+from pycspr.api.rpc_speculative.connection import ConnectionInfo
 from pycspr.api.rpc_speculative.proxy import Proxy
-from pycspr.types import Deploy
-from pycspr.types import BlockID
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import BlockID
 
 
 class Client():
     """Node speculative RPC server client.
 
     """
-    def __init__(self, connection_info: NodeConnectionInfo) -> dict:
+    def __init__(self, connection_info: ConnectionInfo) -> dict:
         """Instance constructor.
 
         :param connection_info: Information required to connect to a node.
 
         """
-        self.proxy = Proxy(connection_info.host, connection_info.port_rpc_speculative)
+        print(connection_info)
+        self.proxy = Proxy(connection_info)
 
-    def speculative_exec(self, deploy: Deploy, block_id: BlockID = None) -> dict:
+    async def speculative_exec(self, deploy: Deploy, block_id: BlockID = None) -> dict:
         """Dispatches a deploy to a node for speculative execution.
 
         :param deploy: A deploy to be processed at a node.
         :param block_id: Identifier of a finalised block.
         :returns: Execution effects of virtual deploy processing.
 
         """
-        return self.proxy.speculative_exec(deploy, block_id)
+        return await self.proxy.speculative_exec(deploy, block_id)
```

### Comparing `pycspr-1.1.3/pycspr/api/rpc_speculative/proxy.py` & `pycspr-1.2.0/pycspr/api/rpc_speculative/proxy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import dataclasses
-
-from pycspr import serialisation
+from pycspr import serializer
 from pycspr.api import constants
 from pycspr.api.rpc import params as param_utils
 from pycspr.api.rpc.proxy import get_response
-from pycspr.types import Deploy
-from pycspr.types import BlockID
+from pycspr.api.rpc_speculative.connection import ConnectionInfo
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import BlockID
 
 
-@dataclasses.dataclass
 class Proxy:
-    """Node JSON-RPC server proxy.
+    """Node speculative JSON-RPC server proxy.
 
     """
-    # Host address.
-    host: str = constants.DEFAULT_HOST
+    def __init__(self, connection_info: ConnectionInfo):
+        """Instance constructor.
+
+        :param connection_info: Information required to connect to a node.
 
-    # Number of exposed speculative RPC port.
-    port: int = constants.DEFAULT_PORT_SPECULATIVE_RPC
+        """
+        self.connection_info = connection_info
 
     @property
     def address(self) -> str:
-        """A node's RPC server base address."""
-        return f"http://{self.host}:{self.port}/rpc"
+        """A node's speculative RPC server base address."""
+        return f"http://{self.connection_info.host}:{self.connection_info.port}/rpc"
 
     def __str__(self):
         """Instance string representation."""
         return self.address
 
-    def speculative_exec(self, deploy: Deploy, block_id: BlockID = None) -> dict:
+    async def speculative_exec(self, deploy: Deploy, block_id: BlockID = None) -> dict:
         """Dispatches a deploy to a node for speculative execution.
 
         :param deploy: A deploy to be processed at a node.
         :param block_id: Identifier of a finalised block.
         :returns: Execution effects of virtual deploy processing.
 
         """
-        params: dict = param_utils.get_block_id(block_id) | {
-            "deploy": serialisation.to_json(deploy)
+        params: dict = param_utils.block_id(block_id) | {
+            "deploy": serializer.to_json(deploy)
         }
 
-        return get_response(
+        return await get_response(
             self.address,
             constants.SPECULATIVE_RPC_EXEC_DEPLOY,
             params,
             "execution_result"
             )
```

### Comparing `pycspr-1.1.3/pycspr/api/sse/client.py` & `pycspr-1.2.0/pycspr/api/sse/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import typing
 
-from pycspr.api.connection import NodeConnectionInfo
 from pycspr.api.rpc import Client as RpcClient
+from pycspr.api.rpc import ConnectionInfo as RpcClientConnectionInfo
+from pycspr.api.sse.connection import ConnectionInfo
 from pycspr.api.sse.proxy import Proxy
-from pycspr.api.sse.types import NodeEventChannel
-from pycspr.api.sse.types import NodeEventInfo
-from pycspr.api.sse.types import NodeEventType
-from pycspr.api.sse.types import SSE_CHANNEL_TO_SSE_EVENT
+from pycspr.types.node.sse import NodeEventChannel
+from pycspr.types.node.sse import NodeEventInfo
+from pycspr.types.node.sse import NodeEventType
+from pycspr.types.node.sse import SSE_CHANNEL_TO_SSE_EVENT
 
 
 class Client():
     """Node SSE server client.
 
     """
-    def __init__(self, connection_info: NodeConnectionInfo, rpc_client: RpcClient = None):
+    def __init__(self, connection_info: ConnectionInfo, rpc_client: RpcClient = None):
         """Instance constructor.
 
         :param connection_info: Information required to connect to a node.
         :param rpc_client: Node RPC client.
 
         """
-        self.proxy = Proxy(connection_info.host, connection_info.port_sse)
+        self.proxy = Proxy(connection_info)
+        self.rpc = rpc_client or RpcClient(
+            RpcClientConnectionInfo(connection_info.host, connection_info.port_rpc)
+        )
 
         # Extension methods -> 2nd order functions.
-        ext = ClientExtensions(self, rpc_client or RpcClient(connection_info))
+        ext = ClientExtensions(self)
         self.await_n_blocks = ext.await_n_blocks
         self.await_n_eras = ext.await_n_eras
         self.await_n_events = ext.await_n_events
         self.await_until_block_n = ext.await_until_block_n
         self.await_until_era_n = ext.await_until_era_n
         self.get_events = ext.get_events
 
@@ -53,23 +57,22 @@
             yield einfo
 
 
 class ClientExtensions():
     """Node SSE server client extensions, i.e. 2nd order functions.
 
     """
-    def __init__(self, client: Client, rpc_client: RpcClient):
+    def __init__(self, client: Client):
         """Instance constructor.
 
         :param client: Node SSE client.
-        :param rpc_client: Node RPC client.
 
         """
         self.client = client
-        self.rpc_client = rpc_client
+        self.rpc_client = client.rpc
 
     async def await_n_blocks(self, offset: int):
         """Awaits until linear block chain has advanced by N blocks.
 
         :param offset: Number of blocks to await.
 
         """
@@ -108,27 +111,27 @@
     async def await_until_block_n(self, future: int) -> dict:
         """Awaits until linear block chain has advanced to block N.
 
         :param future: Height of a future block to await.
         :returns: On-chain block information N block in the future.
 
         """
-        _, current = self.rpc_client.get_chain_heights()
+        _, current = await self.rpc_client.get_chain_heights()
         offset = future - current
         if offset > 0:
             await self.await_n_blocks(offset)
 
     async def await_until_era_n(self, future: int) -> dict:
         """Awaits until consensus has advanced to era N.
 
         :param future: Height of a future era to await.
         :returns: On-chain era information N eras in the future.
 
         """
-        current, _ = self.rpc_client.get_chain_heights()
+        current, _ = await self.rpc_client.get_chain_heights()
         offset = future - current
         if offset > 0:
             await self.await_n_eras(offset)
 
     def get_events(
         self,
         ecallback: typing.Callable[[NodeEventInfo], None],
```

### Comparing `pycspr-1.1.3/pycspr/api/sse/proxy.py` & `pycspr-1.2.0/pycspr/api/sse/proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import dataclasses
 import json
 import typing
 
 import requests
 import sseclient
 
-from pycspr.api import constants
-from pycspr.api.sse.types import NodeEventChannel
-from pycspr.api.sse.types import NodeEventInfo
-from pycspr.api.sse.types import NodeEventType
+from pycspr.api.sse.connection import ConnectionInfo
+from pycspr.types.node.sse import NodeEventChannel
+from pycspr.types.node.sse import NodeEventInfo
+from pycspr.types.node.sse import NodeEventType
 
 
-@dataclasses.dataclass
 class Proxy:
     """Node SSE server proxy.
 
     """
-    # Host address.
-    host: str = constants.DEFAULT_HOST
+    def __init__(self, connection_info: ConnectionInfo):
+        """Instance constructor.
 
-    # Number of exposed SSE port.
-    port: int = constants.DEFAULT_PORT_SSE
+        :param connection_info: Information required to connect to a node.
+
+        """
+        self.connection_info = connection_info
 
     @property
     def address(self) -> str:
-        """A node's SSE server base address."""
-        return f"http://{self.host}:{self.port}/events"
+        """A node's REST server base address."""
+        return f"http://{self.connection_info.host}:{self.connection_info.port}/events"
 
     def __str__(self):
         """Instance string representation."""
         return self.address
 
     def yield_events(
         self,
```

### Comparing `pycspr-1.1.3/pycspr/api/sse/types.py` & `pycspr-1.2.0/pycspr/types/node/sse/simple.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import dataclasses
 import enum
 import typing
 
 
 class NodeEventChannel(enum.Enum):
     """Enumeration over set of exposed node SEE event types.
 
@@ -23,34 +22,16 @@
     DeployExpired = enum.auto()
     Fault = enum.auto()
     FinalitySignature = enum.auto()
     Shutdown = enum.auto()
     Step = enum.auto()
 
 
-@dataclasses.dataclass
-class NodeEventInfo():
-    """Encapsulates emitted event information.
-
-    """
-    # Channel over which event emitted by a node.
-    channel: NodeEventChannel
-
-    # Type of event emitted by a node.
-    typeof: NodeEventType
-
-    # Event ordinal identifier - acts as an offset.
-    idx: int
-
-    # Event payload ... typically data but sometimes a simple string.
-    payload: typing.Union[dict, str]
-
-
 # Map: SSE channel <-> SSE event.
-SSE_CHANNEL_TO_SSE_EVENT = {
+SSE_CHANNEL_TO_SSE_EVENT: typing.Dict[NodeEventChannel, typing.Set[NodeEventType]] = {
     NodeEventChannel.deploys: {
         NodeEventType.ApiVersion,
         NodeEventType.DeployAccepted
     },
     NodeEventChannel.main: {
         NodeEventType.ApiVersion,
         NodeEventType.BlockAdded,
```

### Comparing `pycspr-1.1.3/pycspr/crypto/__init__.py` & `pycspr-1.2.0/pycspr/crypto/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-from pycspr.crypto import cl_checksum
+from pycspr.crypto import checksummer
 from pycspr.crypto.cl_operations import get_account_hash
 from pycspr.crypto.cl_operations import get_account_key
-from pycspr.crypto.cl_operations import get_account_key_algo
 from pycspr.crypto.cl_operations import get_signature_for_deploy_approval
 from pycspr.crypto.cl_operations import verify_deploy_approval_signature
-from pycspr.crypto.defaults import DEFAULT_HASH_ALGO
-from pycspr.crypto.defaults import DEFAULT_KEY_ALGO
 from pycspr.crypto.ecc import get_key_pair
 from pycspr.crypto.ecc import get_key_pair_from_base64
 from pycspr.crypto.ecc import get_key_pair_from_bytes
 from pycspr.crypto.ecc import get_key_pair_from_hex_string
 from pycspr.crypto.ecc import get_key_pair_from_pem_file
 from pycspr.crypto.ecc import get_key_pair_from_seed
 from pycspr.crypto.ecc import get_pvk_pem_file_from_bytes
 from pycspr.crypto.ecc import get_pvk_pem_from_bytes
 from pycspr.crypto.ecc import get_signature
 from pycspr.crypto.ecc import get_signature_from_pem_file
 from pycspr.crypto.ecc import is_signature_valid
-from pycspr.crypto.enums import HashAlgorithm
-from pycspr.crypto.enums import KeyAlgorithm
+from pycspr.crypto.ecc import DEFAULT_KEY_ALGO
 from pycspr.crypto.hashifier import get_hash
+from pycspr.crypto.hashifier import DEFAULT_HASH_ALGO
```

### Comparing `pycspr-1.1.3/pycspr/crypto/cl_checksum.py` & `pycspr-1.2.0/pycspr/crypto/checksummer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import itertools
 import typing
 
-
-from pycspr.crypto.enums import HashAlgorithm
 from pycspr.crypto.hashifier import get_hash
+from pycspr.types.crypto.simple import HashAlgorithm
 
 
 # The number of input bytes, at or below which [`encode`] will checksum-encode the output.
 _SMALL_BYTES_COUNT: int = 75
 
 # The set of characters to which nibbles will be mapped.
 _HEX_CHARS: typing.List[str] = [
     '0', '1', '2', '3', '4', '5', '6', '7', '8', '9',
     'a', 'b', 'c', 'd', 'e', 'f',
     'A', 'B', 'C', 'D', 'E', 'F',
 ]
 
 
-def decode(input: str) -> bytes:
+def decode_bytes(input: str) -> bytes:
     """Maps input hexadecimal string to an array of bytes.
 
     :param input: A checksummed hexadecimal string to be mapped.
     :returns: An array of bytes.
 
     """
     input_bytes: bytes = bytes.fromhex(input)
@@ -34,40 +33,25 @@
     for idx, (i, j) in enumerate(zip(input, _encode(input_bytes))):
         if i != j:
             raise ValueError(f"Checksum contains an invalid byte at position: {idx}")
 
     return input_bytes
 
 
-def encode(input: bytes) -> str:
-    """Encodes input bytes as hexadecimal with mixed-case based checksums
-    following a scheme similar to [EIP-55][1].
-
-    :param input: Input data to be encoded.
-    :returns: Checksummed hexadecimal string.
-
-    """
-    # Return lower case for long inputs.
-    if len(input) > _SMALL_BYTES_COUNT:
-        return input.hex().lower()
-
-    return "".join(_encode(input))
-
-
 def encode_account_key(account_id: typing.Union[str, bytes]) -> str:
     """Encodes an account identifier as a checksummed hexadecimal string.
 
     :param block_id: An account identifier.
     :returns: Checksummed hexadecimal string.
 
     """
     if isinstance(account_id, str):
         account_id = bytes.fromhex(account_id)
 
-    return account_id[:1].hex() + encode(account_id[1:])
+    return account_id[:1].hex() + encode_bytes(account_id[1:])
 
 
 # Synonym due to semantic issues.
 encode_account_id = encode_account_key
 
 
 def encode_block_id(block_id: typing.Union[str, bytes]) -> str:
@@ -76,67 +60,82 @@
     :param block_id: A block identifier.
     :returns: Checksummed hexadecimal string.
 
     """
     if isinstance(block_id, str):
         block_id = bytes.fromhex(block_id)
 
-    return encode(block_id)
+    return encode_bytes(block_id)
+
+
+def encode_bytes(input: bytes) -> str:
+    """Encodes input bytes as hexadecimal with mixed-case based checksums
+    following a scheme similar to [EIP-55][1].
+
+    :param input: Input data to be encoded.
+    :returns: Checksummed hexadecimal string.
+
+    """
+    # Return lower case for long inputs.
+    if len(input) > _SMALL_BYTES_COUNT:
+        return input.hex().lower()
+
+    return "".join(_encode(input))
 
 
 def encode_contract_id(contract_id: typing.Union[str, bytes]) -> str:
     """Encodes a contract identifier as a checksummed hexadecimal string.
 
     :param contract_id: A contract identifier.
     :returns: Checksummed hexadecimal string.
 
     """
     if isinstance(contract_id, str):
         contract_id = bytes.fromhex(contract_id)
 
-    return encode(contract_id)
+    return encode_bytes(contract_id)
 
 
-def encode_deploy_id(deploy_id: typing.Union[str, bytes]) -> str:
+def encode_deploy_hash(deploy_id: typing.Union[str, bytes]) -> str:
     """Encodes a deploy identifier as a checksummed hexadecimal string.
 
     :param deploy_id: A deploy identifier.
     :returns: Checksummed hexadecimal string.
 
     """
     if isinstance(deploy_id, str):
         deploy_id = bytes.fromhex(deploy_id)
 
-    return encode(deploy_id)
+    return encode_bytes(deploy_id)
 
 
 def encode_digest(digest: typing.Union[str, bytes]) -> str:
     """Encodes a digest as a checksummed hexadecimal string.
 
     :param digest: A digest.
     :returns: Checksummed hexadecimal string.
 
     """
     if isinstance(digest, str):
         digest = bytes.fromhex(digest)
 
-    return encode(digest)
+    return encode_bytes(digest)
 
 
 def encode_signature(signature: typing.Union[str, bytes]) -> str:
     """Encodes a digital signature as a checksummed hexadecimal string.
 
     :param signature: A digital signature.
     :returns: Checksummed hexadecimal string.
 
     """
     if isinstance(signature, str):
         signature = bytes.fromhex(signature)
 
-    return signature[:1].hex() + encode(signature[1:])
+    return signature[:1].hex() + encode_bytes(signature[1:])
 
 
 def _encode(input: bytes) -> typing.Iterator[str]:
     """Maps input to iterator of hexadecimal characters.
 
     """
     hash_bits: typing.Iterator[int] = _bytes_to_bits_cycle(
```

### Comparing `pycspr-1.1.3/pycspr/crypto/cl_operations.py` & `pycspr-1.2.0/pycspr/crypto/cl_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from pycspr.crypto.ecc import get_signature
 from pycspr.crypto.ecc import is_signature_valid
-from pycspr.crypto.enums import HashAlgorithm
-from pycspr.crypto.enums import KeyAlgorithm
 from pycspr.crypto.hashifier import get_hash
+from pycspr.types.crypto.complex import PrivateKey
+from pycspr.types.crypto.simple import Digest
+from pycspr.types.crypto.simple import HashAlgorithm
+from pycspr.types.crypto.simple import KeyAlgorithm
+from pycspr.types.crypto.simple import SignatureBytes
 
 
 # Desired length of hash digest.
 _DIGEST_LENGTH = 32
 
 # Map: Key algorithm <-> length of public key.
 _PUBLIC_KEY_LENGTHS = {
@@ -19,15 +22,15 @@
     """Returns an on-chain account identifier (hex format) as derived from an account key.
 
     :param account_key: An on-chain account identifier.
 
     :returns: An on-chain account identifier.
 
     """
-    key_algo: KeyAlgorithm = get_account_key_algo(account_key)
+    key_algo: KeyAlgorithm = KeyAlgorithm(account_key[0])
     public_key: bytes = account_key[1:]
     as_bytes: bytes = \
         bytes(key_algo.name.lower(), "utf-8") + \
         bytearray(1) + \
         public_key
 
     return get_hash(as_bytes, _DIGEST_LENGTH, HashAlgorithm.BLAKE2B)
@@ -43,46 +46,33 @@
     """
     assert len(public_key) == _PUBLIC_KEY_LENGTHS[key_algo], \
            f"Invalid {key_algo.name} public key length."
 
     return bytes([key_algo.value]) + public_key
 
 
-def get_account_key_algo(account_key: bytes) -> KeyAlgorithm:
-    """Returns ECC algorithm identifier associated with an account key.
-
-    :param account_key: An account key associated with a specific ECC algorithm.
-    :returns: An ECC key algorithm identifier.
-
-    """
-    try:
-        return KeyAlgorithm(account_key[0])
-    except ValueError:
-        raise ValueError("Unsupported account key.")
-
-
 def get_signature_for_deploy_approval(
-    deploy_hash: bytes,
-    private_key: bytes,
-    key_algo: KeyAlgorithm
-) -> bytes:
+    deploy_hash: Digest,
+    key_of_approver: PrivateKey
+) -> SignatureBytes:
     """Returns a signature designated to approve a deploy.
 
-    :param deploy_hash: Identifier, i.e. hash, of a deploy to be signed.
-    :param pvk: Secret key.
-    :param algo: Type of ECC algo used to generate secret key.
-    :returns: Digital signature of input data.
+    :param deploy_hash: Digest of a deploy to be signed.
+    :param key_of_approver: Private key of approver.
+    :returns: Digital signature over deploy digest.
 
     """
-    return bytes([key_algo.value]) + get_signature(deploy_hash, private_key, algo=key_algo)
+    return \
+        bytes([key_of_approver.algo.value]) + \
+        get_signature(deploy_hash, key_of_approver.pvk, key_of_approver.algo)
 
 
 def verify_deploy_approval_signature(
-    deploy_hash: bytes,
-    sig: bytes,
+    deploy_hash: Digest,
+    sig: SignatureBytes,
     account_key: bytes
 ) -> bool:
     """Returns a flag indicating whether a deploy signature was signed by private key
        associated with the passed account key.
 
     :param deploy_hash: Hash of a deploy that has been signed.
     :param sig: A digital signature.
@@ -91,10 +81,13 @@
 
     """
     assert len(deploy_hash) == 32, \
            "Invalid deploy hash.  Expected length = 32"
     assert len(sig) == 65, \
            "Invalid deploy approval signature.  Expected length = 65"
 
-    algo = get_account_key_algo(account_key)
-
-    return is_signature_valid(deploy_hash, sig[1:], account_key[1:], algo)
+    return is_signature_valid(
+        deploy_hash,
+        sig[1:],
+        account_key[1:],
+        KeyAlgorithm(account_key[0])
+        )
```

### Comparing `pycspr-1.1.3/pycspr/crypto/ecc.py` & `pycspr-1.2.0/pycspr/crypto/ecc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import base64
 import tempfile
 import typing
 
 from pycspr.crypto import ecc_ed25519 as ed25519
 from pycspr.crypto import ecc_secp256k1 as secp256k1
-from pycspr.crypto.defaults import DEFAULT_KEY_ALGO
-from pycspr.crypto.enums import KeyAlgorithm
+from pycspr.types.crypto.simple import KeyAlgorithm
 
 
-# Map: ECC Algo Type -> ECC Algo Implementation.
+# Map: Key algo Type -> Key algo Implementation.
 ALGOS = {
     KeyAlgorithm.ED25519: ed25519,
     KeyAlgorithm.SECP256K1: secp256k1,
 }
 
+# Default key algorithm.
+DEFAULT_KEY_ALGO = KeyAlgorithm.ED25519
+
 
 def get_key_pair(algo: KeyAlgorithm = DEFAULT_KEY_ALGO) -> typing.Tuple[bytes, bytes]:
     """Returns an ECC key pair, each key is a 32 byte array.
 
     :param algo: Type of ECC algo to be used when generating key pair.
     :returns : 2 member tuple: (private key, public key)
```

### Comparing `pycspr-1.1.3/pycspr/crypto/ecc_ed25519.py` & `pycspr-1.2.0/pycspr/crypto/ecc_ed25519.py`

 * *Files identical despite different names*

### Comparing `pycspr-1.1.3/pycspr/crypto/ecc_secp256k1.py` & `pycspr-1.2.0/pycspr/crypto/ecc_secp256k1.py`

 * *Files identical despite different names*

### Comparing `pycspr-1.1.3/pycspr/crypto/hashifier.py` & `pycspr-1.2.0/pycspr/crypto/hashifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from pycspr.crypto.hashifier_blake2b import get_hash as blake2b
 from pycspr.crypto.hashifier_blake3 import get_hash as blake3
-from pycspr.crypto.defaults import DEFAULT_HASH_ALGO
-from pycspr.crypto.enums import HashAlgorithm
+from pycspr.types.crypto.simple import Digest
+from pycspr.types.crypto.simple import HashAlgorithm
 
 
 # Map: Hash Algo Type -> Hash Algo Implementation.
 ALGOS = {
     HashAlgorithm.BLAKE2B: blake2b,
     HashAlgorithm.BLAKE3: blake3,
 }
 
 # Default length of a hash digest.
-DIGEST_LENGTH = 32
+DEFAULT_DIGEST_LENGTH = 32
+
+# Default hash algo.
+DEFAULT_HASH_ALGO = HashAlgorithm.BLAKE2B
 
 
 def get_hash(
     data: bytes,
-    size: int = DIGEST_LENGTH,
+    size: int = DEFAULT_DIGEST_LENGTH,
     algo: HashAlgorithm = DEFAULT_HASH_ALGO
-) -> bytes:
+) -> Digest:
     """Maps input to a hash function output.
 
     :param data: Data to be hashed.
     :param size: Desired hashing output length.
     :param algo: Type of hashing algo to apply.
-    :returns: Hash of input data.
+    :returns: Digest of input data.
 
     """
     return ALGOS[algo](data, size)
```

### Comparing `pycspr-1.1.3/pycspr/factory/__init__.py` & `pycspr-1.2.0/pycspr/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `pycspr-1.1.3/pycspr/factory/accounts.py` & `pycspr-1.2.0/pycspr/factory/accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import pathlib
 import typing
 
-from pycspr import crypto
-from pycspr.types import PrivateKey
-from pycspr.types import PublicKey
+from pycspr.types.crypto import KeyAlgorithm
+from pycspr.types.crypto import PrivateKey
+from pycspr.types.crypto import PublicKey
+from pycspr.crypto import get_key_pair_from_bytes
+from pycspr.crypto import get_key_pair_from_pem_file
 
 
-def create_private_key(algo: crypto.KeyAlgorithm, pvk: bytes, pbk: bytes) -> PrivateKey:
+def create_private_key(algo: KeyAlgorithm, pvk: bytes, pbk: bytes) -> PrivateKey:
     """Returns an account holder's private key.
 
     :param algo: ECC key algorithm identifier.
     :param pvk: ECC private key.
     :param pbk: ECC public key.
 
     """
     if isinstance(algo, str):
-        algo = crypto.KeyAlgorithm[algo]
+        algo = KeyAlgorithm[algo]
 
     return PrivateKey(pvk, pbk, algo)
 
 
-def create_public_key(algo: crypto.KeyAlgorithm, pbk: bytes) -> PublicKey:
+def create_public_key(algo: KeyAlgorithm, pbk: bytes) -> PublicKey:
     """Returns an account holder's public key.
 
     :param algo: ECC key algorithm identifier.
     :param pbk: ECC public key raw bytes.
 
     """
     return PublicKey(algo, pbk)
@@ -33,47 +35,47 @@
 def create_public_key_from_account_key(account_key: bytes) -> PublicKey:
     """Returns an account holder's public key.
 
     :param account_key: Account key asociated with account;s public key.
     :returns: A public key.
 
     """
-    return create_public_key(crypto.KeyAlgorithm(account_key[0]), account_key[1:])
+    return create_public_key(KeyAlgorithm(account_key[0]), account_key[1:])
 
 
 def parse_private_key(
     fpath: pathlib.Path,
-    algo: typing.Union[str, crypto.KeyAlgorithm] = crypto.KeyAlgorithm.ED25519
+    algo: typing.Union[str, KeyAlgorithm] = KeyAlgorithm.ED25519
 ) -> PrivateKey:
     """Returns on-chain account information deserialised from a secret key held on file system.
 
     :param fpath: Path to secret key pem file associated with the account.
     :param algo: ECC key algorithm identifier.
     :returns: On-chain account information wrapper.
 
     """
-    algo = crypto.KeyAlgorithm[algo] if isinstance(algo, str) else algo
-    (pvk, pbk) = crypto.get_key_pair_from_pem_file(fpath, algo)
+    algo = KeyAlgorithm[algo] if isinstance(algo, str) else algo
+    (pvk, pbk) = get_key_pair_from_pem_file(fpath, algo)
 
     return create_private_key(algo, pvk, pbk)
 
 
 def parse_private_key_bytes(
     pvk: bytes,
-    algo: typing.Union[str, crypto.KeyAlgorithm] = crypto.KeyAlgorithm.ED25519
+    algo: typing.Union[str, KeyAlgorithm] = KeyAlgorithm.ED25519
 ) -> PrivateKey:
     """Returns a user's private key deserialised from a secret key.
 
     :param pvk: A private key.
     :param algo: ECC key algorithm identifier.
     :returns: Private key wrapper.
 
     """
-    algo = crypto.KeyAlgorithm[algo] if isinstance(algo, str) else algo
-    (pvk, pbk) = crypto.get_key_pair_from_bytes(pvk, algo)
+    algo = KeyAlgorithm[algo] if isinstance(algo, str) else algo
+    (pvk, pbk) = get_key_pair_from_bytes(pvk, algo)
 
     return create_private_key(algo, pvk, pbk)
 
 
 def parse_public_key(fpath: pathlib.Path) -> PublicKey:
     """Returns an account holder's public key.
 
@@ -85,19 +87,19 @@
         account_key = bytes.fromhex(fstream.read())
 
     return create_public_key_from_account_key(account_key)
 
 
 def parse_public_key_bytes(
     pbk: bytes,
-    algo: typing.Union[str, crypto.KeyAlgorithm]
+    algo: typing.Union[str, KeyAlgorithm]
 ) -> PublicKey:
     """Returns an account holder's public key.
 
     :param pbk: A public key.
     :param algo: ECC key algorithm identifier.
     :returns: A public key.
 
     """
-    algo = crypto.KeyAlgorithm[algo] if isinstance(algo, str) else algo
+    algo = KeyAlgorithm[algo] if isinstance(algo, str) else algo
 
     return create_public_key(algo, pbk)
```

### Comparing `pycspr-1.1.3/pycspr/factory/deploys.py` & `pycspr-1.2.0/pycspr/factory/deploys.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import datetime
 import random
 import typing
 
-from pycspr import crypto
+from pycspr.types.crypto import PrivateKey
+from pycspr.types.crypto import PublicKey
+from pycspr.crypto import get_signature_for_deploy_approval
 from pycspr.factory.accounts import create_public_key
 from pycspr.factory.digests import create_digest_of_deploy
 from pycspr.factory.digests import create_digest_of_deploy_body
-from pycspr.types import CL_Option
-from pycspr.types import CL_PublicKey
-from pycspr.types import CL_Type_U64
-from pycspr.types import CL_U8
-from pycspr.types import CL_U64
-from pycspr.types import CL_U512
-from pycspr.types import CL_URef
-from pycspr.types import Deploy
-from pycspr.types import DeployArgument
-from pycspr.types import DeployApproval
-from pycspr.types import DeployBody
-from pycspr.types import DeployHeader
-from pycspr.types import DeployParameters
-from pycspr.types import DeployTimeToLive
-from pycspr.types import DeployExecutableItem
-from pycspr.types import ModuleBytes
-from pycspr.types import PrivateKey
-from pycspr.types import PublicKey
-from pycspr.types import Timestamp
-from pycspr.types import Transfer
-from pycspr.types.cl_values import CL_Value
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import DeployBody
+from pycspr.types.node.rpc import DeployHeader
+from pycspr.types.node.rpc import DeployParameters
+from pycspr.types.node.rpc import DeployTimeToLive
+from pycspr.types.cl import CLV_Option
+from pycspr.types.cl import CLT_Type_U64
+from pycspr.types.cl import CLV_U8
+from pycspr.types.cl import CLV_U64
+from pycspr.types.cl import CLV_U512
+from pycspr.types.cl import CLV_URef
+from pycspr.types.cl import CLV_Value
+from pycspr.types.node.rpc import AccountKey
+from pycspr.types.node.rpc import DeployApproval
+from pycspr.types.node.rpc import DeployArgument
+from pycspr.types.node.rpc import DeployExecutableItem
+from pycspr.types.node.rpc import DeployOfModuleBytes
+from pycspr.types.node.rpc import DeployOfTransfer
+from pycspr.types.node.rpc import Timestamp
 from pycspr.utils import constants
-from pycspr.utils import conversion
+from pycspr.utils import convertor
 from pycspr.utils import io as _io
 
 
 def create_deploy(
     params: DeployParameters,
     payment: DeployExecutableItem,
     session: DeployExecutableItem
@@ -64,22 +64,20 @@
     :returns: A deploy approval to be associated with a deploy.
 
     """
     deploy_hash = deploy.hash if isinstance(deploy, Deploy) else deploy
     assert len(deploy_hash) == 32, "Invalid deploy hash"
 
     return DeployApproval(
-        approver.as_public_key,
-        crypto.get_signature_for_deploy_approval(
-            deploy_hash, approver.private_key, approver.key_algo
-            )
+        approver.to_public_key(),
+        get_signature_for_deploy_approval(deploy_hash, approver)
     )
 
 
-def create_deploy_arguments(args: typing.Dict[str, CL_Value]) -> typing.List[DeployArgument]:
+def create_deploy_arguments(args: typing.Dict[str, CLV_Value]) -> typing.List[DeployArgument]:
     """Returns a collection of deploy arguments for interpretation by a node.
 
     :param args: Dictionary of argument name & cl-value pairs.
     :returns: A collection of deploy arguments for interpretation by a node.
 
     """
     return [DeployArgument(k, v) for (k, v) in args.items()]
@@ -106,15 +104,15 @@
     """Returns header information associated with a deploy.
 
     :param body: Deploy body, i.e. it's session/payment execution information.
     :param params: Standard parameters associated with a deploy.
 
     """
     return DeployHeader(
-        account_public_key=params.account_public_key,
+        account=params.account,
         body_hash=body.hash,
         chain_name=params.chain_name,
         dependencies=params.dependencies,
         gas_price=params.gas_price,
         timestamp=params.timestamp,
         ttl=params.ttl,
     )
@@ -142,59 +140,61 @@
         account if isinstance(account, PublicKey) else \
         create_public_key(account.algo, account.pbk)
     timestamp = timestamp or datetime.datetime.now(tz=datetime.timezone.utc).timestamp()
     timestamp = Timestamp(round(timestamp, 3))
     ttl = create_deploy_ttl(ttl) if isinstance(ttl, str) else ttl
 
     return DeployParameters(
-        account_public_key=public_key,
+        account=public_key,
         chain_name=chain_name,
         dependencies=dependencies,
         gas_price=gas_price,
         timestamp=timestamp,
         ttl=ttl,
     )
 
 
 def create_deploy_ttl(humanized_ttl: str = constants.DEFAULT_DEPLOY_TTL) -> DeployTimeToLive:
     """Returns a deploy's time to live after which it will not longer be accepted by a node.
 
     :param humanized_ttl: A humanized ttl, e.g. 2 hours.
 
     """
-    as_milliseconds = conversion.humanized_time_interval_to_milliseconds(humanized_ttl)
+    as_milliseconds = convertor.ms_from_humanized_time_interval(humanized_ttl)
     if as_milliseconds > constants.DEPLOY_TTL_MS_MAX:
-        raise ValueError(f"Invalid deploy ttl. Max = {constants.DEPLOY_TTL_MS_MAX}ms. Actual = {humanized_ttl}.")
+        raise ValueError(
+            f"Invalid deploy ttl. Max={constants.DEPLOY_TTL_MS_MAX}ms. Actual={humanized_ttl}."
+            )
 
     return DeployTimeToLive(
         humanized=humanized_ttl,
         as_milliseconds=as_milliseconds
     )
 
 
 def create_standard_payment(
     amount: int = constants.STANDARD_PAYMENT_FOR_NATIVE_TRANSFERS
-) -> ModuleBytes:
+) -> DeployOfModuleBytes:
     """Returns standard payment execution information.
 
     :param amount: Maximum amount in motes to be used for standard payment.
 
     """
-    return ModuleBytes(
+    return DeployOfModuleBytes(
         args={
-            "amount": CL_U512(amount)
+            "amount": CLV_U512(amount)
         },
         module_bytes=bytes([])
         )
 
 
 def create_transfer(
     params: DeployParameters,
     amount: int,
-    target: bytes,
+    target: AccountKey,
     correlation_id: int = None,
     payment: int = constants.STANDARD_PAYMENT_FOR_NATIVE_TRANSFERS
 ) -> Deploy:
     """Returns a native transfer deploy.
 
     :param params: Standard parameters used when creating a deploy.
     :param amount: Amount in motes to be transferred.
@@ -208,31 +208,31 @@
         create_standard_payment(payment),
         create_transfer_session(amount, target, correlation_id)
         )
 
 
 def create_transfer_session(
     amount: int,
-    target: bytes,
+    target: AccountKey,
     correlation_id: int = None,
-) -> Transfer:
+) -> DeployOfTransfer:
     """Returns session execution information for a native transfer.
 
     :param amount: Amount in motes to be transferred.
     :param target: Target account key.
     :param correlation_id: Identifier used to correlate transfer to internal systems.
     :returns: A native transfer session logic.
 
     """
     correlation_id = correlation_id or random.randint(1, constants.MAX_TRANSFER_ID)
-    return Transfer(
+    return DeployOfTransfer(
         args={
-            "amount": CL_U512(amount),
-            "target": CL_PublicKey.from_account_key(target),
-            "id": CL_Option(CL_U64(correlation_id), CL_Type_U64()),
+            "amount": CLV_U512(amount),
+            "target": convertor.clv_public_key_from_account_key(target),
+            "id": CLV_Option(CLV_U64(correlation_id), CLT_Type_U64()),
         }
     )
 
 
 def create_validator_auction_bid(
     params: DeployParameters,
     amount: int,
@@ -247,52 +247,52 @@
     :param delegation_rate: Percentage charged to a delegator for provided service.
     :param public_key: Public key of validator.
     :param path_to_wasm: Path to compiled delegate.wasm.
     :returns: A standard delegation deploy.
 
     """
     payment = create_standard_payment(constants.STANDARD_PAYMENT_FOR_AUCTION_BID)
-    session = ModuleBytes(
+    session = DeployOfModuleBytes(
         module_bytes=_io.read_wasm(path_to_wasm),
         args={
-            "amount": CL_U512(amount),
-            "delegation_rate": CL_U8(delegation_rate),
-            "public_key": CL_PublicKey.from_public_key(public_key),
+            "amount": CLV_U512(amount),
+            "delegation_rate": CLV_U8(delegation_rate),
+            "public_key": convertor.clv_public_key_from_public_key(public_key),
         }
     )
 
     return create_deploy(params, payment, session)
 
 
 def create_validator_auction_bid_withdrawal(
     params: DeployParameters,
     amount: int,
     public_key: PublicKey,
     path_to_wasm: str,
-    unbond_purse_ref: typing.Union[CL_URef, str],
+    unbond_purse_ref: typing.Union[CLV_URef, str],
 ) -> Deploy:
     """Returns an auction bid withdraw delegation deploy.
 
     :param params: Standard parameters used when creating a deploy.
     :param amount: Amount in motes to be withdrawn from auction.
     :param public_key: Public key of validator.
     :param path_to_wasm: Path to compiled delegate.wasm.
     :param unbond_purse_ref: Validator's purse unforgeable reference to which to withdraw funds.
     :returns: A standard delegation deploy.
 
     """
     payment = create_standard_payment(constants.STANDARD_PAYMENT_FOR_AUCTION_BID_WITHDRAWAL)
-    session = ModuleBytes(
+    session = DeployOfModuleBytes(
         module_bytes=_io.read_wasm(path_to_wasm),
         args={
-            "amount": CL_U512(amount),
-            "public_key": CL_PublicKey.from_public_key(public_key),
+            "amount": CLV_U512(amount),
+            "public_key": convertor.clv_public_key_from_public_key(public_key),
             "unbond_purse":
-                unbond_purse_ref if isinstance(unbond_purse_ref, CL_URef) else
-                CL_URef.from_string(unbond_purse_ref)
+                unbond_purse_ref if isinstance(unbond_purse_ref, CLV_URef) else
+                convertor.clv_uref_from_str(unbond_purse_ref)
         }
     )
 
     return create_deploy(params, payment, session)
 
 
 def create_validator_delegation(
@@ -309,28 +309,28 @@
     :param public_key_of_delegator: Public key of delegator.
     :param public_key_of_validator: Public key of validator.
     :param path_to_wasm: Path to compiled delegate.wasm.
     :returns: A standard delegation deploy.
 
     """
     payment = create_standard_payment(constants.STANDARD_PAYMENT_FOR_DELEGATION)
-    session = ModuleBytes(
+    session = DeployOfModuleBytes(
         module_bytes=_io.read_wasm(path_to_wasm),
         args=[
             DeployArgument(
                 "amount",
-                CL_U512(amount)
+                CLV_U512(amount)
                 ),
             DeployArgument(
                 "delegator",
-                CL_PublicKey.from_public_key(public_key_of_delegator)
+                convertor.clv_public_key_from_public_key(public_key_of_delegator)
                 ),
             DeployArgument(
                 "validator",
-                CL_PublicKey.from_public_key(public_key_of_validator)
+                convertor.clv_public_key_from_public_key(public_key_of_validator)
                 ),
         ]
     )
 
     return create_deploy(params, payment, session)
 
 
@@ -348,17 +348,17 @@
     :param public_key_of_delegator: Public key of delegator.
     :param public_key_of_validator: Public key of validator.
     :param path_to_wasm: Path to compiled delegate.wasm.
     :returns: A standard delegation deploy.
 
     """
     payment = create_standard_payment(constants.STANDARD_PAYMENT_FOR_DELEGATION_WITHDRAWAL)
-    session = ModuleBytes(
+    session = DeployOfModuleBytes(
         module_bytes=_io.read_wasm(path_to_wasm),
         args={
-            "amount": CL_U512(amount),
-            "delegator": CL_PublicKey.from_public_key(public_key_of_delegator),
-            "validator": CL_PublicKey.from_public_key(public_key_of_validator)
+            "amount": CLV_U512(amount),
+            "delegator": convertor.clv_public_key_from_public_key(public_key_of_delegator),
+            "validator": convertor.clv_public_key_from_public_key(public_key_of_validator)
         }
     )
 
     return create_deploy(params, payment, session)
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/binary/__init__.py` & `pycspr-1.2.0/pycspr/serializer/binary/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pycspr.serialisation.binary import cl_type as serialiser_of_cl_types
-from pycspr.serialisation.binary import cl_value as serialiser_of_cl_values
-from pycspr.serialisation.binary import entity as serialiser_of_entites
-from pycspr.types.cl_types import CL_Type
-from pycspr.types.cl_values import CL_Value
+from pycspr.serializer.binary import cl_type as cl_type_serialiser
+from pycspr.serializer.binary import cl_value as cl_value_serialiser
+from pycspr.serializer.binary import node_rpc as node_rpc_serialiser
+from pycspr.types.cl import CLT_Type
+from pycspr.types.cl import CLV_Value
 
 
 def to_bytes(entity: object) -> bytes:
-    if isinstance(entity, CL_Type):
-        return serialiser_of_cl_types.encode(entity)
-    elif isinstance(entity, CL_Value):
-        return serialiser_of_cl_values.encode(entity)
+    if isinstance(entity, CLT_Type):
+        return cl_type_serialiser.encode(entity)
+    elif isinstance(entity, CLV_Value):
+        return cl_value_serialiser.encode(entity)
     else:
-        return serialiser_of_entites.encode(entity)
+        return node_rpc_serialiser.encode(entity)
 
 
 def from_bytes(bstream: bytes, typedef: object = None) -> object:
     if isinstance(typedef, type(None)):
-        return serialiser_of_cl_types.decode(bstream)
-    elif isinstance(typedef, CL_Type):
-        return serialiser_of_cl_values.decode(bstream, typedef)
+        return cl_type_serialiser.decode(bstream)
+    elif isinstance(typedef, CLT_Type):
+        return cl_value_serialiser.decode(bstream, typedef)
     else:
-        return serialiser_of_entites.decode(bstream, typedef)
+        return node_rpc_serialiser.decode(bstream, typedef)
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/binary/cl_type/encoder.py` & `pycspr-1.2.0/pycspr/serializer/binary/cl_type/encoder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,50 @@
-from pycspr.serialisation.binary.cl_value import encode as encode_cl_value
-from pycspr.types import cl_types
-from pycspr.types import cl_values
-from pycspr.types import CL_TypeKey
+from pycspr.serializer.binary.cl_value import encode as encode_cl_value
+from pycspr.types.cl import CLT_Type
+from pycspr.types.cl import CLT_TypeKey
+from pycspr.types.cl import CLV_U32
 
 
-def encode(entity: cl_types.CL_Type) -> bytes:
+def encode(entity: CLT_Type) -> bytes:
     """Encoder: CL type -> an array of bytes.
 
     :param entity: A CL type to be encoded.
     :returns: An array of bytes.
 
     """
     if entity.type_key in _ENCODERS["simple"]:
         return bytes([entity.type_key.value]) + bytes([])
     elif entity.type_key in _ENCODERS["complex"]:
         return bytes([entity.type_key.value]) + _ENCODERS["complex"][entity.type_key](entity)
     else:
         raise ValueError("Unrecognized cl type")
 
 
-def _encode_byte_array(entity: cl_types.CL_Type_ByteArray):
-    return encode_cl_value(cl_values.CL_U32(entity.size))
-
-
-def _encode_list(entity: cl_types.CL_Type_List):
-    return encode(entity.inner_type)
-
-
-def _encode_map(entity: cl_types.CL_Type_Map):
-    return encode(entity.key_type) + encode(entity.value_type)
-
-
-def _encode_option(entity: cl_types.CL_Type_Option):
-    return encode(entity.inner_type)
-
-
-def _encode_tuple_1(entity: cl_types.CL_Type_Tuple1):
-    return encode(entity.t0_type)
-
-
-def _encode_tuple_2(entity: cl_types.CL_Type_Tuple1):
-    return encode(entity.t0_type) + encode(entity.t1_type)
-
-
-def _encode_tuple_3(entity: cl_types.CL_Type_Tuple1):
-    return encode(entity.t0_type) + encode(entity.t1_type) + encode(entity.t2_type)
-
-
 _ENCODERS: dict = {
     "complex": {
-        CL_TypeKey.BYTE_ARRAY: _encode_byte_array,
-        CL_TypeKey.LIST: _encode_list,
-        CL_TypeKey.MAP: _encode_map,
-        CL_TypeKey.OPTION: _encode_option,
-        CL_TypeKey.TUPLE_1: _encode_tuple_1,
-        CL_TypeKey.TUPLE_2: _encode_tuple_2,
-        CL_TypeKey.TUPLE_3: _encode_tuple_3,
+        CLT_TypeKey.BYTE_ARRAY: lambda x: encode_cl_value(CLV_U32(x.size)),
+        CLT_TypeKey.LIST: lambda x: encode(x.inner_type),
+        CLT_TypeKey.MAP: lambda x: encode(x.key_type) + encode(x.value_type),
+        CLT_TypeKey.OPTION: lambda x: encode(x.inner_type),
+        CLT_TypeKey.TUPLE_1: lambda x: encode(x.t0_type),
+        CLT_TypeKey.TUPLE_2: lambda x: encode(x.t0_type) + encode(x.t1_type),
+        CLT_TypeKey.TUPLE_3: lambda x: encode(x.t0_type) + encode(x.t1_type) + encode(x.t2_type),
     },
     "simple": {
-        CL_TypeKey.ANY,
-        CL_TypeKey.BOOL,
-        CL_TypeKey.I32,
-        CL_TypeKey.I64,
-        CL_TypeKey.KEY,
-        CL_TypeKey.PUBLIC_KEY,
-        CL_TypeKey.RESULT,
-        CL_TypeKey.STRING,
-        CL_TypeKey.U8,
-        CL_TypeKey.U32,
-        CL_TypeKey.U64,
-        CL_TypeKey.U128,
-        CL_TypeKey.U256,
-        CL_TypeKey.U512,
-        CL_TypeKey.UNIT,
-        CL_TypeKey.UREF,
+        CLT_TypeKey.ANY,
+        CLT_TypeKey.BOOL,
+        CLT_TypeKey.I32,
+        CLT_TypeKey.I64,
+        CLT_TypeKey.KEY,
+        CLT_TypeKey.PUBLIC_KEY,
+        CLT_TypeKey.RESULT,
+        CLT_TypeKey.STRING,
+        CLT_TypeKey.U8,
+        CLT_TypeKey.U32,
+        CLT_TypeKey.U64,
+        CLT_TypeKey.U128,
+        CLT_TypeKey.U256,
+        CLT_TypeKey.U512,
+        CLT_TypeKey.UNIT,
+        CLT_TypeKey.UREF,
     }
 }
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/binary/entity/decoder.py` & `pycspr-1.2.0/pycspr/serializer/binary/node_rpc/decoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import typing
 
-from pycspr.crypto import KeyAlgorithm
 from pycspr.factory import create_public_key
-from pycspr.serialisation.binary.cl_type import decode as decode_cl_type
-from pycspr.serialisation.binary.cl_value import decode as decode_cl_value
-from pycspr.types import Timestamp
-from pycspr.types import cl_types
-from pycspr.types import Deploy
-from pycspr.types import DeployApproval
-from pycspr.types import DeployArgument
-from pycspr.types import DeployBody
-from pycspr.types import DeployExecutableItem
-from pycspr.types import DeployHeader
-from pycspr.types import DeployTimeToLive
-from pycspr.types import ModuleBytes
-from pycspr.types import StoredContractByHash
-from pycspr.types import StoredContractByHashVersioned
-from pycspr.types import StoredContractByName
-from pycspr.types import StoredContractByNameVersioned
-from pycspr.types import Transfer
+from pycspr.serializer.binary.cl_type import decode as decode_cl_type
+from pycspr.serializer.binary.cl_value import decode as decode_cl_value
+from pycspr.types.cl import CLT_Type_ByteArray
+from pycspr.types.cl import CLT_Type_U32
+from pycspr.types.cl import CLT_Type_U64
+from pycspr.types.cl import CLT_Type_List
+from pycspr.types.cl import CLT_Type_PublicKey
+from pycspr.types.cl import CLT_Type_String
+from pycspr.types.crypto import KeyAlgorithm
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import DeployApproval
+from pycspr.types.node.rpc import DeployArgument
+from pycspr.types.node.rpc import DeployBody
+from pycspr.types.node.rpc import DeployExecutableItem
+from pycspr.types.node.rpc import DeployHeader
+from pycspr.types.node.rpc import DeployTimeToLive
+from pycspr.types.node.rpc import DeployOfModuleBytes
+from pycspr.types.node.rpc import DeployOfStoredContractByHash
+from pycspr.types.node.rpc import DeployOfStoredContractByHashVersioned
+from pycspr.types.node.rpc import DeployOfStoredContractByName
+from pycspr.types.node.rpc import DeployOfStoredContractByNameVersioned
+from pycspr.types.node.rpc import DeployOfTransfer
+from pycspr.types.node.rpc import Timestamp
+from pycspr.utils import convertor
 
 
 def decode(bstream: bytes, typedef: object) -> typing.Tuple[bytes, object]:
     """Decoder: Domain entity <- an array of bytes.
 
     :param bstream: An array of bytes being decoded.
     :param typedef: Deploy related type definition.
@@ -35,15 +41,15 @@
         raise ValueError(f"Cannot decode {typedef} from bytes")
     else:
         return decoder(bstream)
 
 
 def _decode_deploy(bstream: bytes) -> typing.Tuple[bytes, Deploy]:
     bstream, header = decode(bstream, DeployHeader)
-    bstream, deploy_hash = decode_cl_value(bstream, cl_types.CL_Type_ByteArray(32))
+    bstream, deploy_hash = decode_cl_value(bstream, CLT_Type_ByteArray(32))
     bstream, payment = decode(bstream, DeployExecutableItem)
     bstream, session = decode(bstream, DeployExecutableItem)
     bstream, approvals = _decode_deploy_approval_set(bstream)
 
     return bstream, Deploy(
         approvals=approvals,
         hash=deploy_hash.value,
@@ -71,189 +77,210 @@
     )
 
 
 def _decode_deploy_approval_set(
     bstream: bytes
 ) -> typing.Tuple[bytes, typing.List[DeployApproval]]:
     approvals = []
-    bstream, args_length = decode_cl_value(bstream, cl_types.CL_Type_U32())
+    bstream, args_length = decode_cl_value(bstream, CLT_Type_U32())
     for _ in range(args_length.value):
         bstream, approval = decode(bstream, DeployApproval)
         approvals.append(approval)
 
     return bstream, approvals
 
 
 def _decode_deploy_argument(bstream: bytes) -> typing.Tuple[bytes, DeployArgument]:
-    bstream, name = decode_cl_value(bstream, cl_types.CL_Type_String())
-    bstream, val_bytes_length = decode_cl_value(bstream, cl_types.CL_Type_U32())
+    bstream, name = decode_cl_value(bstream, CLT_Type_String())
+    bstream, val_bytes_length = decode_cl_value(bstream, CLT_Type_U32())
     bstream_rem, arg_cl_type = decode_cl_type(bstream[val_bytes_length.value:])
     _, arg_cl_value = decode_cl_value(bstream, arg_cl_type)
 
     return bstream_rem, DeployArgument(name.value, arg_cl_value)
 
 
 def _decode_deploy_argument_set(
     bstream: bytes
 ) -> typing.Tuple[bytes, typing.List[DeployArgument]]:
     args = []
-    bstream, args_length = decode_cl_value(bstream, cl_types.CL_Type_U32())
+    bstream, args_length = decode_cl_value(bstream, CLT_Type_U32())
     for _ in range(args_length.value):
         bstream, arg = decode(bstream, DeployArgument)
         args.append(arg)
 
     return bstream, args
 
 
 def _decode_deploy_body(bstream: bytes) -> typing.Tuple[bytes, DeployBody]:
     bstream, payment = _decode_deploy_executable_item(bstream)
     bstream, session = _decode_deploy_executable_item(bstream)
-    bstream, body_hash = decode_cl_value(bstream, cl_types.CL_Type_ByteArray(32))
+    bstream, body_hash = decode_cl_value(bstream, CLT_Type_ByteArray(32))
 
     return bstream, DeployBody(payment, session, body_hash.value)
 
 
 def _decode_deploy_executable_item(bstream: bytes) -> DeployExecutableItem:
     if bstream[0] == 0:
-        return decode(bstream, ModuleBytes)
+        return decode(bstream, DeployOfModuleBytes)
     elif bstream[0] == 1:
-        return decode(bstream, StoredContractByHash)
+        return decode(bstream, DeployOfStoredContractByHash)
     elif bstream[0] == 2:
-        return decode(bstream, StoredContractByHashVersioned)
+        return decode(bstream, DeployOfStoredContractByHashVersioned)
     elif bstream[0] == 3:
-        return decode(bstream, StoredContractByName)
+        return decode(bstream, DeployOfStoredContractByName)
     elif bstream[0] == 4:
-        return decode(bstream, StoredContractByNameVersioned)
+        return decode(bstream, DeployOfStoredContractByNameVersioned)
     elif bstream[0] == 5:
-        return decode(bstream, Transfer)
+        return decode(bstream, DeployOfTransfer)
 
     raise ValueError("Invalid deploy executable item type tag")
 
 
 def _decode_deploy_header(bstream: bytes) -> typing.Tuple[bytes, DeployHeader]:
     bstream, account_public_key = decode_cl_value(
-        bstream, cl_types.CL_Type_PublicKey()
-        )
-    bstream, timestamp = decode_cl_value(
-        bstream, cl_types.CL_Type_U64()
-        )
-    bstream, ttl = decode_cl_value(
-        bstream, cl_types.CL_Type_U64()
+        bstream, CLT_Type_PublicKey()
         )
+    bstream, timestamp = decode(bstream, Timestamp)
+    bstream, ttl = decode(bstream, DeployTimeToLive)
     bstream, gas_price = decode_cl_value(
-        bstream, cl_types.CL_Type_U64()
+        bstream, CLT_Type_U64()
         )
     bstream, body_hash = decode_cl_value(
-        bstream, cl_types.CL_Type_ByteArray(32)
+        bstream, CLT_Type_ByteArray(32)
         )
     bstream, dependencies = decode_cl_value(
-        bstream, cl_types.CL_Type_List(cl_types.CL_Type_ByteArray(32))
+        bstream, CLT_Type_List(CLT_Type_ByteArray(32))
         )
     bstream, chain_name = decode_cl_value(
-        bstream, cl_types.CL_Type_String()
+        bstream, CLT_Type_String()
         )
 
     return bstream, DeployHeader(
-        account_public_key=account_public_key,
+        account=account_public_key,
         body_hash=body_hash.value,
         chain_name=chain_name.value,
         dependencies=dependencies.vector,
         gas_price=gas_price.value,
-        timestamp=Timestamp(timestamp.value / 1000),
-        ttl=DeployTimeToLive.from_milliseconds(ttl.value)
+        timestamp=timestamp,
+        ttl=ttl
     )
 
 
-def _decode_module_bytes(bstream: bytes) -> typing.Tuple[bytes, ModuleBytes]:
+def _decode_deploy_time_to_live(bstream: bytes) -> typing.Tuple[bytes, DeployTimeToLive]:
+    bstream, ttl = decode_cl_value(
+        bstream, CLT_Type_U64()
+        )
+
+    return bstream, DeployTimeToLive(
+        ttl.value,
+        convertor.humanized_time_interval_from_ms(ttl.value)
+        )
+
+
+def _decode_module_bytes(bstream: bytes) -> typing.Tuple[bytes, DeployOfModuleBytes]:
     bstream = bstream[1:]
-    bstream, length = decode_cl_value(bstream, cl_types.CL_Type_U32())
+    bstream, length = decode_cl_value(bstream, CLT_Type_U32())
     if length.value > 0:
         module_bytes = bstream[:length.value]
         bstream = bstream[length.value:]
     else:
         module_bytes = bytes([])
     bstream, args = _decode_deploy_argument_set(bstream)
 
-    return bstream, ModuleBytes(args, module_bytes)
+    return bstream, DeployOfModuleBytes(args, module_bytes)
 
 
-def _decode_stored_contract_by_hash(bstream: bytes) -> typing.Tuple[bytes, StoredContractByHash]:
+def _decode_stored_contract_by_hash(
+    bstream: bytes
+) -> typing.Tuple[bytes, DeployOfStoredContractByHash]:
     bstream = bstream[1:]
-    bstream, contract_hash = decode_cl_value(bstream, cl_types.CL_Type_ByteArray(32))
-    bstream, entry_point = decode_cl_value(bstream, cl_types.CL_Type_String())
+    bstream, contract_hash = decode_cl_value(bstream, CLT_Type_ByteArray(32))
+    bstream, entry_point = decode_cl_value(bstream, CLT_Type_String())
     bstream, args = _decode_deploy_argument_set(bstream)
 
-    return bstream, StoredContractByHash(
+    return bstream, DeployOfStoredContractByHash(
         args=args,
         entry_point=entry_point.value,
         hash=contract_hash.value
         )
 
 
 def _decode_stored_contract_by_hash_versioned(
     bstream: bytes
-) -> typing.Tuple[bytes, StoredContractByHashVersioned]:
+) -> typing.Tuple[bytes, DeployOfStoredContractByHashVersioned]:
     bstream = bstream[1:]
-    bstream, contract_hash = decode_cl_value(bstream, cl_types.CL_Type_ByteArray(32))
-    bstream, contract_version = decode_cl_value(bstream, cl_types.CL_Type_U32())
-    bstream, entry_point = decode_cl_value(bstream, cl_types.CL_Type_String())
+    bstream, contract_hash = decode_cl_value(bstream, CLT_Type_ByteArray(32))
+    bstream, contract_version = decode_cl_value(bstream, CLT_Type_U32())
+    bstream, entry_point = decode_cl_value(bstream, CLT_Type_String())
     bstream, args = _decode_deploy_argument_set(bstream)
 
-    return bstream, StoredContractByHashVersioned(
+    return bstream, DeployOfStoredContractByHashVersioned(
         args=args,
         entry_point=entry_point.value,
         hash=contract_hash.value,
         version=contract_version.value
         )
 
 
-def _decode_stored_contract_by_name(bstream: bytes) -> typing.Tuple[bytes, StoredContractByName]:
+def _decode_stored_contract_by_name(
+    bstream: bytes
+) -> typing.Tuple[bytes, DeployOfStoredContractByName]:
     bstream = bstream[1:]
-    bstream, contract_name = decode_cl_value(bstream, cl_types.CL_Type_String())
-    bstream, entry_point = decode_cl_value(bstream, cl_types.CL_Type_String())
+    bstream, contract_name = decode_cl_value(bstream, CLT_Type_String())
+    bstream, entry_point = decode_cl_value(bstream, CLT_Type_String())
     bstream, args = _decode_deploy_argument_set(bstream)
 
-    return bstream, StoredContractByName(
+    return bstream, DeployOfStoredContractByName(
         args=args,
         entry_point=entry_point.value,
         name=contract_name.value
         )
 
 
 def _decode_stored_contract_by_name_versioned(
     bstream: bytes
-) -> typing.Tuple[bytes, StoredContractByNameVersioned]:
+) -> typing.Tuple[bytes, DeployOfStoredContractByNameVersioned]:
     bstream = bstream[1:]
-    bstream, contract_name = decode_cl_value(bstream, cl_types.CL_Type_String())
-    bstream, contract_version = decode_cl_value(bstream, cl_types.CL_Type_U32())
-    bstream, entry_point = decode_cl_value(bstream, cl_types.CL_Type_String())
+    bstream, contract_name = decode_cl_value(bstream, CLT_Type_String())
+    bstream, contract_version = decode_cl_value(bstream, CLT_Type_U32())
+    bstream, entry_point = decode_cl_value(bstream, CLT_Type_String())
     bstream, args = _decode_deploy_argument_set(bstream)
 
-    return bstream, StoredContractByNameVersioned(
+    return bstream, DeployOfStoredContractByNameVersioned(
         args=args,
         entry_point=entry_point.value,
         name=contract_name.value,
         version=contract_version.value
         )
 
 
-def _decode_transfer(bstream: bytes) -> typing.Tuple[bytes, Transfer]:
+def _decode_timestamp(bstream: bytes) -> typing.Tuple[bytes, Timestamp]:
+    bstream, ts_ns = decode_cl_value(
+        bstream, CLT_Type_U64()
+        )
+
+    return bstream, Timestamp(ts_ns.value / 1000)
+
+
+def _decode_transfer(bstream: bytes) -> typing.Tuple[bytes, DeployOfTransfer]:
     bstream = bstream[1:]
     bstream, args = _decode_deploy_argument_set(bstream)
 
-    return bstream, Transfer(args)
+    return bstream, DeployOfTransfer(args)
 
 
 _DECODERS = {
     Deploy: _decode_deploy,
     DeployApproval: _decode_deploy_approval,
     DeployArgument: _decode_deploy_argument,
     DeployBody: _decode_deploy_body,
     DeployExecutableItem: _decode_deploy_executable_item,
     DeployHeader: _decode_deploy_header,
-    ModuleBytes: _decode_module_bytes,
-    StoredContractByHash: _decode_stored_contract_by_hash,
-    StoredContractByHashVersioned: _decode_stored_contract_by_hash_versioned,
-    StoredContractByName: _decode_stored_contract_by_name,
-    StoredContractByNameVersioned: _decode_stored_contract_by_name_versioned,
-    Transfer: _decode_transfer
+    DeployOfModuleBytes: _decode_module_bytes,
+    DeployOfStoredContractByHash: _decode_stored_contract_by_hash,
+    DeployOfStoredContractByHashVersioned: _decode_stored_contract_by_hash_versioned,
+    DeployOfStoredContractByName: _decode_stored_contract_by_name,
+    DeployOfStoredContractByNameVersioned: _decode_stored_contract_by_name_versioned,
+    DeployOfTransfer: _decode_transfer,
+    DeployTimeToLive: _decode_deploy_time_to_live,
+    Timestamp: _decode_timestamp,
 }
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/binary/entity/encoder.py` & `pycspr-1.2.0/pycspr/serializer/binary/node_rpc/encoder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import typing
 
-from pycspr.serialisation.binary.cl_type import encode as encode_cl_type
-from pycspr.serialisation.binary.cl_value import encode as encode_cl_value
-from pycspr.serialisation.utils import cl_value_to_cl_type
-from pycspr.types import cl_values
-from pycspr.types.deploys import Deploy
-from pycspr.types.deploys import DeployApproval
-from pycspr.types.deploys import DeployArgument
-from pycspr.types.deploys import DeployBody
-from pycspr.types.deploys import DeployHeader
-from pycspr.types.deploys import ModuleBytes
-from pycspr.types.deploys import StoredContractByHash
-from pycspr.types.deploys import StoredContractByHashVersioned
-from pycspr.types.deploys import StoredContractByName
-from pycspr.types.deploys import StoredContractByNameVersioned
-from pycspr.types.deploys import Transfer
+from pycspr.serializer.binary.cl_type import encode as encode_cl_type
+from pycspr.serializer.binary.cl_value import encode as encode_cl_value
+from pycspr.serializer.utils import cl_value_to_cl_type
+from pycspr.types.cl import CLV_ByteArray
+from pycspr.types.cl import CLV_U32
+from pycspr.types.cl import CLV_U64
+from pycspr.types.cl import CLV_List
+from pycspr.types.cl import CLV_String
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import DeployApproval
+from pycspr.types.node.rpc import DeployArgument
+from pycspr.types.node.rpc import DeployBody
+from pycspr.types.node.rpc import DeployHeader
+from pycspr.types.node.rpc import DeployOfModuleBytes
+from pycspr.types.node.rpc import DeployOfStoredContractByHash
+from pycspr.types.node.rpc import DeployOfStoredContractByHashVersioned
+from pycspr.types.node.rpc import DeployOfStoredContractByName
+from pycspr.types.node.rpc import DeployOfStoredContractByNameVersioned
+from pycspr.types.node.rpc import DeployOfTransfer
+from pycspr.utils import convertor
 
 
 def encode(entity: object) -> bytes:
     """Encoder: Domain entity -> an array of bytes.
 
     :param entity: A deploy related type instance to be encoded.
     :returns: An array of bytes.
@@ -47,119 +52,123 @@
         return entity.signer + entity.signature
     else:
         return entity.signer.account_key + entity.signature
 
 
 def _encode_deploy_approval_set(entities: typing.List[DeployApproval]) -> bytes:
     return \
-        encode_cl_value(cl_values.CL_U32(len(entities))) + \
+        encode_cl_value(CLV_U32(len(entities))) + \
         bytes([i for j in map(encode, entities) for i in j])
 
 
 def _encode_deploy_argument(entity: DeployArgument) -> bytes:
     return \
-        encode_cl_value(cl_values.CL_String(entity.name)) + \
+        encode_cl_value(CLV_String(entity.name)) + \
         _u8_array_to_bytes(encode_cl_value(entity.value)) + \
         encode_cl_type(cl_value_to_cl_type(entity.value))
 
 
 def _encode_deploy_body(entity: DeployBody) -> bytes:
     return encode(entity.payment) + encode(entity.session) + entity.hash
 
 
 def _encode_deploy_header(entity: DeployHeader) -> bytes:
     result = bytes([])
     result += encode_cl_value(
-        cl_values.CL_PublicKey.from_public_key(entity.account_public_key)
+        convertor.clv_public_key_from_public_key(entity.account)
     )
     result += encode_cl_value(
-        cl_values.CL_U64(int(entity.timestamp.value * 1000))
+        CLV_U64(int(entity.timestamp.value * 1000))
     )
     result += encode_cl_value(
-        cl_values.CL_U64(entity.ttl.as_milliseconds)
+        CLV_U64(entity.ttl.as_milliseconds)
     )
     result += encode_cl_value(
-        cl_values.CL_U64(entity.gas_price)
+        CLV_U64(entity.gas_price)
     )
     result += encode_cl_value(
-        cl_values.CL_ByteArray(entity.body_hash)
+        CLV_ByteArray(entity.body_hash)
     )
     result += encode_cl_value(
-        cl_values.CL_List(entity.dependencies)
+        CLV_List(entity.dependencies)
     )
     result += encode_cl_value(
-        cl_values.CL_String(entity.chain_name)
+        CLV_String(entity.chain_name)
     )
 
     return result
 
 
-def _encode_module_bytes(entity: ModuleBytes) -> bytes:
+def _encode_module_bytes(entity: DeployOfModuleBytes) -> bytes:
     return \
         bytes([0]) + \
         _u8_array_to_bytes(list(entity.module_bytes)) + \
         _vector_to_bytes(list(map(encode, entity.arguments)))
 
 
-def _encode_stored_contract_by_hash(entity: StoredContractByHash) -> bytes:
+def _encode_stored_contract_by_hash(entity: DeployOfStoredContractByHash) -> bytes:
     return \
         bytes([1]) + \
-        encode_cl_value(cl_values.CL_ByteArray(entity.hash)) + \
-        encode_cl_value(cl_values.CL_String(entity.entry_point)) + \
+        encode_cl_value(CLV_ByteArray(entity.hash)) + \
+        encode_cl_value(CLV_String(entity.entry_point)) + \
         _vector_to_bytes(list(map(encode, entity.arguments)))
 
 
-def _encode_stored_contract_by_hash_versioned(entity: StoredContractByHashVersioned) -> bytes:
+def _encode_stored_contract_by_hash_versioned(
+    entity: DeployOfStoredContractByHashVersioned
+) -> bytes:
     return \
         bytes([2]) + \
-        encode_cl_value(cl_values.CL_ByteArray(entity.hash)) + \
-        encode_cl_value(cl_values.CL_U32(entity.version)) + \
-        encode_cl_value(cl_values.CL_String(entity.entry_point)) + \
+        encode_cl_value(CLV_ByteArray(entity.hash)) + \
+        encode_cl_value(CLV_U32(entity.version)) + \
+        encode_cl_value(CLV_String(entity.entry_point)) + \
         _vector_to_bytes(list(map(encode, entity.arguments)))
 
 
-def _encode_stored_contract_by_name(entity: StoredContractByName) -> bytes:
+def _encode_stored_contract_by_name(entity: DeployOfStoredContractByName) -> bytes:
     return \
         bytes([3]) + \
-        encode_cl_value(cl_values.CL_String(entity.name)) + \
-        encode_cl_value(cl_values.CL_String(entity.entry_point)) + \
+        encode_cl_value(CLV_String(entity.name)) + \
+        encode_cl_value(CLV_String(entity.entry_point)) + \
         _vector_to_bytes(list(map(encode, entity.arguments)))
 
 
-def _encode_stored_contract_by_name_versioned(entity: StoredContractByNameVersioned) -> bytes:
+def _encode_stored_contract_by_name_versioned(
+    entity: DeployOfStoredContractByNameVersioned
+) -> bytes:
     return \
         bytes([4]) + \
-        encode_cl_value(cl_values.CL_String(entity.name)) + \
-        encode_cl_value(cl_values.CL_U32(entity.version)) + \
-        encode_cl_value(cl_values.CL_String(entity.entry_point)) + \
+        encode_cl_value(CLV_String(entity.name)) + \
+        encode_cl_value(CLV_U32(entity.version)) + \
+        encode_cl_value(CLV_String(entity.entry_point)) + \
         _vector_to_bytes(list(map(encode, entity.arguments)))
 
 
-def _encode_transfer(entity: Transfer) -> bytes:
+def _encode_transfer(entity: DeployOfTransfer) -> bytes:
     return \
         bytes([5]) + \
         _vector_to_bytes(list(map(encode, entity.arguments)))
 
 
 def _u8_array_to_bytes(value: typing.List[int]) -> bytes:
-    return encode_cl_value(cl_values.CL_U32(len(value))) + bytes(value)
+    return encode_cl_value(CLV_U32(len(value))) + bytes(value)
 
 
 def _vector_to_bytes(value: typing.List) -> bytes:
     return \
-        encode_cl_value(cl_values.CL_U32(len(value))) + \
+        encode_cl_value(CLV_U32(len(value))) + \
         bytes([i for j in value for i in j])
 
 
 _ENCODERS = {
     Deploy: _encode_deploy,
     DeployApproval: _encode_deploy_approval,
     DeployArgument: _encode_deploy_argument,
     DeployBody: _encode_deploy_body,
     DeployHeader: _encode_deploy_header,
-    ModuleBytes: _encode_module_bytes,
-    StoredContractByHash: _encode_stored_contract_by_hash,
-    StoredContractByHashVersioned: _encode_stored_contract_by_hash_versioned,
-    StoredContractByName: _encode_stored_contract_by_name,
-    StoredContractByNameVersioned: _encode_stored_contract_by_name_versioned,
-    Transfer: _encode_transfer,
+    DeployOfModuleBytes: _encode_module_bytes,
+    DeployOfStoredContractByHash: _encode_stored_contract_by_hash,
+    DeployOfStoredContractByHashVersioned: _encode_stored_contract_by_hash_versioned,
+    DeployOfStoredContractByName: _encode_stored_contract_by_name,
+    DeployOfStoredContractByNameVersioned: _encode_stored_contract_by_name_versioned,
+    DeployOfTransfer: _encode_transfer,
 }
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/json/__init__.py` & `pycspr-1.2.0/pycspr/serializer/json/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import typing
 
-from pycspr.serialisation.json import cl_type as serializer_of_cl_types
-from pycspr.serialisation.json import cl_value as serializer_of_cl_values
-from pycspr.serialisation.json import entity as serializer_of_entities
-from pycspr.types.cl_types import CL_Type
-from pycspr.types.cl_values import CL_Value
+from pycspr.serializer.json import cl_type as serializer_of_cl_types
+from pycspr.serializer.json import cl_value as serializer_of_cl_values
+from pycspr.serializer.json import node_rpc as serializer_of_entities
+from pycspr.types.cl import CLT_Type
+from pycspr.types.cl import CLV_Value
 
 
 def to_json(entity: object) -> typing.Union[str, dict]:
-    if isinstance(entity, CL_Type):
+    if isinstance(entity, CLT_Type):
         return serializer_of_cl_types.encode(entity)
-    elif isinstance(entity, CL_Value):
+    elif isinstance(entity, CLV_Value):
         return serializer_of_cl_values.encode(entity)
     else:
         return serializer_of_entities.encode(entity)
 
 
 def from_json(obj: dict, typedef: object = None) -> object:
     if isinstance(typedef, type(None)):
         return serializer_of_cl_types.decode(obj)
-    elif issubclass(typedef, CL_Value):
+    elif issubclass(typedef, CLV_Value):
         return serializer_of_cl_values.decode(obj)
     else:
         return serializer_of_entities.decode(obj, typedef)
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/json/cl_value/encoder.py` & `pycspr-1.2.0/pycspr/serializer/json/cl_value/encoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pycspr.crypto import cl_checksum
-from pycspr.serialisation.binary.cl_value import encode as encode_cl_value
-from pycspr.serialisation.json.cl_type import encode as encode_cl_type
-from pycspr.serialisation.utils import cl_value_to_cl_type
-from pycspr.serialisation.utils import cl_value_to_parsed
-from pycspr.types import cl_values
+from pycspr.crypto import checksummer
+from pycspr.serializer.binary.cl_value import encode as encode_cl_value
+from pycspr.serializer.json.cl_type import encode as encode_cl_type
+from pycspr.serializer.utils import cl_value_to_cl_type
+from pycspr.serializer.utils import cl_value_to_parsed
+from pycspr.types.cl import CLV_Value
 
 
-def encode(entity: cl_values.CL_Value) -> dict:
+def encode(entity: CLV_Value) -> dict:
     """Encoder: CL value -> JSON blob.
 
     :param entity: A CL value to be encoded.
     :returns: A JSON compatible dictionary.
 
     """
     return {
         "cl_type": encode_cl_type(cl_value_to_cl_type(entity)),
-        "bytes": cl_checksum.encode(encode_cl_value(entity)),
+        "bytes": checksummer.encode_bytes(encode_cl_value(entity)),
         "parsed": cl_value_to_parsed(entity)
     }
```

### Comparing `pycspr-1.1.3/pycspr/serialisation/json/entity/encoder.py` & `pycspr-1.2.0/pycspr/serializer/json/node_rpc/encoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import typing
 
-from pycspr.crypto import cl_checksum
-from pycspr.serialisation.json.cl_value import encode as encode_cl_value
-from pycspr.types.cl_values import CL_Value
-from pycspr.types.deploys import Deploy
-from pycspr.types.deploys import DeployApproval
-from pycspr.types.deploys import DeployArgument
-from pycspr.types.deploys import DeployHeader
-from pycspr.types.deploys import ModuleBytes
-from pycspr.types.deploys import StoredContractByHash
-from pycspr.types.deploys import StoredContractByHashVersioned
-from pycspr.types.deploys import StoredContractByName
-from pycspr.types.deploys import StoredContractByNameVersioned
-from pycspr.types.deploys import Transfer
+from pycspr.crypto import checksummer
+from pycspr.serializer.json.cl_value import encode as encode_cl_value
+from pycspr.types.node.rpc import Deploy
+from pycspr.types.node.rpc import DeployHeader
+from pycspr.types.cl import CLV_Value
+from pycspr.types.node.rpc import DeployApproval
+from pycspr.types.node.rpc import DeployArgument
+from pycspr.types.node.rpc import DeployOfModuleBytes
+from pycspr.types.node.rpc import DeployOfStoredContractByHash
+from pycspr.types.node.rpc import DeployOfStoredContractByHashVersioned
+from pycspr.types.node.rpc import DeployOfStoredContractByName
+from pycspr.types.node.rpc import DeployOfStoredContractByNameVersioned
+from pycspr.types.node.rpc import DeployOfTransfer
+from pycspr.utils import convertor
 
 
 def encode(entity: object) -> dict:
     """Encoder: Domain entity instance -> JSON blob.
 
     :param entity: A deploy related type instance to be encoded.
     :returns: A JSON compatible dictionary.
@@ -29,108 +30,112 @@
     else:
         return encoder(entity)
 
 
 def _encode_deploy(entity: Deploy) -> dict:
     return {
         "approvals": [encode(i) for i in entity.approvals],
-        "hash": cl_checksum.encode_digest(entity.hash),
+        "hash": checksummer.encode_digest(entity.hash),
         "header": encode(entity.header),
         "payment": encode(entity.payment),
         "session": encode(entity.session)
     }
 
 
 def _encode_deploy_approval(entity: DeployApproval) -> dict:
     return {
-        "signature": cl_checksum.encode_signature(entity.signature),
-        "signer": cl_checksum.encode_account_key(entity.signer.account_key)
+        "signature": checksummer.encode_signature(entity.signature),
+        "signer": checksummer.encode_account_key(entity.signer.account_key)
     }
 
 
-def _encode_deploy_argument(entity: DeployArgument) -> typing.Tuple[str, CL_Value]:
+def _encode_deploy_argument(entity: DeployArgument) -> typing.Tuple[str, CLV_Value]:
     return (entity.name, encode_cl_value(entity.value))
 
 
 def _encode_deploy_header(entity: DeployHeader) -> dict:
     return {
-        "account": cl_checksum.encode_account_key(entity.account_public_key.account_key),
-        "body_hash": cl_checksum.encode_digest(entity.body_hash),
+        "account": checksummer.encode_account_key(entity.account.account_key),
+        "body_hash": checksummer.encode_digest(entity.body_hash),
         "chain_name": entity.chain_name,
         "dependencies": entity.dependencies,
         "gas_price": entity.gas_price,
-        "timestamp": entity.timestamp.to_string(),
-        "ttl": entity.ttl.to_string()
+        "timestamp": convertor.iso_datetime_from_timestamp(entity.timestamp.value),
+        "ttl": entity.ttl.humanized
     }
 
 
-def _encode_module_bytes(entity: ModuleBytes) -> dict:
+def _encode_module_bytes(entity: DeployOfModuleBytes) -> dict:
     return {
         "ModuleBytes": {
             "args": [encode(i) for i in entity.arguments],
-            "module_bytes": cl_checksum.encode(entity.module_bytes)
+            "module_bytes": checksummer.encode_bytes(entity.module_bytes)
         }
     }
 
 
-def _encode_stored_contract_by_hash(entity: StoredContractByHash) -> dict:
+def _encode_stored_contract_by_hash(entity: DeployOfStoredContractByHash) -> dict:
     return {
         "StoredContractByHash": {
             "args": [encode(i) for i in entity.arguments],
             "entry_point": entity.entry_point,
-            "hash": cl_checksum.encode(entity.hash)
+            "hash": checksummer.encode_bytes(entity.hash)
         }
     }
 
 
-def _encode_stored_contract_by_hash_versioned(entity: StoredContractByHashVersioned) -> dict:
+def _encode_stored_contract_by_hash_versioned(
+    entity: DeployOfStoredContractByHashVersioned
+) -> dict:
     return {
-        "StoredContractByHashVersioned": {
+        "StoredVersionedContractByHash": {
             "args": [encode(i) for i in entity.arguments],
             "entry_point": entity.entry_point,
-            "hash": cl_checksum.encode(entity.hash),
+            "hash": checksummer.encode_bytes(entity.hash),
             "version": entity.version
         }
     }
 
 
-def _encode_stored_contract_by_name(entity: StoredContractByName) -> dict:
+def _encode_stored_contract_by_name(entity: DeployOfStoredContractByName) -> dict:
     return {
         "StoredContractByName": {
             "args": [encode(i) for i in entity.arguments],
             "entry_point": entity.entry_point,
             "name": entity.name
         }
     }
 
 
-def _encode_stored_contract_by_name_versioned(entity: StoredContractByNameVersioned) -> dict:
+def _encode_stored_contract_by_name_versioned(
+    entity: DeployOfStoredContractByNameVersioned
+) -> dict:
     return {
-        "StoredContractByNameVersioned": {
+        "StoredVersionedContractByName": {
             "args": [encode(i) for i in entity.arguments],
             "entry_point": entity.entry_point,
             "name": entity.name,
             "version": entity.version
         }
     }
 
 
-def _encode_transfer(entity: Transfer) -> dict:
+def _encode_transfer(entity: DeployOfTransfer) -> dict:
     return {
         "Transfer": {
             "args": [encode(i) for i in entity.arguments],
         }
     }
 
 
 _ENCODERS = {
     Deploy: _encode_deploy,
     DeployApproval: _encode_deploy_approval,
     DeployArgument: _encode_deploy_argument,
     DeployHeader: _encode_deploy_header,
-    ModuleBytes: _encode_module_bytes,
-    StoredContractByHash: _encode_stored_contract_by_hash,
-    StoredContractByHashVersioned: _encode_stored_contract_by_hash_versioned,
-    StoredContractByName: _encode_stored_contract_by_name,
-    StoredContractByNameVersioned: _encode_stored_contract_by_name_versioned,
-    Transfer: _encode_transfer,
+    DeployOfModuleBytes: _encode_module_bytes,
+    DeployOfStoredContractByHash: _encode_stored_contract_by_hash,
+    DeployOfStoredContractByHashVersioned: _encode_stored_contract_by_hash_versioned,
+    DeployOfStoredContractByName: _encode_stored_contract_by_name,
+    DeployOfStoredContractByNameVersioned: _encode_stored_contract_by_name_versioned,
+    DeployOfTransfer: _encode_transfer,
 }
```

### Comparing `pycspr-1.1.3/pycspr/types/cl_types.py` & `pycspr-1.2.0/pycspr/types/cl/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 import enum
 
 
-class CL_TypeKey(enum.Enum):
+class CLT_TypeKey(enum.Enum):
     """Enumeration over set of CL type keys.
 
     """
     ANY = 21
     BOOL = 0
     BYTE_ARRAY = 15
     I32 = 1
@@ -28,281 +28,281 @@
     U256 = 7
     U512 = 8
     UNIT = 9
     UREF = 12
 
 
 @dataclasses.dataclass
-class CL_Type():
+class CLT_Type():
     """Base class encapsulating CL type information associated with a value.
 
     """
     def __eq__(self, other) -> bool:
         return self.type_key == other.type_key
 
 
 @dataclasses.dataclass
-class CL_Type_Any(CL_Type):
+class CLT_Type_Any(CLT_Type):
     """Encapsulates CL type information associated with any value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.ANY
+    type_key: CLT_TypeKey = CLT_TypeKey.ANY
 
 
 @dataclasses.dataclass
-class CL_Type_Bool(CL_Type):
+class CLT_Type_Bool(CLT_Type):
     """Encapsulates CL type information associated with a Boolean value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.BOOL
+    type_key: CLT_TypeKey = CLT_TypeKey.BOOL
 
 
 @dataclasses.dataclass
-class CL_Type_ByteArray(CL_Type):
+class CLT_Type_ByteArray(CLT_Type):
     """Encapsulates CL type information associated with a byte array value.
 
     """
     # Size of associated byte array value.
     size: int
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.BYTE_ARRAY
+    type_key: CLT_TypeKey = CLT_TypeKey.BYTE_ARRAY
 
     def __eq__(self, other) -> bool:
         return self.type_key == other.type_key and self.size == other.size
 
 
 @dataclasses.dataclass
-class CL_Type_I32(CL_Type):
+class CLT_Type_I32(CLT_Type):
     """Encapsulates CL type information associated with a I32 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.I32
+    type_key: CLT_TypeKey = CLT_TypeKey.I32
 
 
 @dataclasses.dataclass
-class CL_Type_I64(CL_Type):
+class CLT_Type_I64(CLT_Type):
     """Encapsulates CL type information associated with a I64 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.I64
+    type_key: CLT_TypeKey = CLT_TypeKey.I64
 
 
 @dataclasses.dataclass
-class CL_Type_Key(CL_Type):
+class CLT_Type_Key(CLT_Type):
     """Encapsulates CL type information associated with a key value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.KEY
+    type_key: CLT_TypeKey = CLT_TypeKey.KEY
 
 
 @dataclasses.dataclass
-class CL_Type_List(CL_Type):
+class CLT_Type_List(CLT_Type):
     """Encapsulates CL type information associated with a list value.
 
     """
     # Inner type within CSPR type system.
-    inner_type: CL_Type
+    inner_type: CLT_Type
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.LIST
+    type_key: CLT_TypeKey = CLT_TypeKey.LIST
 
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and self.inner_type == other.inner_type
 
 
 @dataclasses.dataclass
-class CL_Type_Map(CL_Type):
+class CLT_Type_Map(CLT_Type):
     """Encapsulates CL type information associated with a byte array value.
 
     """
     # Type info of map's key.
-    key_type: CL_Type
+    key_type: CLT_Type
 
     # Type info of map's value.
-    value_type: CL_Type
+    value_type: CLT_Type
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.MAP
+    type_key: CLT_TypeKey = CLT_TypeKey.MAP
 
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and \
                self.key_type == other.key_type and \
                self.value_type == other.value_type
 
 
 @dataclasses.dataclass
-class CL_Type_Option(CL_Type):
+class CLT_Type_Option(CLT_Type):
     """Encapsulates CL type information associated with an optional value.
 
     """
     # Inner type within CSPR type system.
-    inner_type: CL_Type
+    inner_type: CLT_Type
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.OPTION
+    type_key: CLT_TypeKey = CLT_TypeKey.OPTION
 
     def __eq__(self, other) -> bool:
         return self.type_key == other.type_key and self.inner_type == other.inner_type
 
 
 @dataclasses.dataclass
-class CL_Type_PublicKey(CL_Type):
+class CLT_Type_PublicKey(CLT_Type):
     """Encapsulates CL type information associated with a PublicKey value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.PUBLIC_KEY
+    type_key: CLT_TypeKey = CLT_TypeKey.PUBLIC_KEY
 
 
 @dataclasses.dataclass
-class CL_Type_Result(CL_Type):
+class CLT_Type_Result(CLT_Type):
     """Encapsulates CL type information associated with a result value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.RESULT
+    type_key: CLT_TypeKey = CLT_TypeKey.RESULT
 
 
 @dataclasses.dataclass
-class CL_Type_String(CL_Type):
+class CLT_Type_String(CLT_Type):
     """Encapsulates CL type information associated with any value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.STRING
+    type_key: CLT_TypeKey = CLT_TypeKey.STRING
 
 
 @dataclasses.dataclass
-class CL_Type_Tuple1(CL_Type):
+class CLT_Type_Tuple1(CLT_Type):
     """Encapsulates CL type information associated with a 1-ary tuple value value.
 
     """
     # Type of first value within 1-ary tuple value.
-    t0_type: CL_Type
+    t0_type: CLT_Type
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.TUPLE_1
+    type_key: CLT_TypeKey = CLT_TypeKey.TUPLE_1
 
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and self.t0_type == other.t0_type
 
 
 @dataclasses.dataclass
-class CL_Type_Tuple2(CL_Type):
+class CLT_Type_Tuple2(CLT_Type):
     """Encapsulates CL type information associated with a 2-ary tuple value value.
 
     """
     # Type of first value within 1-ary tuple value.
-    t0_type: CL_Type
+    t0_type: CLT_Type
 
     # Type of first value within 2-ary tuple value.
-    t1_type: CL_Type
+    t1_type: CLT_Type
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.TUPLE_2
+    type_key: CLT_TypeKey = CLT_TypeKey.TUPLE_2
 
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and \
                self.t0_type == other.t0_type and \
                self.t1_type == other.t1_type
 
 
 @dataclasses.dataclass
-class CL_Type_Tuple3(CL_Type):
+class CLT_Type_Tuple3(CLT_Type):
     """Encapsulates CL type information associated with a 3-ary tuple value value.
 
     """
     # Type of first value within 1-ary tuple value.
-    t0_type: CL_Type
+    t0_type: CLT_Type
 
     # Type of first value within 2-ary tuple value.
-    t1_type: CL_Type
+    t1_type: CLT_Type
 
     # Type of first value within 3-ary tuple value.
-    t2_type: CL_Type
+    t2_type: CLT_Type
 
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.TUPLE_3
+    type_key: CLT_TypeKey = CLT_TypeKey.TUPLE_3
 
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and \
                self.t0_type == other.t0_type and \
                self.t1_type == other.t1_type and \
                self.t2_type == other.t2_type
 
 
 @dataclasses.dataclass
-class CL_Type_U8(CL_Type):
+class CLT_Type_U8(CLT_Type):
     """Encapsulates CL type information associated with a U8 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.U8
+    type_key: CLT_TypeKey = CLT_TypeKey.U8
 
 
 @dataclasses.dataclass
-class CL_Type_U32(CL_Type):
+class CLT_Type_U32(CLT_Type):
     """Encapsulates CL type information associated with a U32 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.U32
+    type_key: CLT_TypeKey = CLT_TypeKey.U32
 
 
 @dataclasses.dataclass
-class CL_Type_U64(CL_Type):
+class CLT_Type_U64(CLT_Type):
     """Encapsulates CL type information associated with a U64 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.U64
+    type_key: CLT_TypeKey = CLT_TypeKey.U64
 
 
 @dataclasses.dataclass
-class CL_Type_U128(CL_Type):
+class CLT_Type_U128(CLT_Type):
     """Encapsulates CL type information associated with a U128 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.U128
+    type_key: CLT_TypeKey = CLT_TypeKey.U128
 
 
 @dataclasses.dataclass
-class CL_Type_U256(CL_Type):
+class CLT_Type_U256(CLT_Type):
     """Encapsulates CL type information associated with a U256 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.U256
+    type_key: CLT_TypeKey = CLT_TypeKey.U256
 
 
 @dataclasses.dataclass
-class CL_Type_U512(CL_Type):
+class CLT_Type_U512(CLT_Type):
     """Encapsulates CL type information associated with a U512 value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.U512
+    type_key: CLT_TypeKey = CLT_TypeKey.U512
 
 
 @dataclasses.dataclass
-class CL_Type_Unit(CL_Type):
+class CLT_Type_Unit(CLT_Type):
     """Encapsulates CL type information associated with a result value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.UNIT
+    type_key: CLT_TypeKey = CLT_TypeKey.UNIT
 
 
 @dataclasses.dataclass
-class CL_Type_URef(CL_Type):
+class CLT_Type_URef(CLT_Type):
     """Encapsulates CL type information associated with a result value.
 
     """
     # CSPR type key.
-    type_key: CL_TypeKey = CL_TypeKey.UREF
+    type_key: CLT_TypeKey = CLT_TypeKey.UREF
```

### Comparing `pycspr-1.1.3/pycspr/types/cl_values.py` & `pycspr-1.2.0/pycspr/types/cl/values.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,355 +1,324 @@
 import dataclasses
 import enum
 import typing
 
-from pycspr import crypto
-from pycspr.types.keys import PublicKey
-from pycspr.types.cl_types import CL_Type
+from pycspr.crypto import get_account_hash
+from pycspr.crypto import get_account_key
+from pycspr.types.cl.types import CLT_Type
+from pycspr.types.crypto import KeyAlgorithm
 
 
 @dataclasses.dataclass
-class CL_Value():
+class CLV_Value():
     """Represents a CL type value.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_Any(CL_Value):
+class CLV_Any(CLV_Value):
     """Represents a CL type value: any = arbitrary data.
 
     """
     # Associated value.
     value: object
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
 
 @dataclasses.dataclass
-class CL_Bool(CL_Value):
+class CLV_Bool(CLV_Value):
     """Represents a CL type value: boolean.
 
     """
     # Associated value.
     value: bool
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
 
 @dataclasses.dataclass
-class CL_ByteArray(CL_Value):
+class CLV_ByteArray(CLV_Value):
     """Represents a CL type value: byte array.
 
     """
     # Associated value.
     value: bytes
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
     def __len__(self) -> int:
         return len(self.value)
 
 
 @dataclasses.dataclass
-class CL_Int(CL_Value):
+class CLV_Int(CLV_Value):
     """Represents a CL type value: integer.
 
     """
     # Associated value.
     value: int
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
 
 @dataclasses.dataclass
-class CL_I32(CL_Int):
+class CLV_I32(CLV_Int):
     """Represents a CL type value: I32.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_I64(CL_Int):
+class CLV_I64(CLV_Int):
     """Represents a CL type value: I64.
 
     """
     pass
 
 
-class CL_KeyType(enum.Enum):
+class CLV_KeyType(enum.Enum):
     """Enumeration over set of global state key types.
 
     """
     ACCOUNT = 0
     HASH = 1
     UREF = 2
 
 
 @dataclasses.dataclass
-class CL_Key(CL_Value):
+class CLV_Key(CLV_Value):
     """Represents a CL type value: state storage key.
 
     """
     # 32 byte key identifier.
     identifier: bytes
 
     # Key type identifier.
-    key_type: CL_KeyType
+    key_type: CLV_KeyType
 
     def __eq__(self, other) -> bool:
         return self.identifier == other.identifier and self.key_type == other.key_type
 
-    @staticmethod
-    def from_string(value: str) -> "CL_Key":
-        """Factory method: parses input string & returns type instance.
-        """
-        identifier = bytes.fromhex(value.split("-")[-1])
-        if value.startswith("account-hash-"):
-            key_type = CL_KeyType.ACCOUNT
-        elif value.startswith("hash-"):
-            key_type = CL_KeyType.HASH
-        elif value.startswith("uref-"):
-            key_type = CL_KeyType.UREF
-        else:
-            raise ValueError(f"Invalid CL key: {value}")
-
-        return CL_Key(identifier, key_type)
-
 
 @dataclasses.dataclass
-class CL_List(CL_Value):
+class CLV_List(CLV_Value):
     """Represents a CL type value: array of items of identical type.
 
     """
     # Set of associated items.
-    vector: typing.List[CL_Value]
+    vector: typing.List[CLV_Value]
 
     def __eq__(self, other) -> bool:
         return self.vector == other.vector
 
 
 @dataclasses.dataclass
-class CL_Map(CL_Value):
+class CLV_Map(CLV_Value):
     """Represents a CL type value: key-value hash map.
 
     """
     # A map of data represented as a vector of 2 member tuples.
-    value: typing.List[typing.Tuple[CL_Value, CL_Value]]
+    value: typing.List[typing.Tuple[CLV_Value, CLV_Value]]
 
 
 @dataclasses.dataclass
-class CL_Option(CL_Value):
+class CLV_Option(CLV_Value):
     """Represents a CL type value: optional value.
 
     """
     # Associated value.
-    value: typing.Union[None, CL_Value]
+    value: typing.Union[None, CLV_Value]
 
     # Associated optional type.
-    option_type: CL_Type
+    option_type: CLT_Type
 
     def __eq__(self, other) -> bool:
         return self.value == other.value and self.option_type == other.option_type
 
 
 @dataclasses.dataclass
-class CL_PublicKey(CL_Value):
+class CLV_PublicKey(CLV_Value):
     """Represents a CL type value: account holder's public key.
 
     """
     # Algorithm used to generate ECC key pair.
-    algo: crypto.KeyAlgorithm
+    algo: KeyAlgorithm
 
     # Public key as raw bytes.
     pbk: bytes
 
     @property
     def account_hash(self) -> bytes:
         """Returns on-chain account hash."""
-        return crypto.get_account_hash(self.account_key)
+        return get_account_hash(self.account_key)
 
     @property
     def account_key(self) -> bytes:
         """Returns on-chain account key."""
-        return crypto.get_account_key(self.algo, self.pbk)
+        return get_account_key(self.algo, self.pbk)
 
     def __eq__(self, other) -> bool:
         return self.algo == other.algo and self.pbk == other.pbk
 
-    @staticmethod
-    def from_account_key(key: bytes) -> "CL_PublicKey":
-        return CL_PublicKey(crypto.KeyAlgorithm(key[0]), key[1:])
-
-    @staticmethod
-    def from_public_key(key: PublicKey) -> "CL_PublicKey":
-        return CL_PublicKey(key.algo, key.pbk)
-
 
 @dataclasses.dataclass
-class CL_Result(CL_Value):
+class CLV_Result(CLV_Value):
     """Represents a CL type value: function invocation result.
 
     """
     # Associated value.
     value: object
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
 
 @dataclasses.dataclass
-class CL_String(CL_Value):
+class CLV_String(CLV_Value):
     """Represents a CL type value: string.
 
     """
     # Associated value.
     value: str
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
 
 @dataclasses.dataclass
-class CL_Tuple1(CL_Value):
+class CLV_Tuple1(CLV_Value):
     """Represents a CL type value: a 1-ary tuple.
 
     """
     # 1st value within 1-ary tuple value.
-    v0: CL_Value
+    v0: CLV_Value
 
     def __eq__(self, other) -> bool:
         return self.v0 == other.v0
 
 
 @dataclasses.dataclass
-class CL_Tuple2(CL_Value):
+class CLV_Tuple2(CLV_Value):
     """Represents a CL type value: a 2-ary tuple.
 
     """
     # 1st value within 2-ary tuple value.
-    v0: CL_Value
+    v0: CLV_Value
 
     # 2nd value within 2-ary tuple value.
-    v1: CL_Value
+    v1: CLV_Value
 
     def __eq__(self, other) -> bool:
         return self.v0 == other.v0 and self.v1 == other.v1
 
 
 @dataclasses.dataclass
-class CL_Tuple3(CL_Value):
+class CLV_Tuple3(CLV_Value):
     """Represents a CL type value: a 3-ary tuple.
 
     """
     # 1st value within 3-ary tuple value.
-    v0: CL_Value
+    v0: CLV_Value
 
     # 2nd value within 3-ary tuple value.
-    v1: CL_Value
+    v1: CLV_Value
 
     # 3rd value within 3-ary tuple value.
-    v2: CL_Value
+    v2: CLV_Value
 
     def __eq__(self, other) -> bool:
         return self.v0 == other.v0 and self.v1 == other.v1 and self.v2 == other.v2
 
 
 @dataclasses.dataclass
-class CL_U8(CL_Int):
+class CLV_U8(CLV_Int):
     """Represents a CL type value: U8.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_U32(CL_Int):
+class CLV_U32(CLV_Int):
     """Represents a CL type value: U32.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_U64(CL_Int):
+class CLV_U64(CLV_Int):
     """Represents a CL type value: U64.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_U128(CL_Int):
+class CLV_U128(CLV_Int):
     """Represents a CL type value: U128.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_U256(CL_Int):
+class CLV_U256(CLV_Int):
     """Represents a CL type value: U256.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_U512(CL_Int):
+class CLV_U512(CLV_Int):
     """Represents a CL type value: U512.
 
     """
     pass
 
 
 @dataclasses.dataclass
-class CL_Unit(CL_Value):
+class CLV_Unit(CLV_Value):
     """Represents a CL type value: unit, i.e. a null value.
 
     """
     def __eq__(self, other) -> bool:
         return True
 
 
-class CL_URefAccessRights(enum.Enum):
+class CLV_URefAccessRights(enum.Enum):
     """Enumeration over set of CL item access rights.
 
     """
     NONE = 0
     READ = 1
     WRITE = 2
     ADD = 4
     READ_WRITE = 3
     READ_ADD = 5
     ADD_WRITE = 6
     READ_ADD_WRITE = 7
 
 
 @dataclasses.dataclass
-class CL_URef(CL_Value):
+class CLV_URef(CLV_Value):
     """Represents a CL type value: unforgeable reference.
 
     """
     # Access rights granted by issuer.
-    access_rights: CL_URefAccessRights
+    access_rights: CLV_URefAccessRights
 
     # Uref on-chain identifier.
     address: bytes
 
     def __eq__(self, other) -> bool:
         return self.access_rights == other.access_rights and \
                self.address == other.address
-
-    @staticmethod
-    def from_string(as_string: str) -> "CL_URef":
-        _, address, access_rights = as_string.split("-")
-        return CL_URef(
-            CL_URefAccessRights(int(access_rights)),
-            bytes.fromhex(address)
-            )
```

### Comparing `pycspr-1.1.3/pycspr/types/keys.py` & `pycspr-1.2.0/pycspr/types/crypto/complex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,72 @@
 import dataclasses
 
-from pycspr import crypto
+from pycspr.types.crypto.simple import KeyAlgorithm
+from pycspr.types.crypto.simple import PrivateKeyBytes
+from pycspr.types.crypto.simple import PublicKeyBytes
 
 
 @dataclasses.dataclass
 class PublicKey():
     """Encapsulates information associated with an account's public key.
 
     """
     # Algorithm used to generate ECC key pair.
-    algo: crypto.KeyAlgorithm
+    algo: KeyAlgorithm
 
     # Public key as raw bytes.
-    pbk: bytes
-
-    @property
-    def account_hash(self) -> bytes:
-        """Returns on-chain account hash."""
-        return crypto.get_account_hash(self.account_key)
+    pbk: PublicKeyBytes
 
     @property
     def account_key(self) -> bytes:
-        """Returns on-chain account key."""
-        return crypto.get_account_key(self.algo, self.pbk)
+        return bytes([self.algo.value]) + self.pbk
+
+    def to_account_hash(self) -> bytes:
+        """Returns on-chain account address.
+
+        """
+        from pycspr.crypto.cl_operations import get_account_hash
+
+        return get_account_hash(self.account_key)
 
     def __eq__(self, other) -> bool:
         return self.algo == other.algo and self.pbk == other.pbk
 
     def __hash__(self) -> bytes:
         return hash(self.account_key)
 
     def __len__(self) -> int:
-        return len(self.account_key)
+        return len(self.pbk) + 1
 
 
 @dataclasses.dataclass
 class PrivateKey:
     """Encapsulates information associated with an account's private key.
 
     """
     # Private key as bytes - sensitive material !
-    pvk: bytes
+    pvk: PrivateKeyBytes
 
     # Public key as bytes.
-    pbk: bytes
+    pbk: PublicKeyBytes
 
     # Algorithm used to generate ECC key pair.
-    algo: crypto.KeyAlgorithm = crypto.KeyAlgorithm.ED25519
+    algo: KeyAlgorithm = KeyAlgorithm.ED25519
+
+    @property
+    def account_key(self) -> bytes:
+        return bytes([self.algo.value]) + self.pbk
 
     def __eq__(self, other) -> bool:
         return self.algo == other.algo and self.pvk == other.pvk and self.pbk == other.pbk
 
     def __hash__(self) -> bytes:
         return hash(self.pvk)
 
     def __len__(self) -> int:
         return len(self.pvk)
 
-    @property
-    def private_key(self) -> bytes:
-        """Associated private key synonym."""
-        return self.pvk
-
-    @property
-    def public_key(self) -> bytes:
-        """Associated public key synonym."""
-        return self.pbk
-
-    @property
-    def key_algo(self) -> crypto.KeyAlgorithm:
-        """Associated key algorithm synonym."""
-        return self.algo
-
-    @property
-    def account_hash(self) -> bytes:
-        """Gets derived on-chain account hash - i.e. address."""
-        return crypto.get_account_hash(self.account_key)
-
-    @property
-    def account_key(self) -> bytes:
-        """Gets on-chain account key."""
-        return crypto.get_account_key(self.algo, self.pbk)
-
-    @property
-    def as_public_key(self) -> PublicKey:
+    def to_public_key(self) -> PublicKey:
         """Returns public key representation.
 
         """
         return PublicKey(algo=self.algo, pbk=self.pbk)
-
-    def get_signature(self, data: bytes) -> bytes:
-        """Get signature over payload.
-
-        """
-        return crypto.get_signature(data, self.pvk, self.algo)
```

### Comparing `pycspr-1.1.3/pycspr/utils/constants.py` & `pycspr-1.2.0/pycspr/utils/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 # Maximum value of a transfer ID.
 MAX_TRANSFER_ID = (2 ** 63) - 1
 
 # Minimum amount in motes of a wasmless transfer.
 MIN_TRANSFER_AMOUNT_MOTES = 2_500_000_000
 
+# Millisecond durations of relevance.
+MS_1_SECOND: int = 1000
+MS_1_MINUTE: int = 60 * MS_1_SECOND
+MS_1_HOUR: int = 60 * MS_1_MINUTE
+
 # Default number of motes to pay for standard payments.
 STANDARD_PAYMENT_FOR_NATIVE_TRANSFERS = int(1e8)
 
 # Default number of motes to pay for standard delegation.
 STANDARD_PAYMENT_FOR_DELEGATION = int(5e9)
 
 # Default number of motes to pay for standard delegation withdrawal.
```

### Comparing `pycspr-1.1.3/pycspr/utils/io.py` & `pycspr-1.2.0/pycspr/utils/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import json
 import pathlib
 import typing
 
-from pycspr import serialisation
+from pycspr import serializer
 from pycspr import factory
-from pycspr.types import Deploy
+from pycspr.types.node.rpc import Deploy
 
 
 def get_deploy_size_bytes(deploy: Deploy) -> int:
     """Returns size of a deploy in bytes.
 
     :deploy: Deploy to be written in JSON format.
     :returns: Size of deploy in bytes.
 
     """
     size: int = len(deploy.hash)
     for approval in deploy.approvals:
         size += len(approval.signature)
         size += len(approval.signer)
-        size += len(serialisation.to_bytes(deploy.header))
-        size += len(serialisation.to_bytes(
+        size += len(serializer.to_bytes(deploy.header))
+        size += len(serializer.to_bytes(
             factory.create_deploy_body(deploy.payment, deploy.session))
         )
 
     return size
 
 
 def read_deploy(fpath: typing.Union[pathlib.Path, str]) -> Deploy:
     """Reads a deploy from file system.
 
     :fpath: Path to target file.
 
     """
     fpath = pathlib.Path(fpath) if isinstance(fpath, str) else fpath
     with open(str(fpath), "r") as fstream:
-        return serialisation.from_json(json.loads(fstream.read()), Deploy)
+        return serializer.from_json(json.loads(fstream.read()), Deploy)
 
 
 def read_wasm(fpath: typing.Union[pathlib.Path, str]) -> bytes:
     """Read a smart contract from file system.
 
     :fpath: Path to target file.
 
@@ -65,10 +65,10 @@
         raise ValueError("Unrecognized file path type")
 
     fpath = pathlib.Path(fpath) if isinstance(fpath, str) else fpath
     if not force and fpath.exists():
         raise IOError("Deploy has already been written to file system")
 
     with open(str(fpath), "w") as fstream:
-        fstream.writelines(json.dumps(serialisation.to_json(deploy), indent=4))
+        fstream.writelines(json.dumps(serializer.to_json(deploy), indent=4))
 
     return str(fpath)
```

### Comparing `pycspr-1.1.3/pycspr/utils/validation.py` & `pycspr-1.2.0/pycspr/utils/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pycspr import crypto
 from pycspr import factory
-from pycspr.types import Deploy
+from pycspr.types.node.rpc import Deploy
 
 
 class InvalidDeployException(Exception):
     """Exception thrown when a deploy is deemed invalid.
 
     """
     def __init__(self, msg):
@@ -27,12 +27,12 @@
     if deploy.hash != deploy_hash:
         raise InvalidDeployException("Invalid deploy hash")
 
     # Validate deploy approval signatures.
     for approval in deploy.approvals:
         if not crypto.is_signature_valid(
             deploy.hash,
-            approval.sig,
+            approval.signature[1:],
             approval.signer.pbk,
             approval.signer.algo
         ):
             raise InvalidDeployException("Invalid deploy approval signature")
```

### Comparing `pycspr-1.1.3/pyproject.toml` & `pycspr-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycspr"
-version = "1.1.3"
+version = "1.2.0"
 authors = ["Mark A. Greenslade <asladeofgreen@gmail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

### Comparing `pycspr-1.1.3/PKG-INFO` & `pycspr-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycspr
-Version: 1.1.3
+Version: 1.2.0
 Summary: Python library for interacting with a CSPR node.
 Home-page: https://github.com/casper-network/casper-python-sdk
 License: Apache-2.0
 Keywords: Casper Network,Blockchain,Python
 Author: Mark A. Greenslade
 Author-email: asladeofgreen@gmail.com
 Maintainer: Mark A. Greenslade
@@ -39,19 +39,21 @@
 pip3 install pycspr
 ```
 
 ##  Usage
 
 ### Cryptography
 
-* [How To: Hash data ?](how_tos/cryptography/how_to_hash_data.py)
+* [How To: Apply a checksum ?](how_tos/crypto/how_to_apply_a_checksum.py)
 
-* [How To: Create Key Pairs ?](how_tos/cryptography/how_to_create_key_pairs.py)
+* [How To: Create Key Pairs ?](how_tos/crypto/how_to_create_key_pairs.py)
 
-* [How To: Apply a checksum ?](how_tos/cryptography/how_to_apply_a_checksum.py)
+* [How To: Hash data ?](how_tos/crypto/how_to_hash_data.py)
+
+* [How To: Sign data ?](how_tos/crypto/how_to_sign_data.py)
 
 ### Deploys
 
 * [How To: Transfer funds between 2 accounts ?](how_tos/deploys/how_to_transfer.py)
 
 * [How To: Delegate funds to a validator ?](how_tos/deploys/how_to_delegate.py)
```

