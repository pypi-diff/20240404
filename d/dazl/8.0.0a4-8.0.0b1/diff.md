# Comparing `tmp/dazl-8.0.0a4.tar.gz` & `tmp/dazl-8.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dazl-8.0.0a4.tar", max compression
+gzip compressed data, was "dazl-8.0.0b1.tar", max compression
```

## Comparing `dazl-8.0.0a4.tar` & `dazl-8.0.0b1.tar`

### file list

```diff
@@ -1,279 +1,553 @@
--rw-r--r--   0        0        0    11393 2023-01-10 03:35:07.777596 dazl-8.0.0a4/LICENSE
--rw-r--r--   0        0        0     2725 2023-05-01 04:00:01.467390 dazl-8.0.0a4/README.md
--rw-r--r--   0        0        0     2258 2023-09-29 22:25:17.875516 dazl-8.0.0a4/pyproject.toml
--rw-r--r--   0        0        0      848 2023-01-10 03:35:07.817890 dazl-8.0.0a4/python/_dazl_pb/__init__.py
--rw-r--r--   0        0        0      952 2023-10-03 01:19:39.926077 dazl-8.0.0a4/python/_dazl_pb/collections.py
--rw-r--r--   0        0        0      308 2023-05-01 04:00:01.476626 dazl-8.0.0a4/python/_dazl_pb/plugin_go/__init__.py
--rw-r--r--   0        0        0      347 2023-05-01 04:00:01.476691 dazl-8.0.0a4/python/_dazl_pb/plugin_go/_header.py
--rw-r--r--   0        0        0      587 2023-05-01 04:00:01.476753 dazl-8.0.0a4/python/_dazl_pb/plugin_go/plugin.py
--rw-r--r--   0        0        0      531 2023-05-01 04:00:01.476812 dazl-8.0.0a4/python/_dazl_pb/plugin_go/plugin_grpc.py
--rw-r--r--   0        0        0      583 2023-05-01 04:00:01.476875 dazl-8.0.0a4/python/_dazl_pb/plugin_go/plugin_pb.py
--rw-r--r--   0        0        0      308 2023-05-01 04:00:01.477009 dazl-8.0.0a4/python/_dazl_pb/plugin_python/__init__.py
--rw-r--r--   0        0        0      339 2023-01-10 03:35:07.818838 dazl-8.0.0a4/python/_dazl_pb/plugin_python/_header.py
--rw-r--r--   0        0        0      806 2023-10-02 16:56:57.175510 dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin.py
--rw-r--r--   0        0        0      705 2023-10-02 16:56:57.175979 dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_grpc.py
--rw-r--r--   0        0        0     5261 2023-10-02 16:56:57.176560 dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_grpc_pyi.py
--rw-r--r--   0        0        0     2355 2023-10-02 16:56:57.177214 dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_init.py
--rw-r--r--   0        0        0      680 2023-10-02 16:56:57.177808 dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_pb.py
--rw-r--r--   0        0        0     7051 2023-10-02 16:56:57.178321 dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_pb_pyi.py
--rw-r--r--   0        0        0     4559 2023-10-02 16:56:57.178653 dazl-8.0.0a4/python/_dazl_pb/protoc/__init__.py
--rw-r--r--   0        0        0      205 2023-05-01 04:00:01.477936 dazl-8.0.0a4/python/_dazl_pb/protoc/__main__.py
--rw-r--r--   0        0        0      221 2023-05-01 04:00:01.478067 dazl-8.0.0a4/python/_dazl_pb/syntax/__init__.py
--rw-r--r--   0        0        0      601 2023-05-01 04:00:01.478199 dazl-8.0.0a4/python/_dazl_pb/syntax/python/__init__.py
--rw-r--r--   0        0        0      586 2023-10-02 16:56:57.178957 dazl-8.0.0a4/python/_dazl_pb/syntax/python/_basic.py
--rw-r--r--   0        0        0     5238 2023-10-03 01:19:39.926938 dazl-8.0.0a4/python/_dazl_pb/syntax/python/imports.py
--rw-r--r--   0        0        0     2683 2023-10-02 16:56:57.179566 dazl-8.0.0a4/python/_dazl_pb/syntax/python/pb.py
--rw-r--r--   0        0        0     7328 2023-10-02 16:56:57.180035 dazl-8.0.0a4/python/_dazl_pb/syntax/python/symbols.py
--rw-r--r--   0        0        0     2793 2023-10-02 16:56:57.180437 dazl-8.0.0a4/python/_dazl_pb/syntax/python/types.py
--rw-r--r--   0        0        0     1536 2023-10-02 16:56:57.180967 dazl-8.0.0a4/python/_dazl_pb/util/__init__.py
--rw-r--r--   0        0        0     1737 2023-05-01 04:00:01.479150 dazl-8.0.0a4/python/dazl/__init__.py
--rw-r--r--   0        0        0      311 2023-05-01 04:00:01.479255 dazl-8.0.0a4/python/dazl/__main__.py
--rw-r--r--   0        0        0      202 2023-09-29 22:35:11.044267 dazl-8.0.0a4/python/dazl/_gen/__init__.py
--rw-r--r--   0        0        0      202 2023-09-29 22:35:11.044347 dazl-8.0.0a4/python/dazl/_gen/com/__init__.py
--rw-r--r--   0        0        0      202 2023-09-29 22:35:11.044404 dazl-8.0.0a4/python/dazl/_gen/com/daml/__init__.py
--rw-r--r--   0        0        0      202 2023-09-29 22:35:11.044458 dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/__init__.py
--rw-r--r--   0        0        0    52179 2023-09-29 22:35:11.044655 dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py
--rw-r--r--   0        0        0   131556 2023-09-29 22:35:11.044755 dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.pyi
--rw-r--r--   0        0        0     2298 2023-09-29 22:35:11.044845 dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py
--rw-r--r--   0        0        0     1832 2023-09-29 22:35:11.044901 dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.pyi
--rw-r--r--   0        0        0      202 2023-09-29 22:35:11.044957 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/__init__.py
--rw-r--r--   0        0        0      202 2023-09-29 22:35:11.045141 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/__init__.py
--rw-r--r--   0        0        0     6188 2023-09-29 22:35:11.045514 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py
--rw-r--r--   0        0        0     2961 2023-09-29 22:35:11.046033 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py
--rw-r--r--   0        0        0     2021 2023-09-29 22:35:11.046124 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.pyi
--rw-r--r--   0        0        0     4123 2023-09-29 22:35:11.046517 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py
--rw-r--r--   0        0        0     2396 2023-09-29 22:35:11.047029 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4230 2023-09-29 22:35:11.047327 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py
--rw-r--r--   0        0        0     3967 2023-09-29 22:35:11.047684 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py
--rw-r--r--   0        0        0     3482 2023-09-29 22:35:11.047734 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.pyi
--rw-r--r--   0        0        0     6167 2023-09-29 22:35:11.047793 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3579 2023-09-29 22:35:11.048209 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     6247 2023-09-29 22:35:11.048324 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py
--rw-r--r--   0        0        0     6529 2023-09-29 22:35:11.048465 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.pyi
--rw-r--r--   0        0        0    17920 2023-09-29 22:35:11.048891 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py
--rw-r--r--   0        0        0     8410 2023-09-29 22:35:11.049058 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3043 2023-09-29 22:35:11.049172 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py
--rw-r--r--   0        0        0     1793 2023-09-29 22:35:11.049235 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.pyi
--rw-r--r--   0        0        0     3683 2023-09-29 22:35:11.049291 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py
--rw-r--r--   0        0        0     2333 2023-09-29 22:35:11.049351 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2218 2023-09-29 22:35:11.049406 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py
--rw-r--r--   0        0        0      992 2023-09-29 22:35:11.049641 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.pyi
--rw-r--r--   0        0        0     3426 2023-09-29 22:35:11.049694 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py
--rw-r--r--   0        0        0     3011 2023-09-29 22:35:11.049749 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.pyi
--rw-r--r--   0        0        0     6681 2023-09-29 22:35:11.049807 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3660 2023-09-29 22:35:11.049938 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2325 2023-09-29 22:35:11.049993 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py
--rw-r--r--   0        0        0     1340 2023-09-29 22:35:11.050043 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.pyi
--rw-r--r--   0        0        0     4791 2023-09-29 22:35:11.050095 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py
--rw-r--r--   0        0        0     2225 2023-09-29 22:35:11.050223 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5912 2023-09-29 22:35:11.050285 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py
--rw-r--r--   0        0        0     6804 2023-09-29 22:35:11.050418 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.pyi
--rw-r--r--   0        0        0    16483 2023-09-29 22:35:11.050824 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     7590 2023-09-29 22:35:11.050889 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     9131 2023-09-29 22:35:11.051030 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py
--rw-r--r--   0        0        0    12746 2023-09-29 22:35:11.051152 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.pyi
--rw-r--r--   0        0        0    22553 2023-09-29 22:35:11.051287 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11229 2023-09-29 22:35:11.051348 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3879 2023-09-29 22:35:11.051450 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py
--rw-r--r--   0        0        0     3481 2023-09-29 22:35:11.051504 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.pyi
--rw-r--r--   0        0        0     7734 2023-09-29 22:35:11.051943 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py
--rw-r--r--   0        0        0     3690 2023-09-29 22:35:11.052080 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3899 2023-09-29 22:35:11.052134 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py
--rw-r--r--   0        0        0     2724 2023-09-29 22:35:11.052184 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.pyi
--rw-r--r--   0        0        0    10939 2023-09-29 22:35:11.052237 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py
--rw-r--r--   0        0        0     6396 2023-09-29 22:35:11.052335 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2250 2023-09-29 22:35:11.052792 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py
--rw-r--r--   0        0        0      763 2023-09-29 22:35:11.052845 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.pyi
--rw-r--r--   0        0        0     5656 2023-09-29 22:35:11.052980 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py
--rw-r--r--   0        0        0     2220 2023-09-29 22:35:11.053241 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     6717 2023-09-29 22:35:11.053398 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py
--rw-r--r--   0        0        0    11289 2023-09-29 22:35:11.053815 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.pyi
--rw-r--r--   0        0        0     2481 2023-09-29 22:35:11.053931 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py
--rw-r--r--   0        0        0     2714 2023-09-29 22:35:11.053979 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.pyi
--rw-r--r--   0        0        0     2007 2023-09-29 22:35:11.054031 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py
--rw-r--r--   0        0        0     1069 2023-09-29 22:35:11.054080 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.pyi
--rw-r--r--   0        0        0     5333 2023-09-29 22:35:11.054132 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py
--rw-r--r--   0        0        0     7007 2023-09-29 22:35:11.054282 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.pyi
--rw-r--r--   0        0        0     3878 2023-09-29 22:35:11.054427 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py
--rw-r--r--   0        0        0     3525 2023-09-29 22:35:11.054479 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.pyi
--rw-r--r--   0        0        0     5706 2023-09-29 22:35:11.054818 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py
--rw-r--r--   0        0        0     3753 2023-09-29 22:35:11.054958 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     7614 2023-09-29 22:35:11.055332 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py
--rw-r--r--   0        0        0     8148 2023-09-29 22:35:11.055677 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.pyi
--rw-r--r--   0        0        0     2840 2023-09-29 22:35:11.056131 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py
--rw-r--r--   0        0        0     1838 2023-09-29 22:35:11.056180 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.pyi
--rw-r--r--   0        0        0     3609 2023-09-29 22:35:11.056233 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py
--rw-r--r--   0        0        0     2480 2023-09-29 22:35:11.056289 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2941 2023-09-29 22:35:11.056340 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py
--rw-r--r--   0        0        0     1076 2023-09-29 22:35:11.056388 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.pyi
--rw-r--r--   0        0        0     3844 2023-09-29 22:35:11.056434 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py
--rw-r--r--   0        0        0     2333 2023-09-29 22:35:11.056487 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2039 2023-09-29 22:35:11.056536 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py
--rw-r--r--   0        0        0      995 2023-09-29 22:35:11.056582 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.pyi
--rw-r--r--   0        0        0     3815 2023-09-29 22:35:11.056640 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py
--rw-r--r--   0        0        0     4019 2023-09-29 22:35:11.056689 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.pyi
--rw-r--r--   0        0        0     6970 2023-09-29 22:35:11.056744 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py
--rw-r--r--   0        0        0     4809 2023-09-29 22:35:11.056889 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      406 2023-09-29 22:35:11.057255 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/__init__.py
--rw-r--r--   0        0        0     3960 2023-01-10 03:35:07.831406 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2.py
--rw-r--r--   0        0        0      709 2023-09-06 00:21:45.112435 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2.pyi
--rw-r--r--   0        0        0     7185 2023-01-10 03:35:07.831599 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.py
--rw-r--r--   0        0        0     2104 2023-09-22 14:08:55.919281 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2913 2023-09-29 22:35:11.057391 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py
--rw-r--r--   0        0        0     1893 2023-09-29 22:35:11.057438 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.pyi
--rw-r--r--   0        0        0     5129 2023-09-29 22:35:11.057488 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py
--rw-r--r--   0        0        0     3379 2023-09-29 22:35:11.057629 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3327 2023-09-29 22:35:11.057682 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py
--rw-r--r--   0        0        0     2916 2023-09-29 22:35:11.057734 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.pyi
--rw-r--r--   0        0        0     3685 2023-09-29 22:35:11.057787 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py
--rw-r--r--   0        0        0     3572 2023-09-29 22:35:11.057840 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.pyi
--rw-r--r--   0        0        0     6625 2023-09-29 22:35:11.057898 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py
--rw-r--r--   0        0        0     7080 2023-09-29 22:35:11.058172 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.pyi
--rw-r--r--   0        0        0    17982 2023-09-29 22:35:11.058309 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py
--rw-r--r--   0        0        0    11776 2023-09-29 22:35:11.058378 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5817 2023-09-29 22:35:11.058482 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py
--rw-r--r--   0        0        0     8775 2023-09-29 22:35:11.058629 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.pyi
--rw-r--r--   0        0        0     3221 2023-09-29 22:35:11.058722 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py
--rw-r--r--   0        0        0     2746 2023-09-29 22:35:11.058769 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.pyi
--rw-r--r--   0        0        0     3207 2023-09-29 22:35:11.058821 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py
--rw-r--r--   0        0        0     2293 2023-09-29 22:35:11.058870 dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5249 2023-10-02 16:56:57.181569 dazl-8.0.0a4/python/dazl/_logging.py
--rw-r--r--   0        0        0      990 2023-10-03 01:19:39.927248 dazl-8.0.0a4/python/dazl/_repr/__init__.py
--rw-r--r--   0        0        0     1722 2023-10-02 16:56:57.182417 dazl-8.0.0a4/python/dazl/cli/__init__.py
--rw-r--r--   0        0        0      602 2023-05-01 04:00:01.479697 dazl-8.0.0a4/python/dazl/cli/_base.py
--rw-r--r--   0        0        0     2102 2023-10-02 16:56:57.182762 dazl-8.0.0a4/python/dazl/cli/ls.py
--rw-r--r--   0        0        0     3273 2023-10-02 16:56:57.183100 dazl-8.0.0a4/python/dazl/cli/tail.py
--rw-r--r--   0        0        0     1233 2023-05-01 04:00:01.480032 dazl-8.0.0a4/python/dazl/cli/upload.py
--rw-r--r--   0        0        0      490 2023-05-01 04:00:01.480136 dazl-8.0.0a4/python/dazl/cli/version.py
--rw-r--r--   0        0        0     1036 2023-05-01 04:00:01.480249 dazl-8.0.0a4/python/dazl/client/__init__.py
--rw-r--r--   0        0        0     1339 2023-09-06 00:21:45.115623 dazl-8.0.0a4/python/dazl/client/_base_model.py
--rw-r--r--   0        0        0     3620 2023-05-01 04:00:01.480458 dazl-8.0.0a4/python/dazl/client/_conn_settings.py
--rw-r--r--   0        0        0     1419 2023-05-01 04:00:01.480556 dazl-8.0.0a4/python/dazl/client/_events.py
--rw-r--r--   0        0        0    24584 2023-10-02 16:56:57.183787 dazl-8.0.0a4/python/dazl/client/_network_client_impl.py
--rw-r--r--   0        0        0    33712 2023-10-03 01:19:39.927603 dazl-8.0.0a4/python/dazl/client/_party_client_impl.py
--rw-r--r--   0        0        0     4790 2023-10-02 16:56:57.185454 dazl-8.0.0a4/python/dazl/client/_reader_sync.py
--rw-r--r--   0        0        0      870 2023-05-01 04:00:01.481659 dazl-8.0.0a4/python/dazl/client/_run_level.py
--rw-r--r--   0        0        0     2150 2023-05-01 04:00:01.481758 dazl-8.0.0a4/python/dazl/client/_writer_verify.py
--rw-r--r--   0        0        0    68240 2023-10-03 01:19:39.928042 dazl-8.0.0a4/python/dazl/client/api.py
--rw-r--r--   0        0        0    19876 2023-10-02 16:56:57.187115 dazl-8.0.0a4/python/dazl/client/bots.py
--rw-r--r--   0        0        0    11356 2023-10-02 16:56:57.188400 dazl-8.0.0a4/python/dazl/client/commands.py
--rw-r--r--   0        0        0    18771 2023-10-02 16:56:57.188717 dazl-8.0.0a4/python/dazl/client/config.py
--rw-r--r--   0        0        0     1307 2023-10-02 16:56:57.189259 dazl-8.0.0a4/python/dazl/client/errors.py
--rw-r--r--   0        0        0     6863 2023-10-02 16:56:57.189578 dazl-8.0.0a4/python/dazl/client/events.py
--rw-r--r--   0        0        0     1070 2023-10-02 16:56:57.189984 dazl-8.0.0a4/python/dazl/client/ledger.py
--rw-r--r--   0        0        0      952 2023-05-01 04:00:01.482992 dazl-8.0.0a4/python/dazl/client/runner.py
--rw-r--r--   0        0        0     9113 2023-10-02 16:56:57.190322 dazl-8.0.0a4/python/dazl/client/state.py
--rw-r--r--   0        0        0     1533 2023-05-01 04:00:01.483242 dazl-8.0.0a4/python/dazl/damlast/__init__.py
--rw-r--r--   0        0        0      440 2023-05-01 04:00:01.483335 dazl-8.0.0a4/python/dazl/damlast/_base.py
--rw-r--r--   0        0        0     3251 2023-05-01 04:00:01.483445 dazl-8.0.0a4/python/dazl/damlast/_builtins_meta.py
--rw-r--r--   0        0        0     2394 2023-10-02 16:56:57.190530 dazl-8.0.0a4/python/dazl/damlast/builtins.py
--rw-r--r--   0        0        0    91575 2023-05-01 04:00:01.483870 dazl-8.0.0a4/python/dazl/damlast/daml_lf_1.py
--rw-r--r--   0        0        0     6316 2023-05-01 04:00:01.483995 dazl-8.0.0a4/python/dazl/damlast/daml_types.py
--rw-r--r--   0        0        0     1395 2023-05-01 04:00:01.484094 dazl-8.0.0a4/python/dazl/damlast/errors.py
--rw-r--r--   0        0        0    12557 2023-10-02 16:56:57.190973 dazl-8.0.0a4/python/dazl/damlast/expand.py
--rw-r--r--   0        0        0    20477 2023-10-03 01:19:39.928414 dazl-8.0.0a4/python/dazl/damlast/lookup.py
--rw-r--r--   0        0        0     2955 2023-05-01 04:00:01.484511 dazl-8.0.0a4/python/dazl/damlast/parse.py
--rw-r--r--   0        0        0    46143 2023-09-06 00:21:45.115926 dazl-8.0.0a4/python/dazl/damlast/pb_parse.py
--rw-r--r--   0        0        0     8997 2023-10-02 16:56:57.192292 dazl-8.0.0a4/python/dazl/damlast/pkgfile.py
--rw-r--r--   0        0        0     4855 2023-09-06 00:21:45.116091 dazl-8.0.0a4/python/dazl/damlast/protocols.py
--rw-r--r--   0        0        0     2938 2023-05-01 04:00:01.485431 dazl-8.0.0a4/python/dazl/damlast/types.py
--rw-r--r--   0        0        0     5978 2023-10-02 16:56:57.192790 dazl-8.0.0a4/python/dazl/damlast/util.py
--rw-r--r--   0        0        0    14983 2023-10-02 16:56:57.193305 dazl-8.0.0a4/python/dazl/damlast/visitor.py
--rw-r--r--   0        0        0    27127 2023-10-03 01:19:39.928801 dazl-8.0.0a4/python/dazl/ledger/__init__.py
--rw-r--r--   0        0        0    15446 2023-10-03 01:19:39.929356 dazl-8.0.0a4/python/dazl/ledger/__init__.pyi
--rw-r--r--   0        0        0     2324 2023-10-02 16:56:57.193660 dazl-8.0.0a4/python/dazl/ledger/_offsets.py
--rw-r--r--   0        0        0     1652 2023-09-06 00:21:45.116752 dazl-8.0.0a4/python/dazl/ledger/_retry.py
--rw-r--r--   0        0        0     6622 2023-09-06 00:21:45.116915 dazl-8.0.0a4/python/dazl/ledger/aio/__init__.py
--rw-r--r--   0        0        0    11541 2023-10-03 01:19:39.929672 dazl-8.0.0a4/python/dazl/ledger/aio/__init__.pyi
--rw-r--r--   0        0        0     5890 2023-10-02 16:56:57.193971 dazl-8.0.0a4/python/dazl/ledger/aio/pkgloader.py
--rw-r--r--   0        0        0     3404 2023-10-02 16:56:57.194380 dazl-8.0.0a4/python/dazl/ledger/aio/pkgloader_compat.py
--rw-r--r--   0        0        0    23098 2023-10-03 01:19:39.930193 dazl-8.0.0a4/python/dazl/ledger/api_types.py
--rw-r--r--   0        0        0     2117 2023-09-06 00:21:45.117729 dazl-8.0.0a4/python/dazl/ledger/blocking/__init__.py
--rw-r--r--   0        0        0     7466 2023-10-03 01:19:39.930582 dazl-8.0.0a4/python/dazl/ledger/blocking/__init__.pyi
--rw-r--r--   0        0        0     6846 2023-10-02 16:56:57.195239 dazl-8.0.0a4/python/dazl/ledger/blocking/_aiowrapper.py
--rw-r--r--   0        0        0     5937 2023-10-02 16:56:57.195581 dazl-8.0.0a4/python/dazl/ledger/blocking/pkgloader.py
--rw-r--r--   0        0        0    17010 2023-05-01 04:00:01.488602 dazl-8.0.0a4/python/dazl/ledger/config/__init__.py
--rw-r--r--   0        0        0    20203 2023-09-06 00:21:45.118055 dazl-8.0.0a4/python/dazl/ledger/config/access.py
--rw-r--r--   0        0        0    14197 2023-10-02 16:56:57.195940 dazl-8.0.0a4/python/dazl/ledger/config/argv.py
--rw-r--r--   0        0        0      304 2023-05-01 04:00:01.489072 dazl-8.0.0a4/python/dazl/ledger/config/exc.py
--rw-r--r--   0        0        0     2645 2023-10-02 16:56:57.196185 dazl-8.0.0a4/python/dazl/ledger/config/ssl.py
--rw-r--r--   0        0        0     9806 2023-09-06 00:21:45.118274 dazl-8.0.0a4/python/dazl/ledger/config/url.py
--rw-r--r--   0        0        0     4761 2023-10-02 16:56:57.196620 dazl-8.0.0a4/python/dazl/ledger/errors.py
--rw-r--r--   0        0        0      475 2023-05-01 04:00:01.489575 dazl-8.0.0a4/python/dazl/ledger/grpc/__init__.py
--rw-r--r--   0        0        0     1275 2023-05-01 04:00:01.489686 dazl-8.0.0a4/python/dazl/ledger/grpc/__init__.pyi
--rw-r--r--   0        0        0     6459 2023-09-06 00:21:45.118451 dazl-8.0.0a4/python/dazl/ledger/grpc/channel.py
--rw-r--r--   0        0        0    18456 2023-10-03 01:19:39.931294 dazl-8.0.0a4/python/dazl/ledger/grpc/codec_aio.py
--rw-r--r--   0        0        0    47640 2023-10-03 01:19:39.931676 dazl-8.0.0a4/python/dazl/ledger/grpc/conn_aio.py
--rw-r--r--   0        0        0      313 2023-05-01 04:00:01.490340 dazl-8.0.0a4/python/dazl/ledger/pkgcache.py
--rw-r--r--   0        0        0      290 2023-05-01 04:00:01.490468 dazl-8.0.0a4/python/dazl/ledgerutil/__init__.py
--rw-r--r--   0        0        0    17303 2023-09-06 00:21:45.119004 dazl-8.0.0a4/python/dazl/ledgerutil/acs.py
--rw-r--r--   0        0        0     1883 2023-10-03 01:19:39.931888 dazl-8.0.0a4/python/dazl/ledgerutil/fetch.py
--rw-r--r--   0        0        0      208 2023-05-01 04:00:01.490830 dazl-8.0.0a4/python/dazl/metrics/__init__.py
--rw-r--r--   0        0        0      991 2023-05-01 04:00:01.490949 dazl-8.0.0a4/python/dazl/metrics/api.py
--rw-r--r--   0        0        0     1614 2023-05-01 04:00:01.491062 dazl-8.0.0a4/python/dazl/metrics/instrumenters.py
--rw-r--r--   0        0        0     1592 2023-05-01 04:00:01.491473 dazl-8.0.0a4/python/dazl/metrics/prometheus.py
--rw-r--r--   0        0        0      829 2023-05-01 04:00:01.491604 dazl-8.0.0a4/python/dazl/pretty/__init__.py
--rw-r--r--   0        0        0      877 2023-05-01 04:00:01.492023 dazl-8.0.0a4/python/dazl/pretty/pygments_daml_lexer.py
--rw-r--r--   0        0        0      252 2023-05-01 04:00:01.492149 dazl-8.0.0a4/python/dazl/pretty/table/__init__.py
--rw-r--r--   0        0        0      733 2023-05-01 04:00:01.492254 dazl-8.0.0a4/python/dazl/pretty/table/fmt_base.py
--rw-r--r--   0        0        0     1663 2023-05-01 04:00:01.492360 dazl-8.0.0a4/python/dazl/pretty/table/fmt_json.py
--rw-r--r--   0        0        0     5392 2023-05-01 04:00:01.492492 dazl-8.0.0a4/python/dazl/pretty/table/fmt_pretty.py
--rw-r--r--   0        0        0     3162 2023-05-01 04:00:01.492608 dazl-8.0.0a4/python/dazl/pretty/table/model.py
--rw-r--r--   0        0        0     1553 2023-05-01 04:00:01.492716 dazl-8.0.0a4/python/dazl/pretty/table/write.py
--rw-r--r--   0        0        0     3318 2023-10-02 16:56:57.196883 dazl-8.0.0a4/python/dazl/pretty/util.py
--rw-r--r--   0        0        0     1709 2023-05-01 04:00:01.493000 dazl-8.0.0a4/python/dazl/prim/__init__.py
--rw-r--r--   0        0        0     1635 2023-10-02 16:56:57.197062 dazl-8.0.0a4/python/dazl/prim/basic.py
--rw-r--r--   0        0        0     1645 2023-10-02 16:56:57.197274 dazl-8.0.0a4/python/dazl/prim/complex.py
--rw-r--r--   0        0        0     2421 2023-05-01 04:00:01.493354 dazl-8.0.0a4/python/dazl/prim/contracts.py
--rw-r--r--   0        0        0     7009 2023-10-02 16:56:57.197600 dazl-8.0.0a4/python/dazl/prim/datetime.py
--rw-r--r--   0        0        0     1155 2023-05-01 04:00:01.493600 dazl-8.0.0a4/python/dazl/prim/errors.py
--rw-r--r--   0        0        0     1521 2023-05-01 04:00:01.493710 dazl-8.0.0a4/python/dazl/prim/json.py
--rw-r--r--   0        0        0     1398 2023-05-01 04:00:01.493816 dazl-8.0.0a4/python/dazl/prim/map.py
--rw-r--r--   0        0        0     1476 2023-05-01 04:00:01.494212 dazl-8.0.0a4/python/dazl/prim/numbers.py
--rw-r--r--   0        0        0     1001 2023-10-02 16:56:57.197836 dazl-8.0.0a4/python/dazl/prim/party.py
--rw-r--r--   0        0        0      405 2023-05-01 04:00:01.494455 dazl-8.0.0a4/python/dazl/protocols/__init__.py
--rw-r--r--   0        0        0     6120 2023-05-01 04:00:01.494576 dazl-8.0.0a4/python/dazl/protocols/_base.py
--rw-r--r--   0        0        0     9246 2023-05-01 04:00:01.495007 dazl-8.0.0a4/python/dazl/protocols/autodetect.py
--rw-r--r--   0        0        0     2927 2023-10-02 16:56:57.198219 dazl-8.0.0a4/python/dazl/protocols/core.py
--rw-r--r--   0        0        0      920 2023-05-01 04:00:01.495229 dazl-8.0.0a4/python/dazl/protocols/errors.py
--rw-r--r--   0        0        0     6889 2023-10-02 16:56:57.198488 dazl-8.0.0a4/python/dazl/protocols/events.py
--rw-r--r--   0        0        0     2337 2023-05-01 04:00:01.495667 dazl-8.0.0a4/python/dazl/protocols/oauth.py
--rw-r--r--   0        0        0     4619 2023-10-02 16:56:57.198828 dazl-8.0.0a4/python/dazl/protocols/serializers.py
--rw-r--r--   0        0        0      141 2023-01-10 03:35:07.846159 dazl-8.0.0a4/python/dazl/protocols/v1/__init__.py
--rw-r--r--   0        0        0    17052 2023-10-02 16:56:57.199149 dazl-8.0.0a4/python/dazl/protocols/v1/grpc.py
--rw-r--r--   0        0        0    16169 2023-10-02 16:56:57.199585 dazl-8.0.0a4/python/dazl/protocols/v1/pb_parse_event.py
--rw-r--r--   0        0        0     4799 2023-10-02 16:56:57.199999 dazl-8.0.0a4/python/dazl/protocols/v1/pb_ser_command.py
--rw-r--r--   0        0        0      194 2023-01-10 03:35:07.846884 dazl-8.0.0a4/python/dazl/py.typed
--rw-r--r--   0        0        0     4796 2023-10-03 01:19:39.932122 dazl-8.0.0a4/python/dazl/query/__init__.py
--rw-r--r--   0        0        0      270 2023-05-01 04:00:01.496577 dazl-8.0.0a4/python/dazl/scheduler/__init__.py
--rw-r--r--   0        0        0     1318 2023-10-02 16:56:57.200560 dazl-8.0.0a4/python/dazl/scheduler/_base.py
--rw-r--r--   0        0        0     5076 2023-05-01 04:00:01.496805 dazl-8.0.0a4/python/dazl/scheduler/_invoker.py
--rw-r--r--   0        0        0     2062 2023-10-02 16:56:57.200782 dazl-8.0.0a4/python/dazl/scheduler/_invoker.pyi
--rw-r--r--   0        0        0      575 2023-05-01 04:00:01.497035 dazl-8.0.0a4/python/dazl/server/__init__.py
--rw-r--r--   0        0        0     3256 2023-05-01 04:00:01.497140 dazl-8.0.0a4/python/dazl/server/management.py
--rw-r--r--   0        0        0     1766 2023-10-02 16:56:57.201024 dazl-8.0.0a4/python/dazl/server/metrics.py
--rw-r--r--   0        0        0      355 2023-05-01 04:00:01.497535 dazl-8.0.0a4/python/dazl/testing/__init__.py
--rw-r--r--   0        0        0     2296 2023-10-02 16:56:57.201250 dazl-8.0.0a4/python/dazl/testing/_cert.py
--rw-r--r--   0        0        0    12650 2023-10-02 16:56:57.201494 dazl-8.0.0a4/python/dazl/testing/_sandbox.py
--rw-r--r--   0        0        0     7157 2023-10-02 16:56:57.201804 dazl-8.0.0a4/python/dazl/testing/connect.py
--rw-r--r--   0        0        0     3610 2023-09-06 00:21:45.119299 dazl-8.0.0a4/python/dazl/testing/connect.pyi
--rw-r--r--   0        0        0      488 2023-05-01 04:00:01.498081 dazl-8.0.0a4/python/dazl/util/__init__.py
--rw-r--r--   0        0        0    25721 2023-10-02 16:56:57.202050 dazl-8.0.0a4/python/dazl/util/asyncio_util.py
--rw-r--r--   0        0        0     4787 2023-10-02 16:56:57.202716 dazl-8.0.0a4/python/dazl/util/config_meta.py
--rw-r--r--   0        0        0      964 2023-05-01 04:00:01.498828 dazl-8.0.0a4/python/dazl/util/enum.py
--rw-r--r--   0        0        0     2665 2023-10-02 16:56:57.202939 dazl-8.0.0a4/python/dazl/util/io.py
--rw-r--r--   0        0        0     1224 2023-05-01 04:00:01.499045 dazl-8.0.0a4/python/dazl/util/notifications.py
--rw-r--r--   0        0        0      490 2023-05-02 01:19:18.057580 dazl-8.0.0a4/python/dazl/util/prim_natural.py
--rw-r--r--   0        0        0     3416 2023-10-02 16:56:57.203247 dazl-8.0.0a4/python/dazl/util/proc_util.py
--rw-r--r--   0        0        0     1352 2023-05-01 04:00:01.499364 dazl-8.0.0a4/python/dazl/util/termcap.py
--rw-r--r--   0        0        0     2347 2023-10-02 16:56:57.203500 dazl-8.0.0a4/python/dazl/util/tools.py
--rw-r--r--   0        0        0      890 2023-05-02 01:19:18.057977 dazl-8.0.0a4/python/dazl/util/typing.py
--rw-r--r--   0        0        0      612 2023-05-01 04:00:01.499689 dazl-8.0.0a4/python/dazl/values/__init__.py
--rw-r--r--   0        0        0     6068 2023-10-02 16:56:57.203908 dazl-8.0.0a4/python/dazl/values/canonical.py
--rw-r--r--   0        0        0    15792 2023-10-02 16:56:57.204248 dazl-8.0.0a4/python/dazl/values/context.py
--rw-r--r--   0        0        0     1881 2023-10-02 16:56:57.204412 dazl-8.0.0a4/python/dazl/values/json.py
--rw-r--r--   0        0        0     3359 2023-10-02 16:56:57.204580 dazl-8.0.0a4/python/dazl/values/mapper.py
--rw-r--r--   0        0        0     9955 2023-10-02 16:56:57.205069 dazl-8.0.0a4/python/dazl/values/protobuf.py
--rw-r--r--   0        0        0     2755 2023-10-02 16:56:57.205314 dazl-8.0.0a4/python/dazl/values/pysample_encoder.py
--rw-r--r--   0        0        0     5018 2023-10-02 16:56:57.205588 dazl-8.0.0a4/python/dazl/values/string.py
--rw-r--r--   0        0        0     4115 1970-01-01 00:00:00.000000 dazl-8.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0    11393 2024-02-17 22:53:35.749987 dazl-8.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2725 2024-02-17 22:53:35.750514 dazl-8.0.0b1/README.md
+-rw-r--r--   0        0        0     2673 2024-02-17 22:53:36.227267 dazl-8.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      333 2024-02-17 22:53:36.227347 dazl-8.0.0b1/python/_dazl/__init__.py
+-rw-r--r--   0        0        0      887 2024-02-17 22:53:36.227408 dazl-8.0.0b1/python/_dazl/__main__.py
+-rw-r--r--   0        0        0     1476 2024-02-17 22:53:36.227467 dazl-8.0.0b1/python/_dazl/_logging.py
+-rw-r--r--   0        0        0      276 2024-02-17 22:53:36.227535 dazl-8.0.0b1/python/_dazl/codegen/__init__.py
+-rw-r--r--   0        0        0     5483 2024-02-17 22:53:36.227613 dazl-8.0.0b1/python/_dazl/codegen/go.py
+-rw-r--r--   0        0        0      347 2024-02-17 22:53:36.227677 dazl-8.0.0b1/python/_dazl/codegen/go_header.py
+-rw-r--r--   0        0        0     1728 2024-02-17 22:53:36.227737 dazl-8.0.0b1/python/_dazl/codegen/python.py
+-rw-r--r--   0        0        0     5092 2024-02-17 22:53:36.227814 dazl-8.0.0b1/python/_dazl/codegen/python_grpc_pyi.py
+-rw-r--r--   0        0        0      339 2024-02-17 22:53:36.227873 dazl-8.0.0b1/python/_dazl/codegen/python_header.py
+-rw-r--r--   0        0        0     2442 2024-02-17 22:53:36.227934 dazl-8.0.0b1/python/_dazl/codegen/python_init.py
+-rw-r--r--   0        0        0      520 2024-02-17 22:53:36.227993 dazl-8.0.0b1/python/_dazl/codegen/util.py
+-rw-r--r--   0        0        0      944 2024-04-03 22:04:33.683110 dazl-8.0.0b1/python/_dazl/collections.py
+-rw-r--r--   0        0        0     4095 2024-02-17 22:53:36.228120 dazl-8.0.0b1/python/_dazl/download/__init__.py
+-rw-r--r--   0        0        0     3147 2024-02-17 22:53:36.228186 dazl-8.0.0b1/python/_dazl/protoc/__init__.py
+-rw-r--r--   0        0        0     2027 2024-04-03 22:04:33.695507 dazl-8.0.0b1/python/_dazl/protopack/__init__.py
+-rw-r--r--   0        0        0     4306 2024-02-17 22:53:36.228348 dazl-8.0.0b1/python/_dazl/protopack/rename.py
+-rw-r--r--   0        0        0     3180 2024-02-17 22:53:36.228419 dazl-8.0.0b1/python/_dazl/protopack/rewrite.py
+-rw-r--r--   0        0        0      221 2024-02-17 22:53:36.228490 dazl-8.0.0b1/python/_dazl/syntax/__init__.py
+-rw-r--r--   0        0        0      601 2024-02-17 22:53:36.228554 dazl-8.0.0b1/python/_dazl/syntax/python/__init__.py
+-rw-r--r--   0        0        0      586 2024-02-17 22:53:36.228610 dazl-8.0.0b1/python/_dazl/syntax/python/_basic.py
+-rw-r--r--   0        0        0     6389 2024-02-17 22:53:36.228696 dazl-8.0.0b1/python/_dazl/syntax/python/imports.py
+-rw-r--r--   0        0        0     2683 2024-02-17 22:53:36.228762 dazl-8.0.0b1/python/_dazl/syntax/python/pb.py
+-rw-r--r--   0        0        0     7328 2024-02-17 22:53:36.228847 dazl-8.0.0b1/python/_dazl/syntax/python/symbols.py
+-rw-r--r--   0        0        0     2793 2024-02-17 22:53:36.228907 dazl-8.0.0b1/python/_dazl/syntax/python/types.py
+-rw-r--r--   0        0        0     2188 2024-02-17 22:53:36.229013 dazl-8.0.0b1/python/_dazl/update.py
+-rw-r--r--   0        0        0     1737 2024-02-17 22:53:35.796705 dazl-8.0.0b1/python/dazl/__init__.py
+-rw-r--r--   0        0        0      311 2024-02-17 22:53:35.796859 dazl-8.0.0b1/python/dazl/__main__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797029 dazl-8.0.0b1/python/dazl/_gen/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797159 dazl-8.0.0b1/python/dazl/_gen/com/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797280 dazl-8.0.0b1/python/dazl/_gen/com/daml/__init__.py
+-rw-r--r--   0        0        0     1525 2024-02-17 22:53:36.229174 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/__init__.py
+-rw-r--r--   0        0        0    52179 2024-02-17 22:53:35.797603 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py
+-rw-r--r--   0        0        0    78370 2024-02-17 22:53:35.797866 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.pyi
+-rw-r--r--   0        0        0     2298 2024-02-17 22:53:35.798460 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py
+-rw-r--r--   0        0        0     1486 2024-02-17 22:53:35.798607 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.798740 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.798859 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/__init__.py
+-rw-r--r--   0        0        0     6188 2024-02-17 22:53:36.229442 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py
+-rw-r--r--   0        0        0     2961 2024-02-17 22:53:35.799137 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py
+-rw-r--r--   0        0        0     1801 2024-02-17 22:53:35.799270 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.pyi
+-rw-r--r--   0        0        0     4390 2024-02-17 22:53:35.799437 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2396 2024-02-17 22:53:35.799592 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4542 2024-02-17 22:53:36.229586 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py
+-rw-r--r--   0        0        0     3967 2024-02-17 22:53:35.799910 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py
+-rw-r--r--   0        0        0     2714 2024-02-17 22:53:35.800064 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.pyi
+-rw-r--r--   0        0        0     6347 2024-02-17 22:53:35.800242 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3579 2024-02-17 22:53:35.800388 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6304 2024-02-17 22:53:35.800524 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py
+-rw-r--r--   0        0        0     4309 2024-02-17 22:53:35.800651 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.pyi
+-rw-r--r--   0        0        0    17920 2024-02-17 22:53:35.800772 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8410 2024-02-17 22:53:35.800952 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3043 2024-02-17 22:53:35.801100 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py
+-rw-r--r--   0        0        0     1634 2024-02-17 22:53:35.801369 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.pyi
+-rw-r--r--   0        0        0     3683 2024-02-17 22:53:35.801517 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2333 2024-02-17 22:53:35.801662 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2218 2024-02-17 22:53:35.801796 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py
+-rw-r--r--   0        0        0     1145 2024-02-17 22:53:35.801924 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.pyi
+-rw-r--r--   0        0        0     3426 2024-02-17 22:53:35.802064 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py
+-rw-r--r--   0        0        0     2113 2024-02-17 22:53:35.802196 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.pyi
+-rw-r--r--   0        0        0     6681 2024-02-17 22:53:35.802377 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3660 2024-02-17 22:53:35.802530 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2325 2024-02-17 22:53:35.802674 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py
+-rw-r--r--   0        0        0      995 2024-02-17 22:53:35.802815 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.pyi
+-rw-r--r--   0        0        0     4791 2024-02-17 22:53:35.802976 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2225 2024-02-17 22:53:35.803122 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6691 2024-02-17 22:53:35.803305 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py
+-rw-r--r--   0        0        0     5361 2024-02-17 22:53:35.803473 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.pyi
+-rw-r--r--   0        0        0    19490 2024-02-17 22:53:35.803626 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9064 2024-02-17 22:53:35.803836 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9901 2024-02-17 22:53:35.804032 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py
+-rw-r--r--   0        0        0     8928 2024-02-17 22:53:35.804213 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.pyi
+-rw-r--r--   0        0        0    25223 2024-02-17 22:53:35.804374 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12691 2024-02-17 22:53:35.804590 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3879 2024-02-17 22:53:35.804732 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py
+-rw-r--r--   0        0        0     2724 2024-02-17 22:53:35.804879 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.pyi
+-rw-r--r--   0        0        0     7734 2024-02-17 22:53:35.805059 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3690 2024-02-17 22:53:35.805215 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3899 2024-02-17 22:53:35.805363 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py
+-rw-r--r--   0        0        0     2096 2024-02-17 22:53:35.805498 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.pyi
+-rw-r--r--   0        0        0    10939 2024-02-17 22:53:35.805669 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6396 2024-02-17 22:53:35.805827 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2250 2024-02-17 22:53:35.805984 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py
+-rw-r--r--   0        0        0      764 2024-02-17 22:53:35.806133 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.pyi
+-rw-r--r--   0        0        0     5656 2024-02-17 22:53:35.806304 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2220 2024-02-17 22:53:35.806432 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6717 2024-02-17 22:53:35.806618 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py
+-rw-r--r--   0        0        0     7479 2024-02-17 22:53:35.806802 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.pyi
+-rw-r--r--   0        0        0     2481 2024-02-17 22:53:35.806959 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py
+-rw-r--r--   0        0        0     1851 2024-02-17 22:53:35.807108 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.pyi
+-rw-r--r--   0        0        0     2007 2024-02-17 22:53:35.807250 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py
+-rw-r--r--   0        0        0     1023 2024-02-17 22:53:35.807378 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.pyi
+-rw-r--r--   0        0        0     5333 2024-02-17 22:53:35.807559 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py
+-rw-r--r--   0        0        0     6277 2024-02-17 22:53:35.807737 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.pyi
+-rw-r--r--   0        0        0     3878 2024-02-17 22:53:35.807846 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py
+-rw-r--r--   0        0        0     2869 2024-02-17 22:53:35.807954 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.pyi
+-rw-r--r--   0        0        0     5706 2024-02-17 22:53:35.808080 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3753 2024-02-17 22:53:35.808181 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7614 2024-02-17 22:53:35.808362 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py
+-rw-r--r--   0        0        0     7919 2024-02-17 22:53:35.808535 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.pyi
+-rw-r--r--   0        0        0     2840 2024-02-17 22:53:35.808687 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py
+-rw-r--r--   0        0        0     1333 2024-02-17 22:53:35.808832 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.pyi
+-rw-r--r--   0        0        0     3789 2024-02-17 22:53:35.808969 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2480 2024-02-17 22:53:35.809097 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2941 2024-02-17 22:53:35.809229 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py
+-rw-r--r--   0        0        0      712 2024-02-17 22:53:35.809371 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.pyi
+-rw-r--r--   0        0        0     4024 2024-02-17 22:53:35.809532 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2333 2024-02-17 22:53:35.809685 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2039 2024-02-17 22:53:35.809821 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py
+-rw-r--r--   0        0        0     1158 2024-02-17 22:53:35.809960 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.pyi
+-rw-r--r--   0        0        0     3815 2024-02-17 22:53:35.810109 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py
+-rw-r--r--   0        0        0     2815 2024-02-17 22:53:35.810258 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.pyi
+-rw-r--r--   0        0        0     6970 2024-02-17 22:53:35.810436 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4809 2024-02-17 22:53:35.810602 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      406 2024-02-17 22:53:35.810747 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/__init__.py
+-rw-r--r--   0        0        0     2913 2024-02-17 22:53:35.810888 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py
+-rw-r--r--   0        0        0     1550 2024-02-17 22:53:35.811025 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.pyi
+-rw-r--r--   0        0        0     5129 2024-02-17 22:53:35.811190 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3379 2024-02-17 22:53:35.811324 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3327 2024-02-17 22:53:35.811469 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py
+-rw-r--r--   0        0        0     2554 2024-02-17 22:53:35.811605 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.pyi
+-rw-r--r--   0        0        0     3685 2024-02-17 22:53:35.811740 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py
+-rw-r--r--   0        0        0     3347 2024-02-17 22:53:35.811873 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.pyi
+-rw-r--r--   0        0        0     6625 2024-02-17 22:53:35.812036 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py
+-rw-r--r--   0        0        0     5153 2024-02-17 22:53:35.812194 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.pyi
+-rw-r--r--   0        0        0    18252 2024-02-17 22:53:35.812341 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11776 2024-02-17 22:53:35.812536 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5817 2024-02-17 22:53:35.812698 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py
+-rw-r--r--   0        0        0     5978 2024-02-17 22:53:35.812851 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.pyi
+-rw-r--r--   0        0        0     3221 2024-02-17 22:53:35.812983 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py
+-rw-r--r--   0        0        0     2064 2024-02-17 22:53:35.813118 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.pyi
+-rw-r--r--   0        0        0     3207 2024-02-17 22:53:35.813255 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2293 2024-02-17 22:53:35.813390 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813522 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813647 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813766 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.814533 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/__init__.py
+-rw-r--r--   0        0        0     1940 2024-02-17 22:53:35.814700 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/__init__.py
+-rw-r--r--   0        0        0    11447 2024-02-17 22:53:36.229775 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.py
+-rw-r--r--   0        0        0     9455 2024-02-17 22:53:35.814982 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.pyi
+-rw-r--r--   0        0        0    29764 2024-02-17 22:53:35.815101 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16810 2024-02-17 22:53:35.815230 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1030 2024-02-17 22:53:35.815381 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/__init__.py
+-rw-r--r--   0        0        0     8612 2024-02-17 22:53:36.229948 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.py
+-rw-r--r--   0        0        0     9794 2024-02-17 22:53:35.815639 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.815757 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.815874 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/__init__.py
+-rw-r--r--   0        0        0     3128 2024-02-17 22:53:36.230077 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-17 22:53:36.230195 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.py
+-rw-r--r--   0        0        0     1153 2024-02-17 22:53:35.816155 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     3526 2024-02-17 22:53:35.816255 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2257 2024-02-17 22:53:35.816350 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4279 2024-02-17 22:53:36.230361 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.py
+-rw-r--r--   0        0        0     2594 2024-02-17 22:53:35.816602 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.pyi
+-rw-r--r--   0        0        0     7501 2024-02-17 22:53:35.816727 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4941 2024-02-17 22:53:35.816854 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3638 2024-02-17 22:53:36.230477 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.py
+-rw-r--r--   0        0        0      858 2024-02-17 22:53:35.817036 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.pyi
+-rw-r--r--   0        0        0    18541 2024-02-17 22:53:35.817152 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11361 2024-02-17 22:53:35.817304 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7888 2024-02-17 22:53:36.230593 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.py
+-rw-r--r--   0        0        0     4680 2024-02-17 22:53:35.817518 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.pyi
+-rw-r--r--   0        0        0    25680 2024-02-17 22:53:35.817632 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.py
+-rw-r--r--   0        0        0    15191 2024-02-17 22:53:35.817820 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3159 2024-02-17 22:53:36.230708 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.py
+-rw-r--r--   0        0        0     1904 2024-02-17 22:53:35.817978 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.pyi
+-rw-r--r--   0        0        0     5932 2024-02-17 22:53:35.818106 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3678 2024-02-17 22:53:35.818203 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4424 2024-02-17 22:53:36.230855 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.py
+-rw-r--r--   0        0        0     2976 2024-02-17 22:53:35.818423 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     3811 2024-02-17 22:53:35.818519 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2393 2024-02-17 22:53:35.818618 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3800 2024-02-17 22:53:36.230977 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.py
+-rw-r--r--   0        0        0     2706 2024-02-17 22:53:35.818787 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.pyi
+-rw-r--r--   0        0        0     5644 2024-02-17 22:53:35.818916 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3720 2024-02-17 22:53:35.819018 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4972 2024-02-17 22:53:36.231102 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.py
+-rw-r--r--   0        0        0     2651 2024-02-17 22:53:35.819215 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0    11631 2024-02-17 22:53:35.819360 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6738 2024-02-17 22:53:36.231234 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3179 2024-02-17 22:53:36.231353 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.py
+-rw-r--r--   0        0        0     2174 2024-02-17 22:53:35.819629 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.pyi
+-rw-r--r--   0        0        0     1916 2024-02-17 22:53:36.231467 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.py
+-rw-r--r--   0        0        0      368 2024-02-17 22:53:35.819790 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.pyi
+-rw-r--r--   0        0        0     3577 2024-02-17 22:53:35.819894 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2236 2024-02-17 22:53:35.819992 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      362 2024-02-17 22:53:35.820123 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/__init__.py
+-rw-r--r--   0        0        0     2632 2024-02-17 22:53:36.231585 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.py
+-rw-r--r--   0        0        0     1523 2024-02-17 22:53:35.820286 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     5711 2024-02-17 22:53:36.231714 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.py
+-rw-r--r--   0        0        0     5898 2024-02-17 22:53:35.820506 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.pyi
+-rw-r--r--   0        0        0      825 2024-02-17 22:53:35.820637 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/__init__.py
+-rw-r--r--   0        0        0     2930 2024-02-17 22:53:36.231843 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.py
+-rw-r--r--   0        0        0     1682 2024-02-17 22:53:35.820805 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     3811 2024-02-17 22:53:35.820905 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2393 2024-02-17 22:53:35.820999 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3392 2024-02-17 22:53:36.231947 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.py
+-rw-r--r--   0        0        0     2186 2024-02-17 22:53:35.821159 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     4358 2024-02-17 22:53:35.821284 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-02-17 22:53:35.821382 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.821508 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/__init__.py
+-rw-r--r--   0        0        0     2030 2024-02-17 22:53:36.232068 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/__init__.py
+-rw-r--r--   0        0        0     2000 2024-02-17 22:53:36.232185 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.py
+-rw-r--r--   0        0        0      368 2024-02-17 22:53:35.821776 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.pyi
+-rw-r--r--   0        0        0     3366 2024-02-17 22:53:35.821875 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2287 2024-02-17 22:53:35.822115 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3159 2024-02-17 22:53:36.232290 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.py
+-rw-r--r--   0        0        0     1796 2024-02-17 22:53:35.822288 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.pyi
+-rw-r--r--   0        0        0     5273 2024-02-17 22:53:35.822416 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3430 2024-02-17 22:53:35.822515 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4927 2024-02-17 22:53:36.232409 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.py
+-rw-r--r--   0        0        0     4070 2024-02-17 22:53:35.822715 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     5949 2024-02-17 22:53:35.822844 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3581 2024-02-17 22:53:35.822946 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5863 2024-02-17 22:53:36.232533 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.py
+-rw-r--r--   0        0        0     3374 2024-02-17 22:53:35.823157 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.pyi
+-rw-r--r--   0        0        0    12411 2024-02-17 22:53:35.823336 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7875 2024-02-17 22:53:35.823465 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2409 2024-02-17 22:53:36.232649 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.py
+-rw-r--r--   0        0        0     1790 2024-02-17 22:53:35.823639 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.pyi
+-rw-r--r--   0        0        0     8931 2024-02-17 22:53:36.232813 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.py
+-rw-r--r--   0        0        0     6904 2024-02-17 22:53:35.823888 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.pyi
+-rw-r--r--   0        0        0    31573 2024-02-17 22:53:35.824004 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16744 2024-02-17 22:53:35.824127 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2015 2024-02-17 22:53:36.232930 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.py
+-rw-r--r--   0        0        0      892 2024-02-17 22:53:35.824306 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.pyi
+-rw-r--r--   0        0        0      274 2024-02-17 22:53:35.824436 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/__init__.py
+-rw-r--r--   0        0        0     1978 2024-02-17 22:53:36.233033 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.py
+-rw-r--r--   0        0        0     1150 2024-02-17 22:53:35.824596 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.824718 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.824840 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/__init__.py
+-rw-r--r--   0        0        0      700 2024-02-17 22:53:35.824967 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/__init__.py
+-rw-r--r--   0        0        0     7382 2024-02-17 22:53:36.233166 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.py
+-rw-r--r--   0        0        0     7065 2024-02-17 22:53:35.825187 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.pyi
+-rw-r--r--   0        0        0     5164 2024-02-17 22:53:35.825306 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3404 2024-02-17 22:53:35.825398 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.825518 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.825643 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/__init__.py
+-rw-r--r--   0        0        0     5756 2024-02-17 22:53:35.825809 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/__init__.py
+-rw-r--r--   0        0        0    10342 2024-02-17 22:53:36.233353 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.py
+-rw-r--r--   0        0        0     7925 2024-02-17 22:53:35.826054 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.pyi
+-rw-r--r--   0        0        0    23356 2024-02-17 22:53:35.826172 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.py
+-rw-r--r--   0        0        0    14253 2024-02-17 22:53:35.826358 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2258 2024-02-17 22:53:36.233483 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.py
+-rw-r--r--   0        0        0      695 2024-02-17 22:53:35.826533 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.pyi
+-rw-r--r--   0        0        0     3721 2024-02-17 22:53:35.826633 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2024-02-17 22:53:35.826853 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5241 2024-02-17 22:53:36.233620 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.py
+-rw-r--r--   0        0        0     3208 2024-02-17 22:53:35.827057 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.pyi
+-rw-r--r--   0        0        0    11122 2024-02-17 22:53:35.827192 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6364 2024-02-17 22:53:35.827314 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11596 2024-02-17 22:53:36.233789 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.py
+-rw-r--r--   0        0        0     9525 2024-02-17 22:53:35.827546 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.pyi
+-rw-r--r--   0        0        0    33250 2024-02-17 22:53:35.827669 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.py
+-rw-r--r--   0        0        0    21002 2024-02-17 22:53:35.827795 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5534 2024-02-17 22:53:36.233920 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.py
+-rw-r--r--   0        0        0     4072 2024-02-17 22:53:35.828006 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.pyi
+-rw-r--r--   0        0        0     9898 2024-02-17 22:53:35.828138 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6176 2024-02-17 22:53:35.828263 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2249 2024-02-17 22:53:36.234035 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.py
+-rw-r--r--   0        0        0      832 2024-02-17 22:53:35.828433 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.pyi
+-rw-r--r--   0        0        0     4589 2024-02-17 22:53:35.828559 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.py
+-rw-r--r--   0        0        0     2395 2024-02-17 22:53:35.828662 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2960 2024-02-17 22:53:36.234150 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.py
+-rw-r--r--   0        0        0     2330 2024-02-17 22:53:35.828823 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.pyi
+-rw-r--r--   0        0        0     3234 2024-02-17 22:53:35.828919 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2091 2024-02-17 22:53:35.829017 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4466 2024-02-17 22:53:36.234278 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.py
+-rw-r--r--   0        0        0     1906 2024-02-17 22:53:35.829213 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.pyi
+-rw-r--r--   0        0        0    19105 2024-02-17 22:53:35.829321 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11105 2024-02-17 22:53:35.829485 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2309 2024-02-17 22:53:36.234404 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.py
+-rw-r--r--   0        0        0      911 2024-02-17 22:53:35.829672 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.pyi
+-rw-r--r--   0        0        0     5364 2024-02-17 22:53:35.829803 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3469 2024-02-17 22:53:35.829908 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2507 2024-02-17 22:53:36.234517 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.py
+-rw-r--r--   0        0        0     1047 2024-02-17 22:53:35.830088 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.pyi
+-rw-r--r--   0        0        0     3634 2024-02-17 22:53:35.830192 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2357 2024-02-17 22:53:35.830293 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5697 2024-02-17 22:53:36.234643 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.py
+-rw-r--r--   0        0        0     5622 2024-02-17 22:53:35.830510 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.pyi
+-rw-r--r--   0        0        0     7628 2024-02-17 22:53:35.830634 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4909 2024-02-17 22:53:35.830760 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.830879 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/__init__.py
+-rw-r--r--   0        0        0     1227 2024-02-17 22:53:35.831005 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/__init__.py
+-rw-r--r--   0        0        0    16269 2024-02-17 22:53:36.234874 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.py
+-rw-r--r--   0        0        0    21287 2024-02-17 22:53:35.831279 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.pyi
+-rw-r--r--   0        0        0     3318 2024-02-17 22:53:36.234997 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.py
+-rw-r--r--   0        0        0     2205 2024-02-17 22:53:35.831462 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.831586 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/__init__.py
+-rw-r--r--   0        0        0     4582 2024-02-17 22:53:36.235225 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/__init__.py
+-rw-r--r--   0        0        0     2069 2024-02-17 22:53:36.235360 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.py
+-rw-r--r--   0        0        0     1456 2024-02-17 22:53:35.831874 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.pyi
+-rw-r--r--   0        0        0     4351 2024-02-17 22:53:36.235489 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.py
+-rw-r--r--   0        0        0     4153 2024-02-17 22:53:35.832097 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.pyi
+-rw-r--r--   0        0        0     3340 2024-02-17 22:53:36.235615 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.py
+-rw-r--r--   0        0        0     3275 2024-02-17 22:53:35.832262 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.pyi
+-rw-r--r--   0        0        0     5709 2024-02-17 22:53:36.235748 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.py
+-rw-r--r--   0        0        0     5991 2024-02-17 22:53:35.832480 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.pyi
+-rw-r--r--   0        0        0     3817 2024-02-17 22:53:36.235861 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.py
+-rw-r--r--   0        0        0     4555 2024-02-17 22:53:35.832670 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.pyi
+-rw-r--r--   0        0        0     2945 2024-02-17 22:53:36.235972 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.py
+-rw-r--r--   0        0        0     2263 2024-02-17 22:53:35.832840 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.pyi
+-rw-r--r--   0        0        0    12436 2024-02-17 22:53:36.236180 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.py
+-rw-r--r--   0        0        0    15054 2024-02-17 22:53:35.833159 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     5560 2024-02-17 22:53:36.236308 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.py
+-rw-r--r--   0        0        0     5503 2024-02-17 22:53:35.833382 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.pyi
+-rw-r--r--   0        0        0     9990 2024-02-17 22:53:36.236477 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.py
+-rw-r--r--   0        0        0    12765 2024-02-17 22:53:35.833666 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.pyi
+-rw-r--r--   0        0        0     1523 2024-02-17 22:53:36.236586 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.py
+-rw-r--r--   0        0        0      709 2024-02-17 22:53:35.833833 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.pyi
+-rw-r--r--   0        0        0     5302 2024-02-17 22:53:36.236709 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.py
+-rw-r--r--   0        0        0     5427 2024-02-17 22:53:35.834062 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.pyi
+-rw-r--r--   0        0        0     2214 2024-02-17 22:53:36.236819 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.py
+-rw-r--r--   0        0        0     1634 2024-02-17 22:53:35.834226 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.pyi
+-rw-r--r--   0        0        0    11115 2024-02-17 22:53:36.236972 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.py
+-rw-r--r--   0        0        0    13925 2024-02-17 22:53:35.834499 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.pyi
+-rw-r--r--   0        0        0     2787 2024-02-17 22:53:35.834625 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/__init__.py
+-rw-r--r--   0        0        0     2404 2024-02-17 22:53:36.237090 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.py
+-rw-r--r--   0        0        0     1515 2024-02-17 22:53:35.834780 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.pyi
+-rw-r--r--   0        0        0     4869 2024-02-17 22:53:36.237227 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.py
+-rw-r--r--   0        0        0     4409 2024-02-17 22:53:35.834991 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.pyi
+-rw-r--r--   0        0        0     3035 2024-02-17 22:53:36.237347 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.py
+-rw-r--r--   0        0        0     2788 2024-02-17 22:53:35.835144 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.pyi
+-rw-r--r--   0        0        0     2945 2024-02-17 22:53:36.237462 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.py
+-rw-r--r--   0        0        0     2263 2024-02-17 22:53:35.835281 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.pyi
+-rw-r--r--   0        0        0     9401 2024-02-17 22:53:36.237635 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.py
+-rw-r--r--   0        0        0    10568 2024-02-17 22:53:35.835548 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     5513 2024-02-17 22:53:36.237766 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.py
+-rw-r--r--   0        0        0     5720 2024-02-17 22:53:35.835760 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.pyi
+-rw-r--r--   0        0        0     7000 2024-02-17 22:53:36.238013 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.py
+-rw-r--r--   0        0        0     8939 2024-02-17 22:53:35.835987 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.pyi
+-rw-r--r--   0        0        0     5100 2024-02-17 22:53:36.238150 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.py
+-rw-r--r--   0        0        0     4441 2024-02-17 22:53:35.836194 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.pyi
+-rw-r--r--   0        0        0     6336 2024-02-17 22:53:36.238289 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.py
+-rw-r--r--   0        0        0     7245 2024-02-17 22:53:35.836409 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.pyi
+-rw-r--r--   0        0        0     2342 2024-02-17 22:53:35.836543 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/__init__.py
+-rw-r--r--   0        0        0     4494 2024-02-17 22:53:36.238432 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.py
+-rw-r--r--   0        0        0     5711 2024-02-17 22:53:35.836833 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.pyi
+-rw-r--r--   0        0        0     3405 2024-02-17 22:53:36.238565 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.py
+-rw-r--r--   0        0        0     2687 2024-02-17 22:53:35.837015 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.pyi
+-rw-r--r--   0        0        0     2797 2024-02-17 22:53:36.238686 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.py
+-rw-r--r--   0        0        0     2318 2024-02-17 22:53:35.837236 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.pyi
+-rw-r--r--   0        0        0     4570 2024-02-17 22:53:36.238816 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.py
+-rw-r--r--   0        0        0     4998 2024-02-17 22:53:35.837489 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     4089 2024-02-17 22:53:36.238938 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.py
+-rw-r--r--   0        0        0     4314 2024-02-17 22:53:35.837659 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.pyi
+-rw-r--r--   0        0        0     4288 2024-02-17 22:53:36.239072 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.py
+-rw-r--r--   0        0        0     3511 2024-02-17 22:53:35.837971 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.pyi
+-rw-r--r--   0        0        0    14188 2024-02-17 22:53:36.239292 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.py
+-rw-r--r--   0        0        0    18723 2024-02-17 22:53:35.838244 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.pyi
+-rw-r--r--   0        0        0      347 2024-02-17 22:53:35.838387 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/__init__.py
+-rw-r--r--   0        0        0     3179 2024-02-17 22:53:36.239423 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.py
+-rw-r--r--   0        0        0     2681 2024-02-17 22:53:35.838556 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     4895 2024-02-17 22:53:36.239540 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.py
+-rw-r--r--   0        0        0     4326 2024-02-17 22:53:35.838746 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.838864 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.838999 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/__init__.py
+-rw-r--r--   0        0        0      501 2024-02-17 22:53:35.839158 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/__init__.py
+-rw-r--r--   0        0        0     5338 2024-02-17 22:53:36.239682 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.py
+-rw-r--r--   0        0        0     4373 2024-02-17 22:53:35.839385 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.839521 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.839653 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/__init__.py
+-rw-r--r--   0        0        0      333 2024-02-17 22:53:35.839777 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/__init__.py
+-rw-r--r--   0        0        0     2582 2024-02-17 22:53:36.239829 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.py
+-rw-r--r--   0        0        0     2054 2024-02-17 22:53:35.839944 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.pyi
+-rw-r--r--   0        0        0      242 2024-02-17 22:53:35.840071 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/__init__.py
+-rw-r--r--   0        0        0     1758 2024-02-17 22:53:36.239960 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.py
+-rw-r--r--   0        0        0      759 2024-02-17 22:53:35.840231 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.840341 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.840467 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/__init__.py
+-rw-r--r--   0        0        0     3459 2024-02-17 22:53:35.840596 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/__init__.py
+-rw-r--r--   0        0        0     2985 2024-02-17 22:53:36.240102 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.py
+-rw-r--r--   0        0        0     1696 2024-02-17 22:53:35.840769 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     7338 2024-02-17 22:53:35.840894 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4621 2024-02-17 22:53:35.841017 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5607 2024-02-17 22:53:36.240240 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.py
+-rw-r--r--   0        0        0     5171 2024-02-17 22:53:35.841241 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.pyi
+-rw-r--r--   0        0        0     8037 2024-02-17 22:53:35.841367 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3606 2024-02-17 22:53:35.841477 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19234 2024-02-17 22:53:36.240352 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.py
+-rw-r--r--   0        0        0    17700 2024-02-17 22:53:35.841687 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.pyi
+-rw-r--r--   0        0        0    26649 2024-02-17 22:53:35.841813 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16371 2024-02-17 22:53:35.842002 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9552 2024-02-17 22:53:36.240545 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.py
+-rw-r--r--   0        0        0     7723 2024-02-17 22:53:35.842226 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.pyi
+-rw-r--r--   0        0        0    23014 2024-02-17 22:53:35.842330 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.py
+-rw-r--r--   0        0        0    13350 2024-02-17 22:53:35.842512 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3466 2024-02-17 22:53:35.842643 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/__init__.py
+-rw-r--r--   0        0        0     3630 2024-02-17 22:53:36.240688 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.py
+-rw-r--r--   0        0        0     1729 2024-02-17 22:53:35.842800 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     9812 2024-02-17 22:53:35.842944 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6137 2024-02-17 22:53:35.843124 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24735 2024-02-17 22:53:36.240808 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.py
+-rw-r--r--   0        0        0    22592 2024-02-17 22:53:35.843772 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.pyi
+-rw-r--r--   0        0        0    40628 2024-02-17 22:53:35.843915 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24755 2024-02-17 22:53:35.844045 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3903 2024-02-17 22:53:36.240954 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.py
+-rw-r--r--   0        0        0     2835 2024-02-17 22:53:35.844235 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.pyi
+-rw-r--r--   0        0        0     6037 2024-02-17 22:53:35.844586 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3624 2024-02-17 22:53:35.844693 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.844828 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/__init__.py
+-rw-r--r--   0        0        0      273 2024-02-17 22:53:35.844970 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/__init__.py
+-rw-r--r--   0        0        0     2657 2024-02-17 22:53:36.241074 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.py
+-rw-r--r--   0        0        0     2008 2024-02-17 22:53:35.845143 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.pyi
+-rw-r--r--   0        0        0      251 2024-02-17 22:53:35.845284 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/__init__.py
+-rw-r--r--   0        0        0     1749 2024-02-17 22:53:36.241182 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.py
+-rw-r--r--   0        0        0      917 2024-02-17 22:53:35.845466 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.pyi
+-rw-r--r--   0        0        0      285 2024-02-17 22:53:35.845607 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/__init__.py
+-rw-r--r--   0        0        0     1672 2024-02-17 22:53:36.241311 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.py
+-rw-r--r--   0        0        0      672 2024-02-17 22:53:35.845773 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.pyi
+-rw-r--r--   0        0        0     5249 2024-02-17 22:53:35.846085 dazl-8.0.0b1/python/dazl/_logging.py
+-rw-r--r--   0        0        0      990 2024-02-17 22:53:35.846274 dazl-8.0.0b1/python/dazl/_repr/__init__.py
+-rw-r--r--   0        0        0     1722 2024-02-17 22:53:35.846434 dazl-8.0.0b1/python/dazl/cli/__init__.py
+-rw-r--r--   0        0        0      602 2024-02-17 22:53:35.846572 dazl-8.0.0b1/python/dazl/cli/_base.py
+-rw-r--r--   0        0        0     2102 2024-02-17 22:53:35.846711 dazl-8.0.0b1/python/dazl/cli/ls.py
+-rw-r--r--   0        0        0     3273 2024-02-17 22:53:35.846854 dazl-8.0.0b1/python/dazl/cli/tail.py
+-rw-r--r--   0        0        0     1233 2024-02-17 22:53:35.846993 dazl-8.0.0b1/python/dazl/cli/upload.py
+-rw-r--r--   0        0        0      490 2024-02-17 22:53:35.847143 dazl-8.0.0b1/python/dazl/cli/version.py
+-rw-r--r--   0        0        0     1036 2024-02-17 22:53:35.847287 dazl-8.0.0b1/python/dazl/client/__init__.py
+-rw-r--r--   0        0        0     1339 2024-02-17 22:53:35.847416 dazl-8.0.0b1/python/dazl/client/_base_model.py
+-rw-r--r--   0        0        0     3620 2024-02-17 22:53:35.847560 dazl-8.0.0b1/python/dazl/client/_conn_settings.py
+-rw-r--r--   0        0        0     1419 2024-02-17 22:53:35.847692 dazl-8.0.0b1/python/dazl/client/_events.py
+-rw-r--r--   0        0        0    24599 2024-02-17 22:53:35.847873 dazl-8.0.0b1/python/dazl/client/_network_client_impl.py
+-rw-r--r--   0        0        0    33712 2024-02-17 22:53:35.848079 dazl-8.0.0b1/python/dazl/client/_party_client_impl.py
+-rw-r--r--   0        0        0     4786 2024-02-17 22:53:35.848254 dazl-8.0.0b1/python/dazl/client/_reader_sync.py
+-rw-r--r--   0        0        0      870 2024-02-17 22:53:35.848380 dazl-8.0.0b1/python/dazl/client/_run_level.py
+-rw-r--r--   0        0        0     2150 2024-02-17 22:53:35.848512 dazl-8.0.0b1/python/dazl/client/_writer_verify.py
+-rw-r--r--   0        0        0    68240 2024-02-17 22:53:35.848739 dazl-8.0.0b1/python/dazl/client/api.py
+-rw-r--r--   0        0        0    19922 2024-04-03 22:04:34.042391 dazl-8.0.0b1/python/dazl/client/bots.py
+-rw-r--r--   0        0        0    11197 2024-02-17 22:53:36.241744 dazl-8.0.0b1/python/dazl/client/commands.py
+-rw-r--r--   0        0        0    18771 2024-02-17 22:53:35.849292 dazl-8.0.0b1/python/dazl/client/config.py
+-rw-r--r--   0        0        0     1307 2024-02-17 22:53:35.849438 dazl-8.0.0b1/python/dazl/client/errors.py
+-rw-r--r--   0        0        0     6863 2024-02-17 22:53:35.849586 dazl-8.0.0b1/python/dazl/client/events.py
+-rw-r--r--   0        0        0     1070 2024-02-17 22:53:35.849718 dazl-8.0.0b1/python/dazl/client/ledger.py
+-rw-r--r--   0        0        0      952 2024-02-17 22:53:35.849848 dazl-8.0.0b1/python/dazl/client/runner.py
+-rw-r--r--   0        0        0     9113 2024-02-17 22:53:35.850034 dazl-8.0.0b1/python/dazl/client/state.py
+-rw-r--r--   0        0        0     1533 2024-02-17 22:53:35.850173 dazl-8.0.0b1/python/dazl/damlast/__init__.py
+-rw-r--r--   0        0        0      440 2024-02-17 22:53:35.850301 dazl-8.0.0b1/python/dazl/damlast/_base.py
+-rw-r--r--   0        0        0     3251 2024-02-17 22:53:35.850563 dazl-8.0.0b1/python/dazl/damlast/_builtins_meta.py
+-rw-r--r--   0        0        0     2394 2024-02-17 22:53:35.850708 dazl-8.0.0b1/python/dazl/damlast/builtins.py
+-rw-r--r--   0        0        0    91575 2024-02-17 22:53:35.850968 dazl-8.0.0b1/python/dazl/damlast/daml_lf_1.py
+-rw-r--r--   0        0        0     6316 2024-02-17 22:53:35.851133 dazl-8.0.0b1/python/dazl/damlast/daml_types.py
+-rw-r--r--   0        0        0     1395 2024-02-17 22:53:35.851261 dazl-8.0.0b1/python/dazl/damlast/errors.py
+-rw-r--r--   0        0        0    12557 2024-02-17 22:53:35.851482 dazl-8.0.0b1/python/dazl/damlast/expand.py
+-rw-r--r--   0        0        0    20477 2024-02-17 22:53:35.851647 dazl-8.0.0b1/python/dazl/damlast/lookup.py
+-rw-r--r--   0        0        0     2955 2024-02-17 22:53:35.851800 dazl-8.0.0b1/python/dazl/damlast/parse.py
+-rw-r--r--   0        0        0    45323 2024-02-17 22:53:35.851985 dazl-8.0.0b1/python/dazl/damlast/pb_parse.py
+-rw-r--r--   0        0        0     8997 2024-02-17 22:53:35.852177 dazl-8.0.0b1/python/dazl/damlast/pkgfile.py
+-rw-r--r--   0        0        0     4855 2024-02-17 22:53:35.852319 dazl-8.0.0b1/python/dazl/damlast/protocols.py
+-rw-r--r--   0        0        0     2938 2024-02-17 22:53:35.852452 dazl-8.0.0b1/python/dazl/damlast/types.py
+-rw-r--r--   0        0        0     5978 2024-02-17 22:53:35.852598 dazl-8.0.0b1/python/dazl/damlast/util.py
+-rw-r--r--   0        0        0    14983 2024-02-17 22:53:35.852807 dazl-8.0.0b1/python/dazl/damlast/visitor.py
+-rw-r--r--   0        0        0    27127 2024-02-17 22:53:35.852970 dazl-8.0.0b1/python/dazl/ledger/__init__.py
+-rw-r--r--   0        0        0    11396 2024-02-17 22:53:36.241948 dazl-8.0.0b1/python/dazl/ledger/__init__.pyi
+-rw-r--r--   0        0        0     2324 2024-02-17 22:53:35.853318 dazl-8.0.0b1/python/dazl/ledger/_offsets.py
+-rw-r--r--   0        0        0     1652 2024-02-17 22:53:35.853444 dazl-8.0.0b1/python/dazl/ledger/_retry.py
+-rw-r--r--   0        0        0     6622 2024-02-17 22:53:35.853593 dazl-8.0.0b1/python/dazl/ledger/aio/__init__.py
+-rw-r--r--   0        0        0    11143 2024-02-17 22:53:36.242145 dazl-8.0.0b1/python/dazl/ledger/aio/__init__.pyi
+-rw-r--r--   0        0        0     5890 2024-02-17 22:53:35.853898 dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader.py
+-rw-r--r--   0        0        0     3404 2024-02-17 22:53:35.854036 dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader_compat.py
+-rw-r--r--   0        0        0    24190 2024-02-17 22:53:36.242330 dazl-8.0.0b1/python/dazl/ledger/api_types.py
+-rw-r--r--   0        0        0     2117 2024-02-17 22:53:35.854345 dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.py
+-rw-r--r--   0        0        0     7058 2024-02-17 22:53:36.242521 dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.pyi
+-rw-r--r--   0        0        0     6846 2024-02-17 22:53:35.854636 dazl-8.0.0b1/python/dazl/ledger/blocking/_aiowrapper.py
+-rw-r--r--   0        0        0     5937 2024-02-17 22:53:35.854781 dazl-8.0.0b1/python/dazl/ledger/blocking/pkgloader.py
+-rw-r--r--   0        0        0    18153 2024-02-17 22:53:36.242680 dazl-8.0.0b1/python/dazl/ledger/config/__init__.py
+-rw-r--r--   0        0        0    20662 2024-02-17 22:53:36.242858 dazl-8.0.0b1/python/dazl/ledger/config/access.py
+-rw-r--r--   0        0        0    14197 2024-02-17 22:53:35.855738 dazl-8.0.0b1/python/dazl/ledger/config/argv.py
+-rw-r--r--   0        0        0      304 2024-02-17 22:53:35.855868 dazl-8.0.0b1/python/dazl/ledger/config/exc.py
+-rw-r--r--   0        0        0      343 2024-02-17 22:53:36.242964 dazl-8.0.0b1/python/dazl/ledger/config/log.py
+-rw-r--r--   0        0        0     2881 2024-02-17 22:53:36.243096 dazl-8.0.0b1/python/dazl/ledger/config/ssl.py
+-rw-r--r--   0        0        0    10455 2024-04-03 22:04:34.069311 dazl-8.0.0b1/python/dazl/ledger/config/url.py
+-rw-r--r--   0        0        0     4761 2024-02-17 22:53:35.856335 dazl-8.0.0b1/python/dazl/ledger/errors.py
+-rw-r--r--   0        0        0      475 2024-02-17 22:53:35.856470 dazl-8.0.0b1/python/dazl/ledger/grpc/__init__.py
+-rw-r--r--   0        0        0     1188 2024-02-17 22:53:36.243409 dazl-8.0.0b1/python/dazl/ledger/grpc/__init__.pyi
+-rw-r--r--   0        0        0     6459 2024-02-17 22:53:35.856863 dazl-8.0.0b1/python/dazl/ledger/grpc/channel.py
+-rw-r--r--   0        0        0    18849 2024-02-17 22:53:35.857023 dazl-8.0.0b1/python/dazl/ledger/grpc/codec_aio.py
+-rw-r--r--   0        0        0    47346 2024-02-17 22:53:36.243593 dazl-8.0.0b1/python/dazl/ledger/grpc/conn_aio.py
+-rw-r--r--   0        0        0      313 2024-02-17 22:53:35.857372 dazl-8.0.0b1/python/dazl/ledger/pkgcache.py
+-rw-r--r--   0        0        0      290 2024-02-17 22:53:35.857502 dazl-8.0.0b1/python/dazl/ledgerutil/__init__.py
+-rw-r--r--   0        0        0    17303 2024-02-17 22:53:35.857651 dazl-8.0.0b1/python/dazl/ledgerutil/acs.py
+-rw-r--r--   0        0        0     1883 2024-02-17 22:53:35.857792 dazl-8.0.0b1/python/dazl/ledgerutil/fetch.py
+-rw-r--r--   0        0        0      208 2024-02-17 22:53:35.857969 dazl-8.0.0b1/python/dazl/metrics/__init__.py
+-rw-r--r--   0        0        0      991 2024-02-17 22:53:35.858113 dazl-8.0.0b1/python/dazl/metrics/api.py
+-rw-r--r--   0        0        0     1614 2024-02-17 22:53:35.858277 dazl-8.0.0b1/python/dazl/metrics/instrumenters.py
+-rw-r--r--   0        0        0     1592 2024-02-17 22:53:35.858537 dazl-8.0.0b1/python/dazl/metrics/prometheus.py
+-rw-r--r--   0        0        0      829 2024-02-17 22:53:35.858713 dazl-8.0.0b1/python/dazl/pretty/__init__.py
+-rw-r--r--   0        0        0      877 2024-02-17 22:53:35.858915 dazl-8.0.0b1/python/dazl/pretty/pygments_daml_lexer.py
+-rw-r--r--   0        0        0      252 2024-02-17 22:53:35.859109 dazl-8.0.0b1/python/dazl/pretty/table/__init__.py
+-rw-r--r--   0        0        0      733 2024-02-17 22:53:35.859269 dazl-8.0.0b1/python/dazl/pretty/table/fmt_base.py
+-rw-r--r--   0        0        0     1663 2024-02-17 22:53:35.859475 dazl-8.0.0b1/python/dazl/pretty/table/fmt_json.py
+-rw-r--r--   0        0        0     5392 2024-02-17 22:53:35.859789 dazl-8.0.0b1/python/dazl/pretty/table/fmt_pretty.py
+-rw-r--r--   0        0        0     3162 2024-02-17 22:53:35.860082 dazl-8.0.0b1/python/dazl/pretty/table/model.py
+-rw-r--r--   0        0        0     1553 2024-02-17 22:53:35.860329 dazl-8.0.0b1/python/dazl/pretty/table/write.py
+-rw-r--r--   0        0        0     3318 2024-02-17 22:53:35.860492 dazl-8.0.0b1/python/dazl/pretty/util.py
+-rw-r--r--   0        0        0     1733 2024-02-17 22:53:36.243742 dazl-8.0.0b1/python/dazl/prim/__init__.py
+-rw-r--r--   0        0        0     1635 2024-02-17 22:53:35.860901 dazl-8.0.0b1/python/dazl/prim/basic.py
+-rw-r--r--   0        0        0     1645 2024-02-17 22:53:35.861044 dazl-8.0.0b1/python/dazl/prim/complex.py
+-rw-r--r--   0        0        0     2421 2024-02-17 22:53:35.861220 dazl-8.0.0b1/python/dazl/prim/contracts.py
+-rw-r--r--   0        0        0     7009 2024-02-17 22:53:35.861382 dazl-8.0.0b1/python/dazl/prim/datetime.py
+-rw-r--r--   0        0        0     1155 2024-02-17 22:53:35.861521 dazl-8.0.0b1/python/dazl/prim/errors.py
+-rw-r--r--   0        0        0     1521 2024-02-17 22:53:35.861669 dazl-8.0.0b1/python/dazl/prim/json.py
+-rw-r--r--   0        0        0     1398 2024-02-17 22:53:35.861826 dazl-8.0.0b1/python/dazl/prim/map.py
+-rw-r--r--   0        0        0     1476 2024-02-17 22:53:35.861995 dazl-8.0.0b1/python/dazl/prim/numbers.py
+-rw-r--r--   0        0        0     1144 2024-04-03 22:04:34.052818 dazl-8.0.0b1/python/dazl/prim/party.py
+-rw-r--r--   0        0        0      405 2024-02-17 22:53:35.862535 dazl-8.0.0b1/python/dazl/protocols/__init__.py
+-rw-r--r--   0        0        0     6120 2024-02-17 22:53:35.862723 dazl-8.0.0b1/python/dazl/protocols/_base.py
+-rw-r--r--   0        0        0     9246 2024-02-17 22:53:35.863100 dazl-8.0.0b1/python/dazl/protocols/autodetect.py
+-rw-r--r--   0        0        0     2927 2024-02-17 22:53:35.863392 dazl-8.0.0b1/python/dazl/protocols/core.py
+-rw-r--r--   0        0        0      891 2024-02-17 22:53:36.243999 dazl-8.0.0b1/python/dazl/protocols/errors.py
+-rw-r--r--   0        0        0     6889 2024-02-17 22:53:35.863784 dazl-8.0.0b1/python/dazl/protocols/events.py
+-rw-r--r--   0        0        0     2337 2024-02-17 22:53:35.864028 dazl-8.0.0b1/python/dazl/protocols/oauth.py
+-rw-r--r--   0        0        0     4619 2024-02-17 22:53:35.864252 dazl-8.0.0b1/python/dazl/protocols/serializers.py
+-rw-r--r--   0        0        0      141 2024-02-17 22:53:35.864476 dazl-8.0.0b1/python/dazl/protocols/v1/__init__.py
+-rw-r--r--   0        0        0    17052 2024-02-17 22:53:35.864680 dazl-8.0.0b1/python/dazl/protocols/v1/grpc.py
+-rw-r--r--   0        0        0    16229 2024-02-17 22:53:35.864920 dazl-8.0.0b1/python/dazl/protocols/v1/pb_parse_event.py
+-rw-r--r--   0        0        0     4799 2024-02-17 22:53:35.865063 dazl-8.0.0b1/python/dazl/protocols/v1/pb_ser_command.py
+-rw-r--r--   0        0        0      194 2024-02-17 22:53:35.865241 dazl-8.0.0b1/python/dazl/py.typed
+-rw-r--r--   0        0        0     4796 2024-02-17 22:53:35.865561 dazl-8.0.0b1/python/dazl/query/__init__.py
+-rw-r--r--   0        0        0      270 2024-02-17 22:53:35.865783 dazl-8.0.0b1/python/dazl/scheduler/__init__.py
+-rw-r--r--   0        0        0     1318 2024-02-17 22:53:35.865997 dazl-8.0.0b1/python/dazl/scheduler/_base.py
+-rw-r--r--   0        0        0     5076 2024-02-17 22:53:35.866174 dazl-8.0.0b1/python/dazl/scheduler/_invoker.py
+-rw-r--r--   0        0        0     2062 2024-02-17 22:53:35.866302 dazl-8.0.0b1/python/dazl/scheduler/_invoker.pyi
+-rw-r--r--   0        0        0      575 2024-02-17 22:53:35.866428 dazl-8.0.0b1/python/dazl/server/__init__.py
+-rw-r--r--   0        0        0     3256 2024-02-17 22:53:35.866567 dazl-8.0.0b1/python/dazl/server/management.py
+-rw-r--r--   0        0        0     1766 2024-02-17 22:53:35.866693 dazl-8.0.0b1/python/dazl/server/metrics.py
+-rw-r--r--   0        0        0      355 2024-02-17 22:53:35.866819 dazl-8.0.0b1/python/dazl/testing/__init__.py
+-rw-r--r--   0        0        0     2296 2024-02-17 22:53:35.866945 dazl-8.0.0b1/python/dazl/testing/_cert.py
+-rw-r--r--   0        0        0    12650 2024-02-17 22:53:35.867157 dazl-8.0.0b1/python/dazl/testing/_sandbox.py
+-rw-r--r--   0        0        0     7137 2024-02-17 22:53:36.244158 dazl-8.0.0b1/python/dazl/testing/connect.py
+-rw-r--r--   0        0        0     3403 2024-02-17 22:53:36.244285 dazl-8.0.0b1/python/dazl/testing/connect.pyi
+-rw-r--r--   0        0        0      488 2024-02-17 22:53:35.867581 dazl-8.0.0b1/python/dazl/util/__init__.py
+-rw-r--r--   0        0        0    19677 2024-02-17 22:53:36.244448 dazl-8.0.0b1/python/dazl/util/asyncio_util.py
+-rw-r--r--   0        0        0     4795 2024-04-03 22:04:34.110861 dazl-8.0.0b1/python/dazl/util/config_meta.py
+-rw-r--r--   0        0        0      964 2024-02-17 22:53:35.868034 dazl-8.0.0b1/python/dazl/util/enum.py
+-rw-r--r--   0        0        0     2657 2024-04-03 22:04:34.095373 dazl-8.0.0b1/python/dazl/util/io.py
+-rw-r--r--   0        0        0      521 2024-02-17 22:53:36.244591 dazl-8.0.0b1/python/dazl/util/prim_natural.py
+-rw-r--r--   0        0        0     3515 2024-02-17 22:53:36.244719 dazl-8.0.0b1/python/dazl/util/proc_util.py
+-rw-r--r--   0        0        0     1391 2024-02-17 22:53:36.244841 dazl-8.0.0b1/python/dazl/util/termcap.py
+-rw-r--r--   0        0        0     2347 2024-02-17 22:53:35.868846 dazl-8.0.0b1/python/dazl/util/tools.py
+-rw-r--r--   0        0        0      890 2024-02-17 22:53:35.868988 dazl-8.0.0b1/python/dazl/util/typing.py
+-rw-r--r--   0        0        0      612 2024-02-17 22:53:35.869136 dazl-8.0.0b1/python/dazl/values/__init__.py
+-rw-r--r--   0        0        0     6068 2024-02-17 22:53:35.869300 dazl-8.0.0b1/python/dazl/values/canonical.py
+-rw-r--r--   0        0        0    15792 2024-02-17 22:53:35.869533 dazl-8.0.0b1/python/dazl/values/context.py
+-rw-r--r--   0        0        0     1881 2024-02-17 22:53:35.869663 dazl-8.0.0b1/python/dazl/values/json.py
+-rw-r--r--   0        0        0     3359 2024-02-17 22:53:35.869788 dazl-8.0.0b1/python/dazl/values/mapper.py
+-rw-r--r--   0        0        0     9955 2024-02-17 22:53:35.869972 dazl-8.0.0b1/python/dazl/values/protobuf.py
+-rw-r--r--   0        0        0     2755 2024-02-17 22:53:35.870119 dazl-8.0.0b1/python/dazl/values/pysample_encoder.py
+-rw-r--r--   0        0        0     5018 2024-02-17 22:53:35.870284 dazl-8.0.0b1/python/dazl/values/string.py
+-rw-r--r--   0        0        0     4166 1970-01-01 00:00:00.000000 dazl-8.0.0b1/PKG-INFO
```

### Comparing `dazl-8.0.0a4/LICENSE` & `dazl-8.0.0b1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates
+   Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dazl-8.0.0a4/README.md` & `dazl-8.0.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 =============================================
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/digital-asset/dazl-client/blob/main/LICENSE)
 <a href="https://circleci.com/gh/digital-asset/dazl-client">
 <img src="https://circleci.com/gh/digital-asset/dazl-client.svg?style=svg">
 </a>
 
-Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All Rights Reserved.
+Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All Rights Reserved.
 SPDX-License-Identifier: Apache-2.0
 
 
 Rich Python bindings for accessing Ledger API-based applications.
 
 Documentation
 -------------
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 Daml Python bindings (formerly known as dazl)
 ============================================= [![License](https://
 img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/
 digital-asset/dazl-client/blob/main/LICENSE) _[_h_t_t_p_s_:_/_/_c_i_r_c_l_e_c_i_._c_o_m_/_g_h_/_d_i_g_i_t_a_l_-
-_a_s_s_e_t_/_d_a_z_l_-_c_l_i_e_n_t_._s_v_g_?_s_t_y_l_e_=_s_v_g_]Copyright (c) 2017-2023 Digital Asset
+_a_s_s_e_t_/_d_a_z_l_-_c_l_i_e_n_t_._s_v_g_?_s_t_y_l_e_=_s_v_g_]Copyright (c) 2017-2024 Digital Asset
 (Switzerland) GmbH and/or its affiliates. All Rights Reserved. SPDX-License-
 Identifier: Apache-2.0 Rich Python bindings for accessing Ledger API-based
 applications. Documentation ------------- The user documentation is available
 online [here](https://digital-asset.github.io/dazl-client). Installation ------
 ------ If you just want to use the library, you can install it locally with
 `pip`: ```sh pip install --user dazl ``` Requirements ------------ * Python
 3.7+ * [Daml Connect](https://www.daml.com) * Python gRPC libraries (1.32.0 or
```

### Comparing `dazl-8.0.0a4/pyproject.toml` & `dazl-8.0.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "dazl"
-version = "8.0.0a4"
+version = "8.0.0b1"
 description = "high-level Ledger API client for Daml ledgers"
 license = "Apache-2.0"
 authors = ["Davin K. Tanabe <davin.tanabe@digitalasset.com>"]
 readme = 'README.md'
 repository = "https://github.com/digital-asset/dazl-client"
 homepage = "https://github.com/digital-asset/dazl-client"
 keywords = ["daml", "blockchain", "dlt", "distributed ledger", "digital asset"]
-packages = [{ include = "dazl", from = "python" }, { include = "_dazl_pb", from = "python" }]
+packages = [{ include = "dazl", from = "python" }, { include = "_dazl", from = "python" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = { version = "*", optional = true }
 google-auth = { version = "*", optional = true }
 googleapis_common_protos = "^1"
 grpcio = ">=1.50.0"
@@ -25,58 +25,70 @@
 pygments = { version = "*", optional = true }
 pyOpenSSL = { version = "*", optional = true }
 requests = "*"
 semver = "*"
 toposort = "*"
 typing_extensions = { version = "*" }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.extras]
+oauth = ["google-auth", "oauthlib"]
+prometheus = ["prometheus_client"]
+pygments = ["pygments"]
+server = ["aiohttp"]
+tls-testing = ["pyOpenSSL"]
+
+[tool.poetry.scripts]
+dazl = 'dazl.cli:main'
+
+[tool.poetry.group.dev.dependencies]
 black = "*"
 cryptography = "*"
 grpc-stubs = "*"
 grpcio-tools = ">=1.50.0"
 isort = "^5"
+jinja2 = "^3"
 mypy = "*"
 pyjwt = "*"
 pytest = "*"
 pytest-asyncio = "*"
+rich = "^13.7.0"
 setuptools = "*"
 sphinx = "*"
 sphinx-autobuild = "*"
 sphinx-markdown-builder = "*"
 types-protobuf = "*"
 types-pyOpenSSL = "*"
 types-requests = "*"
 types-setuptools = "*"
 watchdog = "*"
 
-[tool.poetry.extras]
-oauth = ["google-auth", "oauthlib"]
-prometheus = ["prometheus_client"]
-pygments = ["pygments"]
-server = ["aiohttp"]
-tls-testing = ["pyOpenSSL"]
-
-[tool.poetry.scripts]
-dazl = 'dazl.cli:main'
-protoc-gen-dazl-go = '_dazl_pb.plugin_go:main'
-protoc-gen-dazl-python = '_dazl_pb.plugin_python:main'
-
 [tool.black]
 line-length = 100
 
 [tool.isort]
 add_imports = ["from __future__ import annotations"]
 combine_as_imports = true
 combine_star = true
 force_sort_within_sections = true
 group_by_package = true
 include_trailing_comma = true
 line_length = 100
 multi_line_output = 3
 
+[tool.mypy]
+cache_dir = '.cache/mypy'
+namespace_packages = true
+
+[[tool.mypy.overrides]]
+module = ['google._upb.*', 'google.auth.transport.*', 'google.oauth2.credentials.*', 'google.protobuf.pyext.*', 'google.rpc.*', 'google.rpc.status_pb2.*', 'grpc._cython.*', 'grpc.aio.*', 'grpc_tools.*', 'prometheus_client.*', 'psutil.*', 'pygments.*', 'semver.*', 'toposort.*']
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 cache_dir = ".cache/pytest"
 log_cli = true
 log_cli_level = "DEBUG"
 junit_family = "xunit1"
 testpaths = ["python/tests/structure", "python/tests/unit"]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/collections.py` & `dazl-8.0.0b1/python/_dazl/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from collections import defaultdict
 from types import MappingProxyType
 from typing import Any, Collection, DefaultDict, Mapping, Optional, Protocol, Set, TypeVar
 
 __all__ = ["merge"]
 
 
 class SupportsLessThan(Protocol):
-    def __lt__(self, other: Any, /) -> bool:
-        ...
+    def __lt__(self, other: Any, /) -> bool: ...
 
 
 K = TypeVar("K")
 V = TypeVar("V", bound=SupportsLessThan)  # noqa: Y001
 
 
 def merge(*m: Optional[Mapping[K, Collection[V]]]) -> Mapping[K, Collection[V]]:
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_grpc_pyi.py` & `dazl-8.0.0b1/python/_dazl/codegen/python_grpc_pyi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from io import StringIO
-import os
+from pathlib import Path
 from typing import TextIO
 
-from google.protobuf.compiler.plugin_pb2 import CodeGeneratorRequest, CodeGeneratorResponse
-from google.protobuf.descriptor_pb2 import FileDescriptorProto, ServiceDescriptorProto
+from google.protobuf.descriptor_pb2 import (
+    FileDescriptorProto,
+    FileDescriptorSet,
+    ServiceDescriptorProto,
+)
 
-from .. import util
 from ..syntax.python import ImportContext, SymbolTable, Usage, all_decl, py_service_package
-from ._header import HEADER
+from .python_header import HEADER
+from .util import get_root_name
 
-__all__ = ["run_plugin"]
+__all__ = ["write_grpc_pyi_files"]
 
 
-def run_plugin(request: CodeGeneratorRequest) -> CodeGeneratorResponse:
+def write_grpc_pyi_files(fds: FileDescriptorSet, to: Path) -> None:
     """
     Generate .pyi (typing stubs files) for gPRC services.
     """
     # build a mapping of all types that we'll ever need to generate any of the requested files
     symbol_table = SymbolTable()
-    for fd in request.proto_file:
-        symbol_table.load_file(fd)
+    for f in fds.file:
+        symbol_table.load_file(f)
 
-    request = util.services_only(request)
+    for f in fds.file:
+        if f.service:
+            root_name, _ = get_root_name(f.name)
+            content = typing_file(f, ImportContext(symbol_table))
+            p = to / (root_name + "_pb2_grpc.pyi")
+            p.write_text(content)
 
-    return CodeGeneratorResponse(
-        file=[
-            typing_file(pf, ImportContext(symbol_table))
-            for pf in request.proto_file
-            if pf.name in request.file_to_generate
-        ]
-    )
 
-
-def typing_file(fd: FileDescriptorProto, ictx: ImportContext) -> CodeGeneratorResponse.File:
-    name = os.path.splitext(fd.name)[0] + "_pb2_grpc.pyi"
+def typing_file(fd: FileDescriptorProto, ictx: ImportContext) -> str:
     with StringIO() as buf:
         for sd in fd.service:
             write_service(buf, sd, ictx)
 
         body = buf.getvalue()
 
     ictx.add_system_import("", "builtins as _builtins")
@@ -50,15 +49,15 @@
     ictx.add_import("", "grpc as _grpc")
     ictx.add_import("grpc", "aio as _grpc_aio")
 
     imports = ictx.py_import_block(py_service_package(fd.name))
 
     all_str = all_decl(md.name + "Stub" for md in fd.service)
 
-    return CodeGeneratorResponse.File(name=name, content=f"{HEADER}\n{imports}\n{all_str}\n{body}")
+    return f"{HEADER}\n{imports}\n{all_str}\n{body}"
 
 
 def write_service(buf: TextIO, sd: ServiceDescriptorProto, ictx: ImportContext) -> None:
     buf.write("\n")
 
     with StringIO() as stub_buf, StringIO() as abuf, StringIO() as bbuf:
         astub = f"_{sd.name}AsyncStub"
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/plugin_python/plugin_init.py` & `dazl-8.0.0b1/python/_dazl/codegen/python_init.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from collections import defaultdict
-from io import StringIO
-from os.path import basename, dirname, splitext
+from os.path import basename, dirname
+from pathlib import Path
 from typing import DefaultDict, Set
 
-from google.protobuf.compiler.plugin_pb2 import CodeGeneratorRequest, CodeGeneratorResponse
+from google.protobuf.descriptor_pb2 import FileDescriptorSet
 
 from ..syntax.python import all_decl
-from ._header import HEADER
+from .python_header import HEADER
+from .util import get_root_name
 
-__all__ = ["run_plugin"]
+__all__ = ["write_init_files"]
 
 
-def run_plugin(request: CodeGeneratorRequest) -> CodeGeneratorResponse:
+def write_init_files(fds: FileDescriptorSet, to: Path) -> None:
     """
-    Create `__init__.py` files for all directories.
+    Write __init__.py files next to the generated Protobuf files.
     """
-    directories = set()
+    plan = defaultdict(list)
+
+    # organize our Protobuf files by enclosing directory
+    for fd in fds.file:
+        if (
+            fd.name.startswith("com/daml") or fd.name.startswith("com/digitalasset")
+        ) and not fd.name.endswith(".pyi"):
+            plan[dirname(fd.name)].append(fd)
+
+    # for each directory we identified, make sure there is an entry for all of their parent
+    # directories too; we may also want to generate empty __init__ files
+    for directory in list(plan):
+        components = directory.split("/")
+        for i in range(0, len(components)):
+            _ = plan["/".join(components[:i])]
+
+    for directory, files in plan.items():
+        import_map = defaultdict(set)  # type: DefaultDict[str, Set[str]]
+        for file in files:
+            current_module_base = basename(get_root_name(file.name)[0])
 
-    # for all of the requested files, add those files' parent directories, and the parents of all
-    # THOSE directories
-    for proto_dir in {dirname(f) for f in request.file_to_generate}:
-        components = proto_dir.split("/")
-        for i in range(0, len(components) + 1):
-            directories.add("/".join(components[:i]))
-
-    return CodeGeneratorResponse(
-        file=[package_file(proto_dir, request) for proto_dir in sorted(directories)]
-    )
-
-
-def package_file(proto_dir: str, request: CodeGeneratorRequest) -> CodeGeneratorResponse.File:
-    proto_package = proto_dir.replace("/", ".")
-
-    import_map = defaultdict(set)  # type: DefaultDict[str, Set[str]]
-    for file in request.proto_file:
-        if file.package == proto_package:
-            current_module_base = splitext(basename(file.name))[0]
             current_module_pb = "." + current_module_base + "_pb2"
             current_module_grpc = "." + current_module_base + "_pb2_grpc"
             for e in file.enum_type:
                 import_map[current_module_pb].add(e.name)
             for m in file.message_type:
                 import_map[current_module_pb].add(m.name)
             for s in file.service:
                 import_map[current_module_grpc].add(s.name + "Stub")
 
-    with StringIO() as buf:
-        buf.write(HEADER)
-        buf.write("\n")
-        all_symbols = set()
-        for f, i in import_map.items():
-            buf.write(f"from {f} import {', '.join(sorted(i))}\n")
-            all_symbols.update(i)
-        buf.write("\n")
-        buf.write(all_decl(sorted(all_symbols)))
-
-        return CodeGeneratorResponse.File(name=f"{proto_dir}/__init__.py", content=buf.getvalue())
+        d = to / directory
+        d.mkdir(parents=True, exist_ok=True)
+        p = d / "__init__.py"
+        with p.open("w") as buf:
+            buf.write(HEADER)
+            buf.write("\n")
+
+            all_symbols = set()  # type: Set[str]
+            for f, imports in import_map.items():
+                buf.write(f"from {f} import {', '.join(sorted(imports))}\n")
+                all_symbols.update(imports)
+            buf.write("\n")
+            buf.write(all_decl(sorted(all_symbols)))
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/syntax/python/__init__.py` & `dazl-8.0.0b1/python/_dazl/syntax/python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from ._basic import all_decl
 from .imports import ImportContext, rewrite_file_content
 from .pb import py_message_package, py_scalar_type, py_service_package
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/syntax/python/_basic.py` & `dazl-8.0.0b1/python/_dazl/syntax/python/_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from io import StringIO
 from typing import Iterable
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/syntax/python/imports.py` & `dazl-8.0.0b1/python/_dazl/syntax/python/imports.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from collections import defaultdict
 from io import StringIO
+from os.path import commonprefix
 import re
 from typing import Collection, DefaultDict, Dict, Iterable, Mapping, Sequence, Set, Union
 
 from google.protobuf.descriptor_pb2 import FieldDescriptorProto
 
 from .symbols import SymbolTable, Usage
 from .types import PyType
@@ -56,15 +57,15 @@
         relative_imports = {}  # type: Dict[str, Collection[str]]
 
         for from_, imports_ in sorted(self.required_imports().items()):
             if from_ == relative_to:
                 # we don't need to include imports to our own file
                 continue
 
-            elif from_.startswith("com.daml."):
+            elif from_.startswith("com.daml.") or from_.startswith("com.digitalasset."):
                 # rewrite our own imports as relative imports
                 relative_imports[relative_package(relative_to, from_)] = imports_
 
             else:
                 absolute_imports[from_] = imports_
 
         import_groups = [
@@ -126,24 +127,49 @@
     :param name: The name of the ``.proto`` file.
     :param content: The original content from the Protobuf compiler.
     :return: The contents of the file, with imports modified.
     """
     current_module = name.rpartition("/")[0].replace("/", ".")
     with StringIO() as out_buf, StringIO(content) as in_buf:
         for line in in_buf.readlines():
-            out_buf.write(rewrite_import(current_module, line))
+            if should_ignore_for_mypy(line):
+                out_buf.write(line.rstrip() + "  # type: ignore\n")
+            else:
+                out_buf.write(rewrite_import(current_module, line))
         return out_buf.getvalue()
 
 
+def should_ignore_for_mypy(line: str) -> bool:
+    """
+    Determine if the specified line of Python code might make mypy upset.
+    """
+    return (
+        # the default pyi plugin doesn't add type annotations for slots
+        # for empty messages, and mypy gets upset about this
+        line.strip() == "__slots__ = []"
+        or
+        # the Value object in the Ledger API names a field bool, and so
+        # mypy gets annoyed with the generated code because `bool` is seen
+        # as a type as well as a variable, even though it's legal Python
+        "bool: bool" in line
+    )
+
+
 def rewrite_import(parent_module: str, line: str) -> str:
     result = FROM.match(line)
     if result:
         module_name = result.group(1)
         identifier_name = result.group(2)
         local_name = result.group(3)
-        if module_name.startswith("google."):
-            # don't rewrite Google imports; simply do nothing
-            return line
+
         if module_name == parent_module:
             return f"from . import {identifier_name} as {local_name}\n"
+        elif module_name.startswith("com.digitalasset.") or module_name.startswith("com.daml."):
+            module_components = module_name.split(".")
+            parent_components = parent_module.split(".")
+
+            prefix_len = len(commonprefix((module_components, parent_components)))
+            dots_up = len(parent_components) - prefix_len
+
+            return f"from .{dots_up * '.'}{'.'.join(module_components[prefix_len:])} import {identifier_name} as {local_name}\n"
 
     return line
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/syntax/python/pb.py` & `dazl-8.0.0b1/python/_dazl/syntax/python/pb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import os
 from typing import Optional
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/syntax/python/symbols.py` & `dazl-8.0.0b1/python/_dazl/syntax/python/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Dict, List, Tuple, Union
```

### Comparing `dazl-8.0.0a4/python/_dazl_pb/syntax/python/types.py` & `dazl-8.0.0b1/python/_dazl/syntax/python/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Collection, Mapping, Optional
 
 from ...collections import merge
```

### Comparing `dazl-8.0.0a4/python/dazl/__init__.py` & `dazl-8.0.0b1/python/dazl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains the Python API for interacting with the Ledger API.
 """
 from __future__ import annotations
 
@@ -60,8 +60,8 @@
     from google.protobuf.pyext import _message
 
     _message.SetAllowOversizeProtos(True)
 except ImportError:
     pass
 
 
-__version__ = "8.0.0a4"
+__version__ = "8.0.0b1"
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/daml_lf_1_15/daml_lf_1.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/daml_lf_1_15/daml_lf.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 from .contract_metadata_pb2 import ContractMetadata
 from .value_pb2 import Enum, GenMap, Identifier, List, Map, Optional, Record, RecordField, Value, Variant
-from .commands_pb2 import Command, Commands, CreateAndExerciseCommand, CreateCommand, DisclosedContract, ExerciseByKeyCommand, ExerciseCommand
-from .completion_pb2 import Completion
 from .event_pb2 import ArchivedEvent, CreatedEvent, Event, ExercisedEvent, InterfaceView
-from .experimental_features_pb2 import AcsActiveAtOffsetFeature, CommandDeduplicationFeatures, CommandDeduplicationPeriodSupport, CommandDeduplicationType, ExperimentalCommitterEventLog, ExperimentalContractIds, ExperimentalExplicitDisclosure, ExperimentalFeatures, ExperimentalOptionalLedgerId, ExperimentalSelfServiceErrorCodes, ExperimentalStaticTime, ExperimentalUserAndPartyLocalMetadataExtensions
-from .ledger_offset_pb2 import LedgerOffset
-from .transaction_pb2 import Transaction, TransactionTree, TreeEvent
 from .transaction_filter_pb2 import Filters, InclusiveFilters, InterfaceFilter, TransactionFilter
 from .active_contracts_service_pb2 import GetActiveContractsRequest, GetActiveContractsResponse
 from .active_contracts_service_pb2_grpc import ActiveContractsServiceStub
+from .completion_pb2 import Completion
+from .ledger_offset_pb2 import LedgerOffset
 from .command_completion_service_pb2 import Checkpoint, CompletionEndRequest, CompletionEndResponse, CompletionStreamRequest, CompletionStreamResponse
 from .command_completion_service_pb2_grpc import CommandCompletionServiceStub
+from .commands_pb2 import Command, Commands, CreateAndExerciseCommand, CreateCommand, DisclosedContract, ExerciseByKeyCommand, ExerciseCommand
+from .transaction_pb2 import Transaction, TransactionTree, TreeEvent
 from .command_service_pb2 import SubmitAndWaitForTransactionIdResponse, SubmitAndWaitForTransactionResponse, SubmitAndWaitForTransactionTreeResponse, SubmitAndWaitRequest
 from .command_service_pb2_grpc import CommandServiceStub
 from .command_submission_service_pb2 import SubmitRequest
 from .command_submission_service_pb2_grpc import CommandSubmissionServiceStub
 from .event_query_service_pb2 import GetEventsByContractIdRequest, GetEventsByContractIdResponse, GetEventsByContractKeyRequest, GetEventsByContractKeyResponse
 from .event_query_service_pb2_grpc import EventQueryServiceStub
+from .experimental_features_pb2 import AcsActiveAtOffsetFeature, CommandDeduplicationFeatures, CommandDeduplicationPeriodSupport, CommandDeduplicationType, ExperimentalCommitterEventLog, ExperimentalContractIds, ExperimentalExplicitDisclosure, ExperimentalFeatures, ExperimentalOptionalLedgerId, ExperimentalSelfServiceErrorCodes, ExperimentalStaticTime, ExperimentalUserAndPartyLocalMetadataExtensions
 from .ledger_configuration_service_pb2 import GetLedgerConfigurationRequest, GetLedgerConfigurationResponse, LedgerConfiguration
 from .ledger_configuration_service_pb2_grpc import LedgerConfigurationServiceStub
 from .ledger_identity_service_pb2 import GetLedgerIdentityRequest, GetLedgerIdentityResponse
 from .ledger_identity_service_pb2_grpc import LedgerIdentityServiceStub
 from .package_service_pb2 import GetPackageRequest, GetPackageResponse, GetPackageStatusRequest, GetPackageStatusResponse, HashFunction, ListPackagesRequest, ListPackagesResponse, PackageStatus
 from .package_service_pb2_grpc import PackageServiceStub
 from .transaction_service_pb2 import GetFlatTransactionResponse, GetLatestPrunedOffsetsRequest, GetLatestPrunedOffsetsResponse, GetLedgerEndRequest, GetLedgerEndResponse, GetTransactionByEventIdRequest, GetTransactionByIdRequest, GetTransactionResponse, GetTransactionTreesResponse, GetTransactionsRequest, GetTransactionsResponse
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/active_contracts_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import active_contracts_service_pb2 as com_dot_daml_dot_ledger_dot_api_dot_v1_dot_active__contracts__service__pb2
 
 
 class ActiveContractsServiceStub(object):
     """Allows clients to initialize themselves according to a fairly recent state of the ledger without reading through all transactions that were committed since the ledger's creation.
+    In V2 Ledger API this service is not available anymore. Use v2.StateService instead.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -24,14 +25,15 @@
                 request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_active__contracts__service__pb2.GetActiveContractsRequest.SerializeToString,
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_active__contracts__service__pb2.GetActiveContractsResponse.FromString,
                 )
 
 
 class ActiveContractsServiceServicer(object):
     """Allows clients to initialize themselves according to a fairly recent state of the ledger without reading through all transactions that were committed since the ledger's creation.
+    In V2 Ledger API this service is not available anymore. Use v2.StateService instead.
     """
 
     def GetActiveContracts(self, request, context):
         """Returns a stream of the snapshot of the active contracts at a ledger offset.
         If there are no active contracts, the stream returns a single response message with the offset at which the snapshot has been taken.
         Clients SHOULD use the offset in the last GetActiveContractsResponse message to continue streaming transactions with the transaction service.
         Clients SHOULD NOT assume that the set of active contracts they receive reflects the state at the ledger end.
@@ -53,14 +55,15 @@
             'com.daml.ledger.api.v1.ActiveContractsService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ActiveContractsService(object):
     """Allows clients to initialize themselves according to a fairly recent state of the ledger without reading through all transactions that were committed since the ledger's creation.
+    In V2 Ledger API this service is not available anymore. Use v2.StateService instead.
     """
 
     @staticmethod
     def GetActiveContracts(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
-from .object_meta_pb2 import ObjectMeta
 from .config_management_service_pb2 import GetTimeModelRequest, GetTimeModelResponse, SetTimeModelRequest, SetTimeModelResponse, TimeModel
 from .config_management_service_pb2_grpc import ConfigManagementServiceStub
 from .identity_provider_config_service_pb2 import CreateIdentityProviderConfigRequest, CreateIdentityProviderConfigResponse, DeleteIdentityProviderConfigRequest, DeleteIdentityProviderConfigResponse, GetIdentityProviderConfigRequest, GetIdentityProviderConfigResponse, IdentityProviderConfig, ListIdentityProviderConfigsRequest, ListIdentityProviderConfigsResponse, UpdateIdentityProviderConfigRequest, UpdateIdentityProviderConfigResponse
 from .identity_provider_config_service_pb2_grpc import IdentityProviderConfigServiceStub
 from .metering_report_service_pb2 import GetMeteringReportRequest, GetMeteringReportResponse
 from .metering_report_service_pb2_grpc import MeteringReportServiceStub
+from .object_meta_pb2 import ObjectMeta
 from .package_management_service_pb2 import ListKnownPackagesRequest, ListKnownPackagesResponse, PackageDetails, UploadDarFileRequest, UploadDarFileResponse
 from .package_management_service_pb2_grpc import PackageManagementServiceStub
 from .participant_pruning_service_pb2 import PruneRequest, PruneResponse
 from .participant_pruning_service_pb2_grpc import ParticipantPruningServiceStub
-from .party_management_service_pb2 import AllocatePartyRequest, AllocatePartyResponse, GetParticipantIdRequest, GetParticipantIdResponse, GetPartiesRequest, GetPartiesResponse, ListKnownPartiesRequest, ListKnownPartiesResponse, PartyDetails, UpdatePartyDetailsRequest, UpdatePartyDetailsResponse
+from .party_management_service_pb2 import AllocatePartyRequest, AllocatePartyResponse, GetParticipantIdRequest, GetParticipantIdResponse, GetPartiesRequest, GetPartiesResponse, ListKnownPartiesRequest, ListKnownPartiesResponse, PartyDetails, UpdatePartyDetailsRequest, UpdatePartyDetailsResponse, UpdatePartyIdentityProviderRequest, UpdatePartyIdentityProviderResponse
 from .party_management_service_pb2_grpc import PartyManagementServiceStub
-from .user_management_service_pb2 import CreateUserRequest, CreateUserResponse, DeleteUserRequest, DeleteUserResponse, GetUserRequest, GetUserResponse, GrantUserRightsRequest, GrantUserRightsResponse, ListUserRightsRequest, ListUserRightsResponse, ListUsersRequest, ListUsersResponse, RevokeUserRightsRequest, RevokeUserRightsResponse, Right, UpdateUserRequest, UpdateUserResponse, User
+from .user_management_service_pb2 import CreateUserRequest, CreateUserResponse, DeleteUserRequest, DeleteUserResponse, GetUserRequest, GetUserResponse, GrantUserRightsRequest, GrantUserRightsResponse, ListUserRightsRequest, ListUserRightsResponse, ListUsersRequest, ListUsersResponse, RevokeUserRightsRequest, RevokeUserRightsResponse, Right, UpdateUserIdentityProviderRequest, UpdateUserIdentityProviderResponse, UpdateUserRequest, UpdateUserResponse, User
 from .user_management_service_pb2_grpc import UserManagementServiceStub
 
 __all__ = [
     "AllocatePartyRequest",
     "AllocatePartyResponse",
     "ConfigManagementServiceStub",
     "CreateIdentityProviderConfigRequest",
@@ -72,14 +72,18 @@
     "SetTimeModelRequest",
     "SetTimeModelResponse",
     "TimeModel",
     "UpdateIdentityProviderConfigRequest",
     "UpdateIdentityProviderConfigResponse",
     "UpdatePartyDetailsRequest",
     "UpdatePartyDetailsResponse",
+    "UpdatePartyIdentityProviderRequest",
+    "UpdatePartyIdentityProviderResponse",
+    "UpdateUserIdentityProviderRequest",
+    "UpdateUserIdentityProviderResponse",
     "UpdateUserRequest",
     "UpdateUserResponse",
     "UploadDarFileRequest",
     "UploadDarFileResponse",
     "User",
     "UserManagementServiceStub",
 ]
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/config_management_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
@@ -12,14 +12,15 @@
 class ConfigManagementServiceStub(object):
     """Status: experimental interface, will change before it is deemed production
     ready
 
     The ledger configuration management service provides methods for the ledger administrator
     to change the current ledger configuration. The services provides methods to modify
     different aspects of the configuration.
+    In V2 Ledger API this service is not available anymore.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -39,14 +40,15 @@
 class ConfigManagementServiceServicer(object):
     """Status: experimental interface, will change before it is deemed production
     ready
 
     The ledger configuration management service provides methods for the ledger administrator
     to change the current ledger configuration. The services provides methods to modify
     different aspects of the configuration.
+    In V2 Ledger API this service is not available anymore.
     """
 
     def GetTimeModel(self, request, context):
         """Return the currently active time model and the current configuration generation.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -82,14 +84,15 @@
 class ConfigManagementService(object):
     """Status: experimental interface, will change before it is deemed production
     ready
 
     The ledger configuration management service provides methods for the ledger administrator
     to change the current ledger configuration. The services provides methods to modify
     different aspects of the configuration.
+    In V2 Ledger API this service is not available anymore.
     """
 
     @staticmethod
     def GetTimeModel(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/identity_provider_config_service.proto
 """Generated protocol buffer code."""
@@ -14,40 +14,40 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nCcom/daml/ledger/api/v1/admin/identity_provider_config_service.proto\x12\x1c\x63om.daml.ledger.api.v1.admin\x1a google/protobuf/field_mask.proto\"\xa4\x01\n\x16IdentityProviderConfig\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\x12%\n\x0eis_deactivated\x18\x02 \x01(\x08R\risDeactivated\x12\x16\n\x06issuer\x18\x03 \x01(\tR\x06issuer\x12\x19\n\x08jwks_url\x18\x04 \x01(\tR\x07jwksUrl\"\x95\x01\n#CreateIdentityProviderConfigRequest\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"\x96\x01\n$CreateIdentityProviderConfigResponse\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"T\n GetIdentityProviderConfigRequest\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\"\x93\x01\n!GetIdentityProviderConfigResponse\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"$\n\"ListIdentityProviderConfigsRequest\"\x97\x01\n#ListIdentityProviderConfigsResponse\x12p\n\x19identity_provider_configs\x18\x01 \x03(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x17identityProviderConfigs\"\xd2\x01\n#UpdateIdentityProviderConfigRequest\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\x12;\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\"\x96\x01\n$UpdateIdentityProviderConfigResponse\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"W\n#DeleteIdentityProviderConfigRequest\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\"&\n$DeleteIdentityProviderConfigResponse2\xdb\x06\n\x1dIdentityProviderConfigService\x12\xa5\x01\n\x1c\x43reateIdentityProviderConfig\x12\x41.com.daml.ledger.api.v1.admin.CreateIdentityProviderConfigRequest\x1a\x42.com.daml.ledger.api.v1.admin.CreateIdentityProviderConfigResponse\x12\x9c\x01\n\x19GetIdentityProviderConfig\x12>.com.daml.ledger.api.v1.admin.GetIdentityProviderConfigRequest\x1a?.com.daml.ledger.api.v1.admin.GetIdentityProviderConfigResponse\x12\xa5\x01\n\x1cUpdateIdentityProviderConfig\x12\x41.com.daml.ledger.api.v1.admin.UpdateIdentityProviderConfigRequest\x1a\x42.com.daml.ledger.api.v1.admin.UpdateIdentityProviderConfigResponse\x12\xa2\x01\n\x1bListIdentityProviderConfigs\x12@.com.daml.ledger.api.v1.admin.ListIdentityProviderConfigsRequest\x1a\x41.com.daml.ledger.api.v1.admin.ListIdentityProviderConfigsResponse\x12\xa5\x01\n\x1c\x44\x65leteIdentityProviderConfig\x12\x41.com.daml.ledger.api.v1.admin.DeleteIdentityProviderConfigRequest\x1a\x42.com.daml.ledger.api.v1.admin.DeleteIdentityProviderConfigResponseB\xb3\x01\n\x1c\x63om.daml.ledger.api.v1.adminB\'IdentityProviderConfigServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\xaa\x02\x1c\x43om.Daml.Ledger.Api.V1.Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nCcom/daml/ledger/api/v1/admin/identity_provider_config_service.proto\x12\x1c\x63om.daml.ledger.api.v1.admin\x1a google/protobuf/field_mask.proto\"\xc0\x01\n\x16IdentityProviderConfig\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\x12%\n\x0eis_deactivated\x18\x02 \x01(\x08R\risDeactivated\x12\x16\n\x06issuer\x18\x03 \x01(\tR\x06issuer\x12\x19\n\x08jwks_url\x18\x04 \x01(\tR\x07jwksUrl\x12\x1a\n\x08\x61udience\x18\x05 \x01(\tR\x08\x61udience\"\x95\x01\n#CreateIdentityProviderConfigRequest\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"\x96\x01\n$CreateIdentityProviderConfigResponse\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"T\n GetIdentityProviderConfigRequest\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\"\x93\x01\n!GetIdentityProviderConfigResponse\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"$\n\"ListIdentityProviderConfigsRequest\"\x97\x01\n#ListIdentityProviderConfigsResponse\x12p\n\x19identity_provider_configs\x18\x01 \x03(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x17identityProviderConfigs\"\xd2\x01\n#UpdateIdentityProviderConfigRequest\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\x12;\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\"\x96\x01\n$UpdateIdentityProviderConfigResponse\x12n\n\x18identity_provider_config\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.IdentityProviderConfigR\x16identityProviderConfig\"W\n#DeleteIdentityProviderConfigRequest\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\"&\n$DeleteIdentityProviderConfigResponse2\xdb\x06\n\x1dIdentityProviderConfigService\x12\xa5\x01\n\x1c\x43reateIdentityProviderConfig\x12\x41.com.daml.ledger.api.v1.admin.CreateIdentityProviderConfigRequest\x1a\x42.com.daml.ledger.api.v1.admin.CreateIdentityProviderConfigResponse\x12\x9c\x01\n\x19GetIdentityProviderConfig\x12>.com.daml.ledger.api.v1.admin.GetIdentityProviderConfigRequest\x1a?.com.daml.ledger.api.v1.admin.GetIdentityProviderConfigResponse\x12\xa5\x01\n\x1cUpdateIdentityProviderConfig\x12\x41.com.daml.ledger.api.v1.admin.UpdateIdentityProviderConfigRequest\x1a\x42.com.daml.ledger.api.v1.admin.UpdateIdentityProviderConfigResponse\x12\xa2\x01\n\x1bListIdentityProviderConfigs\x12@.com.daml.ledger.api.v1.admin.ListIdentityProviderConfigsRequest\x1a\x41.com.daml.ledger.api.v1.admin.ListIdentityProviderConfigsResponse\x12\xa5\x01\n\x1c\x44\x65leteIdentityProviderConfig\x12\x41.com.daml.ledger.api.v1.admin.DeleteIdentityProviderConfigRequest\x1a\x42.com.daml.ledger.api.v1.admin.DeleteIdentityProviderConfigResponseB\xb3\x01\n\x1c\x63om.daml.ledger.api.v1.adminB\'IdentityProviderConfigServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\xaa\x02\x1c\x43om.Daml.Ledger.Api.V1.Adminb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'com.daml.ledger.api.v1.admin.identity_provider_config_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.daml.ledger.api.v1.adminB\'IdentityProviderConfigServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\252\002\034Com.Daml.Ledger.Api.V1.Admin'
   _globals['_IDENTITYPROVIDERCONFIG']._serialized_start=136
-  _globals['_IDENTITYPROVIDERCONFIG']._serialized_end=300
-  _globals['_CREATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=303
-  _globals['_CREATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=452
-  _globals['_CREATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=455
-  _globals['_CREATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=605
-  _globals['_GETIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=607
-  _globals['_GETIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=691
-  _globals['_GETIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=694
-  _globals['_GETIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=841
-  _globals['_LISTIDENTITYPROVIDERCONFIGSREQUEST']._serialized_start=843
-  _globals['_LISTIDENTITYPROVIDERCONFIGSREQUEST']._serialized_end=879
-  _globals['_LISTIDENTITYPROVIDERCONFIGSRESPONSE']._serialized_start=882
-  _globals['_LISTIDENTITYPROVIDERCONFIGSRESPONSE']._serialized_end=1033
-  _globals['_UPDATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=1036
-  _globals['_UPDATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=1246
-  _globals['_UPDATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=1249
-  _globals['_UPDATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=1399
-  _globals['_DELETEIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=1401
-  _globals['_DELETEIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=1488
-  _globals['_DELETEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=1490
-  _globals['_DELETEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=1528
-  _globals['_IDENTITYPROVIDERCONFIGSERVICE']._serialized_start=1531
-  _globals['_IDENTITYPROVIDERCONFIGSERVICE']._serialized_end=2390
+  _globals['_IDENTITYPROVIDERCONFIG']._serialized_end=328
+  _globals['_CREATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=331
+  _globals['_CREATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=480
+  _globals['_CREATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=483
+  _globals['_CREATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=633
+  _globals['_GETIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=635
+  _globals['_GETIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=719
+  _globals['_GETIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=722
+  _globals['_GETIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=869
+  _globals['_LISTIDENTITYPROVIDERCONFIGSREQUEST']._serialized_start=871
+  _globals['_LISTIDENTITYPROVIDERCONFIGSREQUEST']._serialized_end=907
+  _globals['_LISTIDENTITYPROVIDERCONFIGSRESPONSE']._serialized_start=910
+  _globals['_LISTIDENTITYPROVIDERCONFIGSRESPONSE']._serialized_end=1061
+  _globals['_UPDATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=1064
+  _globals['_UPDATEIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=1274
+  _globals['_UPDATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=1277
+  _globals['_UPDATEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=1427
+  _globals['_DELETEIDENTITYPROVIDERCONFIGREQUEST']._serialized_start=1429
+  _globals['_DELETEIDENTITYPROVIDERCONFIGREQUEST']._serialized_end=1516
+  _globals['_DELETEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_start=1518
+  _globals['_DELETEIDENTITYPROVIDERCONFIGRESPONSE']._serialized_end=1556
+  _globals['_IDENTITYPROVIDERCONFIGSERVICE']._serialized_start=1559
+  _globals['_IDENTITYPROVIDERCONFIGSERVICE']._serialized_end=2418
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/metering_report_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/object_meta.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/package_management_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/participant_pruning_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/party_management_service.proto
 """Generated protocol buffer code."""
@@ -15,15 +15,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import object_meta_pb2 as com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_object__meta__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;com/daml/ledger/api/v1/admin/party_management_service.proto\x12\x1c\x63om.daml.ledger.api.v1.admin\x1a.com/daml/ledger/api/v1/admin/object_meta.proto\x1a google/protobuf/field_mask.proto\"\x19\n\x17GetParticipantIdRequest\"A\n\x18GetParticipantIdResponse\x12%\n\x0eparticipant_id\x18\x01 \x01(\tR\rparticipantId\"_\n\x11GetPartiesRequest\x12\x18\n\x07parties\x18\x01 \x03(\tR\x07parties\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"e\n\x12GetPartiesResponse\x12O\n\rparty_details\x18\x01 \x03(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"K\n\x17ListKnownPartiesRequest\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\"k\n\x18ListKnownPartiesResponse\x12O\n\rparty_details\x18\x01 \x03(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"\xe0\x01\n\x14\x41llocatePartyRequest\x12\"\n\rparty_id_hint\x18\x01 \x01(\tR\x0bpartyIdHint\x12!\n\x0c\x64isplay_name\x18\x02 \x01(\tR\x0b\x64isplayName\x12O\n\x0elocal_metadata\x18\x03 \x01(\x0b\x32(.com.daml.ledger.api.v1.admin.ObjectMetaR\rlocalMetadata\x12\x30\n\x14identity_provider_id\x18\x04 \x01(\tR\x12identityProviderId\"h\n\x15\x41llocatePartyResponse\x12O\n\rparty_details\x18\x01 \x01(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"\xa9\x01\n\x19UpdatePartyDetailsRequest\x12O\n\rparty_details\x18\x01 \x01(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\x12;\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\"m\n\x1aUpdatePartyDetailsResponse\x12O\n\rparty_details\x18\x01 \x01(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"\xe5\x01\n\x0cPartyDetails\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12!\n\x0c\x64isplay_name\x18\x02 \x01(\tR\x0b\x64isplayName\x12\x19\n\x08is_local\x18\x03 \x01(\x08R\x07isLocal\x12O\n\x0elocal_metadata\x18\x04 \x01(\x0b\x32(.com.daml.ledger.api.v1.admin.ObjectMetaR\rlocalMetadata\x12\x30\n\x14identity_provider_id\x18\x05 \x01(\tR\x12identityProviderId2\x95\x05\n\x16PartyManagementService\x12\x81\x01\n\x10GetParticipantId\x12\x35.com.daml.ledger.api.v1.admin.GetParticipantIdRequest\x1a\x36.com.daml.ledger.api.v1.admin.GetParticipantIdResponse\x12o\n\nGetParties\x12/.com.daml.ledger.api.v1.admin.GetPartiesRequest\x1a\x30.com.daml.ledger.api.v1.admin.GetPartiesResponse\x12\x81\x01\n\x10ListKnownParties\x12\x35.com.daml.ledger.api.v1.admin.ListKnownPartiesRequest\x1a\x36.com.daml.ledger.api.v1.admin.ListKnownPartiesResponse\x12x\n\rAllocateParty\x12\x32.com.daml.ledger.api.v1.admin.AllocatePartyRequest\x1a\x33.com.daml.ledger.api.v1.admin.AllocatePartyResponse\x12\x87\x01\n\x12UpdatePartyDetails\x12\x37.com.daml.ledger.api.v1.admin.UpdatePartyDetailsRequest\x1a\x38.com.daml.ledger.api.v1.admin.UpdatePartyDetailsResponseB\xac\x01\n\x1c\x63om.daml.ledger.api.v1.adminB PartyManagementServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\xaa\x02\x1c\x43om.Daml.Ledger.Api.V1.Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;com/daml/ledger/api/v1/admin/party_management_service.proto\x12\x1c\x63om.daml.ledger.api.v1.admin\x1a.com/daml/ledger/api/v1/admin/object_meta.proto\x1a google/protobuf/field_mask.proto\"\x19\n\x17GetParticipantIdRequest\"A\n\x18GetParticipantIdResponse\x12%\n\x0eparticipant_id\x18\x01 \x01(\tR\rparticipantId\"_\n\x11GetPartiesRequest\x12\x18\n\x07parties\x18\x01 \x03(\tR\x07parties\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"e\n\x12GetPartiesResponse\x12O\n\rparty_details\x18\x01 \x03(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"K\n\x17ListKnownPartiesRequest\x12\x30\n\x14identity_provider_id\x18\x01 \x01(\tR\x12identityProviderId\"k\n\x18ListKnownPartiesResponse\x12O\n\rparty_details\x18\x01 \x03(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"\xe0\x01\n\x14\x41llocatePartyRequest\x12\"\n\rparty_id_hint\x18\x01 \x01(\tR\x0bpartyIdHint\x12!\n\x0c\x64isplay_name\x18\x02 \x01(\tR\x0b\x64isplayName\x12O\n\x0elocal_metadata\x18\x03 \x01(\x0b\x32(.com.daml.ledger.api.v1.admin.ObjectMetaR\rlocalMetadata\x12\x30\n\x14identity_provider_id\x18\x04 \x01(\tR\x12identityProviderId\"h\n\x15\x41llocatePartyResponse\x12O\n\rparty_details\x18\x01 \x01(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"\xa9\x01\n\x19UpdatePartyDetailsRequest\x12O\n\rparty_details\x18\x01 \x01(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\x12;\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\"m\n\x1aUpdatePartyDetailsResponse\x12O\n\rparty_details\x18\x01 \x01(\x0b\x32*.com.daml.ledger.api.v1.admin.PartyDetailsR\x0cpartyDetails\"\xe5\x01\n\x0cPartyDetails\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12!\n\x0c\x64isplay_name\x18\x02 \x01(\tR\x0b\x64isplayName\x12\x19\n\x08is_local\x18\x03 \x01(\x08R\x07isLocal\x12O\n\x0elocal_metadata\x18\x04 \x01(\x0b\x32(.com.daml.ledger.api.v1.admin.ObjectMetaR\rlocalMetadata\x12\x30\n\x14identity_provider_id\x18\x05 \x01(\tR\x12identityProviderId\"\xb8\x01\n\"UpdatePartyIdentityProviderRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12=\n\x1bsource_identity_provider_id\x18\x02 \x01(\tR\x18sourceIdentityProviderId\x12=\n\x1btarget_identity_provider_id\x18\x03 \x01(\tR\x18targetIdentityProviderId\"%\n#UpdatePartyIdentityProviderResponse2\xbc\x06\n\x16PartyManagementService\x12\x81\x01\n\x10GetParticipantId\x12\x35.com.daml.ledger.api.v1.admin.GetParticipantIdRequest\x1a\x36.com.daml.ledger.api.v1.admin.GetParticipantIdResponse\x12o\n\nGetParties\x12/.com.daml.ledger.api.v1.admin.GetPartiesRequest\x1a\x30.com.daml.ledger.api.v1.admin.GetPartiesResponse\x12\x81\x01\n\x10ListKnownParties\x12\x35.com.daml.ledger.api.v1.admin.ListKnownPartiesRequest\x1a\x36.com.daml.ledger.api.v1.admin.ListKnownPartiesResponse\x12x\n\rAllocateParty\x12\x32.com.daml.ledger.api.v1.admin.AllocatePartyRequest\x1a\x33.com.daml.ledger.api.v1.admin.AllocatePartyResponse\x12\x87\x01\n\x12UpdatePartyDetails\x12\x37.com.daml.ledger.api.v1.admin.UpdatePartyDetailsRequest\x1a\x38.com.daml.ledger.api.v1.admin.UpdatePartyDetailsResponse\x12\xa4\x01\n\x1dUpdatePartyIdentityProviderId\x12@.com.daml.ledger.api.v1.admin.UpdatePartyIdentityProviderRequest\x1a\x41.com.daml.ledger.api.v1.admin.UpdatePartyIdentityProviderResponseB\xac\x01\n\x1c\x63om.daml.ledger.api.v1.adminB PartyManagementServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\xaa\x02\x1c\x43om.Daml.Ledger.Api.V1.Adminb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'com.daml.ledger.api.v1.admin.party_management_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.daml.ledger.api.v1.adminB PartyManagementServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\252\002\034Com.Daml.Ledger.Api.V1.Admin'
@@ -45,10 +45,14 @@
   _globals['_ALLOCATEPARTYRESPONSE']._serialized_end=986
   _globals['_UPDATEPARTYDETAILSREQUEST']._serialized_start=989
   _globals['_UPDATEPARTYDETAILSREQUEST']._serialized_end=1158
   _globals['_UPDATEPARTYDETAILSRESPONSE']._serialized_start=1160
   _globals['_UPDATEPARTYDETAILSRESPONSE']._serialized_end=1269
   _globals['_PARTYDETAILS']._serialized_start=1272
   _globals['_PARTYDETAILS']._serialized_end=1501
-  _globals['_PARTYMANAGEMENTSERVICE']._serialized_start=1504
-  _globals['_PARTYMANAGEMENTSERVICE']._serialized_end=2165
+  _globals['_UPDATEPARTYIDENTITYPROVIDERREQUEST']._serialized_start=1504
+  _globals['_UPDATEPARTYIDENTITYPROVIDERREQUEST']._serialized_end=1688
+  _globals['_UPDATEPARTYIDENTITYPROVIDERRESPONSE']._serialized_start=1690
+  _globals['_UPDATEPARTYIDENTITYPROVIDERRESPONSE']._serialized_end=1727
+  _globals['_PARTYMANAGEMENTSERVICE']._serialized_start=1730
+  _globals['_PARTYMANAGEMENTSERVICE']._serialized_end=2558
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
@@ -14,14 +14,16 @@
     and managing the participant-local party metadata.
 
     The authorization rules for its RPCs are specified on the ``<RpcName>Request``
     messages as boolean expressions over these facts:
     (1) ``HasRight(r)`` denoting whether the authenticated user has right ``r`` and
     (2) ``IsAuthenticatedIdentityProviderAdmin(idp)`` denoting whether ``idp`` is equal to the ``identity_provider_id``
     of the authenticated user and the user has an IdentityProviderAdmin right.
+    If `identity_provider_id` is set to an empty string, then it's effectively set to the value of access token's 'iss' field if that is provided.
+    If `identity_provider_id` remains an empty string, the default identity provider will be assumed.
 
     The fields of request messages (and sub-messages) are marked either as ``Optional`` or ``Required``:
     (1) ``Optional`` denoting the client may leave the field unset when sending a request.
     (2) ``Required`` denoting the client must set the field to a non-default value when sending a request.
 
     A party details resource is described by the ``PartyDetails`` message,
     A party details resource, once it has been created, can be modified using the ``UpdatePartyDetails`` RPC.
@@ -55,25 +57,32 @@
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.AllocatePartyResponse.FromString,
                 )
         self.UpdatePartyDetails = channel.unary_unary(
                 '/com.daml.ledger.api.v1.admin.PartyManagementService/UpdatePartyDetails',
                 request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyDetailsRequest.SerializeToString,
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyDetailsResponse.FromString,
                 )
+        self.UpdatePartyIdentityProviderId = channel.unary_unary(
+                '/com.daml.ledger.api.v1.admin.PartyManagementService/UpdatePartyIdentityProviderId',
+                request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyIdentityProviderRequest.SerializeToString,
+                response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyIdentityProviderResponse.FromString,
+                )
 
 
 class PartyManagementServiceServicer(object):
     """This service allows inspecting the party management state of the ledger known to the participant
     and managing the participant-local party metadata.
 
     The authorization rules for its RPCs are specified on the ``<RpcName>Request``
     messages as boolean expressions over these facts:
     (1) ``HasRight(r)`` denoting whether the authenticated user has right ``r`` and
     (2) ``IsAuthenticatedIdentityProviderAdmin(idp)`` denoting whether ``idp`` is equal to the ``identity_provider_id``
     of the authenticated user and the user has an IdentityProviderAdmin right.
+    If `identity_provider_id` is set to an empty string, then it's effectively set to the value of access token's 'iss' field if that is provided.
+    If `identity_provider_id` remains an empty string, the default identity provider will be assumed.
 
     The fields of request messages (and sub-messages) are marked either as ``Optional`` or ``Required``:
     (1) ``Optional`` denoting the client may leave the field unset when sending a request.
     (2) ``Required`` denoting the client must set the field to a non-default value when sending a request.
 
     A party details resource is described by the ``PartyDetails`` message,
     A party details resource, once it has been created, can be modified using the ``UpdatePartyDetails`` RPC.
@@ -132,14 +141,21 @@
         """Update selected modifiable participant-local attributes of a party details resource.
         Can update the participant's local information for local parties.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UpdatePartyIdentityProviderId(self, request, context):
+        """Update the assignment of a party from one IDP to another.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_PartyManagementServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetParticipantId': grpc.unary_unary_rpc_method_handler(
                     servicer.GetParticipantId,
                     request_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.GetParticipantIdRequest.FromString,
                     response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.GetParticipantIdResponse.SerializeToString,
@@ -160,14 +176,19 @@
                     response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.AllocatePartyResponse.SerializeToString,
             ),
             'UpdatePartyDetails': grpc.unary_unary_rpc_method_handler(
                     servicer.UpdatePartyDetails,
                     request_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyDetailsRequest.FromString,
                     response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyDetailsResponse.SerializeToString,
             ),
+            'UpdatePartyIdentityProviderId': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdatePartyIdentityProviderId,
+                    request_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyIdentityProviderRequest.FromString,
+                    response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyIdentityProviderResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.daml.ledger.api.v1.admin.PartyManagementService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -176,14 +197,16 @@
     and managing the participant-local party metadata.
 
     The authorization rules for its RPCs are specified on the ``<RpcName>Request``
     messages as boolean expressions over these facts:
     (1) ``HasRight(r)`` denoting whether the authenticated user has right ``r`` and
     (2) ``IsAuthenticatedIdentityProviderAdmin(idp)`` denoting whether ``idp`` is equal to the ``identity_provider_id``
     of the authenticated user and the user has an IdentityProviderAdmin right.
+    If `identity_provider_id` is set to an empty string, then it's effectively set to the value of access token's 'iss' field if that is provided.
+    If `identity_provider_id` remains an empty string, the default identity provider will be assumed.
 
     The fields of request messages (and sub-messages) are marked either as ``Optional`` or ``Required``:
     (1) ``Optional`` denoting the client may leave the field unset when sending a request.
     (2) ``Required`` denoting the client must set the field to a non-default value when sending a request.
 
     A party details resource is described by the ``PartyDetails`` message,
     A party details resource, once it has been created, can be modified using the ``UpdatePartyDetails`` RPC.
@@ -270,7 +293,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.daml.ledger.api.v1.admin.PartyManagementService/UpdatePartyDetails',
             com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyDetailsRequest.SerializeToString,
             com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyDetailsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdatePartyIdentityProviderId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/com.daml.ledger.api.v1.admin.PartyManagementService/UpdatePartyIdentityProviderId',
+            com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyIdentityProviderRequest.SerializeToString,
+            com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_party__management__service__pb2.UpdatePartyIdentityProviderResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
 from grpc import aio as _grpc_aio
 
-from .party_management_service_pb2 import AllocatePartyRequest, AllocatePartyResponse, GetParticipantIdRequest, GetParticipantIdResponse, GetPartiesRequest, GetPartiesResponse, ListKnownPartiesRequest, ListKnownPartiesResponse, UpdatePartyDetailsRequest, UpdatePartyDetailsResponse
+from .party_management_service_pb2 import AllocatePartyRequest, AllocatePartyResponse, GetParticipantIdRequest, GetParticipantIdResponse, GetPartiesRequest, GetPartiesResponse, ListKnownPartiesRequest, ListKnownPartiesResponse, UpdatePartyDetailsRequest, UpdatePartyDetailsResponse, UpdatePartyIdentityProviderRequest, UpdatePartyIdentityProviderResponse
 
 __all__ = [
     "PartyManagementServiceStub",
 ]
 
 
 # noinspection PyPep8Naming,DuplicatedCode
@@ -24,23 +24,26 @@
     @_typing.overload
     def __new__(cls, channel: _grpc_aio.Channel) -> _PartyManagementServiceAsyncStub: ...  # type: ignore
     def GetParticipantId(self, __1: GetParticipantIdRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[GetParticipantIdResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, GetParticipantIdResponse]]: ...
     def GetParties(self, __1: GetPartiesRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[GetPartiesResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, GetPartiesResponse]]: ...
     def ListKnownParties(self, __1: ListKnownPartiesRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[ListKnownPartiesResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, ListKnownPartiesResponse]]: ...
     def AllocateParty(self, __1: AllocatePartyRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[AllocatePartyResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, AllocatePartyResponse]]: ...
     def UpdatePartyDetails(self, __1: UpdatePartyDetailsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[UpdatePartyDetailsResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, UpdatePartyDetailsResponse]]: ...
+    def UpdatePartyIdentityProviderId(self, __1: UpdatePartyIdentityProviderRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[UpdatePartyIdentityProviderResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, UpdatePartyIdentityProviderResponse]]: ...
 
 # noinspection PyPep8Naming,DuplicatedCode
 class _PartyManagementServiceBlockingStub(PartyManagementServiceStub):
     def GetParticipantId(self, __1: GetParticipantIdRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> GetParticipantIdResponse: ...
     def GetParties(self, __1: GetPartiesRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> GetPartiesResponse: ...
     def ListKnownParties(self, __1: ListKnownPartiesRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> ListKnownPartiesResponse: ...
     def AllocateParty(self, __1: AllocatePartyRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> AllocatePartyResponse: ...
     def UpdatePartyDetails(self, __1: UpdatePartyDetailsRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> UpdatePartyDetailsResponse: ...
+    def UpdatePartyIdentityProviderId(self, __1: UpdatePartyIdentityProviderRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> UpdatePartyIdentityProviderResponse: ...
 
 # noinspection PyPep8Naming,DuplicatedCode
 class _PartyManagementServiceAsyncStub(PartyManagementServiceStub):
     def GetParticipantId(self, __1: GetParticipantIdRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, GetParticipantIdResponse]: ...  # type: ignore
     def GetParties(self, __1: GetPartiesRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, GetPartiesResponse]: ...  # type: ignore
     def ListKnownParties(self, __1: ListKnownPartiesRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, ListKnownPartiesResponse]: ...  # type: ignore
     def AllocateParty(self, __1: AllocatePartyRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, AllocatePartyResponse]: ...  # type: ignore
     def UpdatePartyDetails(self, __1: UpdatePartyDetailsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, UpdatePartyDetailsResponse]: ...  # type: ignore
+    def UpdatePartyIdentityProviderId(self, __1: UpdatePartyIdentityProviderRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, UpdatePartyIdentityProviderResponse]: ...  # type: ignore
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/admin/user_management_service.proto
 """Generated protocol buffer code."""
@@ -15,15 +15,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import object_meta_pb2 as com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_object__meta__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:com/daml/ledger/api/v1/admin/user_management_service.proto\x12\x1c\x63om.daml.ledger.api.v1.admin\x1a.com/daml/ledger/api/v1/admin/object_meta.proto\x1a google/protobuf/field_mask.proto\"\xda\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rprimary_party\x18\x02 \x01(\tR\x0cprimaryParty\x12%\n\x0eis_deactivated\x18\x03 \x01(\x08R\risDeactivated\x12\x44\n\x08metadata\x18\x04 \x01(\x0b\x32(.com.daml.ledger.api.v1.admin.ObjectMetaR\x08metadata\x12\x30\n\x14identity_provider_id\x18\x05 \x01(\tR\x12identityProviderId\"\xfa\x03\n\x05Right\x12\x63\n\x11participant_admin\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.Right.ParticipantAdminH\x00R\x10participantAdmin\x12L\n\ncan_act_as\x18\x02 \x01(\x0b\x32,.com.daml.ledger.api.v1.admin.Right.CanActAsH\x00R\x08\x63\x61nActAs\x12O\n\x0b\x63\x61n_read_as\x18\x03 \x01(\x0b\x32-.com.daml.ledger.api.v1.admin.Right.CanReadAsH\x00R\tcanReadAs\x12s\n\x17identity_provider_admin\x18\x04 \x01(\x0b\x32\x39.com.daml.ledger.api.v1.admin.Right.IdentityProviderAdminH\x00R\x15identityProviderAdmin\x1a\x12\n\x10ParticipantAdmin\x1a \n\x08\x43\x61nActAs\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x1a!\n\tCanReadAs\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x1a\x17\n\x15IdentityProviderAdminB\x06\n\x04kind\"\x88\x01\n\x11\x43reateUserRequest\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\x12;\n\x06rights\x18\x02 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\"L\n\x12\x43reateUserResponse\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\"[\n\x0eGetUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"I\n\x0fGetUserResponse\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\"\x88\x01\n\x11UpdateUserRequest\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\x12;\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\"L\n\x12UpdateUserResponse\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\"^\n\x11\x44\x65leteUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"\x14\n\x12\x44\x65leteUserResponse\"\x80\x01\n\x10ListUsersRequest\x12\x1d\n\npage_token\x18\x02 \x01(\tR\tpageToken\x12\x1b\n\tpage_size\x18\x03 \x01(\x05R\x08pageSize\x12\x30\n\x14identity_provider_id\x18\x04 \x01(\tR\x12identityProviderId\"u\n\x11ListUsersResponse\x12\x38\n\x05users\x18\x01 \x03(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x05users\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"\xa0\x01\n\x16GrantUserRightsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12;\n\x06rights\x18\x02 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\x12\x30\n\x14identity_provider_id\x18\x03 \x01(\tR\x12identityProviderId\"p\n\x17GrantUserRightsResponse\x12U\n\x14newly_granted_rights\x18\x01 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x12newlyGrantedRights\"\xa1\x01\n\x17RevokeUserRightsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12;\n\x06rights\x18\x02 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\x12\x30\n\x14identity_provider_id\x18\x03 \x01(\tR\x12identityProviderId\"q\n\x18RevokeUserRightsResponse\x12U\n\x14newly_revoked_rights\x18\x01 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x12newlyRevokedRights\"b\n\x15ListUserRightsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"U\n\x16ListUserRightsResponse\x12;\n\x06rights\x18\x01 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights2\xc1\x07\n\x15UserManagementService\x12o\n\nCreateUser\x12/.com.daml.ledger.api.v1.admin.CreateUserRequest\x1a\x30.com.daml.ledger.api.v1.admin.CreateUserResponse\x12\x66\n\x07GetUser\x12,.com.daml.ledger.api.v1.admin.GetUserRequest\x1a-.com.daml.ledger.api.v1.admin.GetUserResponse\x12o\n\nUpdateUser\x12/.com.daml.ledger.api.v1.admin.UpdateUserRequest\x1a\x30.com.daml.ledger.api.v1.admin.UpdateUserResponse\x12o\n\nDeleteUser\x12/.com.daml.ledger.api.v1.admin.DeleteUserRequest\x1a\x30.com.daml.ledger.api.v1.admin.DeleteUserResponse\x12l\n\tListUsers\x12..com.daml.ledger.api.v1.admin.ListUsersRequest\x1a/.com.daml.ledger.api.v1.admin.ListUsersResponse\x12~\n\x0fGrantUserRights\x12\x34.com.daml.ledger.api.v1.admin.GrantUserRightsRequest\x1a\x35.com.daml.ledger.api.v1.admin.GrantUserRightsResponse\x12\x81\x01\n\x10RevokeUserRights\x12\x35.com.daml.ledger.api.v1.admin.RevokeUserRightsRequest\x1a\x36.com.daml.ledger.api.v1.admin.RevokeUserRightsResponse\x12{\n\x0eListUserRights\x12\x33.com.daml.ledger.api.v1.admin.ListUserRightsRequest\x1a\x34.com.daml.ledger.api.v1.admin.ListUserRightsResponseB\xab\x01\n\x1c\x63om.daml.ledger.api.v1.adminB\x1fUserManagementServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\xaa\x02\x1c\x43om.Daml.Ledger.Api.V1.Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:com/daml/ledger/api/v1/admin/user_management_service.proto\x12\x1c\x63om.daml.ledger.api.v1.admin\x1a.com/daml/ledger/api/v1/admin/object_meta.proto\x1a google/protobuf/field_mask.proto\"\xda\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rprimary_party\x18\x02 \x01(\tR\x0cprimaryParty\x12%\n\x0eis_deactivated\x18\x03 \x01(\x08R\risDeactivated\x12\x44\n\x08metadata\x18\x04 \x01(\x0b\x32(.com.daml.ledger.api.v1.admin.ObjectMetaR\x08metadata\x12\x30\n\x14identity_provider_id\x18\x05 \x01(\tR\x12identityProviderId\"\xfa\x03\n\x05Right\x12\x63\n\x11participant_admin\x18\x01 \x01(\x0b\x32\x34.com.daml.ledger.api.v1.admin.Right.ParticipantAdminH\x00R\x10participantAdmin\x12L\n\ncan_act_as\x18\x02 \x01(\x0b\x32,.com.daml.ledger.api.v1.admin.Right.CanActAsH\x00R\x08\x63\x61nActAs\x12O\n\x0b\x63\x61n_read_as\x18\x03 \x01(\x0b\x32-.com.daml.ledger.api.v1.admin.Right.CanReadAsH\x00R\tcanReadAs\x12s\n\x17identity_provider_admin\x18\x04 \x01(\x0b\x32\x39.com.daml.ledger.api.v1.admin.Right.IdentityProviderAdminH\x00R\x15identityProviderAdmin\x1a\x12\n\x10ParticipantAdmin\x1a \n\x08\x43\x61nActAs\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x1a!\n\tCanReadAs\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x1a\x17\n\x15IdentityProviderAdminB\x06\n\x04kind\"\x88\x01\n\x11\x43reateUserRequest\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\x12;\n\x06rights\x18\x02 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\"L\n\x12\x43reateUserResponse\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\"[\n\x0eGetUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"I\n\x0fGetUserResponse\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\"\x88\x01\n\x11UpdateUserRequest\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\x12;\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\"L\n\x12UpdateUserResponse\x12\x36\n\x04user\x18\x01 \x01(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x04user\"^\n\x11\x44\x65leteUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"\x14\n\x12\x44\x65leteUserResponse\"\x80\x01\n\x10ListUsersRequest\x12\x1d\n\npage_token\x18\x02 \x01(\tR\tpageToken\x12\x1b\n\tpage_size\x18\x03 \x01(\x05R\x08pageSize\x12\x30\n\x14identity_provider_id\x18\x04 \x01(\tR\x12identityProviderId\"u\n\x11ListUsersResponse\x12\x38\n\x05users\x18\x01 \x03(\x0b\x32\".com.daml.ledger.api.v1.admin.UserR\x05users\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"\xa0\x01\n\x16GrantUserRightsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12;\n\x06rights\x18\x02 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\x12\x30\n\x14identity_provider_id\x18\x03 \x01(\tR\x12identityProviderId\"p\n\x17GrantUserRightsResponse\x12U\n\x14newly_granted_rights\x18\x01 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x12newlyGrantedRights\"\xa1\x01\n\x17RevokeUserRightsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12;\n\x06rights\x18\x02 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\x12\x30\n\x14identity_provider_id\x18\x03 \x01(\tR\x12identityProviderId\"q\n\x18RevokeUserRightsResponse\x12U\n\x14newly_revoked_rights\x18\x01 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x12newlyRevokedRights\"b\n\x15ListUserRightsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x30\n\x14identity_provider_id\x18\x02 \x01(\tR\x12identityProviderId\"U\n\x16ListUserRightsResponse\x12;\n\x06rights\x18\x01 \x03(\x0b\x32#.com.daml.ledger.api.v1.admin.RightR\x06rights\"\xba\x01\n!UpdateUserIdentityProviderRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12=\n\x1bsource_identity_provider_id\x18\x02 \x01(\tR\x18sourceIdentityProviderId\x12=\n\x1btarget_identity_provider_id\x18\x03 \x01(\tR\x18targetIdentityProviderId\"$\n\"UpdateUserIdentityProviderResponse2\xe5\x08\n\x15UserManagementService\x12o\n\nCreateUser\x12/.com.daml.ledger.api.v1.admin.CreateUserRequest\x1a\x30.com.daml.ledger.api.v1.admin.CreateUserResponse\x12\x66\n\x07GetUser\x12,.com.daml.ledger.api.v1.admin.GetUserRequest\x1a-.com.daml.ledger.api.v1.admin.GetUserResponse\x12o\n\nUpdateUser\x12/.com.daml.ledger.api.v1.admin.UpdateUserRequest\x1a\x30.com.daml.ledger.api.v1.admin.UpdateUserResponse\x12o\n\nDeleteUser\x12/.com.daml.ledger.api.v1.admin.DeleteUserRequest\x1a\x30.com.daml.ledger.api.v1.admin.DeleteUserResponse\x12l\n\tListUsers\x12..com.daml.ledger.api.v1.admin.ListUsersRequest\x1a/.com.daml.ledger.api.v1.admin.ListUsersResponse\x12~\n\x0fGrantUserRights\x12\x34.com.daml.ledger.api.v1.admin.GrantUserRightsRequest\x1a\x35.com.daml.ledger.api.v1.admin.GrantUserRightsResponse\x12\x81\x01\n\x10RevokeUserRights\x12\x35.com.daml.ledger.api.v1.admin.RevokeUserRightsRequest\x1a\x36.com.daml.ledger.api.v1.admin.RevokeUserRightsResponse\x12{\n\x0eListUserRights\x12\x33.com.daml.ledger.api.v1.admin.ListUserRightsRequest\x1a\x34.com.daml.ledger.api.v1.admin.ListUserRightsResponse\x12\xa1\x01\n\x1cUpdateUserIdentityProviderId\x12?.com.daml.ledger.api.v1.admin.UpdateUserIdentityProviderRequest\x1a@.com.daml.ledger.api.v1.admin.UpdateUserIdentityProviderResponseB\xab\x01\n\x1c\x63om.daml.ledger.api.v1.adminB\x1fUserManagementServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\xaa\x02\x1c\x43om.Daml.Ledger.Api.V1.Adminb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'com.daml.ledger.api.v1.admin.user_management_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.daml.ledger.api.v1.adminB\037UserManagementServiceOuterClassZKgithub.com/digital-asset/dazl-client/v7/go/api/com/daml/ledger/api/v1/admin\252\002\034Com.Daml.Ledger.Api.V1.Admin'
@@ -67,10 +67,14 @@
   _globals['_REVOKEUSERRIGHTSREQUEST']._serialized_end=2313
   _globals['_REVOKEUSERRIGHTSRESPONSE']._serialized_start=2315
   _globals['_REVOKEUSERRIGHTSRESPONSE']._serialized_end=2428
   _globals['_LISTUSERRIGHTSREQUEST']._serialized_start=2430
   _globals['_LISTUSERRIGHTSREQUEST']._serialized_end=2528
   _globals['_LISTUSERRIGHTSRESPONSE']._serialized_start=2530
   _globals['_LISTUSERRIGHTSRESPONSE']._serialized_end=2615
-  _globals['_USERMANAGEMENTSERVICE']._serialized_start=2618
-  _globals['_USERMANAGEMENTSERVICE']._serialized_end=3579
+  _globals['_UPDATEUSERIDENTITYPROVIDERREQUEST']._serialized_start=2618
+  _globals['_UPDATEUSERIDENTITYPROVIDERREQUEST']._serialized_end=2804
+  _globals['_UPDATEUSERIDENTITYPROVIDERRESPONSE']._serialized_start=2806
+  _globals['_UPDATEUSERIDENTITYPROVIDERRESPONSE']._serialized_end=2842
+  _globals['_USERMANAGEMENTSERVICE']._serialized_start=2845
+  _globals['_USERMANAGEMENTSERVICE']._serialized_end=3970
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
@@ -16,15 +16,16 @@
     The authorization rules for its RPCs are specified on the ``<RpcName>Request``
     messages as boolean expressions over these facts:
     (1) ``HasRight(r)`` denoting whether the authenticated user has right ``r`` and
     (2) ``IsAuthenticatedUser(uid)`` denoting whether ``uid`` is the empty string or equal to the id of the authenticated user.
     (3) ``IsAuthenticatedIdentityProviderAdmin(idp)`` denoting whether ``idp`` is equal to the ``identity_provider_id``
     of the authenticated user and the user has an IdentityProviderAdmin right.
     If `user_id` is set to the empty string (the default), then the data for the authenticated user will be retrieved.
-    If `identity_provider_id` is set to the empty string, the default identity provider will be assumed.
+    If `identity_provider_id` is set to an empty string, then it's effectively set to the value of access token's 'iss' field if that is provided.
+    If `identity_provider_id` remains an empty string, the default identity provider will be assumed.
 
     The fields of request messages (and sub-messages) are marked either as ``Optional`` or ``Required``:
     (1) ``Optional`` denoting the client may leave the field unset when sending a request.
     (2) ``Required`` denoting the client must set the field to a non-default value when sending a request.
 
     A user resource consists of:
     (1) a set of properties represented by the ``User`` message,
@@ -77,28 +78,34 @@
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.RevokeUserRightsResponse.FromString,
                 )
         self.ListUserRights = channel.unary_unary(
                 '/com.daml.ledger.api.v1.admin.UserManagementService/ListUserRights',
                 request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.ListUserRightsRequest.SerializeToString,
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.ListUserRightsResponse.FromString,
                 )
+        self.UpdateUserIdentityProviderId = channel.unary_unary(
+                '/com.daml.ledger.api.v1.admin.UserManagementService/UpdateUserIdentityProviderId',
+                request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.UpdateUserIdentityProviderRequest.SerializeToString,
+                response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.UpdateUserIdentityProviderResponse.FromString,
+                )
 
 
 class UserManagementServiceServicer(object):
     """Service to manage users and their rights for interacting with the Ledger API
     served by a participant node.
 
     The authorization rules for its RPCs are specified on the ``<RpcName>Request``
     messages as boolean expressions over these facts:
     (1) ``HasRight(r)`` denoting whether the authenticated user has right ``r`` and
     (2) ``IsAuthenticatedUser(uid)`` denoting whether ``uid`` is the empty string or equal to the id of the authenticated user.
     (3) ``IsAuthenticatedIdentityProviderAdmin(idp)`` denoting whether ``idp`` is equal to the ``identity_provider_id``
     of the authenticated user and the user has an IdentityProviderAdmin right.
     If `user_id` is set to the empty string (the default), then the data for the authenticated user will be retrieved.
-    If `identity_provider_id` is set to the empty string, the default identity provider will be assumed.
+    If `identity_provider_id` is set to an empty string, then it's effectively set to the value of access token's 'iss' field if that is provided.
+    If `identity_provider_id` remains an empty string, the default identity provider will be assumed.
 
     The fields of request messages (and sub-messages) are marked either as ``Optional`` or ``Required``:
     (1) ``Optional`` denoting the client may leave the field unset when sending a request.
     (2) ``Required`` denoting the client must set the field to a non-default value when sending a request.
 
     A user resource consists of:
     (1) a set of properties represented by the ``User`` message,
@@ -163,14 +170,21 @@
     def ListUserRights(self, request, context):
         """List the set of all rights granted to a user.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UpdateUserIdentityProviderId(self, request, context):
+        """Update the assignment of a user from one IDP to another.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_UserManagementServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateUser': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateUser,
                     request_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.CreateUserRequest.FromString,
                     response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.CreateUserResponse.SerializeToString,
@@ -206,14 +220,19 @@
                     response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.RevokeUserRightsResponse.SerializeToString,
             ),
             'ListUserRights': grpc.unary_unary_rpc_method_handler(
                     servicer.ListUserRights,
                     request_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.ListUserRightsRequest.FromString,
                     response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.ListUserRightsResponse.SerializeToString,
             ),
+            'UpdateUserIdentityProviderId': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateUserIdentityProviderId,
+                    request_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.UpdateUserIdentityProviderRequest.FromString,
+                    response_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.UpdateUserIdentityProviderResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.daml.ledger.api.v1.admin.UserManagementService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -224,15 +243,16 @@
     The authorization rules for its RPCs are specified on the ``<RpcName>Request``
     messages as boolean expressions over these facts:
     (1) ``HasRight(r)`` denoting whether the authenticated user has right ``r`` and
     (2) ``IsAuthenticatedUser(uid)`` denoting whether ``uid`` is the empty string or equal to the id of the authenticated user.
     (3) ``IsAuthenticatedIdentityProviderAdmin(idp)`` denoting whether ``idp`` is equal to the ``identity_provider_id``
     of the authenticated user and the user has an IdentityProviderAdmin right.
     If `user_id` is set to the empty string (the default), then the data for the authenticated user will be retrieved.
-    If `identity_provider_id` is set to the empty string, the default identity provider will be assumed.
+    If `identity_provider_id` is set to an empty string, then it's effectively set to the value of access token's 'iss' field if that is provided.
+    If `identity_provider_id` remains an empty string, the default identity provider will be assumed.
 
     The fields of request messages (and sub-messages) are marked either as ``Optional`` or ``Required``:
     (1) ``Optional`` denoting the client may leave the field unset when sending a request.
     (2) ``Required`` denoting the client must set the field to a non-default value when sending a request.
 
     A user resource consists of:
     (1) a set of properties represented by the ``User`` message,
@@ -374,7 +394,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.daml.ledger.api.v1.admin.UserManagementService/ListUserRights',
             com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.ListUserRightsRequest.SerializeToString,
             com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.ListUserRightsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdateUserIdentityProviderId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/com.daml.ledger.api.v1.admin.UserManagementService/UpdateUserIdentityProviderId',
+            com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.UpdateUserIdentityProviderRequest.SerializeToString,
+            com_dot_daml_dot_ledger_dot_api_dot_v1_dot_admin_dot_user__management__service__pb2.UpdateUserIdentityProviderResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
 from grpc import aio as _grpc_aio
 
-from .user_management_service_pb2 import CreateUserRequest, CreateUserResponse, DeleteUserRequest, DeleteUserResponse, GetUserRequest, GetUserResponse, GrantUserRightsRequest, GrantUserRightsResponse, ListUserRightsRequest, ListUserRightsResponse, ListUsersRequest, ListUsersResponse, RevokeUserRightsRequest, RevokeUserRightsResponse, UpdateUserRequest, UpdateUserResponse
+from .user_management_service_pb2 import CreateUserRequest, CreateUserResponse, DeleteUserRequest, DeleteUserResponse, GetUserRequest, GetUserResponse, GrantUserRightsRequest, GrantUserRightsResponse, ListUserRightsRequest, ListUserRightsResponse, ListUsersRequest, ListUsersResponse, RevokeUserRightsRequest, RevokeUserRightsResponse, UpdateUserIdentityProviderRequest, UpdateUserIdentityProviderResponse, UpdateUserRequest, UpdateUserResponse
 
 __all__ = [
     "UserManagementServiceStub",
 ]
 
 
 # noinspection PyPep8Naming,DuplicatedCode
@@ -27,29 +27,32 @@
     def GetUser(self, __1: GetUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[GetUserResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, GetUserResponse]]: ...
     def UpdateUser(self, __1: UpdateUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[UpdateUserResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, UpdateUserResponse]]: ...
     def DeleteUser(self, __1: DeleteUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[DeleteUserResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, DeleteUserResponse]]: ...
     def ListUsers(self, __1: ListUsersRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[ListUsersResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, ListUsersResponse]]: ...
     def GrantUserRights(self, __1: GrantUserRightsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[GrantUserRightsResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, GrantUserRightsResponse]]: ...
     def RevokeUserRights(self, __1: RevokeUserRightsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[RevokeUserRightsResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, RevokeUserRightsResponse]]: ...
     def ListUserRights(self, __1: ListUserRightsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[ListUserRightsResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, ListUserRightsResponse]]: ...
+    def UpdateUserIdentityProviderId(self, __1: UpdateUserIdentityProviderRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[UpdateUserIdentityProviderResponse, _grpc_aio.UnaryUnaryCall[_typing.Any, UpdateUserIdentityProviderResponse]]: ...
 
 # noinspection PyPep8Naming,DuplicatedCode
 class _UserManagementServiceBlockingStub(UserManagementServiceStub):
     def CreateUser(self, __1: CreateUserRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> CreateUserResponse: ...
     def GetUser(self, __1: GetUserRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> GetUserResponse: ...
     def UpdateUser(self, __1: UpdateUserRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> UpdateUserResponse: ...
     def DeleteUser(self, __1: DeleteUserRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> DeleteUserResponse: ...
     def ListUsers(self, __1: ListUsersRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> ListUsersResponse: ...
     def GrantUserRights(self, __1: GrantUserRightsRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> GrantUserRightsResponse: ...
     def RevokeUserRights(self, __1: RevokeUserRightsRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> RevokeUserRightsResponse: ...
     def ListUserRights(self, __1: ListUserRightsRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> ListUserRightsResponse: ...
+    def UpdateUserIdentityProviderId(self, __1: UpdateUserIdentityProviderRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> UpdateUserIdentityProviderResponse: ...
 
 # noinspection PyPep8Naming,DuplicatedCode
 class _UserManagementServiceAsyncStub(UserManagementServiceStub):
     def CreateUser(self, __1: CreateUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, CreateUserResponse]: ...  # type: ignore
     def GetUser(self, __1: GetUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, GetUserResponse]: ...  # type: ignore
     def UpdateUser(self, __1: UpdateUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, UpdateUserResponse]: ...  # type: ignore
     def DeleteUser(self, __1: DeleteUserRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, DeleteUserResponse]: ...  # type: ignore
     def ListUsers(self, __1: ListUsersRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, ListUsersResponse]: ...  # type: ignore
     def GrantUserRights(self, __1: GrantUserRightsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, GrantUserRightsResponse]: ...  # type: ignore
     def RevokeUserRights(self, __1: RevokeUserRightsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, RevokeUserRightsResponse]: ...  # type: ignore
     def ListUserRights(self, __1: ListUserRightsRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, ListUserRightsResponse]: ...  # type: ignore
+    def UpdateUserIdentityProviderId(self, __1: UpdateUserIdentityProviderRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, UpdateUserIdentityProviderResponse]: ...  # type: ignore
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/command_completion_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/command_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/command_submission_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/commands.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/completion.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/contract_metadata.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/event.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/event_query_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/experimental_features.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/ledger_configuration_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import ledger_configuration_service_pb2 as com_dot_daml_dot_ledger_dot_api_dot_v1_dot_ledger__configuration__service__pb2
 
 
 class LedgerConfigurationServiceStub(object):
     """LedgerConfigurationService allows clients to subscribe to changes of the ledger configuration.
+    In V2 Ledger API this service is not available anymore.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -24,14 +25,15 @@
                 request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_ledger__configuration__service__pb2.GetLedgerConfigurationRequest.SerializeToString,
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_ledger__configuration__service__pb2.GetLedgerConfigurationResponse.FromString,
                 )
 
 
 class LedgerConfigurationServiceServicer(object):
     """LedgerConfigurationService allows clients to subscribe to changes of the ledger configuration.
+    In V2 Ledger API this service is not available anymore.
     """
 
     def GetLedgerConfiguration(self, request, context):
         """Returns the latest configuration as the first response, and publishes configuration updates in the same stream.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -50,14 +52,15 @@
             'com.daml.ledger.api.v1.LedgerConfigurationService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class LedgerConfigurationService(object):
     """LedgerConfigurationService allows clients to subscribe to changes of the ledger configuration.
+    In V2 Ledger API this service is not available anymore.
     """
 
     @staticmethod
     def GetLedgerConfiguration(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/ledger_identity_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import ledger_identity_service_pb2 as com_dot_daml_dot_ledger_dot_api_dot_v1_dot_ledger__identity__service__pb2
 
 
 class LedgerIdentityServiceStub(object):
     """DEPRECATED: This service is now deprecated and ledger identity string is optional for all Ledger API requests.
 
     Allows clients to verify that the server they are communicating with exposes the ledger they wish to operate on.
+    In V2 Ledger API this service is not available anymore.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -28,14 +29,15 @@
                 )
 
 
 class LedgerIdentityServiceServicer(object):
     """DEPRECATED: This service is now deprecated and ledger identity string is optional for all Ledger API requests.
 
     Allows clients to verify that the server they are communicating with exposes the ledger they wish to operate on.
+    In V2 Ledger API this service is not available anymore.
     """
 
     def GetLedgerIdentity(self, request, context):
         """Clients may call this RPC to return the identifier of the ledger they are connected to.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -56,14 +58,15 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class LedgerIdentityService(object):
     """DEPRECATED: This service is now deprecated and ledger identity string is optional for all Ledger API requests.
 
     Allows clients to verify that the server they are communicating with exposes the ledger they wish to operate on.
+    In V2 Ledger API this service is not available anymore.
     """
 
     @staticmethod
     def GetLedgerIdentity(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/ledger_offset.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/package_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
 from google.protobuf.empty_pb2 import Empty
 from grpc import aio as _grpc_aio
 
-from .reset_service_pb2 import ResetRequest
+from .domain_initialization_service_pb2 import DomainInitRequest
 
 __all__ = [
-    "ResetServiceStub",
+    "DomainInitializationServiceStub",
 ]
 
 
 # noinspection PyPep8Naming,DuplicatedCode
-class ResetServiceStub:
+class DomainInitializationServiceStub:
     @classmethod  # type: ignore
     @_typing.overload
-    def __new__(cls, channel: _grpc.Channel) -> _ResetServiceBlockingStub: ...  # type: ignore
+    def __new__(cls, channel: _grpc.Channel) -> _DomainInitializationServiceBlockingStub: ...  # type: ignore
     @classmethod  # type: ignore
     @_typing.overload
-    def __new__(cls, channel: _grpc_aio.Channel) -> _ResetServiceAsyncStub: ...  # type: ignore
-    def Reset(self, __1: ResetRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[Empty, _grpc_aio.UnaryUnaryCall[_typing.Any, Empty]]: ...
+    def __new__(cls, channel: _grpc_aio.Channel) -> _DomainInitializationServiceAsyncStub: ...  # type: ignore
+    def Init(self, __1: DomainInitRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _typing.Union[Empty, _grpc_aio.UnaryUnaryCall[_typing.Any, Empty]]: ...
 
 # noinspection PyPep8Naming,DuplicatedCode
-class _ResetServiceBlockingStub(ResetServiceStub):
-    def Reset(self, __1: ResetRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> Empty: ...
+class _DomainInitializationServiceBlockingStub(DomainInitializationServiceStub):
+    def Init(self, __1: DomainInitRequest, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_typing.Tuple[_typing.Tuple[str, _typing.Union[str, bytes]], ...]] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> Empty: ...
 
 # noinspection PyPep8Naming,DuplicatedCode
-class _ResetServiceAsyncStub(ResetServiceStub):
-    def Reset(self, __1: ResetRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, Empty]: ...  # type: ignore
+class _DomainInitializationServiceAsyncStub(DomainInitializationServiceStub):
+    def Init(self, __1: DomainInitRequest, *, timeout: _typing.Optional[float] = ..., metadata: _typing.Optional[_grpc_aio.Metadata] = ..., credentials: _typing.Optional[_grpc.CallCredentials] = ..., wait_for_ready: _typing.Optional[bool] = ..., compression: _typing.Optional[_grpc.Compression] = ...) -> _grpc_aio.UnaryUnaryCall[_typing.Any, Empty]: ...  # type: ignore
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/testing/time_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/transaction_filter.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/transaction.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/transaction_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import transaction_service_pb2 as com_dot_daml_dot_ledger_dot_api_dot_v1_dot_transaction__service__pb2
 
 
 class TransactionServiceStub(object):
     """Allows clients to read transactions from the ledger.
+    In V2 Ledger API this service is not available anymore. Use v2.UpdateService instead.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -59,14 +60,15 @@
                 request_serializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_transaction__service__pb2.GetLatestPrunedOffsetsRequest.SerializeToString,
                 response_deserializer=com_dot_daml_dot_ledger_dot_api_dot_v1_dot_transaction__service__pb2.GetLatestPrunedOffsetsResponse.FromString,
                 )
 
 
 class TransactionServiceServicer(object):
     """Allows clients to read transactions from the ledger.
+    In V2 Ledger API this service is not available anymore. Use v2.UpdateService instead.
     """
 
     def GetTransactions(self, request, context):
         """Read the ledger's filtered transaction stream for a set of parties.
         Lists only creates and archives, but not other events.
         Omits all events on transient contracts, i.e., contracts that were both created and archived in the same transaction.
         """
@@ -175,14 +177,15 @@
             'com.daml.ledger.api.v1.TransactionService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class TransactionService(object):
     """Allows clients to read transactions from the ledger.
+    In V2 Ledger API this service is not available anymore. Use v2.UpdateService instead.
     """
 
     @staticmethod
     def GetTransactions(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/value.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: com/daml/ledger/api/v1/version_service.proto
 """Generated protocol buffer code."""
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi` & `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 # fmt: off
 # isort: skip_file
 
 import builtins as _builtins, typing as _typing
 
 import grpc as _grpc
```

### Comparing `dazl-8.0.0a4/python/dazl/_logging.py` & `dazl-8.0.0b1/python/dazl/_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Logging utilities used in `dazl`.
 
 This is an internal API and not meant to be used directly outside of dazl; symbols declared in this
 file may change at any time.
```

### Comparing `dazl-8.0.0a4/python/dazl/_repr/__init__.py` & `dazl-8.0.0b1/python/dazl/_repr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 Default ``repr`` rules for dazl.
 
 THIS IS NOT A PUBLIC API, AND ITS CONTENTS ARE SUBJECT TO CHANGE AT ANY TIME!
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/cli/__init__.py` & `dazl-8.0.0b1/python/dazl/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Simple command-line handlers.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/cli/_base.py` & `dazl-8.0.0b1/python/dazl/cli/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from argparse import ArgumentParser
 
 
 class CliCommand:
```

### Comparing `dazl-8.0.0a4/python/dazl/cli/ls.py` & `dazl-8.0.0b1/python/dazl/cli/ls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from argparse import ArgumentParser
 
 from .. import LOG, Network
```

### Comparing `dazl-8.0.0a4/python/dazl/cli/tail.py` & `dazl-8.0.0b1/python/dazl/cli/tail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from argparse import ArgumentParser
 from asyncio import ensure_future, get_event_loop
 import datetime
```

### Comparing `dazl-8.0.0a4/python/dazl/cli/upload.py` & `dazl-8.0.0b1/python/dazl/cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
 from argparse import ArgumentParser
 from pathlib import Path
```

### Comparing `dazl-8.0.0a4/python/dazl/client/__init__.py` & `dazl-8.0.0b1/python/dazl/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 :mod:`dazl.client` package
 ==========================
 
 The :mod:`dazl.client` module a high-level view of the Ledger API in a friendly way.
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_base_model.py` & `dazl-8.0.0b1/python/dazl/client/_base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This model contains definitions for the data classes used at the client layer of this library.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_conn_settings.py` & `dazl-8.0.0b1/python/dazl/client/_conn_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import NamedTuple, Optional, Tuple, Union
 from urllib.parse import urlparse
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_events.py` & `dazl-8.0.0b1/python/dazl/client/_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Awaitable, Callable, TypeVar, Union
 
 from ..protocols.events import BaseEvent
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_network_client_impl.py` & `dazl-8.0.0b1/python/dazl/client/_network_client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import asyncio
 from asyncio import Future, ensure_future, gather, sleep, wait_for
 from collections import defaultdict
@@ -15,14 +15,15 @@
     Any,
     Awaitable,
     Callable,
     Collection,
     Dict,
     List,
     Optional,
+    Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
 from .. import LOG
@@ -510,15 +511,15 @@
             pi.stop_writer()
 
         # wait for writers to finish their writing
         await gather(*self._writers, return_exceptions=True)
         LOG.info("network_run: finished.")
         self._writers = []
 
-    async def beat(self, party_impls: Collection[_PartyClientImpl]) -> Tuple[Optional[str], bool]:
+    async def beat(self, party_impls: Sequence[_PartyClientImpl], /) -> Tuple[Optional[str], bool]:
         """
         Called periodically to schedule reads and writes.
         """
         from ._reader_sync import run_iteration
 
         offset, completions = await run_iteration(party_impls)
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_party_client_impl.py` & `dazl-8.0.0b1/python/dazl/client/_party_client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import asyncio
 from asyncio import Future, ensure_future, gather, get_event_loop, sleep, wait
 from concurrent.futures import ALL_COMPLETED
 from dataclasses import asdict, dataclass, field, fields, replace
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_reader_sync.py` & `dazl-8.0.0b1/python/dazl/client/_reader_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Functions for ensuring that readers across different parties remain as close in sync to each other
 as practical.
 """
 
 from __future__ import annotations
 
 from asyncio import Future, ensure_future, gather, sleep
-from typing import TYPE_CHECKING, Collection, List, Optional, Tuple
+from typing import TYPE_CHECKING, Collection, List, Optional, Sequence, Tuple
 
 from .. import LOG
 from ..util.asyncio_util import completed, named_gather
 
 if TYPE_CHECKING:
     from ._party_client_impl import _PartyClientImpl
 
 
 async def run_iteration(
-    party_impls: "Collection[_PartyClientImpl]",
-) -> "Tuple[Optional[str], Collection[Future]]":
+    party_impls: Sequence[_PartyClientImpl], /
+) -> Tuple[Optional[str], Sequence[Future]]:
     """
     Read the next set of transactions for the set of parties. This coroutine ends when all
     parties are caught up to the same offset.
 
     :param party_impls:
         A collection of :class:`_PartyClientImpl` will have scheduled invocations.
     :return:
@@ -83,44 +83,44 @@
     LOG.info("Finished catching up.")
 
     LOG.info("Finished reading current ledger state.")
     return offset
 
 
 async def read_transaction_event_stream(
-    party_impls: Collection[_PartyClientImpl],
+    party_impls: Sequence[_PartyClientImpl], /
 ) -> Optional[str]:
     LOG.info("Reading current ledger state...")
     if not party_impls:
         return None
 
     party_impl = next(iter(party_impls))
     offset = await party_impl.read_end()
 
     await gather(*[party_impl.read_transactions(offset, False) for party_impl in party_impls])
     return offset
 
 
 async def read_transactions(
-    party_impls: Collection[_PartyClientImpl], until_offset: Optional[str], raise_events: bool
-) -> Tuple[Collection[str], Future]:
+    party_impls: Sequence[_PartyClientImpl], /, until_offset: Optional[str], raise_events: bool
+) -> Tuple[Sequence[Optional[str]], Future]:
     """
     Read transactions from a collection of PartyImpls.
 
     :param party_impls:
     :param until_offset:
     :param raise_events:
     :return:
         A tuple containing:
-         * a set of the offsets returned from all readers, and
+         * the offsets returned from all readers, and
          * a Future that is resolved when all events across all readers have resolved either
            successfully or unsuccessfully.
     """
     tuples = await gather(*(pi.read_transactions(until_offset, raise_events) for pi in party_impls))
-    offsets = sorted({t[0] for t in tuples})
+    offsets = [t[0] for t in tuples]
     futures = [ensure_future(t[1]) for t in tuples]
     futures = [fut for fut in futures if not fut.done()]
     if not futures:
         return offsets, completed(None)
     elif len(futures):
         return offsets, futures[0]
     else:
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_run_level.py` & `dazl-8.0.0b1/python/dazl/client/_run_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from threading import Event
 
 from ..scheduler import RunLevel
```

### Comparing `dazl-8.0.0a4/python/dazl/client/_writer_verify.py` & `dazl-8.0.0b1/python/dazl/client/_writer_verify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Any
 
 from ..damlast.daml_lf_1 import TypeConName
```

### Comparing `dazl-8.0.0a4/python/dazl/client/api.py` & `dazl-8.0.0b1/python/dazl/client/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 #
 # NOTE TO IMPLEMENTORS
 #
 # This file contains only public API definitions, overloads, and documentation. (This file should
 # be treated more like a C header file than anything else.) The bulk of the implementation is kept
 # in _party_client.py.
```

### Comparing `dazl-8.0.0a4/python/dazl/client/bots.py` & `dazl-8.0.0b1/python/dazl/client/bots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import Future, InvalidStateError, ensure_future, gather, get_event_loop
 from collections import defaultdict
 from dataclasses import dataclass, field, replace
@@ -28,14 +28,15 @@
     overload,
 )
 from uuid import uuid4
 import warnings
 
 from .. import LOG
 from ..ledger import Command, CreateEvent, ExerciseResponse
+from ..ledger.api_types import is_command
 from ..prim import Party
 from ..protocols.events import BaseEvent
 from ..util.asyncio_util import LongRunningAwaitable, Signal, completed, failed, propagate
 from .commands import CommandBuilder
 from .events import EventKey
 
 if TYPE_CHECKING:
@@ -329,20 +330,18 @@
         self._lock = RLock()
 
     def __len__(self) -> int:
         with self._lock:
             return len(self._bots)
 
     @overload
-    def __getitem__(self, i: int) -> Bot:
-        ...
+    def __getitem__(self, i: int) -> Bot: ...
 
     @overload
-    def __getitem__(self, i: slice) -> Sequence[Bot]:
-        ...
+    def __getitem__(self, i: slice) -> Sequence[Bot]: ...
 
     def __getitem__(self, i):
         with self._lock:
             return operator.getitem(self._bots, i)
 
     def __iter__(self):
         with self._lock:
@@ -485,15 +484,15 @@
             ret = callback(*args, **kwargs)
         except BaseException as exception:
             LOG.exception("The callback %r threw an exception!", callback)
             return failed(exception)
 
         if ret is None:
             return completed(None)
-        elif isinstance(ret, (CommandBuilder, Command, list, tuple)):
+        elif is_command(ret) or isinstance(ret, (CommandBuilder, list, tuple)):
             try:
                 ret_fut = submit_fn(ret)
             except BaseException as exception:
                 LOG.exception(
                     "The callback %r returned commands that could not be submitted! (%s)",
                     callback,
                     ret,
@@ -519,15 +518,15 @@
 
                 def cmd_future_finished(_):
                     ret = cmd_fut.result()
                     if ret is None:
                         fut.set_result(None)
                     elif isinstance(ret, (CreateEvent, ExerciseResponse)):
                         fut.set_result(ret)
-                    elif isinstance(ret, (CommandBuilder, Command, list, tuple)):
+                    elif is_command(ret) or isinstance(ret, (CommandBuilder, list, tuple)):
                         propagate(ensure_future(submit_fn(ret)), fut)
                     elif inspect.isawaitable(ret):
                         LOG.error("A callback cannot return an Awaitable of an Awaitable")
                         raise InvalidStateError(
                             "A callback cannot return an Awaitable of an Awaitable"
                         )
```

### Comparing `dazl-8.0.0a4/python/dazl/client/commands.py` & `dazl-8.0.0b1/python/dazl/client/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 Command types that are used in the dazl v5 API.
 
 These symbols are primarily kept for backwards compatibility.
 """
 from __future__ import annotations
@@ -11,29 +11,26 @@
 from datetime import timedelta
 from typing import Any, Collection, List, Mapping, Optional, Sequence, Tuple, Union
 import uuid
 import warnings
 
 from ..damlast import TypeConName
 from ..ledger import Command, CreateAndExerciseCommand, CreateCommand, ExerciseCommand
+from ..ledger.api_types import Commands, is_command
 from ..prim import ContractData, ContractId, Party
 
 __all__ = [
     "CommandBuilder",
     "CommandDefaults",
     "CommandPayload",
-    "CommandsOrCommandSequence",
     "EventHandlerResponse",
     "flatten_command_sequence",
 ]
 
 
-CommandsOrCommandSequence = Union[None, Command, Sequence[Optional[Command]]]
-
-
 # noinspection PyDeprecation
 class CommandBuilder:
     """
     Builder class for generating commands to be sent to the ledger.
     """
 
     @classmethod
@@ -117,15 +114,15 @@
                 template_id=template,
                 payload=create_arguments,
                 choice=choice_name,
                 argument=choice_arguments,
             )
         )
 
-    def append(self, *commands: CommandsOrCommandSequence) -> CommandBuilder:
+    def append(self, *commands: Commands) -> CommandBuilder:
         """
         Append one or more commands, or list of commands to the :class:`CommandBuilder` in flight.
         This method respects the value of ``atomic_default`` that this object was constructed with.
         In order to force commands to be submitted either atomically, use :meth:`append_atomically`.
         To allow these commands to be submitted in parallel use :meth:`append_nonatomically`.
 
         :param commands: One or more commands, or list of commands to be submitted to the ledger.
@@ -135,19 +132,19 @@
             # a command builder that defaults to being atomic will put all commands in a single
             # transaction; build on the very first transaction
             self._commands[0].extend(flatten_command_sequence(commands))
             return self
         else:
             return self.append_nonatomically(*commands)
 
-    def append_atomically(self, *commands: CommandsOrCommandSequence) -> CommandBuilder:
+    def append_atomically(self, *commands: Commands) -> CommandBuilder:
         self._commands.extend([flatten_command_sequence(commands)])
         return self
 
-    def append_nonatomically(self, *commands: CommandsOrCommandSequence) -> CommandBuilder:
+    def append_nonatomically(self, *commands: Commands) -> CommandBuilder:
         self._commands.extend([[cmd] for cmd in flatten_command_sequence(commands)])
         return self
 
     def build(self, defaults: Optional[CommandDefaults] = None) -> Collection[CommandPayload]:
         """
         Return a collection of commands.
         """
@@ -203,34 +200,34 @@
         else:
             return repr(self)
 
     def __repr__(self):
         return f"CommandBuilder({self._commands})"
 
 
-def flatten_command_sequence(commands: Sequence[CommandsOrCommandSequence]) -> List[Command]:
+def flatten_command_sequence(commands: Sequence[Commands]) -> List[Command]:
     """
     Convert a list of mixed commands, ``None``, and list of commands into an ordered sequence of
     non-``None`` commands.
     """
     ret = []  # type: List[Command]
-    errors = []  # type: List[Tuple[Sequence[int], CommandsOrCommandSequence]]
+    errors = []  # type: List[Tuple[Sequence[int], Commands]]
 
     for i, obj in enumerate(commands):
         if obj is not None:
-            if isinstance(obj, Command):
+            if is_command(obj):
                 ret.append(obj)
             else:
                 try:
-                    cmd_iter = iter(obj)
+                    cmd_iter = iter(obj)  # type: ignore
                 except TypeError:
                     errors.append(((i,), obj))
                     continue
                 for j, cmd in enumerate(cmd_iter):
-                    if isinstance(cmd, Command):
+                    if is_command(cmd):
                         ret.append(cmd)
                     else:
                         errors.append(((i, j), cmd))
     if errors:
         raise ValueError(
             f"Failed to interpret some elements as Commands in the list: " f"$[{index}] = {command}"
             for index, command in errors
@@ -291,8 +288,8 @@
         ]
         if missing_fields:
             raise ValueError(
                 f"Some fields are set to None when they are required: " f"{missing_fields}"
             )
 
 
-EventHandlerResponse = Union[CommandsOrCommandSequence, CommandBuilder]
+EventHandlerResponse = Union[None, Commands, CommandBuilder]
```

### Comparing `dazl-8.0.0a4/python/dazl/client/config.py` & `dazl-8.0.0b1/python/dazl/client/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains configuration parameters used by the rest of the library.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/client/errors.py` & `dazl-8.0.0b1/python/dazl/client/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Collection, Union
 
 from ..prim import DazlError, DazlWarning, Party
```

### Comparing `dazl-8.0.0a4/python/dazl/client/events.py` & `dazl-8.0.0b1/python/dazl/client/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Any, Callable, Collection, Iterator, TypeVar
 import warnings
```

### Comparing `dazl-8.0.0a4/python/dazl/client/ledger.py` & `dazl-8.0.0b1/python/dazl/client/ledger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Types that describe the behavior of the ledger itself.
 """
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/client/runner.py` & `dazl-8.0.0b1/python/dazl/client/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Simple methods for instantiating an application written against dazl that incorporate common usage
 patterns.
 """
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/client/state.py` & `dazl-8.0.0b1/python/dazl/client/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import Future, get_event_loop, sleep
 from collections import defaultdict
 from dataclasses import dataclass
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/__init__.py` & `dazl-8.0.0b1/python/dazl/damlast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 :mod:`dazl.damast`
 ==================
 
 The :mod:`dazl.damlast` package contains types and functions for working with Daml-LF Archives.
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/_builtins_meta.py` & `dazl-8.0.0b1/python/dazl/damlast/_builtins_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains supporting infrastructure for built-in method definitions for interpreting
 Daml-LF files.
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/builtins.py` & `dazl-8.0.0b1/python/dazl/damlast/builtins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Define a few DAML values and functions that have been inlined in Python for efficiency and
 simplicity.
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/daml_lf_1.py` & `dazl-8.0.0b1/python/dazl/damlast/daml_lf_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 DAML-LF Archive types
 ---------------------
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/daml_types.py` & `dazl-8.0.0b1/python/dazl/damlast/daml_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 DAML Types
 ----------
 
 Constants and constructor functions for the various primitive DAML types.
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/errors.py` & `dazl-8.0.0b1/python/dazl/damlast/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Error types
 -----------
 
 .. autoclass:: PackageNotFoundError
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/expand.py` & `dazl-8.0.0b1/python/dazl/damlast/expand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import Collection, Mapping, Optional
 import warnings
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/lookup.py` & `dazl-8.0.0b1/python/dazl/damlast/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 DAML-LF fast lookups
 --------------------
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/parse.py` & `dazl-8.0.0b1/python/dazl/damlast/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 DAML-LF Archive parsing
 -----------------------
 
 Functions for creating :class:`Archive` and :class:`Package` instances.
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/pb_parse.py` & `dazl-8.0.0b1/python/dazl/damlast/pb_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
-from typing import List, Literal, Optional, Sequence
+from typing import List, Optional, Sequence
 
 from . import daml_lf_1 as lf
 from .._gen.com.daml.daml_lf_1_15 import daml_lf_1_pb2 as pblf
 
 __all__ = ["ProtobufParser"]
 
-# TODO: Figure out a way to define these literals in daml_lf_1_pb2.pyi where they belong
-# fmt: off
-PrimCon = Literal[0, 1, 2]
-PrimType = Literal[0, 1, 2, 3, 5, 6, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23]
-PrimLit_RoundingMode = Literal[0, 1, 2, 3, 4, 5, 6, 7]
-BuiltinFunction = Literal[0, 1, 2, 3, 6, 107, 108, 109, 110, 111, 121, 122, 7, 8, 9, 10, 11, 12, 20, 21, 96, 97, 98, 99, 100, 101, 124, 125, 126, 127, 128, 129, 130, 23, 24, 25, 147, 33, 34, 112, 36, 37, 67, 89, 39, 40, 113, 42, 43, 68, 90, 45, 46, 114, 48, 49, 69, 91, 51, 52, 115, 54, 55, 70, 92, 57, 58, 116, 60, 61, 71, 63, 94, 95, 103, 104, 117, 136, 93, 72, 73, 74, 75, 76, 77, 118, 119, 78, 79, 80, 120, 81, 82, 83, 84, 85, 86, 87, 123, 131, 132, 133, 134, 135, 88, 102, 105, 106, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146]
-
-# fmt: on
-
 
 # noinspection PyPep8Naming,PyMethodMayBeStatic
 class ProtobufParser:
     def __init__(self, current_package: lf.PackageRef) -> None:
         self.current_package = current_package
         self.current_module = None  # type: Optional[lf.ModuleRef]
         self.interned_strings = []  # type: List[str]
@@ -118,15 +109,15 @@
             raise ValueError(f"unknown sum type value: {sum_name!r}")
 
     def parse_Kind_Arrow(self, pb: pblf.Kind.Arrow) -> lf.Kind.Arrow:
         return lf.Kind.Arrow(
             tuple(self.parse_Kind(param) for param in pb.params), self.parse_Kind(pb.result)
         )
 
-    def parse_PrimType(self, pb: PrimType) -> lf.PrimType:
+    def parse_PrimType(self, pb: pblf.PrimType) -> lf.PrimType:
         return lf.PrimType(pb)
 
     def parse_Type(self, pb: pblf.Type) -> lf.Type:
         sum_name = pb.WhichOneof("Sum")
         if sum_name == "var":
             return self.parse_Type_Var(pb.var)
         elif sum_name == "con":
@@ -178,25 +169,25 @@
 
     def parse_Type_Syn(self, pb: pblf.Type.Syn) -> lf.Type.Syn:
         return lf.Type.Syn(
             tysyn=self.parse_TypeSynName(pb.tysyn),
             args=tuple(self.parse_Type(arg) for arg in pb.args),
         )
 
-    def parse_PrimCon(self, pb: PrimCon) -> lf.PrimCon:
+    def parse_PrimCon(self, pb: pblf.PrimCon) -> lf.PrimCon:
         if pb == 0:
             return lf.PrimCon.CON_UNIT
         elif pb == 1:
             return lf.PrimCon.CON_FALSE
         elif pb == 2:
             return lf.PrimCon.CON_TRUE
         else:
             raise ValueError(f"unknown enum value: {pb!r}")
 
-    def parse_BuiltinFunction(self, pb: BuiltinFunction) -> lf.BuiltinFunction:
+    def parse_BuiltinFunction(self, pb: pblf.BuiltinFunction) -> lf.BuiltinFunction:
         return lf.BuiltinFunction(pb)
 
     def parse_PrimLit(self, pb: pblf.PrimLit) -> lf.PrimLit:
         sum_name = pb.WhichOneof("Sum")
         if sum_name == "int64":
             return lf.PrimLit(int64=pb.int64)
         elif sum_name == "decimal_str":
@@ -216,15 +207,15 @@
         elif sum_name == "date":
             return lf.PrimLit(date=pb.date)
         elif sum_name == "rounding_mode":
             return lf.PrimLit(rounding_mode=self.parse_PrimLit_RoundingMode(pb.rounding_mode))
         else:
             raise ValueError(f"unknown Sum value: {pb!r}")
 
-    def parse_PrimLit_RoundingMode(self, pb: PrimLit_RoundingMode) -> lf.PrimLit.RoundingMode:
+    def parse_PrimLit_RoundingMode(self, pb: pblf.PrimLit.RoundingMode) -> lf.PrimLit.RoundingMode:
         return lf.PrimLit.RoundingMode(pb)
 
     def parse_Expr(self, pb: pblf.Expr) -> lf.Expr:
         location = self.parse_Location(pb.location) if pb.HasField("location") else None
 
         sum_name = pb.WhichOneof("Sum")
         if sum_name == "var_str":
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/pkgfile.py` & `dazl-8.0.0b1/python/dazl/damlast/pkgfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from io import BytesIO
 from os import PathLike
 from pathlib import Path
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/protocols.py` & `dazl-8.0.0b1/python/dazl/damlast/protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, AbstractSet, Any, Collection, Protocol, runtime_checkable
 
 if TYPE_CHECKING:
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/types.py` & `dazl-8.0.0b1/python/dazl/damlast/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Callable
 
 from ._base import T
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/util.py` & `dazl-8.0.0b1/python/dazl/damlast/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Optional, Sequence, Union
 import warnings
```

### Comparing `dazl-8.0.0a4/python/dazl/damlast/visitor.py` & `dazl-8.0.0b1/python/dazl/damlast/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Generic, Optional, TypeVar
 
 from .daml_lf_1 import (
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/__init__.py` & `dazl-8.0.0b1/python/dazl/ledger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 This module contains the types needed to submit commands to and read events from a
 Daml `gRPC Ledger API <https://docs.daml.com/app-dev/ledger-api.html>`_ or
 `HTTP JSON API <https://docs.daml.com/json-api/index.html>`_.
 """
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/_offsets.py` & `dazl-8.0.0b1/python/dazl/ledger/_offsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 Utilities for working with ledger offsets.
 
 This API is _not_ public!
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/_retry.py` & `dazl-8.0.0b1/python/dazl/ledger/_retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import CancelledError, sleep
 from datetime import datetime, timedelta
 from typing import Awaitable, Callable, TypeVar
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/aio/__init__.py` & `dazl-8.0.0b1/python/dazl/ledger/aio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 `asyncio`-flavored protocols and base classes for connecting to a Daml ledger.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/aio/__init__.pyi` & `dazl-8.0.0b1/python/dazl/ledger/aio/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import abc
 from datetime import datetime
 from typing import (
     AbstractSet,
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
-    Collection,
     DefaultDict,
     List,
     Optional,
     Protocol,
     Sequence,
     TypeVar,
     Union,
@@ -25,20 +24,20 @@
 
 from .. import (
     Connection as _Connection,
     PackageService as _PackageService,
     QueryStream as _QueryStream,
 )
 from ...damlast.daml_lf_1 import PackageRef, TypeConName
-from ...prim import ContractData, ContractId, Party, TimeDeltaLike
+from ...prim import ContractData, ContractId, Parties, TimeDeltaLike
 from ...query import Queries, Query
 from ..api_types import (
     ArchiveEvent,
     Boundary,
-    Command,
+    Commands,
     CreateEvent,
     ExerciseResponse,
     MeteringReport,
     PartyInfo,
     Right,
     SubmitResponse,
     User,
@@ -97,130 +96,130 @@
 class Connection(_Connection, PackageService, Protocol):
     async def __aenter__(self: ConnSelf) -> ConnSelf: ...
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None: ...
     async def open(self) -> None: ...
     async def close(self) -> None: ...
     async def submit(
         self,
-        commands: Union[Command, Sequence[Command]],
+        commands: Commands,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> None: ...
     async def create(
         self,
         template_id: Union[str, TypeConName],
         payload: ContractData,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> CreateEvent: ...
     async def exercise(
         self,
         contract_id: ContractId,
         choice_name: str,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ExerciseResponse: ...
     async def create_and_exercise(
         self,
         template_id: Union[str, TypeConName],
         payload: ContractData,
         choice_name: str,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ExerciseResponse: ...
     async def exercise_by_key(
         self,
         template_id: Union[str, TypeConName],
         choice_name: str,
         key: Any,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ExerciseResponse: ...
     async def archive(
         self,
         contract_id: ContractId,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ArchiveEvent: ...
     async def archive_by_key(
         self,
         template_id: str,
         key: Any,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ArchiveEvent: ...
     async def get_ledger_end(self, *, timeout: Optional[TimeDeltaLike] = ...) -> str: ...
     def query(
         self,
         template_id: Union[str, TypeConName] = "*",
         query: Query = None,
         /,
         *,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def query_many(
         self,
         *queries: Queries,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def stream(
         self,
         template_id: Union[str, TypeConName] = "*",
         query: Query = None,
         /,
         *,
         offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def stream_many(
         self,
         *queries: Queries,
         offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     async def get_user(
         self, user_id: Optional[str] = None, /, *, timeout: Optional[TimeDeltaLike] = ...
     ) -> User: ...
     async def create_user(
         self,
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/aio/pkgloader.py` & `dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import ensure_future, gather, get_event_loop, sleep, wait_for
 from concurrent.futures import ThreadPoolExecutor
 from datetime import timedelta
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/aio/pkgloader_compat.py` & `dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Backwards compatibility symbols in support of the to-be-removed dazl.client.pkg_loader module.
 This file is here in order to avoid import cycles.
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/api_types.py` & `dazl-8.0.0b1/python/dazl/ledger/api_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,55 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import abc
 from datetime import datetime
+import sys
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Collection,
     Final,
+    List,
     Mapping,
     NoReturn,
     Optional,
     Sequence,
     Union,
     final,
 )
 import uuid
 
 from .. import _repr
 from ..damlast.daml_lf_1 import TypeConName
 from ..damlast.lookup import parse_type_con_name
-from ..prim import LEDGER_STRING_REGEX, ContractData, ContractId, Party, to_parties
+from ..prim import LEDGER_STRING_REGEX, ContractData, ContractId, Parties, Party, to_parties
 from ..util.typing import safe_cast
 
+if sys.version_info >= (3, 12):
+    from typing import TypeAlias, TypeGuard
+elif sys.version_info >= (3, 10):
+    from typing import TypeGuard
+
+    from typing_extensions import TypeAlias
+else:
+    from typing_extensions import TypeAlias, TypeGuard
+
+
 __all__ = [
     "ActAs",
     "Admin",
     "ArchiveEvent",
     "Boundary",
     "Command",
     "CommandMeta",
+    "Commands",
     "CreateAndExerciseCommand",
     "CreateCommand",
     "CreateEvent",
     "Event",
     "EventOrBoundary",
     "ExerciseByKeyCommand",
     "ExerciseCommand",
@@ -51,90 +64,113 @@
     "User",
     "Version",
     "VersionFeatures",
     "VersionUserManagementFeature",
 ]
 
 
-class Command:
+def is_command(obj: Any, /) -> TypeGuard[Command]:
+    """
+    Determine whether an object is a :class:`Command`.
+
+    This function is equivalent to calling ``isinstance(obj, Command)``. If you are using
+    Python 3.10 or later, ``isinstance(obj, Command)`` should be preferred, but on Python 3.8 and 3.9,
+    ``isinstance(obj, Command)`` will fail to typecheck due to ``Union`` not being understood as a
+    valid argument. If your code must be compatible with Python 3.8 and 3.9 _and_ you wish to use a
+    typechecker, use this convenience function instead.
+    """
+    return isinstance(obj, _Command)
+
+
+def to_commands(*commands: Optional[Commands]) -> Sequence[Command]:
+    cmds = []  # type: List[Command]
+    if commands is not None:
+        for c in commands:
+            if c is not None:
+                if is_command(c):
+                    cmds.append(c)
+                else:
+                    cmds.extend(to_commands(*c))  # type: ignore
+    return cmds
+
+
+class _Command:
     """
     Base class for write-side commands.
 
     This class provides no functionality on its own.
     """
 
     def __setattr__(self, key, value) -> NoReturn:
         """
         Raise :class:`AttributeError`; instances of this class are immutable.
         """
         raise AttributeError("Command instances are read-only")
 
 
-class CreateCommand(Command):
+@final
+class CreateCommand(_Command):
     """
     A command that creates a contract without any predecessors.
+
+    Attributes:
+    - template_id: The template of the contract to be created.
+    - payload: The template arguments for the contract to be created.
     """
 
-    __slots__ = ("_template_id", "_payload")
-    if TYPE_CHECKING:
-        _template_id: TypeConName
-        _payload: ContractData
+    __slots__ = ("template_id", "payload")
+    __match_args__ = ("template_id", "payload")
+    template_id: Final[TypeConName]  # type: ignore
+    payload: Final[ContractData]  # type: ignore
 
     def __init__(self, template_id: Union[str, TypeConName], payload: ContractData):
         """
         Initialize a :class:`CreateCommand`.
 
         :param template_id:
             The template of the contract to be created.
         :param payload:
             The template arguments for the contract to be created.
         """
-        object.__setattr__(self, "_template_id", validate_template_id(template_id))
-        object.__setattr__(self, "_payload", payload)
-
-    @property
-    def template_id(self) -> TypeConName:
-        """
-        Return the template of the contract to be created.
-        """
-        return self._template_id
-
-    @property
-    def payload(self) -> Mapping[str, Any]:
-        """
-        Return the template arguments for the contract to be created.
-        """
-        return self._payload
+        object.__setattr__(self, "template_id", validate_template_id(template_id))
+        object.__setattr__(self, "payload", payload)
 
     def __eq__(self, other: Any, /) -> bool:
         return (
             isinstance(other, CreateCommand)
             and self.template_id == other.template_id
             and self.payload == other.payload
         )
 
     def __repr__(self) -> str:
         return f"CreateCommand({self.template_id}, {self.payload})"
 
 
-class CreateAndExerciseCommand(Command):
+@final
+class CreateAndExerciseCommand(_Command):
     """
     A command that exercises a choice on a newly-created contract in a single transaction.
 
     Instead of creating an instance of this command and submitting it with :meth:`Connection.submit`,
     consider using :meth:`Connection.create_and_exercise` instead, which also gives you access to
     the result of exercising the choice.
+
+    Attributes:
+    - template_id: The template of the contract to be created.
+    - payload: The template arguments for the contract to be created.
+    - choice: The choice to exercise.
+    - argument: The choice arguments. Can be omitted for choices that take no arguments.
     """
 
-    __slots__ = ("_template_id", "_payload", "_choice", "_argument")
-    if TYPE_CHECKING:
-        _template_id: TypeConName
-        _payload: ContractData
-        _choice: str
-        _argument: Any
+    __slots__ = ("template_id", "payload", "choice", "argument")
+    __match_args__ = ("template_id", "payload", "choice", "argument")
+    template_id: Final[TypeConName]  # type: ignore
+    payload: Final[ContractData]  # type: ignore
+    choice: Final[str]  # type: ignore
+    argument: Final[Any]  # type: ignore
 
     def __init__(
         self,
         template_id: Union[str, TypeConName],
         payload: ContractData,
         choice: str,
         argument: Optional[Any] = None,
@@ -147,138 +183,91 @@
         :param payload:
             The template arguments for the contract to be created.
         :param choice:
             The choice to exercise.
         :param argument:
             The choice arguments. Can be omitted for choices that take no arguments.
         """
-        object.__setattr__(self, "_template_id", validate_template_id(template_id))
-        object.__setattr__(self, "_payload", payload)
-        object.__setattr__(self, "_choice", choice)
-        object.__setattr__(self, "_argument", dict(argument) if argument is not None else dict())
-
-    @property
-    def template_id(self) -> TypeConName:
-        """
-        The template of the contract to be created.
-        """
-        return self._template_id
-
-    @property
-    def payload(self) -> ContractData:
-        """
-        The template arguments for the contract to be created.
-        """
-        return self._payload
-
-    @property
-    def choice(self) -> str:
-        """
-        The choice to exercise.
-        """
-        return self._choice
-
-    @property
-    def argument(self) -> Any:
-        """
-        The choice arguments.
-        """
-        return self._argument
+        object.__setattr__(self, "template_id", validate_template_id(template_id))
+        object.__setattr__(self, "payload", payload)
+        object.__setattr__(self, "choice", choice)
+        object.__setattr__(self, "argument", dict(argument) if argument is not None else dict())
 
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, CreateAndExerciseCommand)
             and self.template_id == other.template_id
             and self.payload == other.payload
             and self.choice == other.choice
             and self.argument == other.argument
         )
 
     def __repr__(self) -> str:
         return f"CreateAndExerciseCommand({self.template_id}, {self.payload}, {self.choice!r}, {self.argument})"
 
 
-class ExerciseCommand(Command):
+@final
+class ExerciseCommand(_Command):
     """
     A command that exercises a choice on a contract identified by its contract ID.
 
     Instead of creating an instance of this command and submitting it with :meth:`Connection.submit`,
     consider using :meth:`Connection.exercise` instead, which also gives you access to the result of
     exercising the choice.
     """
 
-    __slots__ = ("_choice", "_contract_id", "_argument")
-    if TYPE_CHECKING:
-        _choice: str
-        _contract_id: ContractId
-        _argument: Optional[Any]
+    __slots__ = ("contract_id", "choice", "argument")
+    __match_args__ = ("contract_id", "choice", "argument")
+    contract_id: Final[ContractId]  # type: ignore
+    choice: Final[str]  # type: ignore
+    argument: Final[Any]  # type: ignore
 
     def __init__(self, contract_id: ContractId, choice: str, argument: Optional[Any] = None):
         """
         Initialize an :class:`ExerciseCommand`.
 
         :param contract_id:
             The contract ID of the contract to exercise.
         :param choice:
             The choice to exercise.
         :param argument:
             The choice arguments. Can be omitted for choices that take no arguments.
         """
-        object.__setattr__(self, "_choice", safe_cast(str, choice))
-        object.__setattr__(self, "_contract_id", safe_cast(ContractId, contract_id))
-        object.__setattr__(self, "_argument", dict(argument) if argument is not None else dict())
-
-    @property
-    def contract_id(self) -> ContractId:
-        """
-        The contract ID of the contract to exercise.
-        """
-        return self._contract_id
-
-    @property
-    def choice(self) -> str:
-        """
-        The choice to exercise.
-        """
-        return self._choice
-
-    @property
-    def argument(self) -> Any:
-        """
-        The choice arguments.
-        """
-        return self._argument
+        object.__setattr__(self, "contract_id", safe_cast(ContractId, contract_id))
+        object.__setattr__(self, "choice", safe_cast(str, choice))
+        object.__setattr__(self, "argument", dict(argument) if argument is not None else dict())
 
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, ExerciseCommand)
-            and self.choice == other.choice
             and self.contract_id == other.contract_id
+            and self.choice == other.choice
             and self.argument == other.argument
         )
 
     def __repr__(self):
-        return f"ExerciseCommand({self.choice!r}, {self.contract_id}, {self.argument})"
+        return f"ExerciseCommand({self.contract_id}, {self.choice!r}, {self.argument})"
 
 
-class ExerciseByKeyCommand(Command):
+@final
+class ExerciseByKeyCommand(_Command):
     """
     A command that exercises a choice on a contract identified by its contract key.
 
     Instead of creating an instance of this command and submitting it with :meth:`Connection.submit`,
     consider using :meth:`Connection.exercise_by_key` instead, which also gives you access to the
     result of exercising the choice.
     """
 
-    __slots__ = ("_template_id", "_key", "_choice", "_argument")
-    if TYPE_CHECKING:
-        _template_id: TypeConName
-        _key: Any
-        _choice: str
-        _argument: Optional[Any]
+    __slots__ = ("template_id", "key", "choice", "argument")
+    __match_args__ = ("template_id", "key", "choice", "argument")
+    template_id: TypeConName
+    key: Any
+    choice: str
+    argument: Optional[Any]
 
     def __init__(
         self,
         template_id: Union[str, TypeConName],
         key: Any,
         choice: str,
         argument: Optional[Any] = None,
@@ -291,60 +280,52 @@
         :param key:
             The contract key of the contract to exercise.
         :param choice:
             The choice to exercise.
         :param argument:
             The choice arguments. Can be omitted for choices that take no arguments.
         """
-        object.__setattr__(self, "_template_id", validate_template_id(template_id))
-        object.__setattr__(self, "_key", key)
-        object.__setattr__(self, "_choice", choice)
-        object.__setattr__(self, "_argument", dict(argument) if argument is not None else dict())
-
-    @property
-    def template_id(self) -> TypeConName:
-        """
-        The contract template type.
-        """
-        return self._template_id
-
-    @property
-    def key(self) -> Any:
-        """
-        The contract key of the contract to exercise.
-        """
-        return self._key
-
-    @property
-    def choice(self) -> str:
-        """
-        The choice to exercise.
-        """
-        return self._choice
-
-    @property
-    def argument(self) -> Any:
-        """
-        The choice arguments.
-        """
-        return self._argument
+        object.__setattr__(self, "template_id", validate_template_id(template_id))
+        object.__setattr__(self, "key", key)
+        object.__setattr__(self, "choice", choice)
+        object.__setattr__(self, "argument", dict(argument) if argument is not None else dict())
 
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, ExerciseByKeyCommand)
             and self.template_id == other.template_id
             and self.key == other.key
             and self.choice == other.choice
             and self.argument == other.argument
         )
 
     def __repr__(self):
         return f"ExerciseByKeyCommand({self.template_id}, {self.key}, {self.choice!r}, {self.argument})"
 
 
+if TYPE_CHECKING:
+    # export Command as a union type so that exhaustive type checking can be performed
+    # in Python 3.8 and Python 3.9, Union types are not allowed to be used for isinstance checks,
+    # so the is_command convenience function should be used instead.
+    if sys.version_info >= (3, 10):
+        Command: TypeAlias = (
+            CreateCommand | ExerciseCommand | CreateAndExerciseCommand | ExerciseByKeyCommand
+        )
+    else:
+        Command: TypeAlias = Union[
+            CreateCommand, ExerciseCommand, CreateAndExerciseCommand, ExerciseByKeyCommand
+        ]
+else:
+    # export Command as an actual type so that isinstance checks can be performed
+    Command = _Command
+
+
+Commands: TypeAlias = Union[Command, Sequence[Command]]
+
+
 class CommandMeta:
     """
     Additional fields that accompany a command submission.
 
     .. py:attribute:: workflow_id
         :type: str | None
 
@@ -366,26 +347,25 @@
 
         An optional set of act-as parties to use to submit this command. Note that for a
         ledger with authorization, these parties must be a subset of the parties in the token.
     """
 
     __slots__ = "workflow_id", "command_id", "read_as", "act_as"
 
-    if TYPE_CHECKING:
-        workflow_id: Optional[str]
-        command_id: Optional[str]
-        read_as: Optional[Sequence[Party]]
-        act_as: Optional[Sequence[Party]]
+    workflow_id: Optional[str]
+    command_id: Optional[str]
+    read_as: Optional[Sequence[Party]]
+    act_as: Optional[Sequence[Party]]
 
     def __init__(
         self,
         workflow_id: Optional[str],
         command_id: Optional[str],
-        read_as: Union[None, Party, Collection[Party]],
-        act_as: Union[None, Party, Collection[Party]],
+        read_as: Optional[Parties],
+        act_as: Optional[Parties],
     ):
         if workflow_id:
             if not LEDGER_STRING_REGEX.match(workflow_id):
                 raise ValueError("workflow_id must be a valid ledger string")
         else:
             workflow_id = None
 
@@ -615,21 +595,31 @@
 
 
 class User:
     """
     Full information about a ``User``.
     """
 
-    __slots__ = ("id", "primary_party")
+    __slots__ = ("id", "primary_party", "resource_version", "annotations")
     id: str
     primary_party: Party
+    resource_version: Optional[str]
+    annotations: Optional[Mapping[str, str]]
 
-    def __init__(self, id: str, primary_party: Party):
+    def __init__(
+        self,
+        id: str,
+        primary_party: Party,
+        resource_version: Optional[str] = None,
+        annotations: Optional[Mapping[str, str]] = None,
+    ):
         self.id = id
         self.primary_party = primary_party
+        self.resource_version = resource_version
+        self.annotations = annotations
 
 
 class Right(abc.ABC):
     """
     Information about an individual right for a :class:`User`.
     """
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/blocking/__init__.py` & `dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 :mod:`dazl.ledger.blocking`
 ===========================
 
 Thread-blocking protocols and base classes for connecting to a Daml ledger.
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/blocking/__init__.pyi` & `dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
+
 from __future__ import annotations
 
 from datetime import datetime
-import sys
 from typing import (
     AbstractSet,
     Any,
-    Collection,
     Iterator,
     Optional,
     Protocol,
     Sequence,
     TypeVar,
     Union,
     runtime_checkable,
@@ -19,20 +18,20 @@
 
 from .. import (
     Connection as _Connection,
     PackageService as _PackageService,
     QueryStream as _QueryStream,
 )
 from ...damlast.daml_lf_1 import PackageRef, TypeConName
-from ...prim import ContractData, ContractId, Party, TimeDeltaLike
+from ...prim import ContractData, ContractId, Parties, TimeDeltaLike
 from ...query import Queries, Query
 from ..api_types import (
     ArchiveEvent,
     Boundary,
-    Command,
+    Commands,
     CreateEvent,
     ExerciseResponse,
     MeteringReport,
     PartyInfo,
     Right,
     User,
     Version,
@@ -55,130 +54,130 @@
 class Connection(_Connection, PackageService, Protocol):
     def __enter__(self: Self) -> Self: ...
     def __exit__(self, exc_type, exc_val, exc_tb) -> None: ...
     def open(self) -> None: ...
     def close(self) -> None: ...
     def submit(
         self,
-        commands: Union[Command, Sequence[Command]],
+        commands: Commands,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> None: ...
     def create(
         self,
         template_id: Union[str, TypeConName],
         payload: ContractData,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> CreateEvent: ...
     def exercise(
         self,
         contract_id: ContractId,
         choice_name: str,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ExerciseResponse: ...
     def create_and_exercise(
         self,
         template_id: Union[str, TypeConName],
         payload: ContractData,
         choice_name: str,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ExerciseResponse: ...
     def exercise_by_key(
         self,
         template_id: Union[str, TypeConName],
         choice_name: str,
         key: Any,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ExerciseResponse: ...
     def archive(
         self,
         contract_id: ContractId,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ArchiveEvent: ...
     def archive_by_key(
         self,
         template_id: str,
         key: Any,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> ArchiveEvent: ...
     def get_ledger_end(self, *, timeout: Optional[TimeDeltaLike] = ...) -> str: ...
     def query(
         self,
         template_id: Union[str, TypeConName] = "*",
         query: Query = None,
         /,
         *,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def query_many(
         self,
         *queries: Queries,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def stream(
         self,
         template_id: Union[str, TypeConName] = "*",
         query: Query = None,
         /,
         *,
         offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def stream_many(
         self,
         *queries: Queries,
         offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = ...,
     ) -> QueryStream: ...
     def get_user(
         self, user_id: Optional[str] = None, /, *, timeout: Optional[TimeDeltaLike] = ...
     ) -> User: ...
     def create_user(
         self,
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/blocking/_aiowrapper.py` & `dazl-8.0.0b1/python/dazl/ledger/blocking/_aiowrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import new_event_loop, run_coroutine_threadsafe, set_event_loop, sleep
 from queue import Queue
 from threading import Thread
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/blocking/pkgloader.py` & `dazl-8.0.0b1/python/dazl/ledger/blocking/pkgloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from concurrent.futures import Future, ThreadPoolExecutor
 from datetime import timedelta
 import threading
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/config/__init__.py` & `dazl-8.0.0b1/python/dazl/ledger/config/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 :mod:`dazl.ledger.config` — connection configuration
 ====================================================
 
 This module contains configuration objects for a :class:`Connection`.
 
@@ -113,26 +113,39 @@
 """
 
 from __future__ import annotations
 
 import itertools
 import logging
 from logging import Logger
-from os import PathLike
-from typing import Collection, Optional, Union
+import sys
+from typing import Optional
 
 from ...damlast.lookup import MultiPackageLookup
-from ...prim import Party, TimeDeltaLike
-from .access import AccessConfig, PropertyBasedAccessConfig, TokenBasedAccessConfig, create_access
+from .access import (
+    AccessConfig,
+    AccessConfigArgs,
+    PropertyBasedAccessConfig,
+    TokenBasedAccessConfig,
+    _AccessConfigArgs,
+    create_access,
+)
 from .argv import configure_parser
-from .ssl import SSLConfig
-from .url import URLConfig, create_url
+from .log import LoggerArgs
+from .ssl import SSLConfig, SSLConfigArgs, _SSLConfigArgs
+from .url import URLConfig, URLConfigArgs, _URLConfigArgs, create_url
+
+if sys.version_info >= (3, 12):
+    from typing import Unpack
+else:
+    from typing_extensions import Unpack
 
 __all__ = [
     "Config",
+    "ConfigArgs",
     "AccessConfig",
     "SSLConfig",
     "URLConfig",
     "TokenBasedAccessConfig",
     "PropertyBasedAccessConfig",
     "create_access",
     "create_url",
@@ -141,50 +154,30 @@
 
 # an incrementing counter that helps keep loggers for individual config connections unique
 # (see https://mail.python.org/pipermail//python-ideas/2016-August/041871.html); this is safe to
 # do even in multithreaded environments because ultimately we're reusing the GIL as our lock
 id_generator = itertools.count()
 
 
+class ConfigArgs(AccessConfigArgs, SSLConfigArgs, URLConfigArgs, LoggerArgs, total=False):
+    logger_name: Optional[str]
+    log_level: Optional[str]
+    lookup: Optional[MultiPackageLookup]
+
+
 # PyCharm thinks ``from .url import ...`` clashes with variables named ``url``
 # (same with ``ssl`` and ``access``).
 # noinspection PyShadowingNames
 class Config:
     """
     Stores configuration for a :class:`Connection`.
     """
 
     @classmethod
-    def create(
-        cls,
-        url: Optional[str] = None,
-        host: Optional[str] = None,
-        port: Optional[int] = None,
-        scheme: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
-        admin: Optional[bool] = False,
-        ledger_id: Optional[str] = None,
-        application_name: Optional[str] = None,
-        oauth_token: Optional[str] = None,
-        oauth_token_file: Optional[str] = None,
-        ca: Optional[bytes] = None,
-        ca_file: Optional[PathLike] = None,
-        cert: Optional[bytes] = None,
-        cert_file: Optional[PathLike] = None,
-        cert_key: Optional[bytes] = None,
-        cert_key_file: Optional[PathLike] = None,
-        connect_timeout: Optional[TimeDeltaLike] = None,
-        retry_timeout: Optional[TimeDeltaLike] = None,
-        use_http_proxy: bool = True,
-        logger: Optional[Logger] = None,
-        logger_name: Optional[str] = None,
-        log_level: Optional[str] = None,
-        lookup: "Optional[MultiPackageLookup]" = None,
-    ) -> "Config":
+    def create(cls, **kwargs: Unpack[ConfigArgs]) -> Config:
         """
         Create a :class:`Config` object from the supplied parameters.
 
         The remote can be configured either by supplying a URL or by supplying a host (and optional
         port and scheme). If none of ``url``, ``host``, ``port``, or ``scheme`` are supplied, then
         environment variables are consulted; if no environment variables are specified either, then
         default values are used.
@@ -313,62 +306,93 @@
         :param log_level:
             The logging level for the logger. The default is ``warn``. Only used if ``logger`` is
             not provided.
         :param lookup:
             An alternate symbol table to use to store package information. You should not normally
             need to set this value.
         """
+        logger = kwargs.get("logger", None)
+        logger_name = kwargs.get("logger_name", None)
+        log_level = kwargs.get("log_level")
         if logger is None:
             if not logger_name:
                 logger_name = f"dazl.conn.{next(id_generator)}"
             logger = logging.getLogger(logger_name)
             if log_level is not None:
                 logger.setLevel(log_level)
 
-        url_config = create_url(
-            url=url,
-            host=host,
-            port=port,
-            scheme=scheme,
-            connect_timeout=connect_timeout,
-            retry_timeout=retry_timeout,
-            use_http_proxy=use_http_proxy,
-            logger=logger,
-        )
-
-        access_config = create_access(
-            read_as=read_as,
-            act_as=act_as,
-            admin=admin,
-            ledger_id=ledger_id,
-            application_name=application_name,
-            oauth_token=oauth_token,
-            oauth_token_file=oauth_token_file,
-            logger=logger,
-        )
-
-        ssl_config = SSLConfig(
-            ca=ca,
-            ca_file=ca_file,
-            cert=cert,
-            cert_file=cert_file,
-            cert_key=cert_key,
-            cert_key_file=cert_key_file,
-            logger=logger,
-        )
+        lookup = kwargs.get("lookup", None)
+
+        url_config_args = _URLConfigArgs()
+        if "url" in kwargs:
+            url_config_args["url"] = kwargs["url"]
+        if "host" in kwargs:
+            url_config_args["host"] = kwargs["host"]
+        if "port" in kwargs:
+            url_config_args["port"] = kwargs["port"]
+        if "scheme" in kwargs:
+            url_config_args["scheme"] = kwargs["scheme"]
+        if "connect_timeout" in kwargs:
+            url_config_args["connect_timeout"] = kwargs["connect_timeout"]
+        if "retry_timeout" in kwargs:
+            url_config_args["retry_timeout"] = kwargs["retry_timeout"]
+        if "use_http_proxy" in kwargs:
+            url_config_args["use_http_proxy"] = kwargs["use_http_proxy"]
+        if logger is not None:
+            url_config_args["logger"] = logger
+
+        url_config = create_url(**url_config_args)
+
+        access_config_args = _AccessConfigArgs()
+        if "read_as" in kwargs:
+            access_config_args["read_as"] = kwargs["read_as"]
+        if "act_as" in kwargs:
+            access_config_args["act_as"] = kwargs["act_as"]
+        if "admin" in kwargs:
+            access_config_args["admin"] = kwargs["admin"]
+        if "ledger_id" in kwargs:
+            access_config_args["ledger_id"] = kwargs["ledger_id"]
+        if "application_name" in kwargs:
+            access_config_args["application_name"] = kwargs["application_name"]
+        if "oauth_token" in kwargs:
+            access_config_args["oauth_token"] = kwargs["oauth_token"]
+        if "oauth_token_file" in kwargs:
+            access_config_args["oauth_token_file"] = kwargs["oauth_token_file"]
+        if logger is not None:
+            access_config_args["logger"] = logger
+
+        access_config = create_access(**access_config_args)
+
+        ssl_config_args = _SSLConfigArgs()
+        if "ca" in kwargs:
+            ssl_config_args["ca"] = kwargs["ca"]
+        if "ca_file" in kwargs:
+            ssl_config_args["ca_file"] = kwargs["ca_file"]
+        if "cert" in kwargs:
+            ssl_config_args["cert"] = kwargs["cert"]
+        if "cert_file" in kwargs:
+            ssl_config_args["cert_file"] = kwargs["cert_file"]
+        if "cert_key" in kwargs:
+            ssl_config_args["cert_key"] = kwargs["cert_key"]
+        if "cert_key_file" in kwargs:
+            ssl_config_args["cert_key_file"] = kwargs["cert_key_file"]
+        if logger is not None:
+            ssl_config_args["logger"] = logger
+
+        ssl_config = SSLConfig(**ssl_config_args)
 
         return cls(access_config, ssl_config, url_config, logger, lookup)
 
     def __init__(
         self,
         access: AccessConfig,
         ssl: SSLConfig,
         url: URLConfig,
         logger: Logger,
-        lookup: "Optional[MultiPackageLookup]" = None,
+        lookup: Optional[MultiPackageLookup] = None,
     ):
         """
         Initialize an instance of :class:`Config`.
         """
         self.access = access
         self.ssl = ssl
         self.url = url
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/config/access.py` & `dazl-8.0.0b1/python/dazl/ledger/config/access.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import base64
 from collections.abc import MutableSet as MutableSetBase, Set as SetBase
 import json
-from logging import Logger
 import os
 from pathlib import Path
+import sys
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Collection,
     Iterator,
     Literal,
     Mapping,
     MutableSet,
     Optional,
     Protocol,
+    TypedDict,
     Union,
     runtime_checkable,
 )
 import warnings
 
 from ... import _repr
-from ...prim import Party
+from ...prim import Parties, Party
 from .exc import ConfigError
+from .log import LoggerArgs
+
+if sys.version_info >= (3, 12):
+    from typing import Unpack
+else:
+    from typing_extensions import Unpack
 
 __all__ = [
     "AccessConfig",
+    "AccessConfigArgs",
+    "_AccessConfigArgs",
     "TokenBasedAccessConfig",
     "PropertyBasedAccessConfig",
     "PartyRights",
     "PartyRightsSet",
     "create_access",
 ]
 
@@ -48,38 +57,50 @@
 def parties_from_env(*env_vars: str) -> AbstractSet[Party]:
     """
     Read the set of parties
     """
     return {Party(p) for env_var in env_vars for p in os.getenv(env_var, "").split(",") if p}
 
 
+class AccessConfigArgs(TypedDict, total=False):
+    read_as: Optional[Parties]
+    act_as: Optional[Parties]
+    admin: Optional[bool]
+    ledger_id: Optional[str]
+    application_name: Optional[str]
+    oauth_token: Optional[str]
+    oauth_token_file: Optional[str]
+
+
+class _AccessConfigArgs(AccessConfigArgs, LoggerArgs, total=False):
+    pass
+
+
 # mypy note: typing.overload cannot properly express a more correct signature for this function,
 #  which is that if oauth_token is supplied, then a TokenBasedAccessConfig class is returned and
 #  otherwise, a PropertyBasedAccessConfig class is returned. Trying to type this properly with
 #  overloads results in:
 #     "Not all union combinations were tried because there are too many unions"
 #  It's also worth nothing that our only usage of this function also supplies all parameters since
 #  we're effectively just passing **kwargs around, so it's not clear a more accurate type helps much
 #  anyway.
-def create_access(
-    *,
-    read_as: Union[None, Party, Collection[Party]] = None,
-    act_as: Union[None, Party, Collection[Party]] = None,
-    admin: Optional[bool] = None,
-    ledger_id: Optional[str] = None,
-    application_name: Optional[str] = None,
-    oauth_token: Optional[str] = None,
-    oauth_token_file: Optional[str] = None,
-    logger: Optional[Logger] = None,
-) -> "AccessConfig":
+def create_access(**kwargs: Unpack[_AccessConfigArgs]) -> AccessConfig:
     """
     Create an appropriate instance of :class:`AccessConfig`.
 
     See :meth:`Config.create` for a more detailed description of these parameters.
     """
+    read_as = kwargs.get("read_as", None)
+    act_as = kwargs.get("act_as", None)
+    admin = kwargs.get("admin", None)
+    ledger_id = kwargs.get("ledger_id", None)
+    application_name = kwargs.get("application_name", None)
+    oauth_token = kwargs.get("oauth_token", None)
+    oauth_token_file = kwargs.get("oauth_token_file", None)
+
     # admin = None is effectively the same as admin = False in this context
     is_property_based = read_as or act_as or admin or ledger_id or application_name
     if not is_property_based and not oauth_token and not oauth_token_file:
         # none of the access-related parameters were passed in, so try to read some from the
         # environment
         act_as = parties_from_env("DAML_LEDGER_ACT_AS", "DAML_LEDGER_PARTY")
         read_as = parties_from_env("DAML_LEDGER_READ_AS", "DABL_PUBLIC_PARTY")
@@ -348,16 +369,16 @@
     Access configuration that is manually specified outside of an authentication/authorization
     framework. Suitable for local testing or when no auth server is available, and the Ledger API
     inherently trusts any caller to provide its own authentication and authorization.
     """
 
     def __init__(
         self,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         admin: Optional[bool] = False,
         ledger_id: Optional[str] = None,
         application_name: Optional[str] = None,
     ):
         """
         Initialize a property-based access configuration.
 
@@ -462,15 +483,15 @@
         """
         Return ``None``, because any token that we are supplying is purely for identification
         purposes and not really a valid server-side issued token.
         """
         return None
 
 
-def parties(p: Union[None, Party, Collection[Party]]) -> Collection[Party]:
+def parties(p: Optional[Parties]) -> Collection[Party]:
     if p is None:
         return []
     elif isinstance(p, str):
         return [Party(p)]
     else:
         return p
 
@@ -537,17 +558,15 @@
     __slots__ = ("_rights", "read_as", "act_as")
 
     def __init__(self):
         self._rights = dict()
         self.read_as = PartyRightsSet(self, False)
         self.act_as = PartyRightsSet(self, True)
 
-    def maybe_add(
-        self, value: "Union[None, Party, Collection[Party]]", has_act_rights: bool
-    ) -> None:
+    def maybe_add(self, value: "Optional[Parties]", has_act_rights: bool) -> None:
         if value is None:
             return
 
         # Party is a fake Python newtype, so isinstance checks don't work on it
         if isinstance(value, str):
             self.add(Party(value), has_act_rights)
         else:
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/config/argv.py` & `dazl-8.0.0b1/python/dazl/ledger/config/argv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 Support for exposing dazl's configuration parameters through :mod:`argparse`.
 """
 from __future__ import annotations
 
 import argparse
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/config/ssl.py` & `dazl-8.0.0b1/python/dazl/ledger/config/ssl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,77 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
-from logging import Logger
 from os import PathLike, fspath
-from typing import TYPE_CHECKING, Optional
+import sys
+from typing import TYPE_CHECKING, Optional, TypedDict
+
+from .log import LoggerArgs
+
+if sys.version_info >= (3, 12):
+    from typing import Unpack
+else:
+    from typing_extensions import Unpack
 
 if TYPE_CHECKING:
     # We refer to the Config class in a docstring and
     # without this import, Sphinx can't resolve the reference
     # noinspection PyUnresolvedReferences
     from . import Config
 
 
+__all__ = ["SSLConfig", "SSLConfigArgs", "_SSLConfigArgs"]
+
+
+class SSLConfigArgs(TypedDict, total=False):
+    ca: Optional[bytes]
+    ca_file: Optional[PathLike]
+    cert: Optional[bytes]
+    cert_file: Optional[PathLike]
+    cert_key: Optional[bytes]
+    cert_key_file: Optional[PathLike]
+
+
+class _SSLConfigArgs(SSLConfigArgs, LoggerArgs, total=False):
+    pass
+
+
 class SSLConfig:
     """
     Configuration parameters that affect SSL connections.
 
     See :meth:`Config.create` for a more detailed description of these parameters.
     """
 
-    def __init__(
-        self,
-        ca: Optional[bytes] = None,
-        ca_file: Optional[PathLike] = None,
-        cert: Optional[bytes] = None,
-        cert_file: Optional[PathLike] = None,
-        cert_key: Optional[bytes] = None,
-        cert_key_file: Optional[PathLike] = None,
-        logger: Optional[Logger] = None,
-    ):
-        self._ca: Optional[bytes]
-        self._cert: Optional[bytes]
-        self._cert_key: Optional[bytes]
+    def __init__(self, **kwargs: Unpack[_SSLConfigArgs]):
+        self._ca = kwargs.get("ca", None)
+        self._cert = kwargs.get("cert", None)
+        self._cert_key = kwargs.get("cert_key", None)
 
-        if ca_file:
-            if ca:
+        if ca_file := kwargs.get("ca_file", None):
+            if self._ca:
                 raise ValueError("ca and ca_file cannot both be specified at the same time")
             with open(fspath(ca_file), "rb") as f:
                 self._ca = f.read()
-        else:
-            self._ca = ca
 
-        if cert_file:
-            if cert:
+        if cert_file := kwargs.get("cert_file", None):
+            if self._cert:
                 raise ValueError("cert and cert_file cannot both be specified at the same time")
             with open(fspath(cert_file), "rb") as f:
                 self._cert = f.read()
-        else:
-            self._cert = cert
 
-        if cert_key_file:
-            if cert_key:
+        if cert_key_file := kwargs.get("cert_key_file", None):
+            if self._cert_key:
                 raise ValueError(
                     "cert_key and cert_key_file cannot both be specified at the same time"
                 )
             with open(fspath(cert_key_file), "rb") as f:
                 self._cert_key = f.read()
-        else:
-            self._cert_key = cert_key
 
     def __bool__(self):
         """
         True if SSL settings are supplied; otherwise False if no SSL settings of any kind were
         supplied.
         """
         return bool(self._ca or self._cert or self._cert_key)
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/config/url.py` & `dazl-8.0.0b1/python/dazl/ledger/config/url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import timedelta
 import ipaddress
 from logging import Logger, getLogger
 import os
 from reprlib import repr
+import sys
 from types import MappingProxyType
-from typing import TYPE_CHECKING, Optional, Protocol, runtime_checkable
+from typing import TYPE_CHECKING, Optional, Protocol, TypedDict, runtime_checkable
 from urllib.parse import urlparse
 import warnings
 
 from ...prim import TimeDeltaLike, to_timedelta
 from .exc import ConfigError, ConfigWarning
+from .log import LoggerArgs
+
+if sys.version_info >= (3, 12):
+    from typing import Unpack
+else:
+    from typing_extensions import Unpack
 
 __all__ = [
     "URLConfig",
+    "URLConfigArgs",
+    "_URLConfigArgs",
     "create_url",
     "KNOWN_SCHEME_PORTS",
     "DEFAULT_CONNECT_TIMEOUT",
     "DEFAULT_RETRY_TIMEOUT",
 ]
 
 if TYPE_CHECKING:
@@ -42,31 +51,44 @@
 # some environment variables that we frequently refer to
 DAML_LEDGER_URL = "DAML_LEDGER_URL"
 DAML_LEDGER_HOST = "DAML_LEDGER_HOST"
 DAML_LEDGER_PORT = "DAML_LEDGER_PORT"
 DAML_LEDGER_SCHEME = "DAML_LEDGER_SCHEME"
 
 
-def create_url(
-    *,
-    url: Optional[str] = None,
-    host: Optional[str] = None,
-    port: Optional[int] = None,
-    scheme: Optional[str] = None,
-    connect_timeout: Optional[TimeDeltaLike] = None,
-    retry_timeout: Optional[TimeDeltaLike] = None,
-    use_http_proxy: Optional[bool] = None,
-    logger: Optional[Logger] = None,
-):
+class URLConfigArgs(TypedDict, total=False):
+    url: Optional[str]
+    host: Optional[str]
+    port: Optional[int]
+    scheme: Optional[str]
+    connect_timeout: Optional[TimeDeltaLike]
+    retry_timeout: Optional[TimeDeltaLike]
+    use_http_proxy: Optional[bool]
+
+
+class _URLConfigArgs(URLConfigArgs, LoggerArgs, total=False):
+    pass
+
+
+def create_url(**kwargs: Unpack[_URLConfigArgs]):
     """
     Create an instance of :class:`URLConfig`, possibly with values taken from environment variables,
     or defaulted if otherwise unspecified.
 
     See :meth:`Config.create` for a more detailed description of these parameters.
     """
+    url = kwargs.get("url", None)
+    host = kwargs.get("host", None)
+    port = kwargs.get("port", None)
+    scheme = kwargs.get("scheme", None)
+    connect_timeout = kwargs.get("connect_timeout", None)
+    retry_timeout = kwargs.get("retry_timeout", None)
+    use_http_proxy = kwargs.get("use_http_proxy", None)
+    logger = kwargs.get("logger", None)
+
     if logger is None:
         logger = getLogger("dazl.conn")
 
     if not url and not host and not port and not scheme:
         # use environment variables to provide default values
         url = os.getenv(DAML_LEDGER_URL)
         host = os.getenv(DAML_LEDGER_HOST)
@@ -122,20 +144,22 @@
     logger.debug("    url=%s", url)
     logger.debug("    connect_timeout=%s", connect_timeout)
     logger.debug("    retry_timeout=%s", retry_timeout)
     logger.debug("    use_http_proxy=%s", use_http_proxy)
 
     return SimpleURLConfig(
         url=url,
-        connect_timeout=to_timedelta(connect_timeout)
-        if connect_timeout is not None
-        else DEFAULT_CONNECT_TIMEOUT,
-        retry_timeout=to_timedelta(retry_timeout)
-        if retry_timeout is not None
-        else DEFAULT_RETRY_TIMEOUT,
+        connect_timeout=(
+            to_timedelta(connect_timeout)
+            if connect_timeout is not None
+            else DEFAULT_CONNECT_TIMEOUT
+        ),
+        retry_timeout=(
+            to_timedelta(retry_timeout) if retry_timeout is not None else DEFAULT_RETRY_TIMEOUT
+        ),
         use_http_proxy=use_http_proxy,
     )
 
 
 @runtime_checkable
 class URLConfig(Protocol):
     """
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/errors.py` & `dazl-8.0.0b1/python/dazl/ledger/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 from typing import TYPE_CHECKING, Callable, Optional, TypeVar
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/grpc/channel.py` & `dazl-8.0.0b1/python/dazl/ledger/grpc/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Any, AsyncIterable, Callable, Iterable, List, Tuple, TypeVar, Union, cast
 from urllib.parse import urlparse
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/grpc/codec_aio.py` & `dazl-8.0.0b1/python/dazl/ledger/grpc/codec_aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 This module contains the mapping between Protobuf objects and Python/dazl types.
 """
 
 from __future__ import annotations
 
@@ -227,15 +227,21 @@
             package_id=package_ref(name),
             module_name=str(module_name(name)),
             entity_name=module_local_name(name),
         )
 
     @staticmethod
     def encode_user(user: User, /) -> lapiadminpb.User:
-        return lapiadminpb.User(id=user.id, primary_party=user.primary_party)
+        return lapiadminpb.User(
+            id=user.id,
+            primary_party=user.primary_party,
+            metadata=lapiadminpb.ObjectMeta(
+                resource_version=user.resource_version, annotations=user.annotations
+            ),
+        )
 
     @staticmethod
     def encode_right(right: Right, /) -> lapiadminpb.Right:
         if right == Admin:
             return lapiadminpb.Right(participant_admin=lapiadminpb.Right.ParticipantAdmin())
         elif isinstance(right, ReadAs):
             return lapiadminpb.Right(can_read_as=lapiadminpb.Right.CanReadAs(party=right.party))
@@ -243,26 +249,26 @@
             return lapiadminpb.Right(can_act_as=lapiadminpb.Right.CanActAs(party=right.party))
         else:
             raise ValueError(f"unknown kind of right: {right!r}")
 
     @staticmethod
     def encode_begin_offset(offset: Optional[str], /) -> lapipb.LedgerOffset:
         if offset is None:
-            return lapipb.LedgerOffset(boundary=0)
+            return lapipb.LedgerOffset(boundary=lapipb.LedgerOffset.LEDGER_BEGIN)
         else:
             return lapipb.LedgerOffset(absolute=offset)
 
     @staticmethod
     def encode_end_offset(offset: Union[str, None, End], /) -> Optional[lapipb.LedgerOffset]:
         if offset is None:
             # there is no ending offset (the stream will never naturally terminate)
             return None
         elif isinstance(offset, End):
             # the offset goes up until the current end of the ledger
-            return lapipb.LedgerOffset(boundary=1)
+            return lapipb.LedgerOffset(boundary=lapipb.LedgerOffset.LEDGER_END)
         else:
             # the offset is absolute
             return lapipb.LedgerOffset(absolute=offset)
 
     async def decode_created_event(self, event: lapipb.CreatedEvent, /) -> CreateEvent:
         cid = self.decode_contract_id(event)
         cdata = await self.decode_value(con(cid.value_type), event.create_arguments)
@@ -378,15 +384,20 @@
                 PackageRef(identifier.package_id), DottedName(identifier.module_name.split("."))
             ),
             DottedName(identifier.entity_name.split(".")).segments,
         )
 
     @staticmethod
     def decode_user(user: lapiadminpb.User, /) -> User:
-        return User(id=user.id, primary_party=Party(user.primary_party))
+        return User(
+            id=user.id,
+            primary_party=Party(user.primary_party),
+            resource_version=user.metadata.resource_version,
+            annotations=dict(user.metadata.annotations),
+        )
 
     @staticmethod
     def decode_right(right: lapiadminpb.Right, /) -> Right:
         kind = right.WhichOneof("kind")
         if kind == "participant_admin":
             return Admin
         elif kind == "can_read_as":
```

### Comparing `dazl-8.0.0a4/python/dazl/ledger/grpc/conn_aio.py` & `dazl-8.0.0b1/python/dazl/ledger/grpc/conn_aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 This module contains the mapping between gRPC calls and Python/dazl types.
 """
 
 from __future__ import annotations
 
@@ -32,14 +32,15 @@
 from ..._gen.com.daml.ledger.api import v1 as lapipb
 from ..._gen.com.daml.ledger.api.v1 import admin as lapiadminpb
 from ...damlast.daml_lf_1 import PackageRef, TypeConName
 from ...damlast.util import is_match
 from ...prim import (
     ContractData,
     ContractId,
+    Parties,
     Party,
     TimeDeltaLike,
     datetime_to_timestamp,
     to_parties,
     to_timedelta,
 )
 from ...query import Filter, Queries, Query, parse_query
@@ -48,22 +49,25 @@
 from ..api_types import (
     ActAs,
     Admin,
     ArchiveEvent,
     Boundary,
     Command,
     CommandMeta,
+    Commands,
     CreateEvent,
     ExerciseResponse,
     MeteringReport,
     PartyInfo,
     ReadAs,
     Right,
     User,
     Version,
+    is_command,
+    to_commands,
 )
 from ..config import Config
 from ..config.access import TokenBasedAccessConfig
 from ..errors import ProtocolWarning, _allow_cancel, _translate_exceptions
 from .channel import create_channel
 from .codec_aio import Codec
 
@@ -153,21 +157,21 @@
     def _retry_timeout(self, timeout: Optional[TimeDeltaLike]) -> timedelta:
         return to_timedelta(timeout) if timeout is not None else self._config.url.retry_timeout
 
     # region Write API
 
     async def submit(
         self,
-        commands: Union[Command, Sequence[Command]],
+        commands: Commands,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> None:
         """
         Submit one or more commands to the Ledger API.
 
         You should generally prefer trying to use :meth:`create`, :meth:`exercise`,
         :meth:`exercise_by_key`, or :meth:`create_and_exercise`, as they are available over both
@@ -175,41 +179,46 @@
         information about what happened.
 
         This method can be used to submit multiple disparate commands as a single transaction, but
         if you find yourself needing to do this, you may want to consider moving more of your logic
         into Daml so that only a single command is needed from the outside in order to satisfy your
         use case.
         """
-        if commands is None:
+        commands = to_commands(commands)
+        if not commands:
             return
-        elif isinstance(commands, Command):
-            commands = [commands]
+
         retry_timeout = self._retry_timeout(timeout)
         stub = lapipb.CommandServiceStub(self.channel)
 
         meta = self._command_meta(
             workflow_id=workflow_id, command_id=command_id, read_as=read_as, act_as=act_as
         )
-        commands = await asyncio.gather(*map(self._codec.encode_command, commands))
-        request = self._submit_and_wait_request(commands, meta)
+
+        if len(commands) == 1:
+            command_seq = [await self._codec.encode_command(commands[0])]
+        else:
+            command_seq = await asyncio.gather(*map(self._codec.encode_command, commands))
+
+        request = self._submit_and_wait_request(command_seq, meta)
         await retry(
             lambda: stub.SubmitAndWait(request, timeout=retry_timeout.total_seconds()),
             timeout=retry_timeout,
         )
 
     async def create(
         self,
         template_id: Union[str, TypeConName],
         payload: ContractData,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> CreateEvent:
         """
         Create a contract for a given template.
 
         :param template_id:
             The template of the contract to be created.
@@ -255,16 +264,16 @@
         contract_id: ContractId,
         choice_name: str,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> ExerciseResponse:
         """
         Exercise a choice on a contract identified by its contract ID.
 
         :param contract_id:
             The contract ID of the contract to exercise.
@@ -318,16 +327,16 @@
         payload: ContractData,
         choice_name: str,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> ExerciseResponse:
         """
         Exercise a choice on a newly-created contract, in a single transaction.
 
         :param template_id:
             The template of the contract to be created (positional argument only).
@@ -384,16 +393,16 @@
         choice_name: str,
         key: Any,
         argument: Optional[ContractData] = None,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> ExerciseResponse:
         """
         Exercise a choice on a contract identified by its contract key.
 
         :param template_id:
             The template of the contract to be created (positional argument only).
@@ -443,16 +452,16 @@
     async def archive(
         self,
         contract_id: ContractId,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> ArchiveEvent:
         """
         Archive a choice on a contract identified by its contract ID.
 
         :param contract_id:
             The contract ID of the contract to exercise.
@@ -488,16 +497,16 @@
         self,
         template_id: str,
         key: Any,
         /,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> ArchiveEvent:
         """
         Exercise a choice on a contract identified by its contract key.
 
         :param template_id:
             The template of the contract to be created (positional argument only).
@@ -557,16 +566,16 @@
         )
 
     def _command_meta(
         self,
         *,
         workflow_id: Optional[str] = None,
         command_id: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
-        act_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
+        act_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ):
         read_as = self._read_as(read_as)
         if act_as is None:
             act_as = self._config.access.act_as
 
         return CommandMeta(
@@ -595,15 +604,15 @@
         self,
         template_id: Union[str, TypeConName] = "*",
         query: Query = None,
         /,
         *,
         begin_offset: Optional[str] = None,
         end_offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> QueryStream:
         """
         Return the create events from the active contract set service as a stream.
 
         If you find yourself repeatedly calling :meth:`query` or :meth:`query_many` over the same
         set of templates, you may want to consider :class:`ACS` instead, which is a utility class
@@ -634,15 +643,15 @@
         )
 
     def query_many(
         self,
         *queries: Queries,
         begin_offset: Optional[str] = None,
         end_offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> QueryStream:
         """
         Return the create events from the active contract set service as a stream.
 
         If you find yourself repeatedly calling :meth:`query` or :meth:`query_many` over the same
         set of templates, you may want to consider :class:`ACS` instead, which is a utility class
@@ -673,15 +682,15 @@
     def stream(
         self,
         template_id: Union[str, TypeConName] = "*",
         query: Query = None,
         /,
         *,
         offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> QueryStream:
         """
         Stream create/archive events.
 
         When ``offset`` is ``None``, create events from the active contract set are returned first,
         followed by a continuous stream of updates (creates/archives).
@@ -710,15 +719,15 @@
             self._retry_timeout(timeout),
         )
 
     def stream_many(
         self,
         *queries: Queries,
         offset: Optional[str] = None,
-        read_as: Union[None, Party, Collection[Party]] = None,
+        read_as: Optional[Parties] = None,
         timeout: Optional[TimeDeltaLike] = None,
     ) -> "QueryStream":
         """
         Stream create/archive events from more than one template ID in the same stream.
 
         When ``offset`` is ``None``, create events from the active contract set are returned first,
         followed by a continuous stream of updates (creates/archives).
@@ -741,15 +750,15 @@
             self,
             parse_query(*queries, server_side_filters=False),
             from_offset_until_forever(offset),
             self._read_as(read_as),
             self._retry_timeout(timeout),
         )
 
-    def _read_as(self, read_as: Union[None, Party, Collection[Party]] = None) -> Collection[Party]:
+    def _read_as(self, read_as: Optional[Parties] = None) -> Collection[Party]:
         if read_as is None:
             return self.config.access.read_as
         else:
             return to_parties(read_as)
 
     # endregion
```

### Comparing `dazl-8.0.0a4/python/dazl/ledgerutil/acs.py` & `dazl-8.0.0b1/python/dazl/ledgerutil/acs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from asyncio import CancelledError, Future, InvalidStateError, ensure_future, get_event_loop, sleep
 from collections.abc import Mapping as MappingBase
 from types import MappingProxyType
 from typing import (
```

### Comparing `dazl-8.0.0a4/python/dazl/ledgerutil/fetch.py` & `dazl-8.0.0b1/python/dazl/ledgerutil/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Optional, Union
 
 from ..damlast import TypeConName
```

### Comparing `dazl-8.0.0a4/python/dazl/metrics/api.py` & `dazl-8.0.0b1/python/dazl/metrics/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
 from datetime import timedelta
```

### Comparing `dazl-8.0.0a4/python/dazl/metrics/instrumenters.py` & `dazl-8.0.0b1/python/dazl/metrics/instrumenters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
 from asyncio import AbstractEventLoop, get_event_loop
 from datetime import datetime, timedelta
```

### Comparing `dazl-8.0.0a4/python/dazl/metrics/prometheus.py` & `dazl-8.0.0b1/python/dazl/metrics/prometheus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
 from datetime import timedelta
 from typing import TYPE_CHECKING, ClassVar, Optional
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/__init__.py` & `dazl-8.0.0b1/python/dazl/pretty/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 :mod:`dazl.pretty` package
 ==========================
 
 This module contains utilities for pretty-printing various types in dazl.
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/pygments_daml_lexer.py` & `dazl-8.0.0b1/python/dazl/pretty/pygments_daml_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from pygments.lexer import inherit
 from pygments.lexers.haskell import HaskellLexer
 from pygments.token import Keyword
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/table/fmt_base.py` & `dazl-8.0.0b1/python/dazl/pretty/table/fmt_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from .model import Formatter
 
 __all__ = ["DEFAULT_FORMATTER_NAME", "get_formatter"]
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/table/fmt_json.py` & `dazl-8.0.0b1/python/dazl/pretty/table/fmt_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Formatting module for outputting captures.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/table/fmt_pretty.py` & `dazl-8.0.0b1/python/dazl/pretty/table/fmt_pretty.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Pretty print format that orders templates by ID, and attempts to render a more compact
 representation.
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/table/model.py` & `dazl-8.0.0b1/python/dazl/pretty/table/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import datetime
 from typing import AbstractSet, Dict, Iterable, Iterator, List, Optional
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/table/write.py` & `dazl-8.0.0b1/python/dazl/pretty/table/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains utilities for deterministically outputting contract information.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/pretty/util.py` & `dazl-8.0.0b1/python/dazl/pretty/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
 from typing import Sequence
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/__init__.py` & `dazl-8.0.0b1/python/dazl/prim/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Contains primitive declarations and functions for working with "native" Python types as they
 correspond to types over the Ledger API.
 """
 
@@ -31,15 +31,15 @@
     to_datetime,
     to_timedelta,
 )
 from .errors import DazlError, DazlWarning
 from .json import JSONEncoder
 from .map import FrozenDict
 from .numbers import decimal_to_str, to_decimal, to_int
-from .party import Party, to_parties, to_party
+from .party import Parties, Party, to_parties, to_party
 
 __all__ = [
     "LEDGER_STRING_REGEX",
     "NAME_STRING_REGEX",
     "PACKAGE_ID_STRING_REGEX",
     "PARTY_ID_STRING_REGEX",
     "to_bool",
@@ -63,10 +63,11 @@
     "DazlWarning",
     "JSONEncoder",
     "FrozenDict",
     "decimal_to_str",
     "to_decimal",
     "to_int",
     "Party",
+    "Parties",
     "to_party",
     "to_parties",
 ]
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/basic.py` & `dazl-8.0.0b1/python/dazl/prim/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import re
 from typing import Any, Optional
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/complex.py` & `dazl-8.0.0b1/python/dazl/prim/complex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Contains functions for working with "native" Python types as they correspond to types over the
 Ledger API.
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/contracts.py` & `dazl-8.0.0b1/python/dazl/prim/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Mapping
 
 if TYPE_CHECKING:
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/datetime.py` & `dazl-8.0.0b1/python/dazl/prim/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import date, datetime, timedelta, timezone
 from decimal import Decimal
 from functools import partial
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/errors.py` & `dazl-8.0.0b1/python/dazl/prim/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
 __all__ = ["DazlError", "DazlWarning", "DazlImportError"]
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/json.py` & `dazl-8.0.0b1/python/dazl/prim/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import date, datetime
 from decimal import Decimal
 import json
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/map.py` & `dazl-8.0.0b1/python/dazl/prim/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 __all__ = ["FrozenDict", "to_hashable"]
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/numbers.py` & `dazl-8.0.0b1/python/dazl/prim/numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from decimal import Decimal
 from typing import Any, Optional
```

### Comparing `dazl-8.0.0a4/python/dazl/prim/party.py` & `dazl-8.0.0b1/python/dazl/prim/party.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+import sys
 from typing import Any, Collection, NewType, Sequence, Union, overload
 
 from .basic import to_str
 
-__all__ = ["Party", "to_party", "to_parties"]
+if sys.version_info >= (3, 11):
+    from typing import TypeAlias
+else:
+    from typing_extensions import TypeAlias
+
+__all__ = ["Party", "Parties", "to_party", "to_parties"]
 
 Party = NewType("Party", str)
+Parties: TypeAlias = Union[Party, Collection[Party]]
 
 
 def to_party(o: Any, /) -> Party:
     return Party(to_str(o))
 
 
 @overload
-def to_parties(o: None, /) -> None:
-    ...
+def to_parties(o: None, /) -> None: ...
 
 
 @overload
-def to_parties(o: Union[str, Party, Collection[str], Collection[Party]], /) -> Sequence[Party]:
-    ...
+def to_parties(o: Union[str, Collection[str], Parties], /) -> Sequence[Party]: ...
 
 
-def to_parties(
-    o: Union[None, str, Party, Collection[str], Collection[Party]], /
-) -> Union[None, Sequence[Party]]:
+def to_parties(o: Union[None, str, Collection[str], Parties], /) -> Union[None, Sequence[Party]]:
     """
     Return the specified object as a collection of parties.
 
     :param o:
         The object to convert to a set of parties.
     """
     if o is None:
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/_base.py` & `dazl-8.0.0b1/python/dazl/protocols/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains the abstract base class that defines the protocol for interacting with a
 process that implements the Ledger API.
 """
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/autodetect.py` & `dazl-8.0.0b1/python/dazl/protocols/autodetect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import datetime
 from functools import partial
 from threading import Event, RLock, Thread
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/core.py` & `dazl-8.0.0b1/python/dazl/protocols/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from typing import Any, Awaitable, Callable, Collection, Mapping, Optional, Sequence, TypeVar, Union
 
 from ..prim import ContractData, ContractId, Party
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/errors.py` & `dazl-8.0.0b1/python/dazl/protocols/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from ..prim import DazlError
 
 __all__ = [
     "ConnectionTimeoutError",
     "UserTerminateRequest",
     "StreamError",
     "ProtocolWarning",
-    "CallbackReturnWarning",
 ]
 
 
 class ConnectionTimeoutError(DazlError):
     """
     Raised when a connection failed to be established before the connection timeout elapsed.
     """
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/events.py` & `dazl-8.0.0b1/python/dazl/protocols/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 # TODO: `automodule reading` directive doesn't appear to work here, have to list each class individually.
 """
 Read-Side Types
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/oauth.py` & `dazl-8.0.0b1/python/dazl/protocols/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/serializers.py` & `dazl-8.0.0b1/python/dazl/protocols/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 # This module will likely be deprecated in v8.
 from typing import Any, Sequence
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/v1/grpc.py` & `dazl-8.0.0b1/python/dazl/protocols/v1/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Support for the gRPC-based Ledger API.
 """
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/v1/pb_parse_event.py` & `dazl-8.0.0b1/python/dazl/protocols/v1/pb_parse_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Conversion methods from Ledger API Protobuf-generated types to dazl/Pythonic types.
 """
 from __future__ import annotations
 
@@ -222,20 +222,20 @@
 
 def serialize_transactions_request(
     f: TransactionFilter, ledger_id: str, party: Party
 ) -> lapipb.GetTransactionsRequest:
     if f.current_offset is not None:
         ledger_offset = lapipb.LedgerOffset(absolute=f.current_offset)
     else:
-        ledger_offset = lapipb.LedgerOffset(boundary=0)
+        ledger_offset = lapipb.LedgerOffset(boundary=lapipb.LedgerOffset.LEDGER_BEGIN)
 
     if f.destination_offset is not None:
         final_offset = lapipb.LedgerOffset(absolute=f.destination_offset)
     else:
-        final_offset = lapipb.LedgerOffset(boundary=1)
+        final_offset = lapipb.LedgerOffset(boundary=lapipb.LedgerOffset.LEDGER_END)
 
     return lapipb.GetTransactionsRequest(
         ledger_id=ledger_id,
         begin=ledger_offset,
         end=final_offset,
         filter=serialize_transaction_filter(f, party),
     )
```

### Comparing `dazl-8.0.0a4/python/dazl/protocols/v1/pb_ser_command.py` & `dazl-8.0.0b1/python/dazl/protocols/v1/pb_ser_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Conversion methods to Ledger API Protobuf-generated types from dazl/Pythonic types.
 """
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/query/__init__.py` & `dazl-8.0.0b1/python/dazl/query/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from collections.abc import Mapping as MappingABC
 from typing import Any, Callable, Collection, Dict, Mapping, Optional, Union
```

### Comparing `dazl-8.0.0a4/python/dazl/scheduler/_base.py` & `dazl-8.0.0b1/python/dazl/scheduler/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import os
 from threading import current_thread, main_thread
 from typing import Optional
```

### Comparing `dazl-8.0.0a4/python/dazl/scheduler/_invoker.py` & `dazl-8.0.0b1/python/dazl/scheduler/_invoker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
 The core scheduling of logic, managing the tricky interaction between the man asyncio event loop and
 background threads.
 """
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/scheduler/_invoker.pyi` & `dazl-8.0.0b1/python/dazl/scheduler/_invoker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 # Type definitions for _scheduler.py.
 #
 # These type definitions live in a separate file instead of in _scheduler.py because
```

### Comparing `dazl-8.0.0a4/python/dazl/server/__init__.py` & `dazl-8.0.0b1/python/dazl/server/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from aiohttp import web
 
 from ..client import _NetworkImpl
```

### Comparing `dazl-8.0.0a4/python/dazl/server/management.py` & `dazl-8.0.0b1/python/dazl/server/management.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Endpoints for managing parties/bots connected via a dazl client.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/server/metrics.py` & `dazl-8.0.0b1/python/dazl/server/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass
 from typing import TYPE_CHECKING, Collection, Mapping
```

### Comparing `dazl-8.0.0a4/python/dazl/testing/_cert.py` & `dazl-8.0.0b1/python/dazl/testing/_cert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from typing import Collection, Optional
 
 
 class Certificate:
```

### Comparing `dazl-8.0.0a4/python/dazl/testing/_sandbox.py` & `dazl-8.0.0b1/python/dazl/testing/_sandbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import get_event_loop
 from contextlib import ExitStack
 from datetime import timedelta
```

### Comparing `dazl-8.0.0a4/python/dazl/testing/connect.py` & `dazl-8.0.0b1/python/dazl/testing/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from asyncio import gather
 from os import PathLike
 from typing import Callable, Collection, List, Literal, Optional, Sequence, Union
@@ -114,15 +114,15 @@
     def __getitem__(self, item: Literal[0]) -> ConnectionWithParty:
         return self
 
     def __len__(self) -> Literal[1]:
         return 1
 
 
-def as_party_collection(p: Union[None, Party, Collection[Party]]) -> Collection[Party]:
+def as_party_collection(p: Optional[Parties]) -> Collection[Party]:
     if not p:
         return []
     elif isinstance(p, str):
         return [Party(o) for o in p.split(",")]
     else:
         return p
```

### Comparing `dazl-8.0.0a4/python/dazl/testing/connect.pyi` & `dazl-8.0.0b1/python/dazl/testing/connect.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,93 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from collections.abc import Sequence as Seq
 from os import PathLike
 from typing import (
     AsyncContextManager,
     BinaryIO,
     Callable,
-    Collection,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
     overload,
 )
 
 from ..ledger.aio import Connection
-from ..prim import Party
+from ..prim import Parties, Party
 
 __all__ = ["connect_with_new_party"]
 NameGenFn = Callable[[int], Optional[str]]
 
 @overload
 def connect_with_new_party(
     *,
     party_count: Literal[1] = 1,
     url: Optional[str] = None,
-    read_as: Union[None, Party, Collection[Party]] = None,
-    act_as: Union[None, Party, Collection[Party]] = None,
+    read_as: Optional[Parties] = None,
+    act_as: Optional[Parties] = None,
     admin: Optional[bool] = False,
     ledger_id: Optional[str] = None,
     dar: Union[None, str, bytes, PathLike, BinaryIO] = None,
     identifier_hint: Union[None, str, NameGenFn] = None,
     display_name: Union[None, str, NameGenFn] = None,
 ) -> AsyncContextManager[ConnectionWithParty]: ...
 @overload
 def connect_with_new_party(
     *,
     party_count: Literal[2],
     url: Optional[str] = None,
-    read_as: Union[None, Party, Collection[Party]] = None,
-    act_as: Union[None, Party, Collection[Party]] = None,
+    read_as: Optional[Parties] = None,
+    act_as: Optional[Parties] = None,
     admin: Optional[bool] = False,
     ledger_id: Optional[str] = None,
     dar: Union[None, str, bytes, PathLike, BinaryIO] = None,
     identifier_hint: Union[None, str, NameGenFn] = None,
     display_name: Union[None, str, NameGenFn] = None,
 ) -> AsyncContextManager[Tuple[ConnectionWithParty, ConnectionWithParty]]: ...
 @overload
 def connect_with_new_party(
     *,
     party_count: Literal[3],
     url: Optional[str] = None,
-    read_as: Union[None, Party, Collection[Party]] = None,
-    act_as: Union[None, Party, Collection[Party]] = None,
+    read_as: Optional[Parties] = None,
+    act_as: Optional[Parties] = None,
     admin: Optional[bool] = False,
     ledger_id: Optional[str] = None,
     dar: Union[None, str, bytes, PathLike, BinaryIO] = None,
     identifier_hint: Union[None, str, NameGenFn] = None,
     display_name: Union[None, str, NameGenFn] = None,
 ) -> AsyncContextManager[Tuple[ConnectionWithParty, ConnectionWithParty, ConnectionWithParty]]: ...
 @overload
 def connect_with_new_party(
     *,
     party_count: Literal[4],
     url: Optional[str] = None,
-    read_as: Union[None, Party, Collection[Party]] = None,
-    act_as: Union[None, Party, Collection[Party]] = None,
+    read_as: Optional[Parties] = None,
+    act_as: Optional[Parties] = None,
     admin: Optional[bool] = False,
     ledger_id: Optional[str] = None,
     dar: Union[None, str, bytes, PathLike, BinaryIO] = None,
     identifier_hint: Union[None, str, NameGenFn] = None,
     display_name: Union[None, str, NameGenFn] = None,
 ) -> AsyncContextManager[
     Tuple[ConnectionWithParty, ConnectionWithParty, ConnectionWithParty, ConnectionWithParty]
 ]: ...
 @overload
 def connect_with_new_party(
     *,
     party_count: int,
     url: Optional[str] = None,
-    read_as: Union[None, Party, Collection[Party]] = None,
-    act_as: Union[None, Party, Collection[Party]] = None,
+    read_as: Optional[Parties] = None,
+    act_as: Optional[Parties] = None,
     admin: Optional[bool] = False,
     ledger_id: Optional[str] = None,
     dar: Union[None, str, bytes, PathLike, BinaryIO] = None,
     identifier_hint: Union[None, str, NameGenFn] = None,
     display_name: Union[None, str, NameGenFn] = None,
 ) -> AsyncContextManager[Sequence[ConnectionWithParty]]: ...
```

### Comparing `dazl-8.0.0a4/python/dazl/util/asyncio_util.py` & `dazl-8.0.0b1/python/dazl/util/asyncio_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,38 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains utilities to help work with ``asyncio``.
 """
 from __future__ import annotations
 
 from asyncio import (
     AbstractEventLoop,
-    AbstractEventLoopPolicy,
     CancelledError,
     Future,
     InvalidStateError,
     Queue as AQueue,
     ensure_future,
     gather,
     get_event_loop,
-    new_event_loop,
+    get_running_loop,
 )
 from dataclasses import dataclass
-from functools import partial, wraps
+from functools import wraps
 from inspect import isawaitable, iscoroutinefunction
-from queue import Queue
-import sys
-import threading
 from typing import (
     Any,
     Awaitable,
     Callable,
     Generator,
     Generic,
     Iterable,
     List,
     Optional,
-    Sequence,
     Tuple,
     TypeVar,
     Union,
     cast,
     no_type_check,
 )
 import warnings
@@ -50,89 +45,14 @@
 U = TypeVar("U")
 
 _PENDING = "PENDING"
 _CANCELLED = "CANCELLED"
 _FINISHED = "FINISHED"
 
 
-def non_reentrant(async_fn):
-    if not iscoroutinefunction(async_fn):
-        raise ValueError("expected a coroutine function")
-
-    calls = []
-
-    @wraps(async_fn)
-    async def _wrap(*args, **kwargs):
-        if not calls:
-            calls.append(None)
-            try:
-                return await async_fn(*args, **kwargs)
-            finally:
-                calls.pop()
-        else:
-            raise InvalidStateError("calls to %r cannot be re-entrant", async_fn)
-
-    return _wrap
-
-
-def isolated_async(async_fn):
-    """
-    Wrap an async function in a thread with its own event loop.
-
-    This function runs by itself in an event loop created specifically for this object on its own thread.
-
-    This function can be used as a decorator to convert an ``async def`` method to a simple method that blocks while
-    executing the method on a background thread.
-
-    :param async_fn:
-        The ``async`` function to invoke.
-    :return:
-        A function that, when invoked, passes its parameters to the underlying function on a background thread in an
-        isolated event loop.
-    """
-    queue = Queue()
-
-    @wraps(async_fn)
-    def invoke(*args, **kwargs):
-        """
-        Invoke the wrapped ``async`` method on a background thread, passing in the specified
-        arguments, and returning the value that the wrapped method returns, or raises an Exception
-        if the ``async`` function throws.
-
-        :param args: The positional arguments to pass.
-        :param kwargs: The keyword arguments to pass.
-        :return: The value from the ``async`` function.
-        """
-        thread = threading.Thread(target=partial(_main, args, kwargs))
-        thread.start()
-        thread.join()
-
-        result, typ, value, traceback = queue.get()
-        if typ is not None:
-            # if we have exception information, then an exception was thrown; rethrow it
-            raise typ(value).with_traceback(traceback)
-
-        else:
-            # we don't have an exception, so assume the result is what we need to pass back
-            return result
-
-    def _main(args, kwargs):
-        try:
-            loop = new_event_loop()
-            result = loop.run_until_complete(async_fn(*args, **kwargs))
-            loop.close()
-
-            queue.put_nowait((result, None, None, None))
-        except:
-            typ, value, traceback = sys.exc_info()
-            queue.put_nowait((None, typ, value, traceback))
-
-    return invoke
-
-
 def await_then(awaitable: Awaitable[T_co], func: Callable[[T_co], U]) -> Awaitable[U]:
     """
     Call a function on the result of an Awaitable, and then return an Awaitable that is resolved
     with that result.
 
     If the Awaitable is already "done", then the function is invoked immediately with the result
     of that Awaitable and an immediately-completed Future is returned with the result of that
@@ -241,26 +161,22 @@
 
     if isinstance(result, FailedInvocation):
         raise result.ex
 
     return result
 
 
-def completed(value, loop=None) -> Future:
-    if loop is None:
-        loop = get_event_loop()
-    fut = loop.create_future()
+def completed(value) -> Future:
+    fut = get_event_loop().create_future()
     fut.set_result(value)
     return fut
 
 
-def failed(exception: BaseException, loop=None) -> Future:
-    if loop is None:
-        loop = get_event_loop()
-    fut = loop.create_future()
+def failed(exception: BaseException) -> Future:
+    fut = get_event_loop().create_future()
     fut.set_exception(exception)
     return fut
 
 
 def propagate(from_: Future, to: Future) -> None:
     """
     Copy the value that ``from_`` is completed with to ``to``, whenever ``from_`` is completed.
@@ -342,19 +258,17 @@
 
 class LongRunningAwaitable:
     """
     An :class:`Awaitable` that "finishes" once all of the futures that have been added to it are
     finished.
     """
 
-    def __init__(self, awaitables: Optional[Iterable[Awaitable[Any]]] = None):
+    def __init__(self) -> None:
         self._fut = get_event_loop().create_future()
         self._coros = []  # type: List[Awaitable[Any]]
-        if awaitables is not None:
-            self.extend(awaitables)
 
     def append(self, *awaitables: Awaitable[Any]) -> None:
         self.extend(awaitables)
 
     def extend(self, awaitables: Iterable[Awaitable[Any]]):
         for a in awaitables:
             f = ensure_future(a)
@@ -502,18 +416,18 @@
         Future for validation purposes, it is necessary for this property to behave in strange ways.
         If this property is accessed in a context where this is a currently running loop, this
         Future will adopt the current running loop as its own, but ONLY if a loop has not yet been
         set. This will usually do the right thing, but in some cases it may be necessary for callers
         to invoke :meth:`set_loop` directly.
         """
         if self.__loop is None:
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", DeprecationWarning)
-                # noinspection PyDeprecation
+            try:
                 self.__loop = get_running_loop()
+            except RuntimeError:
+                pass
         return self.__loop
 
     def set_loop(self, loop: AbstractEventLoop) -> None:
         """
         Set the loop affinity for this future.
 
         It is an error to call this function more than once with different values for the loop.
@@ -653,110 +567,25 @@
         if not self.done():
             self._asyncio_future_blocking = True
             yield self  # This tells Task to wait for completion.
         assert self.done(), "yield from wasn't used with future"
         return self.result()  # May raise too.
 
 
-class DeferredStartTask:
-    """
-    A :class:`Task`-like object that delays starting its coroutine until the :meth:`start` method is
-    called.
-    """
-
-    _asyncio_future_blocking = False
-
-    def __init__(self, cb: Callable[[], Future], start=False, name=None):
-        if not callable(cb):
-            raise ValueError("cb must be callable")
-
-        if start:
-            self._future = cb()
-            self._callback = None
-        else:
-            self._future = get_event_loop().create_future()
-            self._callback = cb
-
-        # This is required to be compatible with the interface of a Future.
-        self._loop = self._future._loop
-        self._name = name or repr(cb)
-
-    def start(self) -> None:
-        """
-        Actually invoke the underlying function (but only if it hasn't been invoked already).
-        """
-        cb = self._callback
-        if cb is not None:
-            self._callback = None
-            propagate(from_=ensure_future(cb()), to=self._future)
-
-    def started(self) -> bool:
-        return self._callback is None
-
-    def cancelled(self) -> bool:
-        return self._future.cancelled()
-
-    def cancel(self) -> bool:
-        self._callback = None
-        return self._future.cancel()
-
-    def result(self) -> Any:
-        return self._future.result()
-
-    def done(self) -> bool:
-        return self._future.done()
-
-    def exception(self) -> Optional[BaseException]:
-        return self._future.exception()
-
-    def add_done_callback(self, callback: "Callable[[Future], Any]", context=None) -> None:
-        if context is None:
-            self._future.add_done_callback(callback)
-        else:
-            self._future.add_done_callback(callback, context=context)  # type: ignore
-
-    def __await__(self):
-        return self._future.__await__()
-
-    def __repr__(self):
-        state = self._future._state if self.started() else "NOT_STARTED"
-        return f"DeferredStartTask({self._name!r}, state={state})"
-
-
-@no_type_check
-def get_running_loop() -> Optional[AbstractEventLoop]:
-    warnings.warn(
-        "get_running_loop() is deprecated, as support for Python 3.6 will be dropped in dazl 8. "
-        "Use Python 3.7+'s asyncio.get_running_loop() instead.",
-        DeprecationWarning,
-    )
-    try:
-        from asyncio import get_running_loop
-
-        try:
-            return get_running_loop()
-        except RuntimeError:
-            return None
-    except ImportError:
-        # noinspection PyProtectedMember
-        from asyncio import _get_running_loop
-
-        return _get_running_loop()
-
-
 # noinspection PyDeprecation
 def safe_create_future():
     warnings.warn(
         "safe_create_future() is deprecated; there is no planned replacement.",
         DeprecationWarning,
         stacklevel=2,
     )
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", DeprecationWarning)
+    try:
         loop = get_running_loop()
+    except RuntimeError:
+        loop = None
     return loop.create_future() if loop is not None else ContextFreeFuture()
 
 
 @no_type_check
 def named_gather(name: str, *awaitables, return_exceptions=False):
     g = gather(*awaitables, return_exceptions=return_exceptions)
     g.__repr__ = staticmethod(lambda _: f"<Gather {name}>")
@@ -790,24 +619,7 @@
     # noinspection PyDeprecation
     def wait(self) -> Awaitable[None]:
         if self._fut is None:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", DeprecationWarning)
                 self._fut = safe_create_future()
         return self._fut
-
-
-class UnsettableEventLoopPolicy(AbstractEventLoopPolicy):
-    def get_event_loop(self) -> AbstractEventLoop:
-        raise Exception("Called get_event_loop")
-
-    def set_event_loop(self, loop: Optional[AbstractEventLoop]) -> None:
-        raise Exception("Called set_event_loop")
-
-    def new_event_loop(self) -> AbstractEventLoop:
-        raise Exception("Called new_event_loop")
-
-    def get_child_watcher(self) -> Any:
-        raise Exception("get_child_watcher")
-
-    def set_child_watcher(self, watcher: Any) -> None:
-        raise Exception("set_child_watcher")
```

### Comparing `dazl-8.0.0a4/python/dazl/util/config_meta.py` & `dazl-8.0.0b1/python/dazl/util/config_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains utilities required by :mod:`dazl.client.config`.
 """
 
 from __future__ import annotations
@@ -30,17 +30,17 @@
         metadata={
             "dazl.config": ConfigParameter(
                 description=description,
                 param_type=param_type,
                 default_value=default_value,
                 long_aliases=frozenset([long_alias]) if long_alias else frozenset(),
                 short_aliases=frozenset([short_alias]) if short_alias else frozenset(),
-                deprecated_aliases=frozenset([deprecated_alias])
-                if deprecated_alias
-                else frozenset(),
+                deprecated_aliases=(
+                    frozenset([deprecated_alias]) if deprecated_alias else frozenset()
+                ),
                 environment_variable=environment_variable,
             )
         },
     )
 
 
 @no_type_check
```

### Comparing `dazl-8.0.0a4/python/dazl/util/enum.py` & `dazl-8.0.0b1/python/dazl/util/enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from enum import Enum
```

### Comparing `dazl-8.0.0a4/python/dazl/util/io.py` & `dazl-8.0.0b1/python/dazl/util/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Utilities for dealing with the file system.
 """
 
 from __future__ import annotations
@@ -10,21 +10,19 @@
 from io import BufferedIOBase
 from pathlib import Path
 import socket
 from typing import BinaryIO, Optional, Union, overload
 
 
 @overload
-def get_bytes(_: None) -> None:
-    ...
+def get_bytes(_: None) -> None: ...
 
 
 @overload
-def get_bytes(_: "Union[bytes, str, Path, BinaryIO]") -> bytes:
-    ...
+def get_bytes(_: "Union[bytes, str, Path, BinaryIO]") -> bytes: ...
 
 
 def get_bytes(src):
     """
     Read the contents of a file as ``bytes``. If ``src`` is ``None``, then ``None`` is returned
     instead.
     """
```

### Comparing `dazl-8.0.0a4/python/dazl/util/proc_util.py` & `dazl-8.0.0b1/python/dazl/util/proc_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import datetime
 import logging
 from subprocess import Popen, TimeoutExpired
 import sys
 from threading import Event, Thread
 import time
 
 from ..prim import DazlError, TimeDeltaLike, to_timedelta
 
+__all__ = ["kill_process_tree", "wait_for_process_port", "ProcessLogger", "ProcessDiedException"]
+
 
 def kill_process_tree(process: Popen):
     """
     Kill a process and its children.
     """
     #
     # noinspection PyBroadException
```

### Comparing `dazl-8.0.0a4/python/dazl/util/termcap.py` & `dazl-8.0.0b1/python/dazl/util/termcap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains helper methods for detecting terminal capabilities.
 """
 
 from __future__ import annotations
 
 from subprocess import DEVNULL, PIPE, Popen
 from typing import Optional, Tuple
 
+__all__ = ["termsize", "print_termcap"]
 
-def termsize() -> "Tuple[Optional[int], Optional[int]]":
+
+def termsize() -> Tuple[Optional[int], Optional[int]]:
     """
     Return the current size of the terminal. If the current terminal is not a tty, then
     ``(None, None)`` is returned.
     """
     try:
         with Popen(["stty", "size"], stdout=PIPE, stderr=DEVNULL) as proc:
             term_size_str = proc.stdout.read().decode("utf8") if proc.stdout is not None else None
```

### Comparing `dazl-8.0.0a4/python/dazl/util/tools.py` & `dazl-8.0.0b1/python/dazl/util/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains miscellaneous utility methods that don't really fit anywhere else.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/util/typing.py` & `dazl-8.0.0b1/python/dazl/util/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This module contains helper utilities for working within the constraints of Python's type system.
 """
 
 from __future__ import annotations
```

### Comparing `dazl-8.0.0a4/python/dazl/values/__init__.py` & `dazl-8.0.0b1/python/dazl/values/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 :mod:`dazl.values` package
 ==========================
 
 The :mod:`dazl.values` module contains utilities for converting between different representations
```

### Comparing `dazl-8.0.0a4/python/dazl/values/canonical.py` & `dazl-8.0.0b1/python/dazl/values/canonical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Any, Mapping, Tuple
 
 from ..damlast.daml_lf_1 import DefDataType, Type
```

### Comparing `dazl-8.0.0a4/python/dazl/values/context.py` & `dazl-8.0.0b1/python/dazl/values/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Mapping, NoReturn, Optional, Sequence
 import warnings
```

### Comparing `dazl-8.0.0a4/python/dazl/values/json.py` & `dazl-8.0.0b1/python/dazl/values/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Mappers for translating to and from native Python types.
 
 Documentation for this encoding format can be found at:
 https://docs.daml.com/json-api/lf-value-specification.html
```

### Comparing `dazl-8.0.0a4/python/dazl/values/mapper.py` & `dazl-8.0.0b1/python/dazl/values/mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Protocol
 
 from ..damlast.daml_lf_1 import DefDataType, Type
```

### Comparing `dazl-8.0.0a4/python/dazl/values/protobuf.py` & `dazl-8.0.0b1/python/dazl/values/protobuf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import collections.abc
 from typing import Any, Optional, Type as PyType, TypeVar
```

### Comparing `dazl-8.0.0a4/python/dazl/values/pysample_encoder.py` & `dazl-8.0.0b1/python/dazl/values/pysample_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import Any
 
 from ..damlast.daml_lf_1 import DefDataType, Type as DamlType
```

### Comparing `dazl-8.0.0a4/python/dazl/values/string.py` & `dazl-8.0.0b1/python/dazl/values/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
+# Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import json
 from typing import Any
```

### Comparing `dazl-8.0.0a4/PKG-INFO` & `dazl-8.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dazl
-Version: 8.0.0a4
+Version: 8.0.0b1
 Summary: high-level Ledger API client for Daml ledgers
 Home-page: https://github.com/digital-asset/dazl-client
 License: Apache-2.0
 Keywords: daml,blockchain,dlt,distributed ledger,digital asset
 Author: Davin K. Tanabe
 Author-email: davin.tanabe@digitalasset.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: oauth
 Provides-Extra: prometheus
 Provides-Extra: pygments
 Provides-Extra: server
 Provides-Extra: tls-testing
 Requires-Dist: aiohttp ; extra == "server"
 Requires-Dist: google-auth ; extra == "oauth"
@@ -39,15 +40,15 @@
 =============================================
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/digital-asset/dazl-client/blob/main/LICENSE)
 <a href="https://circleci.com/gh/digital-asset/dazl-client">
 <img src="https://circleci.com/gh/digital-asset/dazl-client.svg?style=svg">
 </a>
 
-Copyright (c) 2017-2023 Digital Asset (Switzerland) GmbH and/or its affiliates. All Rights Reserved.
+Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All Rights Reserved.
 SPDX-License-Identifier: Apache-2.0
 
 
 Rich Python bindings for accessing Ledger API-based applications.
 
 Documentation
 -------------
```

#### html2text {}

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1 Name: dazl Version: 8.0.0a4 Summary: high-level Ledger
+Metadata-Version: 2.1 Name: dazl Version: 8.0.0b1 Summary: high-level Ledger
 API client for Daml ledgers Home-page: https://github.com/digital-asset/dazl-
 client License: Apache-2.0 Keywords: daml,blockchain,dlt,distributed
 ledger,digital asset Author: Davin K. Tanabe Author-email:
 davin.tanabe@digitalasset.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
-Extra: oauth Provides-Extra: prometheus Provides-Extra: pygments Provides-
-Extra: server Provides-Extra: tls-testing Requires-Dist: aiohttp ; extra ==
-"server" Requires-Dist: google-auth ; extra == "oauth" Requires-Dist:
-googleapis_common_protos (>=1,<2) Requires-Dist: grpcio (>=1.50.0) Requires-
-Dist: oauthlib ; extra == "oauth" Requires-Dist: prometheus_client ; extra ==
-"prometheus" Requires-Dist: protobuf (>=4) Requires-Dist: pyOpenSSL ; extra ==
-"tls-testing" Requires-Dist: pygments ; extra == "pygments" Requires-Dist:
-requests Requires-Dist: semver Requires-Dist: toposort Requires-Dist:
-typing_extensions Project-URL: Repository, https://github.com/digital-asset/
-dazl-client Description-Content-Type: text/markdown Daml Python bindings
-(formerly known as dazl) ============================================= [!
-[License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://
-github.com/digital-asset/dazl-client/blob/main/LICENSE) _[_h_t_t_p_s_:_/_/_c_i_r_c_l_e_c_i_._c_o_m_/
-_g_h_/_d_i_g_i_t_a_l_-_a_s_s_e_t_/_d_a_z_l_-_c_l_i_e_n_t_._s_v_g_?_s_t_y_l_e_=_s_v_g_]Copyright (c) 2017-2023 Digital
-Asset (Switzerland) GmbH and/or its affiliates. All Rights Reserved. SPDX-
-License-Identifier: Apache-2.0 Rich Python bindings for accessing Ledger API-
-based applications. Documentation ------------- The user documentation is
-available online [here](https://digital-asset.github.io/dazl-client).
-Installation ------------ If you just want to use the library, you can install
-it locally with `pip`: ```sh pip install --user dazl ``` Requirements ---------
---- * Python 3.7+ * [Daml Connect](https://www.daml.com) * Python gRPC
-libraries (1.32.0 or later) and Protobuf Examples -------- All of the examples
-below assume you imported `dazl`, and are running a ledger with the default
-scenario generated with `daml new`. Connect to the ledger and submit a single
-command: ```py import asyncio import dazl async def main(): async with
-dazl.connect(url='http://localhost:6865', act_as='Alice') as client: contract =
-{ 'issuer' : 'Alice', 'owner' : 'Alice', 'name' : 'hello world!' } await
-client.create('Main:Asset', contract) asyncio.run(main()) ``` Connect to the
-ledger as a single party, print all contracts, and close: ```py import asyncio
-import dazl from dazl.ledgerutil import ACS async def main(): async with
-dazl.connect(url='http://localhost:6865', read_as='Alice') as conn: async with
-ACS(conn, {"*": {}}) as acs: snapshot = await acs.read() print(snapshot)
-asyncio.run(main()) ``` Building locally ---------------- You will need
-additional dependencies to build locally: * GNU Make 4.3 or later * [Poetry]
-(https://python-poetry.org/) for build/dependency management Once you have
-these prerequisites in place: ```sh make build ``` If you see errors about
-incompatible python versions, switch your environment to python3 using `poetry
-env use python3`, for instance. Tests ----- Tests in the Daml Python bindings
-are written using [pytest](https://docs.pytest.org/en/latest/). You can run
-them by doing: ```sh make test ``` Support ------- The Daml Python bindings
-library are supported under the Daml Enterprise license. If you do not have a
-Daml Enterprise license and are in need of support, have questions or just want
-to engage in friendly conversation anything Daml, contact us on our [Daml
-Community Forum](https://discuss.daml.com).
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Provides-Extra: oauth Provides-Extra:
+prometheus Provides-Extra: pygments Provides-Extra: server Provides-Extra: tls-
+testing Requires-Dist: aiohttp ; extra == "server" Requires-Dist: google-auth ;
+extra == "oauth" Requires-Dist: googleapis_common_protos (>=1,<2) Requires-
+Dist: grpcio (>=1.50.0) Requires-Dist: oauthlib ; extra == "oauth" Requires-
+Dist: prometheus_client ; extra == "prometheus" Requires-Dist: protobuf (>=4)
+Requires-Dist: pyOpenSSL ; extra == "tls-testing" Requires-Dist: pygments ;
+extra == "pygments" Requires-Dist: requests Requires-Dist: semver Requires-
+Dist: toposort Requires-Dist: typing_extensions Project-URL: Repository, https:
+//github.com/digital-asset/dazl-client Description-Content-Type: text/markdown
+Daml Python bindings (formerly known as dazl)
+============================================= [![License](https://
+img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/
+digital-asset/dazl-client/blob/main/LICENSE) _[_h_t_t_p_s_:_/_/_c_i_r_c_l_e_c_i_._c_o_m_/_g_h_/_d_i_g_i_t_a_l_-
+_a_s_s_e_t_/_d_a_z_l_-_c_l_i_e_n_t_._s_v_g_?_s_t_y_l_e_=_s_v_g_]Copyright (c) 2017-2024 Digital Asset
+(Switzerland) GmbH and/or its affiliates. All Rights Reserved. SPDX-License-
+Identifier: Apache-2.0 Rich Python bindings for accessing Ledger API-based
+applications. Documentation ------------- The user documentation is available
+online [here](https://digital-asset.github.io/dazl-client). Installation ------
+------ If you just want to use the library, you can install it locally with
+`pip`: ```sh pip install --user dazl ``` Requirements ------------ * Python
+3.7+ * [Daml Connect](https://www.daml.com) * Python gRPC libraries (1.32.0 or
+later) and Protobuf Examples -------- All of the examples below assume you
+imported `dazl`, and are running a ledger with the default scenario generated
+with `daml new`. Connect to the ledger and submit a single command: ```py
+import asyncio import dazl async def main(): async with dazl.connect(url='http:
+//localhost:6865', act_as='Alice') as client: contract = { 'issuer' : 'Alice',
+'owner' : 'Alice', 'name' : 'hello world!' } await client.create('Main:Asset',
+contract) asyncio.run(main()) ``` Connect to the ledger as a single party,
+print all contracts, and close: ```py import asyncio import dazl from
+dazl.ledgerutil import ACS async def main(): async with dazl.connect(url='http:
+//localhost:6865', read_as='Alice') as conn: async with ACS(conn, {"*": {}}) as
+acs: snapshot = await acs.read() print(snapshot) asyncio.run(main()) ```
+Building locally ---------------- You will need additional dependencies to
+build locally: * GNU Make 4.3 or later * [Poetry](https://python-poetry.org/
+) for build/dependency management Once you have these prerequisites in place:
+```sh make build ``` If you see errors about incompatible python versions,
+switch your environment to python3 using `poetry env use python3`, for
+instance. Tests ----- Tests in the Daml Python bindings are written using
+[pytest](https://docs.pytest.org/en/latest/). You can run them by doing: ```sh
+make test ``` Support ------- The Daml Python bindings library are supported
+under the Daml Enterprise license. If you do not have a Daml Enterprise license
+and are in need of support, have questions or just want to engage in friendly
+conversation anything Daml, contact us on our [Daml Community Forum](https://
+discuss.daml.com).
```

