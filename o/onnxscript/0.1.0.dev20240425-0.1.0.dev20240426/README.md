# Comparing `tmp/onnxscript-0.1.0.dev20240425.tar.gz` & `tmp/onnxscript-0.1.0.dev20240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240425.tar", last modified: Thu Apr 25 00:01:47 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240426.tar", last modified: Fri Apr 26 00:01:07 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240425.tar` & `onnxscript-0.1.0.dev20240426.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.058006 onnxscript-0.1.0.dev20240425/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.018006 onnxscript-0.1.0.dev20240425/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.022006 onnxscript-0.1.0.dev20240425/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.014006 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.026006 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.034006 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.014006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.014006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.034006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.034006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.038006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.038006 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.042006 onnxscript-0.1.0.dev20240425/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.042006 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.046006 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.050006 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.050006 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1253 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36263 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.050006 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41987 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:01:47.054006 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-25 00:01:47.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-25 00:01:46.000000 onnxscript-0.1.0.dev20240425/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-25 00:01:47.058006 onnxscript-0.1.0.dev20240425/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-25 00:00:55.000000 onnxscript-0.1.0.dev20240425/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.025172 onnxscript-0.1.0.dev20240426/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.025172 onnxscript-0.1.0.dev20240426/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.021172 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.041172 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.021172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.021172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.045172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.045172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.045172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.049172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.049172 onnxscript-0.1.0.dev20240426/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.049172 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.057172 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.057172 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37876 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240425/LICENSE` & `onnxscript-0.1.0.dev20240426/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/PKG-INFO` & `onnxscript-0.1.0.dev20240426/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240425
+Version: 0.1.0.dev20240426
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240425/README.md` & `onnxscript-0.1.0.dev20240426/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240426/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240426/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240426/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240426/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240426/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/main.py` & `onnxscript-0.1.0.dev20240426/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240426/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Sequence
+from typing import Sequence, Union
 
 __all__ = [
     # Modules
     "function_rule",
     "pattern",
     # Functions
     "rewrite",
@@ -12,28 +12,32 @@
 
 import onnx
 
 from onnxscript import ir
 from onnxscript.optimizer import remove_unused, remove_unused_function
 from onnxscript.rewriter import function_rule, pattern
 
+RewriteRuleSet = pattern.RewriteRuleSet
 PatternRewriteRule = pattern.RewriteRule
 FunctionRewriteRule = function_rule.FunctionRewriteRule
 
 
 def rewrite(
     model: onnx.ModelProto,
     function_rewrite_rules: Sequence[type[FunctionRewriteRule]] = (),
-    pattern_rewrite_rules: Sequence[PatternRewriteRule] = (),
+    pattern_rewrite_rules: Union[Sequence[PatternRewriteRule], RewriteRuleSet] = (),
 ) -> onnx.ModelProto:
     model_ir = ir.serde.deserialize_model(model)
     if function_rewrite_rules:
         for rule_cls in function_rewrite_rules:
             count, model_ir = rule_cls().apply_to_model(model_ir)
             print(f"Applied {count} of onnxruntime specific function rewrite rules.")
     if pattern_rewrite_rules:
-        count = pattern.RewriteRuleSet(pattern_rewrite_rules).apply_to_model(model_ir)
+        if not isinstance(pattern_rewrite_rules, RewriteRuleSet):
+            # Create a pattern rule-set using provided rules
+            pattern_rewrite_rules = pattern.RewriteRuleSet(pattern_rewrite_rules)
+        count = pattern_rewrite_rules.apply_to_model(model_ir)
         print(f"Applied {count} of general pattern rewrite rules.")
     model = ir.serde.serialize_model(model_ir)
     remove_unused.remove_unused_nodes(model)
     remove_unused_function.remove_unused_functions(model)
     return model
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,42 +136,33 @@
     # Constants in pattern. See https://github.com/microsoft/onnx-rewriter/issues/192.
     reshape_a = op.Reshape(input_a, shape_a)
     reshape_b = op.Reshape(input_b, shape_b)
     matmul = op.MatMul(reshape_a, reshape_b)
     return op.Reshape(matmul, shape_c)
 
 
-def matmul_with_two_shape_inputs(input_a, input_b, shape_a, shape_b, shape_c):
-    del shape_a  # Unused
-    del shape_b  # Unused
-    del shape_c  # Unused
+def matmul(op, input_a, input_b, **_):
     return op.MatMul(input_a, input_b)
 
 
 def one_reshape_matmul_reshape_pattern(input_a, input_b, shape_a, shape_c):
     reshape_a = op.Reshape(input_a, shape_a)
     matmul = op.MatMul(reshape_a, input_b)
     return op.Reshape(matmul, shape_c)
 
 
-def matmul_with_one_shape_input(input_a, input_b, shape_a, shape_c):
-    del shape_a  # Unused
-    del shape_c  # Unused
-    return op.MatMul(input_a, input_b)
-
-
 # Register the rewrite rules
 two_reshapes_matmul_reshape_rule = pattern.RewriteRule(
     two_reshapes_matmul_reshape_pattern,
-    matmul_with_two_shape_inputs,
+    matmul,
     check_if_need_reshape,
 )
 one_reshape_matmul_reshape_rule = pattern.RewriteRule(
     one_reshape_matmul_reshape_pattern,
-    matmul_with_one_shape_input,
+    matmul,
     # We can use the same check_if_need_reshape function for both the rules,
     # as one_reshape_matmul_reshape_pattern is a subset of two_reshapes_matmul_reshape_pattern.
     check_if_need_reshape,
 )
 
 # NOTE: The order of the rules is important. Larger pattern should be checked first.
 rules = pattern.RewriteRuleSet(
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     reshape_a = op.Reshape(input_a, shape_a)
     # TODO: Temporary workaround to support benchmodels.
     # Tracked by https://github.com/microsoft/onnx-rewriter/issues/197.
     gemm = op.Gemm(reshape_a, input_b, input_c, alpha=1.0, beta=1.0)
     return op.Reshape(gemm, shape_c)
 
 
-def matmul_add(input_a, input_b, input_c, shape_a, shape_d):
+def matmul_add(op, input_a, input_b, input_c, **_):
     matmul = op.MatMul(input_a, input_b)
     return op.Add(matmul, input_c)
 
 
 rule = pattern.RewriteRule(reshape_gemm_reshape_pattern, matmul_add, check_if_need_reshape)
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/generic_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,44 +7,15 @@
 from typing import Any, Callable, Iterator, Sequence
 
 import onnx
 
 import onnxscript
 import onnxscript.rewriter.pattern as orp
 from onnxscript import ir
-from onnxscript.rewriter import _ir_utils, _tape
-
-
-class _SimpleBuilder:
-    """temporary adaptor for building 'generic patterns'."""
-
-    # TODO(justinchuby): Merge with the rest of pattern building methods
-    def __init__(self):
-        self.tape = _tape.Tape()
-
-    def __getattr__(self, op_type: str) -> Any:
-        return lambda *args, **kwargs: self._make_node(op_type, args, kwargs)
-
-    def _make_node(self, op_type: str, inputs: Sequence[ir.Value], kwargs: dict[str, Any]):
-        domain = kwargs.pop("domain", "")
-        output_names = kwargs.pop("output_names", 1)
-        if isinstance(output_names, Sequence):
-            num_outputs = len(output_names)
-        else:
-            assert isinstance(output_names, int)
-            num_outputs = output_names
-        if num_outputs == 1:
-            return self.tape.op(op_type, inputs=inputs, attributes=kwargs, domain=domain)
-        return self.tape.op_multi_output(
-            op_type, inputs=inputs, attributes=kwargs, domain=domain, num_outputs=num_outputs
-        )
-
-    @property
-    def nodes(self) -> Sequence[ir.Node]:
-        return self.tape.nodes
+from onnxscript.rewriter import _ir_utils
 
 
 class PatternMatchResult:
     """Stores information about a match if a match was successful.
 
     * pattern: the instance of :class:`GenericPattern` which found this result
     * model_nodes: matched nodes coming from the model
@@ -138,15 +109,15 @@
 
     def matches(self, node: ir.Node, model: ir.Model) -> orp.MatchResult:
         del model
         del node
         raise RuntimeError(f"This pattern {self} is meant to replace not to only match.")
 
     def try_rewrite(
-        self, model: ir.Model, node: ir.Node
+        self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
     ) -> tuple[int, list[ir.Node], list[ir.Node]] | None:
         """See :meth:`RewriteRule.try_rewrite`."""
 
         deleted_nodes: list[ir.Node] = []
         added_nodes: list[ir.Node] = []
         matched: set[ir.Node] = set()
         match_count = 0
@@ -335,15 +306,15 @@
                 kwargs[p.name] = p.default
             else:
                 args.append(p.name)
 
         assert len(kwargs) == 0, f"Attributes are not supported yet but kwargs={kwargs}"
 
         inputs = [ir.Input(name=name) for name in args]
-        builder = _SimpleBuilder()
+        builder = orp.RewriterContext()
         outputs = func(builder, *inputs, **kwargs)
         if isinstance(outputs, ir.Value):
             outputs = [outputs]
         graph = ir.Graph(inputs=inputs, outputs=outputs, nodes=builder.nodes)
         graph.outputs[:] = outputs
         return graph
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/no_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def div_by_1(x):
     return x / 1
 
 
 # Replacement
-def identity(x):
+def identity(op, x):
     return op.Identity(x)
 
 
 mul_by_1_rule = pattern.RewriteRule(mul_by_1, identity)
 add_0_rule = pattern.RewriteRule(add_0, identity)
 sub_0_rule = pattern.RewriteRule(sub_0, identity)
 div_by_1_rule = pattern.RewriteRule(div_by_1, identity)
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,28 +28,30 @@
         groups=groups,
     )
     transposed = op.Transpose(group_norm, perm=[0, 3, 1, 2])
     return torch_module_op.submodule("torch_nn_modules_activation_SiLU")(transposed)
 
 
 def group_normalization_with_silu(
+    op,
     input,
     weight,
     bias,
     epsilon,
     groups,
 ):
-    group_norm = msft_op.GroupNorm(
+    group_norm = op.GroupNorm(
         input,
         weight,
         bias,
         activation=1,
         channels_last=1,
         epsilon=epsilon,
         groups=groups,
+        domain="com.microsoft",
     )
     return op.Transpose(group_norm, perm=[0, 3, 1, 2])
 
 
 group_normalization_merge_silu_submodule_rule = pattern.RewriteRule(
     group_normalization_and_silu_submodule,
     group_normalization_with_silu,
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,65 +101,56 @@
     adjusted_input_shape,
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
     bias_full,
     epsilon,
-    match_bindings: dict[str, ir.Value | Any] | None = None,
 ):
     adjusted_input = op.Reshape(input_x, adjusted_input_shape)
     inst_norm = op.InstanceNormalization(
         adjusted_input, weight_for_norm, bias_for_norm, epsilon=epsilon
     )
     adjusted_inst_norm = op.Reshape(inst_norm, original_input_shape)
     mul = op.Mul(adjusted_inst_norm, weight_full)
     return op.Add(mul, bias_full)
 
 
-def group_normalization(
-    input_x,
-    adjusted_input_shape,
-    original_input_shape,
-    weight_for_norm,
-    bias_for_norm,
-    weight_full,
-    bias_full,
-    epsilon,
-    match_bindings: dict[str, ir.Value],
-):
+def group_normalization(op, input_x, weight_for_norm, weight_full, bias_full, epsilon, **_):
     # com.microsoft.GroupNorm only supports NHWC for now
     nhwc_input = op.Transpose(input_x, perm=[0, 2, 3, 1])
     # com.microsoft.GroupNorm only supports gamma and beta as float type
     weight_full = op.Cast(weight_full, to=onnx.TensorProto.FLOAT)
     reshape_to_1d = op.Constant(value_ints=[-1])
     weight_full = op.Reshape(weight_full, reshape_to_1d)
     bias_full = op.Cast(bias_full, to=onnx.TensorProto.FLOAT)
     bias_full = op.Reshape(bias_full, reshape_to_1d)
     # re-obtain attribute groups
-    if "weight_for_norm" not in match_bindings:
-        raise ValueError("weight_for_norm is not found in match_bindings")
-    if match_bindings["weight_for_norm"].shape is None:
+    # TODO(rama): Earlier check implies weight_for_norm is a constant tensor?
+    # If not, we should add a check that shape[0] is not symbolic.
+    shape = weight_for_norm.shape
+    if shape is None:
         raise ValueError("weight_for_norm shape not known")
-    groups = match_bindings["weight_for_norm"].shape[0]
-    output = msft_op.GroupNorm(
+    groups = shape[0]
+    output = op.GroupNorm(
         nhwc_input,
         weight_full,
         bias_full,
         activation=0,
         channels_last=1,
         epsilon=epsilon,
         groups=groups,
+        domain="com.microsoft",
     )
     return op.Transpose(output, perm=[0, 3, 1, 2])
 
 
 # Register the rewrite rules
 instance_norm_to_group_norm_rule = pattern.RewriteRule(
     instance_simulates_group_normalization_pattern,
-    pattern.ReplacementPatternFunction(group_normalization, delay_run=True),
+    group_normalization,
     check_if_simulated_instance_norm_is_used,
 )
 
 # NOTE: instance_norm_to_group_norm_rule is subset of instance_norm_to_group_norm_with_silu_rule,
 # so we need to run instance_norm_to_group_norm_with_silu_rule first.
 rules = pattern.RewriteRuleSet([instance_norm_to_group_norm_rule])
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 def softmax_with_fp32_upcast(input, axis):
     upcast = op.Cast(input, to=onnx.TensorProto.FLOAT)
     softmax = op.Softmax(upcast, axis=axis)  # pylint: disable=redefined-outer-name
     return op.Cast(softmax, to=onnx.TensorProto.FLOAT16)
 
 
-def softmax(input, axis):
+def softmax(op, input, axis):
     return op.Softmax(input, axis=axis)
 
 
 def softmax_with_fp32_upcast_without_axis(input):
     upcast = op.Cast(input, to=onnx.TensorProto.FLOAT)
     softmax = op.Softmax(upcast)  # pylint: disable=redefined-outer-name
     return op.Cast(softmax, to=onnx.TensorProto.FLOAT16)
 
 
-def softmax_without_axis(input):
+def softmax_without_axis(op, input):
     return op.Softmax(input)
 
 
 def check_if_fp16_input(match_bindings: dict[str, ir.Value | Any]) -> bool:
     input_val = match_bindings.get("input")
     if input_val is None:
         logger.warning(
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/pattern.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
+import dataclasses
 import inspect
 import itertools
 import math
-from typing import Any, Callable, Sequence
+from typing import Any, Callable, List, Optional, Sequence, Tuple
 
 import numpy as np
 import onnx
 import onnx.numpy_helper
 import onnx.printer
 
 from onnxscript import ir
 from onnxscript.ir import _convenience
-from onnxscript.rewriter import _ir_utils
+from onnxscript.rewriter import _ir_utils, _tape
 
 # Overview of the pattern module: The classes below are used to define both
 # patterns (that we search for) and replacements for rewrite rules.
 # The matches() method of a pattern is used to check if an IR component
 # matches the pattern.
-# The to_ir() method of a pattern is used to create a new IR component
 # TODO: Ensure that all matches() methods have same type signature (where
-# appropriate) and that all to_ir() methods have same type signature (where
 # appropriate).
 
 
 class PythonPattern:
     def __init__(self, value: int | str | Sequence, name: str | None = None) -> None:
         self._value = value
         self._name = name
@@ -36,17 +35,14 @@
     @property
     def name(self) -> str | None:
         return self._name
 
     def matches(self, value: int | str | Sequence) -> bool:
         return value == self.value
 
-    def to_ir(self, model, bindings=None) -> int | str | Sequence:
-        return self.value
-
 
 class StringConstantPattern:
     def __init__(self, value: str, name: str) -> None:
         self._value = value
         self._name = name
 
     @property
@@ -56,17 +52,14 @@
     @property
     def name(self) -> str:
         return self._name
 
     def matches(self, attr: ir.AttrString) -> bool:
         return attr.value == self.value
 
-    def to_ir(self, model, bindings=None) -> ir.AttrString:
-        return ir.AttrString(value=self.value, name=self.name)
-
 
 class IntConstantPattern:
     def __init__(self, value: int, name: str) -> None:
         self._value = value
         self._name = name
 
     @property
@@ -76,17 +69,14 @@
     @property
     def name(self) -> str:
         return self._name
 
     def matches(self, attr: ir.AttrInt64) -> bool:
         return attr.value == self.value
 
-    def to_ir(self, model, bindings=None) -> ir.AttrInt64:
-        return ir.AttrInt64(value=self.value, name=self.name)
-
 
 class ListConstantPattern:
     def __init__(self, value: Sequence[int | str | float], name: str) -> None:
         self._value = value
         self._name = name
 
     @property
@@ -97,43 +87,28 @@
     def name(self) -> str:
         return self._name
 
     def matches(self, attr: ir.AttrFloat32s | ir.AttrInt64s | ir.AttrStrings) -> bool:
         # TODO: Need more data points to determine if this is the right way to compare lists.
         return attr.value == self.value
 
-    def to_ir(self, model, bindings=None) -> ir.AttrFloat32s | ir.AttrInt64s | ir.AttrStrings:
-        the_first_non_none_item = next((item for item in self.value if item is not None), None)
-        if isinstance(the_first_non_none_item, int):
-            return ir.AttrInt64s(value=self.value, name=self.name)  # type: ignore
-        if isinstance(the_first_non_none_item, str):
-            return ir.AttrStrings(value=self.value, name=self.name)  # type: ignore
-        if isinstance(the_first_non_none_item, float):
-            return ir.AttrFloat32s(value=self.value, name=self.name)  # type: ignore
-        raise TypeError(
-            f"Cannot convert list of {type(the_first_non_none_item)} to ConstantPattern"
-        )
-
 
 class PrefixPattern:
     """This pattern is used to simplify submodule opset pattern matching."""
 
     def __init__(self, value: str) -> None:
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     def matches(self, value: str) -> bool:
         return value.startswith(self.value)
 
-    def to_ir(self, model, bindings=None) -> str:
-        raise NotImplementedError("PrefixPattern should not be converted to IR")
-
 
 class FloatConstantPattern:
     def __init__(
         self, value: float, name: str, rel_tol: float = 1e-5, abs_tol: float = 1e-8
     ) -> None:
         self._value = value
         self._name = name
@@ -149,17 +124,14 @@
         return self._name
 
     def matches(self, attr: ir.AttrFloat32):
         return math.isclose(
             attr.value, self.value, rel_tol=self._rel_tol, abs_tol=self._abs_tol
         )
 
-    def to_ir(self, model, bindings=None) -> ir.AttrFloat32:
-        return ir.AttrFloat32(self.name, self.value)
-
 
 class TensorConstantPattern:
     def __init__(
         self, value: ir.TensorProtocol, name, rel_tol: float = 1e-3, abs_tol: float = 1e-3
     ) -> None:
         self._value = value
         self._name = name
@@ -182,17 +154,14 @@
                 attr.value,
                 self._value,
                 rtol=self._rel_tol,
                 atol=self._abs_tol,
             )
         )
 
-    def to_ir(self, model, bindings=None) -> ir.AttrTensor:
-        return ir.AttrTensor(self.name, self.value)
-
 
 def _make_constant_pattern(
     value: float | int | Sequence | ir.TensorProtocol, name: str
 ) -> (
     IntConstantPattern
     | FloatConstantPattern
     | TensorConstantPattern
@@ -234,92 +203,54 @@
         attr_val: int | float | Sequence | Var | ir.TensorProtocol | ir.Value,
         model: ir.Model,
     ) -> MatchResult:
         if isinstance(self.value_pattern, Var):
             return self.value_pattern.matches(attr_val, model)  # type: ignore[arg-type]
         return self.value_pattern.matches(attr_val)
 
-    def to_ir(self, model: ir.Model, rewrite_cache: RewriteCache, bindings=None) -> ir.Value:
-        if isinstance(self.value_pattern, Var):
-            val, nodes = self.value_pattern.to_ir(
-                model, bindings, 1, rewrite_cache
-            )  # TODO: handle multiple outputs
-            return val
-        # constant pattern
-        return self.value_pattern.to_ir(model, bindings)
-
 
 class OpsetPattern:
     """Represents an opset pattern.
 
     It is used primarily to create a NodePattern (via OpPattern).
     Example usage:
     ::
 
         z = op.Matmul(x, y)
 
     Here, `op` is an instance of OpsetPattern and `op.Matmul` is an instance
     of OpPattern, and  `op.Matmul(x, y)` is an instance of NodePattern.
 
     An opset pattern is also matched against the actual opset used in the
-    input model. Typically, we match against an ONNX opset (ignoring the
-    version), but we can match against a specific version of the opset too.
-    However, it is preferable that version-dependences are handled at the
-    level of a rewrite rule, rather than at the level of a pattern.
-
+    input model.
     """
 
-    def __init__(
-        self,
-        domain_pattern: PythonPattern | PrefixPattern,
-        version_pattern: PythonPattern | AnyPattern,
-    ) -> None:
+    def __init__(self, domain_pattern: PythonPattern | PrefixPattern | str) -> None:
+        if isinstance(domain_pattern, str):
+            domain_pattern = PythonPattern(domain_pattern)
         self.domain_pattern = domain_pattern
-        self.version_pattern = version_pattern
-
-    @classmethod
-    def singleton(cls, domain: str, version: int) -> OpsetPattern:
-        return cls(PythonPattern(domain), PythonPattern(version))
-
-    @classmethod
-    def domain(cls, domain: str) -> OpsetPattern:
-        return cls(PythonPattern(domain), AnyPattern())
 
     @classmethod
     def domain_prefix(cls, domain: str) -> OpsetPattern:
-        return cls(PrefixPattern(domain), AnyPattern())
+        return cls(PrefixPattern(domain))
 
-    def matches(self, opset):
-        domain, version = opset
-        return self.domain_pattern.matches(domain) and self.version_pattern.matches(version)
-
-    def to_ir(self, model, bindings=None) -> str:
-        domain = self.domain_pattern.to_ir(model, bindings)
-        assert isinstance(domain, str), f"Expected str, got {type(domain)}"
-        # TODO: Should we ban other custom domains?
-        if domain not in model.opset_imports:
-            assert isinstance(
-                self.version_pattern, PythonPattern
-            ), f"custom domain {domain} needs to have a specific version."
-            model.opset_imports[self.domain_pattern.value] = self.version_pattern.value
-        return domain
+    def matches(self, domain):
+        return self.domain_pattern.matches(domain)
 
     def __getattr__(self, name: str) -> Any:
         return OpPattern(self, PythonPattern(name))
 
     def submodule(self, name: str) -> Any:
         """This method is used to match against submodule ops with prefix."""
         return OpPattern(self, PrefixPattern(name))
 
 
-opset17 = OpsetPattern.singleton("", 17)
-
-onnxop = OpsetPattern.domain("")
+onnxop = OpsetPattern("")
 
-msft_op = OpsetPattern.singleton("com.microsoft", 1)
+msft_op = OpsetPattern("com.microsoft")
 
 torch_module_op = OpsetPattern.domain_prefix("pkg.torch")
 
 
 class OpPattern:
     """A utility class to build a NodePattern.
 
@@ -339,14 +270,15 @@
         opset_pattern: OpsetPattern,
         op_name_pattern: PythonPattern | PrefixPattern,
     ) -> None:
         self.opset_pattern = opset_pattern
         self.op_name_pattern = op_name_pattern
 
     def __call__(self, *args, **kwargs):
+        # TODO(rama): Unify with convention used elsewhere.
         if "_num_outputs" in kwargs:
             num_outputs = kwargs["_num_outputs"]
             del kwargs["_num_outputs"]
         else:
             num_outputs = 1
         attributes = {
             name: AttrPattern(value=value, name=name) for (name, value) in kwargs.items()
@@ -355,16 +287,16 @@
         if num_outputs == 1:
             return NodeOutputPattern(node_pattern, 0)
         else:
             return [NodeOutputPattern(node_pattern, i) for i in range(num_outputs)]
 
 
 def _to_value_pattern(
-    x: ValuePattern | int | float,
-) -> NodeOutputPattern | Constant | Var | ValuePattern:
+    x: ValuePattern | int | float | None,
+) -> NodeOutputPattern | Constant | ValuePattern | None:
     """Promotes an input-value used to construct a NodePattern to a ValuePattern.
 
     Example usage:
     ::
         x = op.MatMul(a, b)
         z = op.Add(x, 0)
 
@@ -372,15 +304,15 @@
     `0` is a constant (int) value, and is automatically promoted to a ValuePattern.
 
     Note that this is a shorthand for creating a Constant pattern. The user can more
     explicitly write this as:
     ::
         z = op.Add(x, op.Constant(0))
     """
-    if isinstance(x, ValuePattern):
+    if x is None or isinstance(x, ValuePattern):
         return x
     if isinstance(x, (int, float, Sequence)):
         return Constant(x)
     # TODO(titaiwang): Could this be wrapped Constant?
     raise TypeError(f"Cannot convert {type(x)} to ValuePattern")
 
 
@@ -429,16 +361,15 @@
         return self.matched_values
 
     def fail(self):
         self.success = False
         self.matched_values = None
         self.bindings = {}
 
-    def extend(self, other: MatchResult | bool, model):
-        del model  # Unused
+    def extend(self, other: MatchResult | bool):
         if not self.success:
             return
         if not other:
             self.fail()
             return
         if isinstance(other, bool):
             return
@@ -457,16 +388,33 @@
 class ValuePattern:
     """Base class for all patterns that match against IR values.
 
     This is used primarily to provide operator overloadings for arithmetic
     operations, so that we can write patterns like `x + 1` and `1 + x`.
     """
 
-    def __init__(self) -> None:
-        pass
+    def __init__(self, name: str | None) -> None:
+        self.name = name
+
+    def __repr__(self) -> str:
+        return f"ValuePattern({self.name!r})"
+
+    def matches(self, value: ir.Value, model: ir.Model):
+        if self.name is None:
+            return MatchResult([], {})
+        return MatchResult([], {self.name: value})
+
+    def commute(self) -> Sequence[ValuePattern]:
+        """Return a list of commuted patterns.
+
+        This is used to handle commutative operations like addition and multiplication.
+        A single pattern is converted into a list of equivalent patterns by swapping
+        the parameters of commutative operations.
+        """
+        return [self]
 
     def __add__(self, other):
         return onnxop.Add(self, other)
 
     def __radd__(self, other):
         return onnxop.Add(other, self)
 
@@ -500,200 +448,121 @@
     a specific output of a node.
     """
 
     def __init__(
         self,
         domain: OpsetPattern,
         op: PythonPattern | PrefixPattern,
-        inputs: Sequence[int | float | ValuePattern],
+        inputs: Sequence[int | float | ValuePattern | None],
         attributes: dict[str, AttrPattern],
     ):
         self.domain = domain
         self.op = op
         self.inputs = [_to_value_pattern(x) for x in inputs]
         self.attributes = attributes
         self.bound_value = None
 
-    def matches(self, value: ir.Value, model: ir.Model):
-        if self.bound_value is not None:
-            # DAG-matching, not Tree-matching.
-            if self.bound_value.is_same_as(value):
-                return MatchResult([])
-            else:
-                return MatchResult.FAIL()
-        node = value.producer()
-        if node is None:
-            # Eg., value could be an input parameter, which will not match a value
-            # computed by the op in this pattern.
-            return MatchResult.FAIL()
-        return self.matches_node(node, model)
-
     def matches_node(self, node: ir.Node, model: ir.Model) -> MatchResult:
         """Examine if the IR node matches the self pattern."""
-        node_version = model.graph.opset_imports.get(node.domain, 0)
-        if not self.domain.matches((node.domain, node_version)):
+        if not self.domain.matches(node.domain):
             return MatchResult.FAIL()
         if not self.op.matches(node.op_type):
             return MatchResult.FAIL()
         match = MatchResult([])
         # TODO: We should add filtered logging starting from here to emit why
         # matching failed. This should cut a lot of noises compared to logging everything,
         # because at least the starting node op_type is already matched.
         for arg_value, previous_node_output_pattern in zip(node.inputs, self.inputs):
             # previous_node_output_pattern could be a Var, if it's the original arg.
+            if arg_value is None and previous_node_output_pattern is None:
+                continue
+            if arg_value is None or previous_node_output_pattern is None:
+                return MatchResult.FAIL()
             sub_match = previous_node_output_pattern.matches(arg_value, model)  # type: ignore[attr-defined]
-            match.extend(sub_match, model)
+            match.extend(sub_match)
             if not match:  # If sub-match failed,
                 return match
         # Sub-graphs not handled yet.
         for name, attr_pattern in self.attributes.items():
             attr_value = node.attributes.get(name)
             if attr_value is None:
                 return MatchResult.FAIL()
             sub_match = attr_pattern.matches(attr_value, model)  # type: ignore[arg-type]
             if not sub_match:
                 return MatchResult.FAIL()
-            match.extend(sub_match, model)
+            match.extend(sub_match)
         for name in node.attributes:
             # TODO: Support matching default values for attributes.
             if name not in self.attributes:
                 return MatchResult.FAIL()
         assert match.values is not None, "Matched values should not be None."
         match.values.append(node)  #  type: ignore[attr-defined]
         return match
 
-    def to_ir(
-        self,
-        model: ir.Model,
-        bindings: dict[str, ir.Value | Any],
-        num_outputs: int,
-        rewrite_cache: RewriteCache,
-    ) -> tuple[Sequence[ir.Value], Sequence[ir.Node]]:
-        domain = self.domain.to_ir(model)
-        op = self.op.to_ir(model)
-        assert isinstance(op, str), f"Expected str, got {type(op)}"
-        inputs = []
-        nodes: list[ir.Node] = []
-        for val_pattern in self.inputs:
-            if (
-                value_and_node := rewrite_cache.get_node_output_pattern(val_pattern)  # type: ignore[arg-type]
-            ) is not None:
-                val, n = value_and_node
-            else:
-                val, n = val_pattern.to_ir(model, bindings, 1, rewrite_cache)  # type: ignore[attr-defined]
-                rewrite_cache.set_node_output_pattern_with_ir(val_pattern, val, n)  # type: ignore[arg-type]
-                nodes.extend(n)  # type: ignore[arg-type]
-            # If one of the inputs was a the output of a previous node,
-            # unpack the new output ir value that is created for that node
-            if isinstance(val, tuple):
-                # TODO: Move implementation of output_index to NodeOutputPatter.to_ir
-                inputs.append(val[val_pattern.output_index])
-            else:
-                inputs.append(val)
-        attributes = (
-            attr_pattern.to_ir(model, rewrite_cache, bindings)
-            for attr_pattern in self.attributes.values()
-        )
-        new_node = ir.Node(
-            domain=domain,
-            op_type=op,
-            inputs=inputs,
-            attributes=attributes,  # type: ignore[arg-type]
-            num_outputs=num_outputs,
-        )
-        nodes.append(new_node)
-        return new_node.outputs, nodes
-
     def commute(self) -> Sequence[NodePattern]:
-        list_of_lists = [pattern.commute() for pattern in self.inputs]  # type: ignore[attr-defined]
+        list_of_lists = [
+            [None] if pattern is None else pattern.commute() for pattern in self.inputs
+        ]  # type: ignore[attr-defined]
 
         def enumerate_inputs(inputs, index):
             if index >= len(inputs):
                 yield []
             else:
                 for pattern in inputs[index]:
                     for rest in enumerate_inputs(inputs, index + 1):
                         yield [pattern, *rest]
 
         inputs = list(enumerate_inputs(list_of_lists, 0))
-        if self.domain.matches(("", None)) and (
-            self.op.matches("Add") or self.op.matches("Mul")
-        ):
+        if self.domain.matches("") and (self.op.matches("Add") or self.op.matches("Mul")):
             # TODO: handle cases where number of inputs is not 2.
             swapped = [[x[1], x[0]] for x in inputs]
             inputs.extend(swapped)
         return [NodePattern(self.domain, self.op, input, self.attributes) for input in inputs]
 
 
 class NodeOutputPattern(ValuePattern):
     """Represents a pattern that matches against a specific output of a Node.
 
     This is the primary pattern used to match against computed values, that
     is values computed using a specific op.
     """
 
-    def __init__(self, node_pattern: NodePattern, output_index: int) -> None:
+    def __init__(
+        self, node_pattern: NodePattern, output_index: int, name: str | None = None
+    ) -> None:
+        super().__init__(name)
         self.node_pattern = node_pattern
         self.output_index = output_index
 
     def matches(self, value: ir.Value, model: ir.Model):
         """Match the StaticValueInfo from IR with the `matches_node()` in node pattern."""
         node = value.producer()
         if node is None:
             return MatchResult.FAIL()
         if value.index() != self.output_index:
             return MatchResult.FAIL()
         return self.node_pattern.matches_node(node, model)
 
-    def to_ir(
-        self,
-        model: ir.Model,
-        bindings: dict[str, ir.Value | Any],
-        num_outputs: int,
-        rewrite_cache: RewriteCache,
-    ) -> tuple[Sequence[ir.Value], Sequence[ir.Node]]:
-        assert self.output_index == 0, "TODO: handle multiple outputs"
-        return self.node_pattern.to_ir(model, bindings, num_outputs, rewrite_cache)
-
-
-class Var(ValuePattern):
-    """Represents a pattern variable."""
-
-    def __init__(self, name: str) -> None:
-        self.pattern_var_name = name
-        self.bound_value = None
-
-    def __repr__(self) -> str:
-        return f"Var({self.pattern_var_name!r})"
-
-    def matches(self, value: ir.Value, model: ir.Model):
-        return MatchResult([], {self.pattern_var_name: value})
+    def commute(self) -> Sequence[ValuePattern]:
+        return [
+            NodeOutputPattern(pattern, self.output_index, self.name)
+            for pattern in self.node_pattern.commute()
+        ]
 
-    def to_ir(
-        self,
-        model: ir.Model,
-        bindings: dict[str, ir.Value | Any],
-        num_outputs: int,
-        rewrite_cache: RewriteCache,
-    ) -> tuple[ir.Value, Sequence]:
-        del model  # Unused
-        del num_outputs  # Unused
-        del rewrite_cache  # Unused
-        return bindings[self.pattern_var_name], []
 
-    def commute(self) -> Sequence[ValuePattern]:
-        return [self]
+Var = ValuePattern
 
 
 class Constant(ValuePattern):
     """Represents a pattern that matches against a scalar constant value."""
 
     def __init__(
         self, value: int | float, rel_tol: float = 1e-5, abs_tol: float = 1e-8
     ) -> None:
+        super().__init__(None)
         self.value = value
         self.rel_tol = rel_tol
         self.abs_tol = abs_tol
 
     def match_scalar(self, scalar_value, return_value: Sequence[ir.Node]):
         if math.isclose(scalar_value, self.value, rel_tol=self.rel_tol, abs_tol=self.abs_tol):
             return MatchResult(return_value)
@@ -752,26 +621,24 @@
         node_pattern = node_output_pattern.node_pattern
         num_outputs = 1
     elif isinstance(node_output_pattern, Sequence):
         node_pattern = node_output_pattern[0].node_pattern
         num_outputs = len(node_output_pattern)
         for i, p in enumerate(node_output_pattern):
             assert isinstance(p, NodeOutputPattern)
-            assert p.node_pattern is node_pattern
-            assert p.output_index == i
+            if (p.node_pattern is not node_pattern) or (p.output_index != i):
+                raise NotImplementedError(
+                    "Multi-output pattern not handled by this API. "
+                    "Use other APIs to handle multi-output patterns."
+                )
     else:
         raise TypeError(f"Invalid type {type(node_output_pattern)} for pattern")
     return node_pattern, num_outputs
 
 
-# Currently, the replacement graph function is the same as the pattern function.
-# This may change in the future.
-_handle_replacement_return_value = _handle_pattern_return_value
-
-
 def _valid_to_replace(matched_nodes: Sequence[Any]) -> bool:
     """Check that values computed by the matched_nodes, except for the last one, are used only by the matched_nodes."""
     # * Must check that all values matched by pattern are used only by pattern,
     # except for the value that is replaced.
     # * Must ensure that replacement subgraph does not use any of the deleted
     # (intermediate) values. (Not necessary for now. Guaranteed.)
     deleted_nodes = matched_nodes[:-1]
@@ -796,71 +663,107 @@
     def __init__(self, function: Callable) -> None:
         self._function = function
 
     @property
     def function(self) -> Callable:
         return self._function
 
-    def get_pattern(self, *variables: Sequence[Var]) -> tuple[NodePattern, int]:
+    def get_pattern(self, variables: Sequence[Var]) -> tuple[NodePattern, int]:
         node_output_pattern = self._function(*variables)
         return _handle_pattern_return_value(node_output_pattern)
 
 
+# A type representing the domains/versions used in creating a replacement subgraph
+UsedOpsets = List[Tuple[str, Optional[int]]]
+
+
+class RewriterContext:
+    """Context parameter used to build the replacement pattern."""
+
+    # TODO(justinchuby): Merge with the rest of pattern building methods
+    def __init__(self):
+        self._tape = _tape.Tape()
+        self._used_opsets: UsedOpsets = []
+
+    def __getattr__(self, op_type: str) -> Any:
+        return lambda *args, **kwargs: self._make_node(op_type, args, kwargs)
+
+    def _make_node(self, op_type: str, inputs: Sequence[ir.Value], kwargs: dict[str, Any]):
+        domain = kwargs.pop("domain", "")
+        version = kwargs.pop("version", None)
+        self._used_opsets.append((domain, version))
+        outputs = kwargs.pop("outputs", 1)
+        if isinstance(outputs, Sequence):
+            num_outputs = len(outputs)
+        else:
+            assert isinstance(outputs, int)
+            num_outputs = outputs
+        if num_outputs == 1:
+            return self._tape.op(op_type, inputs=inputs, attributes=kwargs, domain=domain)
+        return self._tape.op_multi_output(
+            op_type, inputs=inputs, attributes=kwargs, domain=domain, num_outputs=num_outputs
+        )
+
+    @property
+    def nodes(self) -> Sequence[ir.Node]:
+        # TODO(rama): The current tape-based implementation will not track nodes added
+        # via overloaded operators, eg., `x + y`. One possible way to fix this is to
+        # have values/nodes know which tape they belong to (instead of a graph/function).
+        # However, it is unclear we need this feature for rewriting: we could also
+        # identify the nodes to be inserted from the replacement values (by tracing back).
+        return self._tape.nodes
+
+    @property
+    def used_opsets(self) -> UsedOpsets:
+        return self._used_opsets
+
+
+@dataclasses.dataclass
+class ReplacementSubgraph:
+    """A subgraph that will replace the matched pattern."""
+
+    new_values: Sequence[ir.Value]
+    new_nodes: Sequence[ir.Node]
+    used_opsets: UsedOpsets
+
+
 class ReplacementPatternFunction:
     """The replacement pattern that will replace the targeted pattern.
 
     Attributes:
         function (Callable): The replacement function that will be used to replace the matched pattern.
-        delay_run (bool): If True, the replacement function will not be run until the matched pattern is found.
-            This is useful when we want to extract certain metavalue from the matched pattern and use it in the
-            replacement pattern.
     """
 
-    def __init__(self, function, *, delay_run: bool = False):
+    def __init__(self, function) -> None:
         self._function = function
-        self._delay_run = delay_run
-
-    @property
-    def function(self) -> Callable:
-        return self._function
-
-    @property
-    def delay_run(self) -> bool:
-        return self._delay_run
 
-    # TODO: How do we merge it with to_ir function?
-    def get_pattern(
+    def get_replacement(
         self,
-        *vars: Sequence[Var],
         match_bindings: dict[str, ir.Value | Any] | None = None,
-    ) -> tuple[NodePattern | None, int | None]:
-        if self._delay_run:
-            if match_bindings is None:
-                return None, None
-            node_output_pattern = self._function(*vars, match_bindings)
-        else:
-            node_output_pattern = self._function(*vars)
-        return _handle_pattern_return_value(node_output_pattern)
-
+    ) -> ReplacementSubgraph:
+        context = RewriterContext()
+        new_values = self._function(context, **match_bindings)
+        if not isinstance(new_values, Sequence):
+            new_values = [new_values]
+        return ReplacementSubgraph(new_values, context.nodes, context.used_opsets)
 
-class RewriteCache:
-    def __init__(self):
-        self._node_output_pattern_to_ir: dict[NodeOutputPattern, tuple[ir.Value, ir.Node]] = (
-            dict()
-        )
-
-    def get_node_output_pattern(
-        self, node_output_pattern: NodeOutputPattern
-    ) -> tuple[ir.Value, ir.Node] | None:
-        return self._node_output_pattern_to_ir.get(node_output_pattern, None)
 
-    def set_node_output_pattern_with_ir(
-        self, node_output_pattern: NodeOutputPattern, value: ir.Value, node: ir.Node
-    ) -> None:
-        self._node_output_pattern_to_ir[node_output_pattern] = (value, node)
+def _update_opset_imports(
+    graph_or_function: ir.Graph | ir.Function, delta: ReplacementSubgraph
+):
+    imports = graph_or_function.opset_imports
+    for domain, version in delta.used_opsets:
+        if domain not in imports:
+            # use 1 as default version if not explicitly specified
+            imports[domain] = version if version is not None else 1
+        elif version is not None and version != imports[domain]:
+            raise ValueError(
+                f"Multiple versions of opset {domain} used. "
+                f"Expected version {imports[domain]}, but got {version}."
+            )
 
 
 class RewriteRule:
     def __init__(
         self,
         target_pattern: TargetPatternFunction | Callable | None = None,
         replacement_pattern: ReplacementPatternFunction | Callable | None = None,
@@ -875,19 +778,17 @@
                 will be used to replace the matched pattern.
             condition_function: The condition function that
                 will be used to check if the pattern matches the IR with ir.Values
                 constraints in consideration.
 
         """
         if target_pattern is None:
-            # NOTE: commute() generated rules will have target_pattern as None
-            # ReplacementPatternFunction is still needed in try_rewrite
+            # NOTE: this is a default-constructor. Caller responsible for filling in the fields.
             assert replacement_pattern is None
             assert condition_function is None
-            self._replacement_pattern = ReplacementPatternFunction(replacement_pattern)
             return
         elif replacement_pattern is None:
             raise ValueError(
                 "replacement_pattern must be provided if target_pattern is provided"
             )
         # TODO: Do we want to tolerate Callable inputs?
         if callable(target_pattern):
@@ -896,29 +797,20 @@
             replacement_pattern = ReplacementPatternFunction(replacement_pattern)
 
         self._target_pattern = target_pattern
         self._replacement_pattern = replacement_pattern
         self._condition_function = condition_function
 
         _pattern_vars = inspect.signature(self._target_pattern.function).parameters
-        _replacement_vars = inspect.signature(self._replacement_pattern.function).parameters
-        # TODO: accept _replacement_vars being subset of _pattern_vars?
-        assert len(_pattern_vars) == len(_replacement_vars)
 
         self._vars = [Var(v) for v in _pattern_vars]
         # Get the last node pattern and number of outputs from the pattern function
         self._target_node_pattern, self._target_num_outputs = self._target_pattern.get_pattern(
-            *self._vars  # type: ignore[arg-type]
-        )
-        # NOTE: Return Nones if the replacement pattern is delayed running
-        self._replace_node_pattern, _replacement_num_outputs = replacement_pattern.get_pattern(
-            *self._vars  # type: ignore[arg-type]
+            self._vars  # type: ignore[arg-type]
         )
-        if _replacement_num_outputs is not None:
-            assert self._target_num_outputs == _replacement_num_outputs
 
     def matches(self, node: ir.Node, model: ir.Model) -> MatchResult:
         """Check if the node from IR matches the pattern."""
         if len(node.outputs) != self._target_num_outputs:
             return MatchResult.FAIL()
         match = self._target_node_pattern.matches_node(node, model)
         if (
@@ -926,38 +818,38 @@
             and match
             and not self._condition_function(match.bindings)
         ):
             return MatchResult.FAIL()
         return match
 
     def try_rewrite(
-        self, model: ir.Model, node: ir.Node
-    ) -> tuple[Sequence[Any], Sequence[ir.Node]] | None:
+        self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
+    ):  # TODO(rama) -> ReplacementSubgraph | None:
         """If the node matches the pattern, then replace the node with the replacement pattern."""
         match = self.matches(node, model)
         if match:
             assert match.values is not None, "Matched values should not be None."
             if _valid_to_replace(match.values):
