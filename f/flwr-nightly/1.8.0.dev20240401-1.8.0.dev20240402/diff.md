# Comparing `tmp/flwr_nightly-1.8.0.dev20240401.tar.gz` & `tmp/flwr_nightly-1.8.0.dev20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.8.0.dev20240401.tar", max compression
+gzip compressed data, was "flwr_nightly-1.8.0.dev20240402.tar", max compression
```

## Comparing `flwr_nightly-1.8.0.dev20240401.tar` & `flwr_nightly-1.8.0.dev20240402.tar`

### file list

```diff
@@ -1,211 +1,212 @@
--rw-r--r--   0        0        0    11358 2024-04-01 23:05:40.679554 flwr_nightly-1.8.0.dev20240401/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-01 23:05:40.679554 flwr_nightly-1.8.0.dev20240401/README.md
--rw-r--r--   0        0        0     5863 2024-04-01 23:05:54.083566 flwr_nightly-1.8.0.dev20240401/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     2184 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0     4675 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/flower_toml.py
--rw-r--r--   0        0        0      789 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5016 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0      714 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3675 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      269 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/flower.toml.tpl
--rw-r--r--   0        0        0      408 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      507 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      697 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0       30 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/requirements.numpy.txt.tpl
--rw-r--r--   0        0        0      106 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/requirements.pytorch.txt.tpl
--rw-r--r--   0        0        0      209 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/requirements.tensorflow.txt.tpl
--rw-r--r--   0        0        0      789 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     2300 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1187 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    25445 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8315 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8717 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     8525 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2377 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    14447 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     1006 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2084 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2273 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    11773 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     3016 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11669 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7782 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3115 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     4670 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     4316 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     7325 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     9042 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2491 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24302 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5271 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3450 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7344 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      820 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     9660 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0     4586 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5592 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4761 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3036 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     6734 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12041 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0     8707 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    22005 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     6036 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0      913 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12655 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29187 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    20054 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15685 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15257 1970-01-01 00:00:00.000000 flwr_nightly-1.8.0.dev20240401/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-02 23:05:23.567786 flwr_nightly-1.8.0.dev20240402/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-02 23:05:23.567786 flwr_nightly-1.8.0.dev20240402/README.md
+-rw-r--r--   0        0        0     5863 2024-04-02 23:05:39.559815 flwr_nightly-1.8.0.dev20240402/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     2184 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0     4675 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/flower_toml.py
+-rw-r--r--   0        0        0      789 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3675 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      269 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/flower.toml.tpl
+-rw-r--r--   0        0        0      408 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      507 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      697 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0       30 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/requirements.numpy.txt.tpl
+-rw-r--r--   0        0        0      106 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/requirements.pytorch.txt.tpl
+-rw-r--r--   0        0        0      209 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/requirements.tensorflow.txt.tpl
+-rw-r--r--   0        0        0      789 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     2300 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1187 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    26114 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-02 23:05:23.979786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8717 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     8560 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2377 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    14482 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     1006 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     3016 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11669 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-02 23:05:23.983786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7782 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3115 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     4670 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4356 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     7571 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     9042 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2491 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24302 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3450 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7344 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      820 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0    10106 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0     4586 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5592 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-02 23:05:23.987786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4761 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3036 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3273 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     6734 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0     9586 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    23985 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6058 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-02 23:05:23.991786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-02 23:05:23.995786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15685 2024-04-02 23:05:23.995786 flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15257 1970-01-01 00:00:00.000000 flwr_nightly-1.8.0.dev20240402/PKG-INFO
```

### Comparing `flwr_nightly-1.8.0.dev20240401/LICENSE` & `flwr_nightly-1.8.0.dev20240402/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/README.md` & `flwr_nightly-1.8.0.dev20240402/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/pyproject.toml` & `flwr_nightly-1.8.0.dev20240402/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.8.0-dev20240401"
+version = "1.8.0-dev20240402"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/example.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/flower_toml.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/flower_toml.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/utils.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_BIDI,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPES,
+    ErrorCode,
 )
 from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log, warn_deprecated_feature
 from flwr.common.message import Error
 from flwr.common.object_ref import load_app, validate
 from flwr.common.retry_invoker import RetryInvoker, exponential
 
@@ -479,43 +480,57 @@
 
                 # Retrieve context for this run
                 context = node_state.retrieve_context(run_id=message.metadata.run_id)
 
                 # Create an error reply message that will never be used to prevent
                 # the used-before-assignment linting error
                 reply_message = message.create_error_reply(
-                    error=Error(code=0, reason="Unknown")
+                    error=Error(code=ErrorCode.UNKNOWN, reason="Unknown")
                 )
 
                 # Handle app loading and task message
                 try:
                     # Load ClientApp instance
                     client_app: ClientApp = load_client_app_fn()
 
+                    # Execute ClientApp
                     reply_message = client_app(message=message, context=context)
-                    # Update node state
-                    node_state.update_context(
-                        run_id=message.metadata.run_id,
-                        context=context,
-                    )
                 except Exception as ex:  # pylint: disable=broad-exception-caught
-                    log(ERROR, "ClientApp raised an exception", exc_info=ex)
 
                     # Legacy grpc-bidi
                     if transport in ["grpc-bidi", None]:
