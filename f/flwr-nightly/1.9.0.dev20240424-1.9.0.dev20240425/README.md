# Comparing `tmp/flwr_nightly-1.9.0.dev20240424.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240424.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240425.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240424.tar` & `flwr_nightly-1.9.0.dev20240425.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0    11358 2024-04-24 23:05:14.917695 flwr_nightly-1.9.0.dev20240424/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-24 23:05:14.921696 flwr_nightly-1.9.0.dev20240424/README.md
--rw-r--r--   0        0        0     5776 2024-04-24 23:05:29.445950 flwr_nightly-1.9.0.dev20240424/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     5597 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5404 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1911 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      371 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      489 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      558 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      538 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      537 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2331 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4153 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1262 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    24670 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4761 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-24 23:05:15.337703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      793 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     3861 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     4553 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4173 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-24 23:05:15.341703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24199 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5287 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3503 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7370 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      862 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11418 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5604 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-24 23:05:15.345703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4796 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    11651 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    27167 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7709 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15694 2024-04-24 23:05:15.349703 flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240424/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-25 23:05:28.517547 flwr_nightly-1.9.0.dev20240425/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-25 23:05:28.517547 flwr_nightly-1.9.0.dev20240425/README.md
+-rw-r--r--   0        0        0     5776 2024-04-25 23:05:42.069651 flwr_nightly-1.9.0.dev20240425/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     4899 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5989 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      667 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1911 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      371 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      590 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      570 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      569 2024-04-25 23:05:28.933550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2334 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1262 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    24670 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4761 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      793 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     3861 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-25 23:05:28.937550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4553 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4173 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24199 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5287 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      862 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-25 23:05:28.941550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4796 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    11651 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    27167 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7709 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-25 23:05:28.945550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15694 2024-04-25 23:05:28.949550 flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240425/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240424/LICENSE` & `flwr_nightly-1.9.0.dev20240425/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/README.md` & `flwr_nightly-1.9.0.dev20240425/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/pyproject.toml` & `flwr_nightly-1.9.0.dev20240425/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240424"
+version = "1.9.0.dev20240425"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/config_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,71 +10,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utility to validate the `pyproject.toml` file."""
 
-import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 import tomli
-import typer
 
 from flwr.common import object_ref
 
 
-def validate_project_dir(project_dir: Path) -> Optional[Dict[str, Any]]:
-    """Check if a Flower App directory is valid."""
-    config = load(str(project_dir / "pyproject.toml"))
-    if config is None:
-        typer.secho(
-            "❌ Project configuration could not be loaded. "
-            "`pyproject.toml` does not exist.",
-            fg=typer.colors.RED,
-            bold=True,
-        )
-        return None
-
-    if not validate(config):
-        typer.secho(
-            "❌ Project configuration is invalid.",
-            fg=typer.colors.RED,
-            bold=True,
-        )
-        return None
-
-    if "publisher" not in config["flower"]:
-        typer.secho(
-            "❌ Project configuration is missing required `publisher` field.",
-            fg=typer.colors.RED,
-            bold=True,
-        )
-        return None
-
-    return config
-
-
 def load_and_validate_with_defaults(
-    path: Optional[str] = None,
+    path: Optional[Path] = None,
 ) -> Tuple[Optional[Dict[str, Any]], List[str], List[str]]:
     """Load and validate pyproject.toml as dict.
 
     Returns
     -------
     Tuple[Optional[config], List[str], List[str]]
         A tuple with the optional config in case it exists and is valid
         and associated errors and warnings.
     """
     config = load(path)
 
     if config is None:
         errors = [
-            "Project configuration could not be loaded. pyproject.toml does not exist."
+            "Project configuration could not be loaded. "
+            "`pyproject.toml` does not exist."
         ]
         return (None, errors, [])
 
     is_valid, errors, warnings = validate(config)
 
     if not is_valid:
         return (None, errors, warnings)
@@ -86,30 +54,31 @@
         }
     }
     config = apply_defaults(config, defaults)
 
     return (config, errors, warnings)
 
 
-def load(path: Optional[str] = None) -> Optional[Dict[str, Any]]:
+def load(path: Optional[Path] = None) -> Optional[Dict[str, Any]]:
     """Load pyproject.toml and return as dict."""
     if path is None:
-        cur_dir = os.getcwd()
-        toml_path = os.path.join(cur_dir, "pyproject.toml")
+        cur_dir = Path.cwd()
+        toml_path = cur_dir / "pyproject.toml"
     else:
         toml_path = path
 
-    if not os.path.isfile(toml_path):
+    if not toml_path.is_file():
         return None
 
-    with open(toml_path, encoding="utf-8") as toml_file:
+    with toml_path.open(encoding="utf-8") as toml_file:
         data = tomli.loads(toml_file.read())
         return data
 
 
+# pylint: disable=too-many-branches
 def validate_fields(config: Dict[str, Any]) -> Tuple[bool, List[str], List[str]]:
     """Validate pyproject.toml fields."""
     errors = []
     warnings = []
 
     if "project" not in config:
         errors.append("Missing [project] section")
@@ -123,21 +92,24 @@
         if "license" not in config["project"]:
             warnings.append('Recommended property "license" missing in [project]')
         if "authors" not in config["project"]:
             warnings.append('Recommended property "authors" missing in [project]')
 
     if "flower" not in config:
         errors.append("Missing [flower] section")
-    elif "components" not in config["flower"]:
-        errors.append("Missing [flower.components] section")
     else:
-        if "serverapp" not in config["flower"]["components"]:
-            errors.append('Property "serverapp" missing in [flower.components]')
-        if "clientapp" not in config["flower"]["components"]:
-            errors.append('Property "clientapp" missing in [flower.components]')
+        if "publisher" not in config["flower"]:
+            errors.append('Property "publisher" missing in [flower]')
+        if "components" not in config["flower"]:
+            errors.append("Missing [flower.components] section")
+        else:
+            if "serverapp" not in config["flower"]["components"]:
+                errors.append('Property "serverapp" missing in [flower.components]')
+            if "clientapp" not in config["flower"]["components"]:
+                errors.append('Property "clientapp" missing in [flower.components]')
 
     return len(errors) == 0, errors, warnings
 
 
 def validate(config: Dict[str, Any]) -> Tuple[bool, List[str], List[str]]:
     """Validate pyproject.toml."""
     is_valid, errors, warnings = validate_fields(config)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/new.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower command line interface `new` command."""
 
 import os