-                # NOTE: delayed running as the replacement pattern needs bindings
-                if self._replacement_pattern.delay_run:
-                    # bindings will be consumed by the replacement function
-                    self._replace_node_pattern, _replacement_num_outputs = (
-                        self._replacement_pattern.get_pattern(
-                            *self._vars[:-1],  # type: ignore[arg-type]
-                            match_bindings=match.bindings,
-                        )
+                # bindings will be consumed by the replacement function
+                delta = self._replacement_pattern.get_replacement(match.bindings)
+                if len(delta.new_values) != self._target_num_outputs:
+                    raise ValueError(
+                        f"Number of outputs from replacement function does not match the number of outputs from the target pattern. "
+                        f"Expected {self._target_num_outputs}, but got {len(delta.new_values)}."
                     )
-                    assert self._target_num_outputs == _replacement_num_outputs
-                rewrite_cache = RewriteCache()
-                assert self._replace_node_pattern is not None, "Replacement pattern is None."
-                _, _to_insert = self._replace_node_pattern.to_ir(
-                    model, match.bindings, self._target_num_outputs, rewrite_cache
-                )
-
-                return (match.values, _to_insert)  # type: ignore[return-value]
+                # TODO(rama): Check/update opset-imports
+                # (i) Integrate following with the multi-output matcher and code elsewhere:
+                # (ii) Remove the opset imports from deleted nodes?
+                # (iii) Code in the caller (below) checks if match overlaps previous match, which
+                # appears incorrect for single-pattern matcher. Best to alter iteration to apply
+                # each rewrite immediately, instead of accumulating them.
+                # (iv) return delta here
+                _update_opset_imports(graph_or_function, delta)
+                _update_opset_imports(model.graph, delta)
+                return match.values, delta.new_nodes
         return None
 
     def apply_to_model(self, model: ir.Model, *, commute: bool = False):
         # TODO(titaiwang): Why do we need RewriteRuleSet?
         return RewriteRuleSet([self], commute=commute).apply_to_model(model)
 
     def count_matches(self, model: ir.Model, *, commute: bool = False):
@@ -966,15 +858,16 @@
     def commute(self) -> Sequence[RewriteRule]:
         def replace_pattern(new_pattern):
             """Return a shallow copy of self with node_pattern replaced by new_pattern."""
             rule = RewriteRule()
             rule._condition_function = self._condition_function
             rule._target_node_pattern = new_pattern
             rule._target_num_outputs = self._target_num_outputs
-            rule._replace_node_pattern = self._replace_node_pattern
+            rule._replacement_pattern = self._replacement_pattern
+            rule._vars = self._vars
             return rule
 
         return [replace_pattern(p) for p in self._target_node_pattern.commute()]
 
 
 def _apply_deltas(
     graph_or_function: ir.Graph | ir.Function,
@@ -1013,21 +906,29 @@
             # the position to insert must be chosen.
             # we'll try position i
             assert i not in to_insert  # conflicts should avoid that case
             to_insert.append((graph_or_function[i], inserted_nodes))
         else:
             deleted_nodes, inserted_nodes = delta
             # Replace deleted nodes with inserted nodes.
-            # However, we merge the last deleted node and last inserted node
-            # to avoid replacing the values produced by the last deleted node
-            # in all places where they are used. So, we reuse the output
-            # values from the last deleted node and replace the node itself
             # TODO: simplify this
             last_deleted = deleted_nodes[-1]
             last_inserted = inserted_nodes[-1]
+
+            for old_value, new_value in zip(last_deleted.outputs, last_inserted.outputs):
+                # Propagate relevant info from old value to new value
+                # TODO(Rama): Perhaps we should merge old and new types. As of now, new
+                # values don't have type information. Note that this could be a problem
+                # for semantics-altering rewrite-rules: we should allow users to override
+                # this for such rules.
+                new_value.type = old_value.type
+                new_value.shape = old_value.shape
+                new_value.const_value = old_value.const_value
+                new_value.name = old_value.name
+
             # Reconnect the users of the deleted node to use the new outputs
             _convenience.replace_all_uses_with(last_deleted.outputs, last_inserted.outputs)
             # Update graph/function outputs if the node generates output
             replacement_mapping = dict(zip(last_deleted.outputs, last_inserted.outputs))
             for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
                 if graph_or_function_output in replacement_mapping:
                     graph_or_function.outputs[idx] = replacement_mapping[
@@ -1064,15 +965,15 @@
         count = 0
         marked = set()
         # NOTE: Rules should be prioritized in the order they are added to the RewriteRuleSet.
         # And the graph is applied in order.
         for rule in self.rules:
             deltas = []
             for i, node in enumerate(graph_or_function):
-                delta = rule.try_rewrite(model, node)
+                delta = rule.try_rewrite(model, graph_or_function, node)
 
                 if delta is None:
                     continue
 
                 matched_nodes, _ = delta[-2:]
 
                 conflict = False
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240426/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240426/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240426/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240426/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240426/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript/values.py` & `onnxscript-0.1.0.dev20240426/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240426/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240425
+Version: 0.1.0.dev20240426
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240425/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240426/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/pyproject.toml` & `onnxscript-0.1.0.dev20240426/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240425/setup.py` & `onnxscript-0.1.0.dev20240426/setup.py`

 * *Files identical despite different names*