+                        log(ERROR, "Client raised an exception.", exc_info=ex)
                         # Raise exception, crash process
                         raise ex
 
                     # Don't update/change NodeState
 
-                    # Create error message
+                    e_code = ErrorCode.CLIENT_APP_RAISED_EXCEPTION
                     # Reason example: "<class 'ZeroDivisionError'>:<'division by zero'>"
                     reason = str(type(ex)) + ":<'" + str(ex) + "'>"
+                    exc_entity = "ClientApp"
+                    if isinstance(ex, LoadClientAppError):
+                        reason = (
+                            "An exception was raised when attempting to load "
+                            "`ClientApp`"
+                        )
+                        e_code = ErrorCode.LOAD_CLIENT_APP_EXCEPTION
+                        exc_entity = "SuperNode"
+
+                    log(ERROR, "%s raised an exception", exc_entity, exc_info=ex)
+
+                    # Create error message
                     reply_message = message.create_error_reply(
-                        error=Error(code=0, reason=reason)
+                        error=Error(code=e_code, reason=reason)
+                    )
+                else:
+                    # No exception, update node state
+                    node_state.update_context(
+                        run_id=message.metadata.run_id,
+                        context=context,
                     )
 
                 # Send
                 send(reply_message)
                 log(INFO, "Sent reply")
 
             # Unregister node
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client_app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/client_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,23 @@
 from flwr.client.typing import ClientFn, Mod
 from flwr.common import Context, Message, MessageType
 from flwr.common.logger import warn_preview_feature
 
 from .typing import ClientAppCallable
 
 
+class ClientAppException(Exception):
+    """Exception raised when an exception is raised while executing a ClientApp."""
+
+    def __init__(self, message: str):
+        ex_name = self.__class__.__name__
+        self.message = f"\nException {ex_name} occurred. Message: " + message
+        super().__init__(self.message)
+
+
 class ClientApp:
     """Flower ClientApp.
 
     Examples
     --------
     Assuming a typical `Client` implementation named `FlowerClient`, you can wrap it in
     a `ClientApp` as follows:
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         next_interval *= PING_BASE_MULTIPLIER + rd
         if not ping_stop_event.is_set():
             ping_stop_event.wait(next_interval)
 
     def create_node() -> None:
         """Set create_node."""
         # Call FleetAPI
-        create_node_request = CreateNodeRequest()
+        create_node_request = CreateNodeRequest(ping_interval=PING_DEFAULT_INTERVAL)
         create_node_response = retry_invoker.invoke(
             stub.CreateNode,
             request=create_node_request,
         )
 
         # Remember the node and the ping-loop thread
         nonlocal node, ping_thread
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/rest_client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         next_interval: float = PING_DEFAULT_INTERVAL - PING_CALL_TIMEOUT
         next_interval *= PING_BASE_MULTIPLIER + rd
         if not ping_stop_event.is_set():
             ping_stop_event.wait(next_interval)
 
     def create_node() -> None:
         """Set create_node."""
-        create_node_req_proto = CreateNodeRequest()
+        create_node_req_proto = CreateNodeRequest(ping_interval=PING_DEFAULT_INTERVAL)
         create_node_req_bytes: bytes = create_node_req_proto.SerializeToString()
 
         res = retry_invoker.invoke(
             requests.post,
             url=f"{base_url}/{PATH_CREATE_NODE}",
             headers={
                 "Accept": "application/protobuf",
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/typing.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/address.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/constant.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ]
 
 # Constants for ping
 PING_DEFAULT_INTERVAL = 30
 PING_CALL_TIMEOUT = 5
 PING_BASE_MULTIPLIER = 0.8
 PING_RANDOM_RANGE = (-0.1, 0.1)
+PING_MAX_INTERVAL = 1e300
 
 
 class MessageType:
     """Message type."""
 
     TRAIN = "train"
     EVALUATE = "evaluate"
@@ -70,7 +71,20 @@
     """Serialisation type."""
 
     NUMPY = "numpy.ndarray"
 
     def __new__(cls) -> SType:
         """Prevent instantiation."""
         raise TypeError(f"{cls.__name__} cannot be instantiated.")
+
+
+class ErrorCode:
+    """Error codes for Message's Error."""
+
+    UNKNOWN = 0
+    LOAD_CLIENT_APP_EXCEPTION = 1
+    CLIENT_APP_RAISED_EXCEPTION = 2
+    NODE_UNAVAILABLE = 3
+
+    def __new__(cls) -> ErrorCode:
+        """Prevent instantiation."""
+        raise TypeError(f"{cls.__name__} cannot be instantiated.")
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/context.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/date.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/dp.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/grpc.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/logger.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/message.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Message."""
 
 from __future__ import annotations
 
 import time
+import warnings
 from dataclasses import dataclass
 
 from .record import RecordSet
 
 DEFAULT_TTL = 3600
 
 
@@ -307,14 +308,21 @@
         ttl : Optional[float] (default: None)
             Time-to-live for this message in seconds. If unset, it will be set based
             on the remaining time for the received message before it expires. This
             follows the equation:
 
             ttl = msg.meta.ttl - (reply.meta.created_at - msg.meta.created_at)
         """