+import re
 from enum import Enum
 from string import Template
 from typing import Dict, Optional
 
 import typer
 from typing_extensions import Annotated
 
@@ -82,33 +83,32 @@
         Optional[str],
         typer.Argument(metavar="project_name", help="The name of the project"),
     ] = None,
     framework: Annotated[
         Optional[MlFramework],
         typer.Option(case_sensitive=False, help="The ML framework to use"),
     ] = None,
+    username: Annotated[
+        Optional[str],
+        typer.Option(case_sensitive=False, help="The Flower username of the author"),
+    ] = None,
 ) -> None:
     """Create new Flower project."""
     if project_name is None:
-        project_name = prompt_text("Please provide project name")
+        project_name = prompt_text("Please provide the project name")
     if not is_valid_project_name(project_name):
         project_name = prompt_text(
             "Please provide a name that only contains "
-            "characters in {'_', 'a-zA-Z', '0-9'}",
+            "characters in {'-', a-zA-Z', '0-9'}",
             predicate=is_valid_project_name,
             default=sanitize_project_name(project_name),
         )
 
-    print(
-        typer.style(
-            f"🔨 Creating Flower project {project_name}...",
-            fg=typer.colors.GREEN,
-            bold=True,
-        )
-    )
+    if username is None:
+        username = prompt_text("Please provide your Flower username")
 
     if framework is not None:
         framework_str = str(framework.value)
     else:
         framework_value = prompt_options(
             "Please select ML framework by typing in the number",
             [mlf.value for mlf in MlFramework],
@@ -118,37 +118,57 @@
             for name, value in vars(MlFramework).items()
             if value == framework_value
         ]
         framework_str = selected_value[0]
 
     framework_str = framework_str.lower()
 
+    print(
+        typer.style(
+            f"\n🔨 Creating Flower project {project_name}...",
+            fg=typer.colors.GREEN,
+            bold=True,
+        )
+    )
+
     # Set project directory path
     cwd = os.getcwd()
-    pnl = project_name.lower()
-    project_dir = os.path.join(cwd, pnl)
+    package_name = re.sub(r"[-_.]+", "-", project_name).lower()
+    import_name = package_name.replace("-", "_")
+    project_dir = os.path.join(cwd, package_name)
 
     # List of files to render
     files = {
         ".gitignore": {"template": "app/.gitignore.tpl"},
         "README.md": {"template": "app/README.md.tpl"},
         "pyproject.toml": {"template": f"app/pyproject.{framework_str}.toml.tpl"},
-        f"{pnl}/__init__.py": {"template": "app/code/__init__.py.tpl"},
-        f"{pnl}/server.py": {"template": f"app/code/server.{framework_str}.py.tpl"},
-        f"{pnl}/client.py": {"template": f"app/code/client.{framework_str}.py.tpl"},
+        f"{import_name}/__init__.py": {"template": "app/code/__init__.py.tpl"},
+        f"{import_name}/server.py": {
+            "template": f"app/code/server.{framework_str}.py.tpl"
+        },
+        f"{import_name}/client.py": {
+            "template": f"app/code/client.{framework_str}.py.tpl"
+        },
     }
 
     # Depending on the framework, generate task.py file
     frameworks_with_tasks = [
         MlFramework.PYTORCH.value.lower(),
     ]
     if framework_str in frameworks_with_tasks:
-        files[f"{pnl}/task.py"] = {"template": f"app/code/task.{framework_str}.py.tpl"}
-
-    context = {"project_name": project_name}
+        files[f"{import_name}/task.py"] = {
+            "template": f"app/code/task.{framework_str}.py.tpl"
+        }
+
+    context = {
+        "project_name": project_name,
+        "package_name": package_name,
+        "import_name": import_name.replace("-", "_"),
+        "username": username,
+    }
 
     for file_path, value in files.items():
         render_and_create(
             file_path=os.path.join(project_dir, file_path),
             template=value["template"],
             context=context,
         )
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ```bash
 pip install .
 ```
 
 ## Run (Simulation Engine)
 