+        if ttl:
+            warnings.warn(
+                "A custom TTL was set, but note that the SuperLink does not enforce "
+                "the TTL yet. The SuperLink will start enforcing the TTL in a future "
+                "version of Flower.",
+                stacklevel=2,
+            )
         # If no TTL passed, use default for message creation (will update after
         # message creation)
         ttl_ = DEFAULT_TTL if ttl is None else ttl
         # Create reply with error
         message = Message(metadata=self._create_reply_metadata(ttl_), error=error)
 
         if ttl is None:
@@ -345,14 +353,21 @@
             ttl = msg.meta.ttl - (reply.meta.created_at - msg.meta.created_at)
 
         Returns
         -------
         Message
             A new `Message` instance representing the reply.
         """
+        if ttl:
+            warnings.warn(
+                "A custom TTL was set, but note that the SuperLink does not enforce "
+                "the TTL yet. The SuperLink will start enforcing the TTL in a future "
+                "version of Flower.",
+                stacklevel=2,
+            )
         # If no TTL passed, use default for message creation (will update after
         # message creation)
         ttl_ = DEFAULT_TTL if ttl is None else ttl
 
         message = Message(
             metadata=self._create_reply_metadata(ttl_),
             content=content,
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/parameter.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/serde.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/typing.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/version.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 _sym_db = _symbol_database.Default()
 
 
 from flwr.proto import node_pb2 as flwr_dot_proto_dot_node__pb2
 from flwr.proto import task_pb2 as flwr_dot_proto_dot_task__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66lwr/proto/fleet.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x15\x66lwr/proto/task.proto\"\x13\n\x11\x43reateNodeRequest\"4\n\x12\x43reateNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"3\n\x11\x44\x65leteNodeRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"\x14\n\x12\x44\x65leteNodeResponse\"D\n\x0bPingRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x15\n\rping_interval\x18\x02 \x01(\x01\"\x1f\n\x0cPingResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"F\n\x12PullTaskInsRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x10\n\x08task_ids\x18\x02 \x03(\t\"k\n\x13PullTaskInsResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12*\n\rtask_ins_list\x18\x02 \x03(\x0b\x32\x13.flwr.proto.TaskIns\"@\n\x12PushTaskResRequest\x12*\n\rtask_res_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.TaskRes\"\xae\x01\n\x13PushTaskResResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12=\n\x07results\x18\x02 \x03(\x0b\x32,.flwr.proto.PushTaskResResponse.ResultsEntry\x1a.\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"\x1e\n\tReconnect\x12\x11\n\treconnect\x18\x01 \x01(\x04\x32\x86\x03\n\x05\x46leet\x12M\n\nCreateNode\x12\x1d.flwr.proto.CreateNodeRequest\x1a\x1e.flwr.proto.CreateNodeResponse\"\x00\x12M\n\nDeleteNode\x12\x1d.flwr.proto.DeleteNodeRequest\x1a\x1e.flwr.proto.DeleteNodeResponse\"\x00\x12;\n\x04Ping\x12\x17.flwr.proto.PingRequest\x1a\x18.flwr.proto.PingResponse\"\x00\x12P\n\x0bPullTaskIns\x12\x1e.flwr.proto.PullTaskInsRequest\x1a\x1f.flwr.proto.PullTaskInsResponse\"\x00\x12P\n\x0bPushTaskRes\x12\x1e.flwr.proto.PushTaskResRequest\x1a\x1f.flwr.proto.PushTaskResResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66lwr/proto/fleet.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x15\x66lwr/proto/task.proto\"*\n\x11\x43reateNodeRequest\x12\x15\n\rping_interval\x18\x01 \x01(\x01\"4\n\x12\x43reateNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"3\n\x11\x44\x65leteNodeRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"\x14\n\x12\x44\x65leteNodeResponse\"D\n\x0bPingRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x15\n\rping_interval\x18\x02 \x01(\x01\"\x1f\n\x0cPingResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"F\n\x12PullTaskInsRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x10\n\x08task_ids\x18\x02 \x03(\t\"k\n\x13PullTaskInsResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12*\n\rtask_ins_list\x18\x02 \x03(\x0b\x32\x13.flwr.proto.TaskIns\"@\n\x12PushTaskResRequest\x12*\n\rtask_res_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.TaskRes\"\xae\x01\n\x13PushTaskResResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12=\n\x07results\x18\x02 \x03(\x0b\x32,.flwr.proto.PushTaskResResponse.ResultsEntry\x1a.\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"\x1e\n\tReconnect\x12\x11\n\treconnect\x18\x01 \x01(\x04\x32\x86\x03\n\x05\x46leet\x12M\n\nCreateNode\x12\x1d.flwr.proto.CreateNodeRequest\x1a\x1e.flwr.proto.CreateNodeResponse\"\x00\x12M\n\nDeleteNode\x12\x1d.flwr.proto.DeleteNodeRequest\x1a\x1e.flwr.proto.DeleteNodeResponse\"\x00\x12;\n\x04Ping\x12\x17.flwr.proto.PingRequest\x1a\x18.flwr.proto.PingResponse\"\x00\x12P\n\x0bPullTaskIns\x12\x1e.flwr.proto.PullTaskInsRequest\x1a\x1f.flwr.proto.PullTaskInsResponse\"\x00\x12P\n\x0bPushTaskRes\x12\x1e.flwr.proto.PushTaskResRequest\x1a\x1f.flwr.proto.PushTaskResResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flwr.proto.fleet_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._options = None
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_options = b'8\001'
   _globals['_CREATENODEREQUEST']._serialized_start=84
-  _globals['_CREATENODEREQUEST']._serialized_end=103
-  _globals['_CREATENODERESPONSE']._serialized_start=105
-  _globals['_CREATENODERESPONSE']._serialized_end=157
-  _globals['_DELETENODEREQUEST']._serialized_start=159
-  _globals['_DELETENODEREQUEST']._serialized_end=210
-  _globals['_DELETENODERESPONSE']._serialized_start=212
-  _globals['_DELETENODERESPONSE']._serialized_end=232
-  _globals['_PINGREQUEST']._serialized_start=234
-  _globals['_PINGREQUEST']._serialized_end=302
-  _globals['_PINGRESPONSE']._serialized_start=304
-  _globals['_PINGRESPONSE']._serialized_end=335
-  _globals['_PULLTASKINSREQUEST']._serialized_start=337
-  _globals['_PULLTASKINSREQUEST']._serialized_end=407
-  _globals['_PULLTASKINSRESPONSE']._serialized_start=409
-  _globals['_PULLTASKINSRESPONSE']._serialized_end=516
-  _globals['_PUSHTASKRESREQUEST']._serialized_start=518
-  _globals['_PUSHTASKRESREQUEST']._serialized_end=582
-  _globals['_PUSHTASKRESRESPONSE']._serialized_start=585
-  _globals['_PUSHTASKRESRESPONSE']._serialized_end=759
-  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_start=713
-  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_end=759
-  _globals['_RECONNECT']._serialized_start=761
-  _globals['_RECONNECT']._serialized_end=791
-  _globals['_FLEET']._serialized_start=794
-  _globals['_FLEET']._serialized_end=1184
+  _globals['_CREATENODEREQUEST']._serialized_end=126
+  _globals['_CREATENODERESPONSE']._serialized_start=128
+  _globals['_CREATENODERESPONSE']._serialized_end=180
+  _globals['_DELETENODEREQUEST']._serialized_start=182
+  _globals['_DELETENODEREQUEST']._serialized_end=233
+  _globals['_DELETENODERESPONSE']._serialized_start=235
+  _globals['_DELETENODERESPONSE']._serialized_end=255
+  _globals['_PINGREQUEST']._serialized_start=257
+  _globals['_PINGREQUEST']._serialized_end=325
+  _globals['_PINGRESPONSE']._serialized_start=327
+  _globals['_PINGRESPONSE']._serialized_end=358
+  _globals['_PULLTASKINSREQUEST']._serialized_start=360
+  _globals['_PULLTASKINSREQUEST']._serialized_end=430
+  _globals['_PULLTASKINSRESPONSE']._serialized_start=432
+  _globals['_PULLTASKINSRESPONSE']._serialized_end=539
+  _globals['_PUSHTASKRESREQUEST']._serialized_start=541
+  _globals['_PUSHTASKRESREQUEST']._serialized_end=605
+  _globals['_PUSHTASKRESRESPONSE']._serialized_start=608
+  _globals['_PUSHTASKRESRESPONSE']._serialized_end=782
+  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_start=736
+  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_end=782
+  _globals['_RECONNECT']._serialized_start=784
+  _globals['_RECONNECT']._serialized_end=814
+  _globals['_FLEET']._serialized_start=817
+  _globals['_FLEET']._serialized_end=1207
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,21 @@
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class CreateNodeRequest(google.protobuf.message.Message):
     """CreateNode messages"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    PING_INTERVAL_FIELD_NUMBER: builtins.int
+    ping_interval: builtins.float
     def __init__(self,
+        *,
+        ping_interval: builtins.float = ...,
         ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ping_interval",b"ping_interval"]) -> None: ...
 global___CreateNodeRequest = CreateNodeRequest
 
 class CreateNodeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     NODE_FIELD_NUMBER: builtins.int
     @property
     def node(self) -> flwr.proto.node_pb2.Node: ...
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/criterion.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/driver/driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower driver service client."""
 
-
 import time
+import warnings
 from typing import Iterable, List, Optional, Tuple
 
 from flwr.common import DEFAULT_TTL, Message, Metadata, RecordSet
 from flwr.common.serde import message_from_taskres, message_to_taskins
 from flwr.proto.driver_pb2 import (  # pylint: disable=E0611
     CreateRunRequest,
     GetNodesRequest,
@@ -87,15 +87,15 @@
 
     def create_message(  # pylint: disable=too-many-arguments
         self,
         content: RecordSet,
         message_type: str,
         dst_node_id: int,
         group_id: str,
-        ttl: float = DEFAULT_TTL,
+        ttl: Optional[float] = None,
     ) -> Message:
         """Create a new message with specified parameters.
 
         This method constructs a new `Message` with given content and metadata.
         The `run_id` and `src_node_id` will be set automatically.
 
         Parameters
@@ -107,33 +107,43 @@
             The type of the message, defining the action to be executed on
             the receiving end.
         dst_node_id : int
             The ID of the destination node to which the message is being sent.
         group_id : str
             The ID of the group to which this message is associated. In some settings,
             this is used as the FL round.
-        ttl : float (default: common.DEFAULT_TTL)
+        ttl : Optional[float] (default: None)
             Time-to-live for the round trip of this message, i.e., the time from sending
             this message to receiving a reply. It specifies in seconds the duration for
-            which the message and its potential reply are considered valid.
+            which the message and its potential reply are considered valid. If unset,
+            the default TTL (i.e., `common.DEFAULT_TTL`) will be used.
 
         Returns
         -------
         message : Message
             A new `Message` instance with the specified content and metadata.
         """
         _, run_id = self._get_grpc_driver_and_run_id()
+        if ttl:
+            warnings.warn(
+                "A custom TTL was set, but note that the SuperLink does not enforce "
+                "the TTL yet. The SuperLink will start enforcing the TTL in a future "
+                "version of Flower.",
+                stacklevel=2,
+            )
+
+        ttl_ = DEFAULT_TTL if ttl is None else ttl
         metadata = Metadata(
             run_id=run_id,
             message_id="",  # Will be set by the server
             src_node_id=self.node.node_id,
             dst_node_id=dst_node_id,
             reply_to_message="",
             group_id=group_id,
-            ttl=ttl,
+            ttl=ttl_,
             message_type=message_type,
         )
         return Message(metadata=metadata, content=content)
 
     def get_node_ids(self) -> List[int]:
         """Get node IDs."""
         grpc_driver, run_id = self._get_grpc_driver_and_run_id()
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/history.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_config.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 def create_node(
     request: CreateNodeRequest,  # pylint: disable=unused-argument
     state: State,
 ) -> CreateNodeResponse:
     """."""
     # Create node
-    node_id = state.create_node()
+    node_id = state.create_node(ping_interval=request.ping_interval)
     return CreateNodeResponse(node=Node(node_id=node_id, anonymous=False))
 
 
 def delete_node(request: DeleteNodeRequest, state: State) -> DeleteNodeResponse:
     """."""
     # Validate node_id
     if request.node.anonymous or request.node.node_id == 0:
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 import json
 import sys
 import time
 import traceback
 from logging import DEBUG, ERROR, INFO, WARN
 from typing import Callable, Dict, List, Optional
 
-from flwr.client.client_app import ClientApp, LoadClientAppError
+from flwr.client.client_app import ClientApp, ClientAppException, LoadClientAppError
 from flwr.client.node_state import NodeState
+from flwr.common.constant import PING_MAX_INTERVAL, ErrorCode
 from flwr.common.logger import log
 from flwr.common.message import Error
 from flwr.common.object_ref import load_app
 from flwr.common.serde import message_from_taskins, message_to_taskres
 from flwr.proto.task_pb2 import TaskIns  # pylint: disable=E0611
 from flwr.server.superlink.state import StateFactory
 
@@ -39,15 +40,15 @@
 def _register_nodes(
     num_nodes: int, state_factory: StateFactory
 ) -> NodeToPartitionMapping:
     """Register nodes with the StateFactory and create node-id:partition-id mapping."""
     nodes_mapping: NodeToPartitionMapping = {}
     state = state_factory.state()
     for i in range(num_nodes):
-        node_id = state.create_node()
+        node_id = state.create_node(ping_interval=PING_MAX_INTERVAL)
         nodes_mapping[node_id] = i
     log(INFO, "Registered %i nodes", len(nodes_mapping))
     return nodes_mapping
 
 
 # pylint: disable=too-many-arguments,too-many-locals
 async def worker(
@@ -89,17 +90,26 @@
             log(DEBUG, "Terminating async worker: %s", e)
             break
 
         # Exceptions aren't raised but reported as an error message
         except Exception as ex:  # pylint: disable=broad-exception-caught
             log(ERROR, ex)
             log(ERROR, traceback.format_exc())
+
+            if isinstance(ex, ClientAppException):
+                e_code = ErrorCode.CLIENT_APP_RAISED_EXCEPTION
+            elif isinstance(ex, LoadClientAppError):
+                e_code = ErrorCode.LOAD_CLIENT_APP_EXCEPTION
+            else:
+                e_code = ErrorCode.UNKNOWN
+
             reason = str(type(ex)) + ":<'" + str(ex) + "'>"
-            error = Error(code=0, reason=reason)
-            out_mssg = message.create_error_reply(error=error)
+            out_mssg = message.create_error_reply(
+                error=Error(code=e_code, reason=reason)
+            )
 
         finally:
             if out_mssg:
                 # Convert to TaskRes
                 task_res = message_to_taskres(out_mssg)
                 # Store TaskRes in state
                 task_res.task.pushed_at = time.time()
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from uuid import UUID, uuid4
 
 from flwr.common import log, now
 from flwr.proto.task_pb2 import TaskIns, TaskRes  # pylint: disable=E0611
 from flwr.server.superlink.state.state import State
 from flwr.server.utils import validate_task_ins_or_res
 
+from .utils import make_node_unavailable_taskres
+
 
 class InMemoryState(State):
     """In-memory State implementation."""
 
     def __init__(self) -> None:
         # Map node_id to (online_until, ping_interval)
         self.node_ids: Dict[int, Tuple[float, float]] = {}
@@ -125,22 +127,39 @@
         """Get all TaskRes that have not been delivered yet."""
         if limit is not None and limit < 1:
             raise AssertionError("`limit` must be >= 1")
 
         with self.lock:
             # Find TaskRes that were not delivered yet
             task_res_list: List[TaskRes] = []
+            replied_task_ids: Set[UUID] = set()
             for _, task_res in self.task_res_store.items():
-                if (
-                    UUID(task_res.task.ancestry[0]) in task_ids
-                    and task_res.task.delivered_at == ""
-                ):
+                reply_to = UUID(task_res.task.ancestry[0])
+                if reply_to in task_ids and task_res.task.delivered_at == "":
                     task_res_list.append(task_res)
+                    replied_task_ids.add(reply_to)
+                if limit and len(task_res_list) == limit:
+                    break
+
+            # Check if the node is offline
+            for task_id in task_ids - replied_task_ids:
                 if limit and len(task_res_list) == limit:
                     break
+                task_ins = self.task_ins_store.get(task_id)
+                if task_ins is None:
+                    continue
+                node_id = task_ins.task.consumer.node_id
+                online_until, _ = self.node_ids[node_id]
+                # Generate a TaskRes containing an error reply if the node is offline.
+                if online_until < time.time():
+                    err_taskres = make_node_unavailable_taskres(
+                        ref_taskins=task_ins,
+                    )
+                    self.task_res_store[UUID(err_taskres.task_id)] = err_taskres
+                    task_res_list.append(err_taskres)
 
             # Mark all of them as delivered
             delivered_at = now().isoformat()
             for task_res in task_res_list:
                 task_res.task.delivered_at = delivered_at
 
             # Return TaskRes
@@ -178,24 +197,22 @@
     def num_task_res(self) -> int:
         """Calculate the number of task_res in store.
 
         This includes delivered but not yet deleted task_res.
         """
         return len(self.task_res_store)
 
-    def create_node(self) -> int:
+    def create_node(self, ping_interval: float) -> int:
         """Create, store in state, and return `node_id`."""
         # Sample a random int64 as node_id
         node_id: int = int.from_bytes(os.urandom(8), "little", signed=True)
 
         with self.lock:
             if node_id not in self.node_ids:
-                # Default ping interval is 30s
-                # TODO: change 1e9 to 30s  # pylint: disable=W0511
-                self.node_ids[node_id] = (time.time() + 1e9, 1e9)
+                self.node_ids[node_id] = (time.time() + ping_interval, ping_interval)
                 return node_id
         log(ERROR, "Unexpected node registration failure.")
         return 0
 
     def delete_node(self, node_id: int) -> None:
         """Delete a client node."""
         with self.lock:
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from flwr.common import log, now
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.recordset_pb2 import RecordSet  # pylint: disable=E0611
 from flwr.proto.task_pb2 import Task, TaskIns, TaskRes  # pylint: disable=E0611
 from flwr.server.utils.validator import validate_task_ins_or_res
 
 from .state import State
+from .utils import make_node_unavailable_taskres
 
 SQL_CREATE_TABLE_NODE = """
 CREATE TABLE IF NOT EXISTS node(
     node_id         INTEGER UNIQUE,
     online_until    REAL,
     ping_interval   REAL
 );
@@ -340,14 +341,15 @@
             self.query(query, data)
         except sqlite3.IntegrityError:
             log(ERROR, "`run` is invalid")
             return None
 
         return task_id
 
+    # pylint: disable-next=R0914
     def get_task_res(self, task_ids: Set[UUID], limit: Optional[int]) -> List[TaskRes]:
         """Get TaskRes for task_ids.
 
         Usually, the Driver API calls this method to get results for instructions it has
         previously scheduled.
 
         Retrieves all TaskRes for the given `task_ids` and returns and empty list if
@@ -370,15 +372,15 @@
         query = f"""
             SELECT *
             FROM task_res
             WHERE ancestry IN ({placeholders})
             AND delivered_at = ""
         """
 
-        data: Dict[str, Union[str, int]] = {}
+        data: Dict[str, Union[str, float, int]] = {}
 
         if limit is not None:
             query += " LIMIT :limit"
             data["limit"] = limit
 
         query += ";"
 
@@ -404,14 +406,62 @@
             for index, task_id in enumerate(found_task_ids):
                 data[f"id_{index}"] = str(task_id)
 
             # Run query
             rows = self.query(query, data)
 
         result = [dict_to_task_res(row) for row in rows]
+
+        # 1. Query: Fetch consumer_node_id of remaining task_ids
+        # Assume the ancestry field only contains one element
+        data.clear()
+        replied_task_ids: Set[UUID] = {UUID(str(row["ancestry"])) for row in rows}
+        remaining_task_ids = task_ids - replied_task_ids
+        placeholders = ",".join([f":id_{i}" for i in range(len(remaining_task_ids))])
+        query = f"""
+            SELECT consumer_node_id
+            FROM task_ins
+            WHERE task_id IN ({placeholders});
+        """
+        for index, task_id in enumerate(remaining_task_ids):
+            data[f"id_{index}"] = str(task_id)
+        node_ids = [int(row["consumer_node_id"]) for row in self.query(query, data)]
+
+        # 2. Query: Select offline nodes
+        placeholders = ",".join([f":id_{i}" for i in range(len(node_ids))])
+        query = f"""
+            SELECT node_id
+            FROM node
+            WHERE node_id IN ({placeholders})
+            AND online_until < :time;
+        """
+        data = {f"id_{i}": str(node_id) for i, node_id in enumerate(node_ids)}
+        data["time"] = time.time()
+        offline_node_ids = [int(row["node_id"]) for row in self.query(query, data)]
+
+        # 3. Query: Select TaskIns for offline nodes
+        placeholders = ",".join([f":id_{i}" for i in range(len(offline_node_ids))])
+        query = f"""
+            SELECT *
+            FROM task_ins
+            WHERE consumer_node_id IN ({placeholders});
+        """
+        data = {f"id_{i}": str(node_id) for i, node_id in enumerate(offline_node_ids)}
+        task_ins_rows = self.query(query, data)
+
+        # Make TaskRes containing node unavailabe error
+        for row in task_ins_rows:
+            if limit and len(result) == limit:
+                break
+            task_ins = dict_to_task_ins(row)
+            err_taskres = make_node_unavailable_taskres(
+                ref_taskins=task_ins,
+            )
+            result.append(err_taskres)
+
         return result
 
     def num_task_ins(self) -> int:
         """Calculate the number of task_ins in store.
 
         This includes delivered but not yet deleted task_ins.
         """
@@ -464,27 +514,25 @@
 
         with self.conn:
             self.conn.execute(query_1, data)
             self.conn.execute(query_2, data)
 
         return None
 
-    def create_node(self) -> int:
+    def create_node(self, ping_interval: float) -> int:
         """Create, store in state, and return `node_id`."""
         # Sample a random int64 as node_id
         node_id: int = int.from_bytes(os.urandom(8), "little", signed=True)
 
         query = (
             "INSERT INTO node (node_id, online_until, ping_interval) VALUES (?, ?, ?)"
         )
 
         try:
-            # Default ping interval is 30s
-            # TODO: change 1e9 to 30s  # pylint: disable=W0511
-            self.query(query, (node_id, time.time() + 1e9, 1e9))
+            self.query(query, (node_id, time.time() + ping_interval, ping_interval))
         except sqlite3.IntegrityError:
             log(ERROR, "Unexpected node registration failure.")
             return 0
         return node_id
 
     def delete_node(self, node_id: int) -> None:
         """Delete a client node."""
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
 
     @abc.abstractmethod
     def delete_tasks(self, task_ids: Set[UUID]) -> None:
         """Delete all delivered TaskIns/TaskRes pairs."""
 
     @abc.abstractmethod
-    def create_node(self) -> int:
+    def create_node(self, ping_interval: float) -> int:
         """Create, store in state, and return `node_id`."""
 
     @abc.abstractmethod
     def delete_node(self, node_id: int) -> None:
         """Remove `node_id` from state."""
 
     @abc.abstractmethod
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/typing.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/default_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import io
 import timeit
 from logging import INFO
 from typing import Optional, cast
 
 import flwr.common.recordset_compat as compat
-from flwr.common import DEFAULT_TTL, ConfigsRecord, Context, GetParametersIns, log
+from flwr.common import ConfigsRecord, Context, GetParametersIns, log
 from flwr.common.constant import MessageType, MessageTypeLegacy
 
 from ..compat.app_utils import start_update_client_manager_thread
 from ..compat.legacy_context import LegacyContext
 from ..driver import Driver
 from ..typing import Workflow
 from .constant import MAIN_CONFIGS_RECORD, MAIN_PARAMS_RECORD, Key
@@ -123,15 +123,14 @@
         messages = driver.send_and_receive(
             [
                 driver.create_message(
                     content=content,
                     message_type=MessageTypeLegacy.GET_PARAMETERS,
                     dst_node_id=random_client.node_id,
                     group_id="0",
-                    ttl=DEFAULT_TTL,
                 )
             ]
         )
         log(INFO, "Received initial parameters from one random client")
         msg = list(messages)[0]
         paramsrecord = next(iter(msg.content.parameters_records.values()))
 
@@ -222,15 +221,14 @@
     # Build out messages
     out_messages = [
         driver.create_message(
             content=compat.fitins_to_recordset(fitins, True),
             message_type=MessageType.TRAIN,
             dst_node_id=proxy.node_id,
             group_id=str(current_round),
-            ttl=DEFAULT_TTL,
         )
         for proxy, fitins in client_instructions
     ]
 
     # Send instructions to clients and
     # collect `fit` results from all clients participating in this round
     messages = list(driver.send_and_receive(out_messages))
@@ -302,15 +300,14 @@
     # Build out messages
     out_messages = [
         driver.create_message(
             content=compat.evaluateins_to_recordset(evalins, True),
             message_type=MessageType.EVALUATE,
             dst_node_id=proxy.node_id,
             group_id=str(current_round),
-            ttl=DEFAULT_TTL,
         )
         for proxy, evalins in client_instructions
     ]
 
     # Send instructions to clients and
     # collect `evaluate` results from all clients participating in this round
     messages = list(driver.send_and_receive(out_messages))
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import random
 from dataclasses import dataclass, field
 from logging import DEBUG, ERROR, INFO, WARN
 from typing import Dict, List, Optional, Set, Tuple, Union, cast
 
 import flwr.common.recordset_compat as compat
 from flwr.common import (
-    DEFAULT_TTL,
     ConfigsRecord,
     Context,
     FitRes,
     Message,
     MessageType,
     NDArrays,
     RecordSet,
@@ -370,15 +369,14 @@
 
         def make(nid: int) -> Message:
             return driver.create_message(
                 content=content,
                 message_type=MessageType.TRAIN,
                 dst_node_id=nid,
                 group_id=str(cfg[WorkflowKey.CURRENT_ROUND]),
-                ttl=DEFAULT_TTL,
             )
 
         log(
             DEBUG,
             "[Stage 0] Sending configurations to %s clients.",
             len(state.active_node_ids),
         )
@@ -418,15 +416,14 @@
             cfgs_record[Key.STAGE] = Stage.SHARE_KEYS
             content = RecordSet(configs_records={RECORD_KEY_CONFIGS: cfgs_record})
             return driver.create_message(
                 content=content,
                 message_type=MessageType.TRAIN,
                 dst_node_id=nid,
                 group_id=str(cfg[WorkflowKey.CURRENT_ROUND]),
-                ttl=DEFAULT_TTL,
             )
 
         # Broadcast public keys to clients and receive secret key shares
         log(
             DEBUG,
             "[Stage 1] Forwarding public keys to %s clients.",
             len(state.active_node_ids),
@@ -489,15 +486,14 @@
             content = state.nid_to_fitins[nid]
             content.configs_records[RECORD_KEY_CONFIGS] = cfgs_record
             return driver.create_message(
                 content=content,
                 message_type=MessageType.TRAIN,
                 dst_node_id=nid,
                 group_id=str(cfg[WorkflowKey.CURRENT_ROUND]),
-                ttl=DEFAULT_TTL,
             )
 
         log(
             DEBUG,
             "[Stage 2] Forwarding encrypted key shares to %s clients.",
             len(state.active_node_ids),
         )
@@ -560,15 +556,14 @@
             cfgs_record = ConfigsRecord(cfgs_dict)  # type: ignore
             content = RecordSet(configs_records={RECORD_KEY_CONFIGS: cfgs_record})
             return driver.create_message(
                 content=content,
                 message_type=MessageType.TRAIN,
                 dst_node_id=nid,
                 group_id=str(current_round),
-                ttl=DEFAULT_TTL,
             )
 
         log(
             DEBUG,
             "[Stage 3] Requesting key shares from %s clients to remove masks.",
             len(state.active_node_ids),
         )
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/app.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Ray-based Flower Actor and ActorPool implementation."""
 
 import asyncio
 import threading
-import traceback
 from abc import ABC
 from logging import DEBUG, ERROR, WARNING
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 import ray
 from ray import ObjectRef
 from ray.util.actor_pool import ActorPool
 
-from flwr.client.client_app import ClientApp, LoadClientAppError
+from flwr.client.client_app import ClientApp, ClientAppException, LoadClientAppError
 from flwr.common import Context, Message
 from flwr.common.logger import log
 
 ClientAppFn = Callable[[], ClientApp]
 
 
-class ClientException(Exception):
-    """Raised when client side logic crashes with an exception."""
-
-    def __init__(self, message: str):
-        div = ">" * 7
-        self.message = "\n" + div + "A ClientException occurred." + message
-        super().__init__(self.message)
-
-
 class VirtualClientEngineActor(ABC):
     """Abstract base class for VirtualClientEngine Actors."""
 
     def terminate(self) -> None:
         """Manually terminate Actor object."""
         log(WARNING, "Manually terminating %s", self.__class__.__name__)
         ray.actor.exit_actor()
@@ -67,25 +57,15 @@
             # Handle task message
             out_message = app(message=message, context=context)
 
         except LoadClientAppError as load_ex:
             raise load_ex
 
         except Exception as ex:
-            client_trace = traceback.format_exc()
-            mssg = (
-                "\n\tSomething went wrong when running your client run."
-                "\n\tClient "
-                + cid
-                + " crashed when the "
-                + self.__class__.__name__
-                + " was running its run."
-                "\n\tException triggered on the client side: " + client_trace,
-            )
-            raise ClientException(str(mssg)) from ex
+            raise ClientAppException(str(ex)) from ex
 
         return cid, out_message, context
 
 
 @ray.remote
 class ClientAppActor(VirtualClientEngineActor):
     """A Ray Actor class that runs client runs.
```

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.8.0.dev20240402/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240401/PKG-INFO` & `flwr_nightly-1.8.0.dev20240402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.8.0.dev20240401
+Version: 1.8.0.dev20240402
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.8.0.dev20240401 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.8.0.dev20240402 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