-In the `$project_name` directory, use `flwr run` to run a local simulation:
+In the `$import_name` directory, use `flwr run` to run a local simulation:
 
 ```bash
 flwr run
 ```
 
 ## Run (Deployment Engine)
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """$project_name: A Flower / PyTorch app."""
 
 from flwr.client import NumPyClient, ClientApp
 
-from $project_name.task import (
+from $import_name.task import (
     Net,
     DEVICE,
     load_data,
     get_weights,
     set_weights,
     train,
     test,
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """$project_name: A Flower / PyTorch app."""
 
 from flwr.common import ndarrays_to_parameters
 from flwr.server import ServerApp, ServerConfig
 from flwr.server.strategy import FedAvg
 
-from $project_name.task import Net, get_weights
+from $import_name.task import Net, get_weights
 
 
 # Initialize model parameters
 ndarrays = get_weights(Net())
 parameters = ndarrays_to_parameters(ndarrays)
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "$project_name"
+name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
 license = {text = "Apache License (2.0)"}
 dependencies = [
@@ -16,10 +16,13 @@
     "torch==2.2.1",
     "torchvision==0.17.1",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["."]
 
+[flower]
+publisher = "$username"
+
 [flower.components]
-serverapp = "$project_name.server:app"
-clientapp = "$project_name.client:app"
+serverapp = "$import_name.server:app"
+clientapp = "$import_name.client:app"
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "$project_name"
+name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
 license = {text = "Apache License (2.0)"}
 dependencies = [
@@ -15,10 +15,13 @@
     "flwr-datasets[vision]>=0.0.2,<1.0.0",
     "scikit-learn>=1.1.1",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["."]
 
+[flower]
+publisher = "$username"
+
 [flower.components]
-serverapp = "$project_name.server:app"
-clientapp = "$project_name.client:app"
+serverapp = "$import_name.server:app"
+clientapp = "$import_name.client:app"
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "$project_name"
+name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
 license = {text = "Apache License (2.0)"}
 dependencies = [
@@ -15,10 +15,13 @@
     "flwr-datasets[vision]>=0.0.2,<1.0.0",
     "tensorflow>=2.11.1",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["."]
 
+[flower]
+publisher = "$username"
+
 [flower.components]
-serverapp = "$project_name.server:app"
-clientapp = "$project_name.client:app"
+serverapp = "$import_name.server:app"
+clientapp = "$import_name.client:app"
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/run/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """Run Flower project."""
     typer.secho("Loading project configuration... ", fg=typer.colors.BLUE)
 
     config, errors, warnings = config_utils.load_and_validate_with_defaults()
 
     if config is None:
         typer.secho(
-            "Project configuration could not be loaded.\nflower.toml is invalid:\n"
+            "Project configuration could not be loaded.\npyproject.toml is invalid:\n"
             + "\n".join([f"- {line}" for line in errors]),
             fg=typer.colors.RED,
             bold=True,
         )
         sys.exit()
 
     if warnings:
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/cli/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower command line interface utils."""
 
+import re
 from typing import Callable, List, Optional, cast
 
 import typer
 
 
 def prompt_text(
     text: str,
@@ -69,55 +70,55 @@
             continue
 
     result = options[int(index)]
     return result
 
 
 def is_valid_project_name(name: str) -> bool:
-    """Check if the given string is a valid Python module name.
+    """Check if the given string is a valid Python project name.
 
-    A valid module name must start with a letter or an underscore, and can only contain
-    letters, digits, and underscores.
+    A valid project name must start with a letter and can only contain letters, digits,
+    and hyphens.
     """
     if not name:
         return False
 
-    # Check if the first character is a letter or underscore
-    if not (name[0].isalpha() or name[0] == "_"):
+    # Check if the first character is a letter
+    if not name[0].isalpha():
         return False
 
-    # Check if the rest of the characters are valid (letter, digit, or underscore)
+    # Check if the rest of the characters are valid (letter, digit, or dash)
     for char in name[1:]:
-        if not (char.isalnum() or char == "_"):
+        if not (char.isalnum() or char in "-"):
             return False
 
     return True
 
 
 def sanitize_project_name(name: str) -> str:
-    """Sanitize the given string to make it a valid Python module name.
+    """Sanitize the given string to make it a valid Python project name.
 
-    This version replaces hyphens with underscores, removes any characters not allowed
-    in Python module names, makes the string lowercase, and ensures it starts with a
-    valid character.
+    This version replaces spaces, dots, slashes, and underscores with dashes, removes
+    any characters not allowed in Python project names, makes the string lowercase, and
+    ensures it starts with a valid character.
     """
-    # Replace '-' with '_'
-    name_with_underscores = name.replace("-", "_").replace(" ", "_")
+    # Replace whitespace with '_'
+    name_with_hyphens = re.sub(r"[ ./_]", "-", name)
 
     # Allowed characters in a module name: letters, digits, underscore
     allowed_chars = set(
-        "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_"
+        "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-"
     )
 
     # Make the string lowercase
-    sanitized_name = name_with_underscores.lower()
+    sanitized_name = name_with_hyphens.lower()
 
     # Remove any characters not allowed in Python module names
     sanitized_name = "".join(c for c in sanitized_name if c in allowed_chars)
 
     # Ensure the first character is a letter or underscore
-    if sanitized_name and (
+    while sanitized_name and (
         sanitized_name[0].isdigit() or sanitized_name[0] not in allowed_chars
     ):
-        sanitized_name = "_" + sanitized_name
+        sanitized_name = sanitized_name[1:]
 
     return sanitized_name
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/supernode/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/app_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             client_manager.unregister(client_proxy)
             del registered_nodes[node_id]
 
         # Register new nodes
         for node_id in new_nodes:
             client_proxy = DriverClientProxy(
                 node_id=node_id,
-                driver=driver.grpc_driver_helper,  # type: ignore
+                driver=driver,
                 anonymous=False,
                 run_id=driver.run_id,  # type: ignore
             )
             if client_manager.register(client_proxy):
                 registered_nodes[node_id] = client_proxy
             else:
                 raise RuntimeError("Could not register node.")
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,188 +8,188 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower ClientProxy implementation for Driver API."""
+"""Ray-based Flower ClientProxy implementation."""
 
 
-import time
-from typing import List, Optional
+import traceback
+from logging import ERROR
+from typing import Optional
 
 from flwr import common
-from flwr.common import DEFAULT_TTL, MessageType, MessageTypeLegacy, RecordSet
-from flwr.common import recordset_compat as compat
-from flwr.common import serde
-from flwr.proto import driver_pb2, node_pb2, task_pb2  # pylint: disable=E0611
+from flwr.client import ClientFn
+from flwr.client.client_app import ClientApp
+from flwr.client.node_state import NodeState
+from flwr.common import DEFAULT_TTL, Message, Metadata, RecordSet
+from flwr.common.constant import MessageType, MessageTypeLegacy
+from flwr.common.logger import log
+from flwr.common.recordset_compat import (
+    evaluateins_to_recordset,
+    fitins_to_recordset,
+    getparametersins_to_recordset,
+    getpropertiesins_to_recordset,
+    recordset_to_evaluateres,
+    recordset_to_fitres,
+    recordset_to_getparametersres,
+    recordset_to_getpropertiesres,
+)
 from flwr.server.client_proxy import ClientProxy
+from flwr.simulation.ray_transport.ray_actor import VirtualClientEngineActorPool
 
-from ..driver.grpc_driver import GrpcDriverHelper
 
-SLEEP_TIME = 1
-
-
-class DriverClientProxy(ClientProxy):
-    """Flower client proxy which delegates work using the Driver API."""
+class RayActorClientProxy(ClientProxy):
+    """Flower client proxy which delegates work using Ray."""
 
     def __init__(
-        self, node_id: int, driver: GrpcDriverHelper, anonymous: bool, run_id: int
+        self, client_fn: ClientFn, cid: str, actor_pool: VirtualClientEngineActorPool
     ):
-        super().__init__(str(node_id))
-        self.node_id = node_id
-        self.driver = driver
-        self.run_id = run_id
-        self.anonymous = anonymous
+        super().__init__(cid)
+
+        def _load_app() -> ClientApp:
+            return ClientApp(client_fn=client_fn)
+
+        self.app_fn = _load_app
+        self.actor_pool = actor_pool
+        self.proxy_state = NodeState()
+
+    def _submit_job(self, message: Message, timeout: Optional[float]) -> Message:
+        """Sumbit a message to the ActorPool."""
+        run_id = message.metadata.run_id
+
+        # Register state
+        self.proxy_state.register_context(run_id=run_id)
+
+        # Retrieve state
+        state = self.proxy_state.retrieve_context(run_id=run_id)
+
+        try:
+            self.actor_pool.submit_client_job(
+                lambda a, a_fn, mssg, cid, state: a.run.remote(a_fn, mssg, cid, state),
+                (self.app_fn, message, self.cid, state),
+            )
+            out_mssg, updated_context = self.actor_pool.get_client_result(
+                self.cid, timeout
+            )
+
+            # Update state
+            self.proxy_state.update_context(run_id=run_id, context=updated_context)
+
+        except Exception as ex:
+            if self.actor_pool.num_actors == 0:
+                # At this point we want to stop the simulation.
+                # since no more client runs will be executed
+                log(ERROR, "ActorPool is empty!!!")
+            log(ERROR, traceback.format_exc())
+            log(ERROR, ex)
+            raise ex
+
+        return out_mssg
+
+    def _wrap_recordset_in_message(
+        self,
+        recordset: RecordSet,
+        message_type: str,
+        timeout: Optional[float],
+        group_id: Optional[int],
+    ) -> Message:
+        """Wrap a RecordSet inside a Message."""
+        return Message(
+            content=recordset,
+            metadata=Metadata(
+                run_id=0,
+                message_id="",
+                group_id=str(group_id) if group_id is not None else "",
+                src_node_id=0,
+                dst_node_id=int(self.cid),
+                reply_to_message="",
+                ttl=timeout if timeout else DEFAULT_TTL,
+                message_type=message_type,
+                partition_id=int(self.cid),
+            ),
+        )
 
     def get_properties(
         self,
         ins: common.GetPropertiesIns,
         timeout: Optional[float],
         group_id: Optional[int],
     ) -> common.GetPropertiesRes:
         """Return client's properties."""
-        # Ins to RecordSet
-        out_recordset = compat.getpropertiesins_to_recordset(ins)
-        # Fetch response
-        in_recordset = self._send_receive_recordset(
-            out_recordset, MessageTypeLegacy.GET_PROPERTIES, timeout, group_id
+        recordset = getpropertiesins_to_recordset(ins)
+        message = self._wrap_recordset_in_message(
+            recordset,
+            message_type=MessageTypeLegacy.GET_PROPERTIES,
+            timeout=timeout,
+            group_id=group_id,
         )
-        # RecordSet to Res
-        return compat.recordset_to_getpropertiesres(in_recordset)
+
+        message_out = self._submit_job(message, timeout)
+
+        return recordset_to_getpropertiesres(message_out.content)
 
     def get_parameters(
         self,
         ins: common.GetParametersIns,
         timeout: Optional[float],
         group_id: Optional[int],
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
-        # Ins to RecordSet
-        out_recordset = compat.getparametersins_to_recordset(ins)
-        # Fetch response
-        in_recordset = self._send_receive_recordset(
-            out_recordset, MessageTypeLegacy.GET_PARAMETERS, timeout, group_id
+        recordset = getparametersins_to_recordset(ins)
+        message = self._wrap_recordset_in_message(
+            recordset,
+            message_type=MessageTypeLegacy.GET_PARAMETERS,
+            timeout=timeout,
+            group_id=group_id,
         )
-        # RecordSet to Res
-        return compat.recordset_to_getparametersres(in_recordset, False)
+
+        message_out = self._submit_job(message, timeout)
+
+        return recordset_to_getparametersres(message_out.content, keep_input=False)
 
     def fit(
         self, ins: common.FitIns, timeout: Optional[float], group_id: Optional[int]
     ) -> common.FitRes:
         """Train model parameters on the locally held dataset."""
-        # Ins to RecordSet
-        out_recordset = compat.fitins_to_recordset(ins, keep_input=True)
-        # Fetch response
-        in_recordset = self._send_receive_recordset(
-            out_recordset, MessageType.TRAIN, timeout, group_id
+        recordset = fitins_to_recordset(
+            ins, keep_input=True
+        )  # This must stay TRUE since ins are in-memory
+        message = self._wrap_recordset_in_message(
+            recordset,
+            message_type=MessageType.TRAIN,
+            timeout=timeout,
+            group_id=group_id,
         )
-        # RecordSet to Res
-        return compat.recordset_to_fitres(in_recordset, keep_input=False)
+
+        message_out = self._submit_job(message, timeout)
+
+        return recordset_to_fitres(message_out.content, keep_input=False)
 
     def evaluate(
         self, ins: common.EvaluateIns, timeout: Optional[float], group_id: Optional[int]
     ) -> common.EvaluateRes:
         """Evaluate model parameters on the locally held dataset."""
-        # Ins to RecordSet
-        out_recordset = compat.evaluateins_to_recordset(ins, keep_input=True)
-        # Fetch response
-        in_recordset = self._send_receive_recordset(
-            out_recordset, MessageType.EVALUATE, timeout, group_id
+        recordset = evaluateins_to_recordset(
+            ins, keep_input=True
+        )  # This must stay TRUE since ins are in-memory
+        message = self._wrap_recordset_in_message(
+            recordset,
+            message_type=MessageType.EVALUATE,
+            timeout=timeout,
+            group_id=group_id,
         )
-        # RecordSet to Res
-        return compat.recordset_to_evaluateres(in_recordset)
+
+        message_out = self._submit_job(message, timeout)
+
+        return recordset_to_evaluateres(message_out.content)
 
     def reconnect(
         self,
         ins: common.ReconnectIns,
         timeout: Optional[float],
         group_id: Optional[int],
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
         return common.DisconnectRes(reason="")  # Nothing to do here (yet)
-
-    def _send_receive_recordset(
-        self,
-        recordset: RecordSet,
-        task_type: str,
-        timeout: Optional[float],
-        group_id: Optional[int],
-    ) -> RecordSet:
-        task_ins = task_pb2.TaskIns(  # pylint: disable=E1101
-            task_id="",
-            group_id=str(group_id) if group_id is not None else "",
-            run_id=self.run_id,
-            task=task_pb2.Task(  # pylint: disable=E1101
-                producer=node_pb2.Node(  # pylint: disable=E1101
-                    node_id=0,
-                    anonymous=True,
-                ),
-                consumer=node_pb2.Node(  # pylint: disable=E1101
-                    node_id=self.node_id,
-                    anonymous=self.anonymous,
-                ),
-                task_type=task_type,
-                recordset=serde.recordset_to_proto(recordset),
-                ttl=DEFAULT_TTL,
-            ),
-        )
-
-        # This would normally be recorded upon common.Message creation
-        # but this compatibility stack doesn't create Messages,
-        # so we need to inject `created_at` manually (needed for
-        # taskins validation by server.utils.validator)
-        task_ins.task.created_at = time.time()
-
-        push_task_ins_req = driver_pb2.PushTaskInsRequest(  # pylint: disable=E1101
-            task_ins_list=[task_ins]
-        )
-
-        # Send TaskIns to Driver API
-        push_task_ins_res = self.driver.push_task_ins(req=push_task_ins_req)
-
-        if len(push_task_ins_res.task_ids) != 1:
-            raise ValueError("Unexpected number of task_ids")
-
-        task_id = push_task_ins_res.task_ids[0]
-        if task_id == "":
-            raise ValueError(f"Failed to schedule task for node {self.node_id}")
-
-        if timeout:
-            start_time = time.time()
-
-        while True:
-            pull_task_res_req = driver_pb2.PullTaskResRequest(  # pylint: disable=E1101
-                node=node_pb2.Node(node_id=0, anonymous=True),  # pylint: disable=E1101
-                task_ids=[task_id],
-            )
-
-            # Ask Driver API for TaskRes
-            pull_task_res_res = self.driver.pull_task_res(req=pull_task_res_req)
-
-            task_res_list: List[task_pb2.TaskRes] = list(  # pylint: disable=E1101
-                pull_task_res_res.task_res_list
-            )
-            if len(task_res_list) == 1:
-                task_res = task_res_list[0]
-
-                # This will raise an Exception if task_res carries an `error`
-                validate_task_res(task_res=task_res)
-
-                return serde.recordset_from_proto(task_res.task.recordset)
-
-            if timeout is not None and time.time() > start_time + timeout:
-                raise RuntimeError("Timeout reached")
-            time.sleep(SLEEP_TIME)
-
-
-def validate_task_res(
-    task_res: task_pb2.TaskRes,  # pylint: disable=E1101
-) -> None:
-    """Validate if a TaskRes is empty or not."""
-    if not task_res.HasField("task"):
-        raise ValueError("Invalid TaskRes, field `task` missing")
-    if task_res.task.HasField("error"):
-        raise ValueError("Exception during client-side task execution")
-    if not task_res.task.HasField("recordset"):
-        raise ValueError("Invalid TaskRes, both `recordset` and `error` are missing")
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/driver/grpc_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,39 +147,48 @@
         Tuple containing root certificate, server certificate, and private key
         to start a secure SSL-enabled server. The tuple is expected to have
         three bytes elements in the following order:
 
             * CA certificate.
             * server certificate.
             * server private key.
+    fab_id : str (default: None)
+        The identifier of the FAB used in the run.
+    fab_version : str (default: None)
+        The version of the FAB used in the run.
     """
 
     def __init__(
         self,
         driver_service_address: str = DEFAULT_SERVER_ADDRESS_DRIVER,
         root_certificates: Optional[bytes] = None,
+        fab_id: Optional[str] = None,
+        fab_version: Optional[str] = None,
     ) -> None:
         self.addr = driver_service_address
         self.root_certificates = root_certificates
-        self.grpc_driver_helper: Optional[GrpcDriverHelper] = None
+        self.driver_helper: Optional[GrpcDriverHelper] = None
         self.run_id: Optional[int] = None
+        self.fab_id = fab_id if fab_id is not None else ""
+        self.fab_version = fab_version if fab_version is not None else ""
         self.node = Node(node_id=0, anonymous=True)
 
     def _get_grpc_driver_helper_and_run_id(self) -> Tuple[GrpcDriverHelper, int]:
         # Check if the GrpcDriverHelper is initialized
-        if self.grpc_driver_helper is None or self.run_id is None:
+        if self.driver_helper is None or self.run_id is None:
             # Connect and create run
-            self.grpc_driver_helper = GrpcDriverHelper(
+            self.driver_helper = GrpcDriverHelper(
                 driver_service_address=self.addr,
                 root_certificates=self.root_certificates,
             )
-            self.grpc_driver_helper.connect()
-            res = self.grpc_driver_helper.create_run(CreateRunRequest())
+            self.driver_helper.connect()
+            req = CreateRunRequest(fab_id=self.fab_id, fab_version=self.fab_version)
+            res = self.driver_helper.create_run(req)
             self.run_id = res.run_id
-        return self.grpc_driver_helper, self.run_id
+        return self.driver_helper, self.run_id
 
     def _check_message(self, message: Message) -> None:
         # Check if the message is valid
         if not (
             message.metadata.run_id == self.run_id
             and message.metadata.src_node_id == self.node.node_id
             and message.metadata.message_id == ""
@@ -296,11 +305,11 @@
             # Sleep
             time.sleep(3)
         return ret
 
     def close(self) -> None:
         """Disconnect from the SuperLink if connected."""
         # Check if GrpcDriverHelper is initialized
-        if self.grpc_driver_helper is None:
+        if self.driver_helper is None:
             return
         # Disconnect
-        self.grpc_driver_helper.disconnect()
+        self.driver_helper.disconnect()
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/run_serverapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,16 @@
     server_app_dir = args.dir
     server_app_attr = getattr(args, "server-app")
 
     # Initialize GrpcDriver
     driver = GrpcDriver(
         driver_service_address=args.server,
         root_certificates=root_certificates,
+        fab_id=args.fab_id,
+        fab_version=args.fab_version,
     )
 
     # Run the ServerApp with the Driver
     run(driver=driver, server_app_dir=server_app_dir, server_app_attr=server_app_attr)
 
     # Clean up
     driver.close()
@@ -179,9 +181,21 @@
     parser.add_argument(
         "--dir",
         default="",
         help="Add specified directory to the PYTHONPATH and load Flower "
         "app from there."
         " Default: current working directory.",
     )
+    parser.add_argument(
+        "--fab-id",
+        default=None,
+        type=str,
+        help="The identifier of the FAB used in the run.",
+    )
+    parser.add_argument(
+        "--fab-version",
+        default=None,
+        type=str,
+        help="The version of the FAB used in the run.",
+    )
 
     return parser
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,188 +8,143 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Ray-based Flower ClientProxy implementation."""
+"""Flower ClientProxy implementation for Driver API."""
 
 
-import traceback
-from logging import ERROR
+import time
 from typing import Optional
 
 from flwr import common
-from flwr.client import ClientFn
-from flwr.client.client_app import ClientApp
-from flwr.client.node_state import NodeState
-from flwr.common import DEFAULT_TTL, Message, Metadata, RecordSet
-from flwr.common.constant import MessageType, MessageTypeLegacy
-from flwr.common.logger import log
-from flwr.common.recordset_compat import (
-    evaluateins_to_recordset,
-    fitins_to_recordset,
-    getparametersins_to_recordset,
-    getpropertiesins_to_recordset,
-    recordset_to_evaluateres,
-    recordset_to_fitres,
-    recordset_to_getparametersres,
-    recordset_to_getpropertiesres,
-)
+from flwr.common import Message, MessageType, MessageTypeLegacy, RecordSet
+from flwr.common import recordset_compat as compat
 from flwr.server.client_proxy import ClientProxy
-from flwr.simulation.ray_transport.ray_actor import VirtualClientEngineActorPool
 
+from ..driver.driver import Driver
 
-class RayActorClientProxy(ClientProxy):
-    """Flower client proxy which delegates work using Ray."""
+SLEEP_TIME = 1
 
-    def __init__(
-        self, client_fn: ClientFn, cid: str, actor_pool: VirtualClientEngineActorPool
-    ):
-        super().__init__(cid)
-
-        def _load_app() -> ClientApp:
-            return ClientApp(client_fn=client_fn)
-
-        self.app_fn = _load_app
-        self.actor_pool = actor_pool
-        self.proxy_state = NodeState()
-
-    def _submit_job(self, message: Message, timeout: Optional[float]) -> Message:
-        """Sumbit a message to the ActorPool."""
-        run_id = message.metadata.run_id
-
-        # Register state
-        self.proxy_state.register_context(run_id=run_id)
-
-        # Retrieve state
-        state = self.proxy_state.retrieve_context(run_id=run_id)
-
-        try:
-            self.actor_pool.submit_client_job(
-                lambda a, a_fn, mssg, cid, state: a.run.remote(a_fn, mssg, cid, state),
-                (self.app_fn, message, self.cid, state),
-            )
-            out_mssg, updated_context = self.actor_pool.get_client_result(
-                self.cid, timeout
-            )
-
-            # Update state
-            self.proxy_state.update_context(run_id=run_id, context=updated_context)
-
-        except Exception as ex:
-            if self.actor_pool.num_actors == 0:
-                # At this point we want to stop the simulation.
-                # since no more client runs will be executed
-                log(ERROR, "ActorPool is empty!!!")
-            log(ERROR, traceback.format_exc())
-            log(ERROR, ex)
-            raise ex
 
-        return out_mssg
+class DriverClientProxy(ClientProxy):
+    """Flower client proxy which delegates work using the Driver API."""
 
-    def _wrap_recordset_in_message(
-        self,
-        recordset: RecordSet,
-        message_type: str,
-        timeout: Optional[float],
-        group_id: Optional[int],
-    ) -> Message:
-        """Wrap a RecordSet inside a Message."""
-        return Message(
-            content=recordset,
-            metadata=Metadata(
-                run_id=0,
-                message_id="",
-                group_id=str(group_id) if group_id is not None else "",
-                src_node_id=0,
-                dst_node_id=int(self.cid),
-                reply_to_message="",
-                ttl=timeout if timeout else DEFAULT_TTL,
-                message_type=message_type,
-                partition_id=int(self.cid),
-            ),
-        )
+    def __init__(self, node_id: int, driver: Driver, anonymous: bool, run_id: int):
+        super().__init__(str(node_id))
+        self.node_id = node_id
+        self.driver = driver
+        self.run_id = run_id
+        self.anonymous = anonymous
 
     def get_properties(
         self,
         ins: common.GetPropertiesIns,
         timeout: Optional[float],
         group_id: Optional[int],
     ) -> common.GetPropertiesRes:
         """Return client's properties."""
-        recordset = getpropertiesins_to_recordset(ins)
-        message = self._wrap_recordset_in_message(
-            recordset,
-            message_type=MessageTypeLegacy.GET_PROPERTIES,
-            timeout=timeout,
-            group_id=group_id,
+        # Ins to RecordSet
+        out_recordset = compat.getpropertiesins_to_recordset(ins)
+        # Fetch response
+        in_recordset = self._send_receive_recordset(
+            out_recordset, MessageTypeLegacy.GET_PROPERTIES, timeout, group_id
         )
-
-        message_out = self._submit_job(message, timeout)
-
-        return recordset_to_getpropertiesres(message_out.content)
+        # RecordSet to Res
+        return compat.recordset_to_getpropertiesres(in_recordset)
 
     def get_parameters(
         self,
         ins: common.GetParametersIns,
         timeout: Optional[float],
         group_id: Optional[int],
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
-        recordset = getparametersins_to_recordset(ins)
-        message = self._wrap_recordset_in_message(
-            recordset,
-            message_type=MessageTypeLegacy.GET_PARAMETERS,
-            timeout=timeout,
-            group_id=group_id,
+        # Ins to RecordSet
+        out_recordset = compat.getparametersins_to_recordset(ins)
+        # Fetch response
+        in_recordset = self._send_receive_recordset(
+            out_recordset, MessageTypeLegacy.GET_PARAMETERS, timeout, group_id
         )
-
-        message_out = self._submit_job(message, timeout)
-
-        return recordset_to_getparametersres(message_out.content, keep_input=False)
+        # RecordSet to Res
+        return compat.recordset_to_getparametersres(in_recordset, False)
 
     def fit(
         self, ins: common.FitIns, timeout: Optional[float], group_id: Optional[int]
     ) -> common.FitRes:
         """Train model parameters on the locally held dataset."""
-        recordset = fitins_to_recordset(
-            ins, keep_input=True
-        )  # This must stay TRUE since ins are in-memory
-        message = self._wrap_recordset_in_message(
-            recordset,
-            message_type=MessageType.TRAIN,
-            timeout=timeout,
-            group_id=group_id,
+        # Ins to RecordSet
+        out_recordset = compat.fitins_to_recordset(ins, keep_input=True)
+        # Fetch response
+        in_recordset = self._send_receive_recordset(
+            out_recordset, MessageType.TRAIN, timeout, group_id
         )
-
-        message_out = self._submit_job(message, timeout)
-
-        return recordset_to_fitres(message_out.content, keep_input=False)
+        # RecordSet to Res
+        return compat.recordset_to_fitres(in_recordset, keep_input=False)
 
     def evaluate(
         self, ins: common.EvaluateIns, timeout: Optional[float], group_id: Optional[int]
     ) -> common.EvaluateRes:
         """Evaluate model parameters on the locally held dataset."""
-        recordset = evaluateins_to_recordset(
-            ins, keep_input=True
-        )  # This must stay TRUE since ins are in-memory
-        message = self._wrap_recordset_in_message(
-            recordset,
-            message_type=MessageType.EVALUATE,
-            timeout=timeout,
-            group_id=group_id,
+        # Ins to RecordSet
+        out_recordset = compat.evaluateins_to_recordset(ins, keep_input=True)
+        # Fetch response
+        in_recordset = self._send_receive_recordset(
+            out_recordset, MessageType.EVALUATE, timeout, group_id
         )
-
-        message_out = self._submit_job(message, timeout)
-
-        return recordset_to_evaluateres(message_out.content)
+        # RecordSet to Res
+        return compat.recordset_to_evaluateres(in_recordset)
 
     def reconnect(
         self,
         ins: common.ReconnectIns,
         timeout: Optional[float],
         group_id: Optional[int],
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
         return common.DisconnectRes(reason="")  # Nothing to do here (yet)
+
+    def _send_receive_recordset(
+        self,
+        recordset: RecordSet,
+        task_type: str,
+        timeout: Optional[float],
+        group_id: Optional[int],
+    ) -> RecordSet:
+
+        # Create message
+        message = self.driver.create_message(
+            content=recordset,
+            message_type=task_type,
+            dst_node_id=self.node_id,
+            group_id=str(group_id) if group_id else "",
+            ttl=timeout,
+        )
+
+        # Push message
+        message_ids = list(self.driver.push_messages(messages=[message]))
+        if len(message_ids) != 1:
+            raise ValueError("Unexpected number of message_ids")
+
+        message_id = message_ids[0]
+        if message_id == "":
+            raise ValueError(f"Failed to send message to node {self.node_id}")
+
+        if timeout:
+            start_time = time.time()
+
+        while True:
+            messages = list(self.driver.pull_messages(message_ids))
+            if len(messages) == 1:
+                msg: Message = messages[0]
+                if msg.has_error():
+                    raise ValueError(
+                        f"Message contains an Error (reason: {msg.error.reason}). "
+                        "It originated during client-side execution of a message."
+                    )
+                return msg.content
+
+            if timeout is not None and time.time() > start_time + timeout:
+                raise RuntimeError("Timeout reached")
+            time.sleep(SLEEP_TIME)
```

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240425/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240424/PKG-INFO` & `flwr_nightly-1.9.0.dev20240425/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240424
+Version: 1.9.0.dev20240425
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
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240424 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240425 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

