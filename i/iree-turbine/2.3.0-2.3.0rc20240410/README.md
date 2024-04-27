# Comparing `tmp/iree_turbine-2.3.0-py3-none-any.whl.zip` & `tmp/iree_turbine-2.3.0rc20240410-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,90 +1,87 @@
-Zip file size: 162844 bytes, number of entries: 88
--rw-rw-r--  2.0 unx      831 b- defN 24-Apr-27 20:01 iree/turbine/__init__.py
--rw-rw-r--  2.0 unx      515 b- defN 24-Apr-27 20:01 shark_turbine/aot/__init__.py
--rw-rw-r--  2.0 unx    23347 b- defN 24-Apr-27 20:01 shark_turbine/aot/compiled_module.py
--rw-rw-r--  2.0 unx     2815 b- defN 24-Apr-27 20:01 shark_turbine/aot/decompositions.py
--rw-rw-r--  2.0 unx     9877 b- defN 24-Apr-27 20:01 shark_turbine/aot/exporter.py
--rw-rw-r--  2.0 unx    12219 b- defN 24-Apr-27 20:01 shark_turbine/aot/fx_programs.py
--rw-rw-r--  2.0 unx     9661 b- defN 24-Apr-27 20:01 shark_turbine/aot/params.py
--rw-rw-r--  2.0 unx     1023 b- defN 24-Apr-27 20:01 shark_turbine/aot/tensor_traits.py
--rw-rw-r--  2.0 unx      906 b- defN 24-Apr-27 20:01 shark_turbine/aot/builtins/__init__.py
--rw-rw-r--  2.0 unx     7100 b- defN 24-Apr-27 20:01 shark_turbine/aot/builtins/globals.py
--rw-rw-r--  2.0 unx    18037 b- defN 24-Apr-27 20:01 shark_turbine/aot/builtins/jittable.py
--rw-rw-r--  2.0 unx      262 b- defN 24-Apr-27 20:01 shark_turbine/aot/passes/__init__.py
--rw-rw-r--  2.0 unx     3537 b- defN 24-Apr-27 20:01 shark_turbine/aot/passes/functorch.py
--rw-rw-r--  2.0 unx    16691 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/ir_utils.py
--rw-rw-r--  2.0 unx      646 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/__init__.py
--rw-rw-r--  2.0 unx     7507 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/base.py
--rw-rw-r--  2.0 unx    12631 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/exported_program.py
--rw-rw-r--  2.0 unx     9222 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/globals.py
--rw-rw-r--  2.0 unx    12373 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/iree_emitter.py
--rw-rw-r--  2.0 unx    11744 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/primitives.py
--rw-rw-r--  2.0 unx     7211 b- defN 24-Apr-27 20:01 shark_turbine/aot/support/procedural/tracer.py
--rw-rw-r--  2.0 unx      287 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/__init__.py
--rw-rw-r--  2.0 unx     3985 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/decompositions.py
--rw-rw-r--  2.0 unx     8179 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/executor.py
--rw-rw-r--  2.0 unx      814 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/passes.py
--rw-rw-r--  2.0 unx    21970 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/tensor.py
--rw-rw-r--  2.0 unx     7737 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/type_conversion.py
--rw-rw-r--  2.0 unx     2816 b- defN 24-Apr-27 20:01 shark_turbine/dynamo/backends/cpu.py
--rw-rw-r--  2.0 unx      857 b- defN 24-Apr-27 20:01 shark_turbine/importers/ir.py
--rw-rw-r--  2.0 unx     1192 b- defN 24-Apr-27 20:01 shark_turbine/importers/utils.py
--rw-rw-r--  2.0 unx      518 b- defN 24-Apr-27 20:01 shark_turbine/kernel/__init__.py
--rw-rw-r--  2.0 unx     1484 b- defN 24-Apr-27 20:01 shark_turbine/kernel/_support/context.py
--rw-rw-r--  2.0 unx     1157 b- defN 24-Apr-27 20:01 shark_turbine/kernel/_support/dtype.py
--rw-rw-r--  2.0 unx    12390 b- defN 24-Apr-27 20:01 shark_turbine/kernel/_support/indexing.py
--rw-rw-r--  2.0 unx     5147 b- defN 24-Apr-27 20:01 shark_turbine/kernel/_support/regions.py
--rw-rw-r--  2.0 unx     3549 b- defN 24-Apr-27 20:01 shark_turbine/kernel/_support/shaped_type.py
--rw-rw-r--  2.0 unx    15676 b- defN 24-Apr-27 20:01 shark_turbine/kernel/_support/tracing.py
--rw-rw-r--  2.0 unx      103 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/base.py
--rw-rw-r--  2.0 unx    11457 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/builder.py
--rw-rw-r--  2.0 unx     8284 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/dispatch_codegen.py
--rw-rw-r--  2.0 unx     1796 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/host_codegen.py
--rw-rw-r--  2.0 unx      744 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/ir.py
--rw-rw-r--  2.0 unx     8658 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/kernel_codegen.py
--rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/op_matchers.py
--rw-rw-r--  2.0 unx    35543 b- defN 24-Apr-27 20:01 shark_turbine/kernel/compiler/vector_codegen.py
--rw-rw-r--  2.0 unx       94 b- defN 24-Apr-27 20:01 shark_turbine/kernel/gen/__init__.py
--rw-rw-r--  2.0 unx     5342 b- defN 24-Apr-27 20:01 shark_turbine/kernel/gen/kernel.py
--rw-rw-r--  2.0 unx     4886 b- defN 24-Apr-27 20:01 shark_turbine/kernel/gen/thread.py
--rw-rw-r--  2.0 unx      339 b- defN 24-Apr-27 20:01 shark_turbine/kernel/lang/__init__.py
--rw-rw-r--  2.0 unx     1454 b- defN 24-Apr-27 20:01 shark_turbine/kernel/lang/grid.py
--rw-rw-r--  2.0 unx     4476 b- defN 24-Apr-27 20:01 shark_turbine/kernel/lang/kernel_buffer.py
--rw-rw-r--  2.0 unx     1031 b- defN 24-Apr-27 20:01 shark_turbine/kernel/lang/prims.py
--rw-rw-r--  2.0 unx     1331 b- defN 24-Apr-27 20:01 shark_turbine/kernel/lang/types.py
--rw-rw-r--  2.0 unx      149 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/__init__.py
--rw-rw-r--  2.0 unx     1237 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/base.py
--rw-rw-r--  2.0 unx      638 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/control_flow.py
--rw-rw-r--  2.0 unx      581 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/core.py
--rw-rw-r--  2.0 unx      330 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/math.py
--rw-rw-r--  2.0 unx      577 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/memory.py
--rw-rw-r--  2.0 unx      487 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/reduction.py
--rw-rw-r--  2.0 unx      555 b- defN 24-Apr-27 20:01 shark_turbine/kernel/ops/shape_manipulation.py
--rw-rw-r--  2.0 unx      248 b- defN 24-Apr-27 20:01 shark_turbine/ops/__init__.py
--rw-rw-r--  2.0 unx     2598 b- defN 24-Apr-27 20:01 shark_turbine/ops/iree.py
--rw-rw-r--  2.0 unx      272 b- defN 24-Apr-27 20:01 shark_turbine/runtime/__init__.py
--rw-rw-r--  2.0 unx    18221 b- defN 24-Apr-27 20:01 shark_turbine/runtime/device.py
--rw-rw-r--  2.0 unx     3453 b- defN 24-Apr-27 20:01 shark_turbine/runtime/tracing.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-27 20:01 shark_turbine/runtime/op_reg/__init__.py
--rw-rw-r--  2.0 unx    28722 b- defN 24-Apr-27 20:01 shark_turbine/runtime/op_reg/base.py
--rw-rw-r--  2.0 unx     5156 b- defN 24-Apr-27 20:01 shark_turbine/runtime/op_reg/compiler.py
--rw-rw-r--  2.0 unx     8341 b- defN 24-Apr-27 20:01 shark_turbine/runtime/op_reg/eager.py
--rw-rw-r--  2.0 unx      339 b- defN 24-Apr-27 20:01 shark_turbine/support/__init__.py
--rw-rw-r--  2.0 unx     4118 b- defN 24-Apr-27 20:01 shark_turbine/support/conversions.py
--rw-rw-r--  2.0 unx     3182 b- defN 24-Apr-27 20:01 shark_turbine/support/debugging.py
--rw-rw-r--  2.0 unx     1341 b- defN 24-Apr-27 20:01 shark_turbine/support/exceptions.py
--rw-rw-r--  2.0 unx     1142 b- defN 24-Apr-27 20:01 shark_turbine/support/ir_imports.py
--rw-rw-r--  2.0 unx     1255 b- defN 24-Apr-27 20:01 shark_turbine/support/logging.py
--rw-rw-r--  2.0 unx     2365 b- defN 24-Apr-27 20:01 shark_turbine/transforms/builder.py
--rw-rw-r--  2.0 unx     8382 b- defN 24-Apr-27 20:01 shark_turbine/transforms/merger.py
--rw-rw-r--  2.0 unx    10997 b- defN 24-Apr-27 20:01 shark_turbine/transforms/rewriter.py
--rw-rw-r--  2.0 unx    10886 b- defN 24-Apr-27 20:01 shark_turbine/transforms/general/custom_op_expansion.py
--rw-rw-r--  2.0 unx     4995 b- defN 24-Apr-27 20:01 shark_turbine/transforms/general/rename_parameters.py
--rw-rw-r--  2.0 unx     7775 b- defN 24-Apr-27 20:01 shark_turbine/transforms/quantization/mm_group_quant.py
--rw-rw-r--  2.0 unx    12262 b- defN 24-Apr-27 20:22 iree_turbine-2.3.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5351 b- defN 24-Apr-27 20:22 iree_turbine-2.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-27 20:22 iree_turbine-2.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       80 b- defN 24-Apr-27 20:22 iree_turbine-2.3.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       19 b- defN 24-Apr-27 20:22 iree_turbine-2.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8255 b- defN 24-Apr-27 20:22 iree_turbine-2.3.0.dist-info/RECORD
-88 files, 497871 bytes uncompressed, 149520 bytes compressed:  70.0%
+Zip file size: 150377 bytes, number of entries: 85
+-rw-rw-r--  2.0 unx      700 b- defN 24-Apr-10 21:52 iree/turbine/__init__.py
+-rw-rw-r--  2.0 unx      430 b- defN 24-Apr-10 21:46 shark_turbine/aot/__init__.py
+-rw-rw-r--  2.0 unx    23347 b- defN 24-Apr-10 21:46 shark_turbine/aot/compiled_module.py
+-rw-rw-r--  2.0 unx     2815 b- defN 24-Mar-29 02:54 shark_turbine/aot/decompositions.py
+-rw-rw-r--  2.0 unx     9666 b- defN 24-Apr-10 21:46 shark_turbine/aot/exporter.py
+-rw-rw-r--  2.0 unx    12219 b- defN 24-Mar-29 02:54 shark_turbine/aot/fx_programs.py
+-rw-rw-r--  2.0 unx     4751 b- defN 24-Apr-10 21:46 shark_turbine/aot/params.py
+-rw-rw-r--  2.0 unx     1023 b- defN 24-Apr-10 21:46 shark_turbine/aot/tensor_traits.py
+-rw-rw-r--  2.0 unx      884 b- defN 24-Mar-21 23:46 shark_turbine/aot/builtins/__init__.py
+-rw-rw-r--  2.0 unx     5431 b- defN 24-Apr-10 21:46 shark_turbine/aot/builtins/globals.py
+-rw-rw-r--  2.0 unx    18037 b- defN 24-Mar-29 02:54 shark_turbine/aot/builtins/jittable.py
+-rw-rw-r--  2.0 unx      262 b- defN 24-Feb-05 20:48 shark_turbine/aot/passes/__init__.py
+-rw-rw-r--  2.0 unx     3537 b- defN 24-Mar-05 20:36 shark_turbine/aot/passes/functorch.py
+-rw-rw-r--  2.0 unx    15795 b- defN 24-Apr-10 21:46 shark_turbine/aot/support/ir_utils.py
+-rw-rw-r--  2.0 unx      646 b- defN 24-Feb-05 20:48 shark_turbine/aot/support/procedural/__init__.py
+-rw-rw-r--  2.0 unx     7507 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/base.py
+-rw-rw-r--  2.0 unx    11775 b- defN 24-Apr-10 21:46 shark_turbine/aot/support/procedural/exported_program.py
+-rw-rw-r--  2.0 unx     9338 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/globals.py
+-rw-rw-r--  2.0 unx    12373 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/iree_emitter.py
+-rw-rw-r--  2.0 unx    11744 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/primitives.py
+-rw-rw-r--  2.0 unx     7211 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/tracer.py
+-rw-rw-r--  2.0 unx      287 b- defN 24-Feb-05 20:48 shark_turbine/dynamo/__init__.py
+-rw-rw-r--  2.0 unx     4096 b- defN 24-Mar-29 02:54 shark_turbine/dynamo/decompositions.py
+-rw-rw-r--  2.0 unx     8179 b- defN 24-Mar-05 20:36 shark_turbine/dynamo/executor.py
+-rw-rw-r--  2.0 unx      814 b- defN 24-Mar-29 02:54 shark_turbine/dynamo/passes.py
+-rw-rw-r--  2.0 unx    21970 b- defN 24-Mar-21 20:49 shark_turbine/dynamo/tensor.py
+-rw-rw-r--  2.0 unx     7017 b- defN 24-Mar-05 20:36 shark_turbine/dynamo/type_conversion.py
+-rw-rw-r--  2.0 unx     2816 b- defN 24-Mar-21 20:49 shark_turbine/dynamo/backends/cpu.py
+-rw-rw-r--  2.0 unx      857 b- defN 24-Feb-23 23:17 shark_turbine/importers/ir.py
+-rw-rw-r--  2.0 unx     1192 b- defN 24-Mar-05 20:36 shark_turbine/importers/utils.py
+-rw-rw-r--  2.0 unx      518 b- defN 24-Feb-05 20:48 shark_turbine/kernel/__init__.py
+-rw-rw-r--  2.0 unx     1484 b- defN 24-Feb-05 20:48 shark_turbine/kernel/_support/context.py
+-rw-rw-r--  2.0 unx     1157 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/dtype.py
+-rw-rw-r--  2.0 unx    12390 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/indexing.py
+-rw-rw-r--  2.0 unx     5147 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/regions.py
+-rw-rw-r--  2.0 unx     3549 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/shaped_type.py
+-rw-rw-r--  2.0 unx    15676 b- defN 24-Mar-02 22:06 shark_turbine/kernel/_support/tracing.py
+-rw-rw-r--  2.0 unx      103 b- defN 24-Feb-05 20:48 shark_turbine/kernel/compiler/base.py
+-rw-rw-r--  2.0 unx    11457 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/builder.py
+-rw-rw-r--  2.0 unx     8284 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/dispatch_codegen.py
+-rw-rw-r--  2.0 unx     1796 b- defN 24-Feb-22 02:07 shark_turbine/kernel/compiler/host_codegen.py
+-rw-rw-r--  2.0 unx      744 b- defN 24-Feb-22 02:07 shark_turbine/kernel/compiler/ir.py
+-rw-rw-r--  2.0 unx     8658 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/kernel_codegen.py
+-rw-rw-r--  2.0 unx     1770 b- defN 24-Feb-05 20:48 shark_turbine/kernel/compiler/op_matchers.py
+-rw-rw-r--  2.0 unx    35543 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/vector_codegen.py
+-rw-rw-r--  2.0 unx       94 b- defN 24-Mar-02 22:06 shark_turbine/kernel/gen/__init__.py
+-rw-rw-r--  2.0 unx     5342 b- defN 24-Mar-02 22:06 shark_turbine/kernel/gen/kernel.py
+-rw-rw-r--  2.0 unx     4886 b- defN 24-Mar-02 22:06 shark_turbine/kernel/gen/thread.py
+-rw-rw-r--  2.0 unx      339 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/__init__.py
+-rw-rw-r--  2.0 unx     1454 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/grid.py
+-rw-rw-r--  2.0 unx     4476 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/kernel_buffer.py
+-rw-rw-r--  2.0 unx     1031 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/prims.py
+-rw-rw-r--  2.0 unx     1331 b- defN 24-Feb-05 20:48 shark_turbine/kernel/lang/types.py
+-rw-rw-r--  2.0 unx      149 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/__init__.py
+-rw-rw-r--  2.0 unx     1237 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/base.py
+-rw-rw-r--  2.0 unx      638 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/control_flow.py
+-rw-rw-r--  2.0 unx      581 b- defN 24-Feb-26 22:45 shark_turbine/kernel/ops/core.py
+-rw-rw-r--  2.0 unx      330 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/math.py
+-rw-rw-r--  2.0 unx      577 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/memory.py
+-rw-rw-r--  2.0 unx      487 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/reduction.py
+-rw-rw-r--  2.0 unx      555 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/shape_manipulation.py
+-rw-rw-r--  2.0 unx      248 b- defN 24-Feb-05 20:48 shark_turbine/ops/__init__.py
+-rw-rw-r--  2.0 unx     1832 b- defN 24-Mar-28 03:11 shark_turbine/ops/iree.py
+-rw-rw-r--  2.0 unx      272 b- defN 24-Feb-05 20:48 shark_turbine/runtime/__init__.py
+-rw-rw-r--  2.0 unx    12469 b- defN 24-Mar-05 20:36 shark_turbine/runtime/device.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-Feb-05 20:48 shark_turbine/runtime/op_reg/__init__.py
+-rw-rw-r--  2.0 unx    28076 b- defN 24-Mar-29 00:40 shark_turbine/runtime/op_reg/base.py
+-rw-rw-r--  2.0 unx     4442 b- defN 24-Feb-05 20:48 shark_turbine/runtime/op_reg/compiler.py
+-rw-rw-r--  2.0 unx     6341 b- defN 24-Mar-05 20:36 shark_turbine/runtime/op_reg/eager.py
+-rw-rw-r--  2.0 unx      241 b- defN 24-Feb-05 20:48 shark_turbine/support/__init__.py
+-rw-rw-r--  2.0 unx     4118 b- defN 24-Mar-21 20:49 shark_turbine/support/conversions.py
+-rw-rw-r--  2.0 unx     1341 b- defN 24-Feb-05 20:48 shark_turbine/support/exceptions.py
+-rw-rw-r--  2.0 unx     1128 b- defN 24-Apr-10 21:46 shark_turbine/support/ir_imports.py
+-rw-rw-r--  2.0 unx      357 b- defN 24-Mar-05 20:36 shark_turbine/support/logging.py
+-rw-rw-r--  2.0 unx     2365 b- defN 24-Feb-05 20:48 shark_turbine/transforms/builder.py
+-rw-rw-r--  2.0 unx     8202 b- defN 24-Apr-10 21:43 shark_turbine/transforms/merger.py
+-rw-rw-r--  2.0 unx    10997 b- defN 24-Apr-10 21:43 shark_turbine/transforms/rewriter.py
+-rw-rw-r--  2.0 unx     9012 b- defN 24-Mar-28 03:11 shark_turbine/transforms/general/custom_op_expansion.py
+-rw-rw-r--  2.0 unx     4995 b- defN 24-Mar-05 20:36 shark_turbine/transforms/general/rename_parameters.py
+-rw-rw-r--  2.0 unx     7793 b- defN 24-Mar-05 20:36 shark_turbine/transforms/quantization/mm_group_quant.py
+-rw-rw-r--  2.0 unx     6262 b- defN 24-Apr-11 00:12 iree_turbine-2.3.0rc20240410.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 00:12 iree_turbine-2.3.0rc20240410.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       80 b- defN 24-Apr-11 00:12 iree_turbine-2.3.0rc20240410.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       19 b- defN 24-Apr-11 00:12 iree_turbine-2.3.0rc20240410.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8029 b- defN 24-Apr-11 00:12 iree_turbine-2.3.0rc20240410.dist-info/RECORD
+85 files, 457462 bytes uncompressed, 137385 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -189,17 +189,14 @@
 
 Filename: shark_turbine/runtime/__init__.py
 Comment: 
 
 Filename: shark_turbine/runtime/device.py
 Comment: 
 
-Filename: shark_turbine/runtime/tracing.py
-Comment: 
-
 Filename: shark_turbine/runtime/op_reg/__init__.py
 Comment: 
 
 Filename: shark_turbine/runtime/op_reg/base.py
 Comment: 
 
 Filename: shark_turbine/runtime/op_reg/compiler.py
@@ -210,17 +207,14 @@
 
 Filename: shark_turbine/support/__init__.py
 Comment: 
 
 Filename: shark_turbine/support/conversions.py
 Comment: 
 
-Filename: shark_turbine/support/debugging.py
-Comment: 
-
 Filename: shark_turbine/support/exceptions.py
 Comment: 
 
 Filename: shark_turbine/support/ir_imports.py
 Comment: 
 
 Filename: shark_turbine/support/logging.py
@@ -240,26 +234,23 @@
 
 Filename: shark_turbine/transforms/general/rename_parameters.py
 Comment: 
 
 Filename: shark_turbine/transforms/quantization/mm_group_quant.py
 Comment: 
 
-Filename: iree_turbine-2.3.0.dist-info/LICENSE
-Comment: 
-
-Filename: iree_turbine-2.3.0.dist-info/METADATA
+Filename: iree_turbine-2.3.0rc20240410.dist-info/METADATA
 Comment: 
 
-Filename: iree_turbine-2.3.0.dist-info/WHEEL
+Filename: iree_turbine-2.3.0rc20240410.dist-info/WHEEL
 Comment: 
 
-Filename: iree_turbine-2.3.0.dist-info/entry_points.txt
+Filename: iree_turbine-2.3.0rc20240410.dist-info/entry_points.txt
 Comment: 
 
-Filename: iree_turbine-2.3.0.dist-info/top_level.txt
+Filename: iree_turbine-2.3.0rc20240410.dist-info/top_level.txt
 Comment: 
 
-Filename: iree_turbine-2.3.0.dist-info/RECORD
+Filename: iree_turbine-2.3.0rc20240410.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iree/turbine/__init__.py

```diff
@@ -1,12 +1,7 @@
-"""
-The turbine package provides development tools for deploying PyTorch 2 machine
-learning models to cloud and edge devices.
-"""
-
 # Copyright 2024 Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 # TODO: This redirection layer exists while we are migrating from the
```

## shark_turbine/aot/__init__.py

```diff
@@ -1,11 +1,7 @@
-"""
-Toolkit for ahead-of-time (AOT) compilation and export of PyTorch programs.
-"""
-
 # Copyright 2023 Nod Labs, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 from .builtins import *
```

## shark_turbine/aot/exporter.py

```diff
@@ -64,18 +64,14 @@
         self._importer_uses_session = importer_uses_session
 
     @property
     def mlir_module(self) -> Operation:
         """Gets the MLIR module resulting from the last compilation phase."""
         return CompiledModule.get_mlir_module(self.compiled_module)
 
-    def verify(self):
-        """Runs the verifier on the module, raising an exception on failure."""
-        self.mlir_module.verify()
-
     def print_readable(self, large_elements_limit: int = 50):
         """Prints a human readable version of the current compilation IR."""
         self.mlir_module.print(large_elements_limit=large_elements_limit)
 
     def save_mlir(self, file_path: Union[str, Path]):
         """Saves the current compilation IR to a path on disk.
 
@@ -282,18 +278,17 @@
             exported_program = exported_program.run_decompositions(current_decomps)
 
         TransformedModule = CompiledModule.create_from_dict(
             "LambdaCompiledModule",
             {(function_name or "main"): exported_program},
             export_name=module_name or "module",
         )
-    elif issubclass(mdl, CompiledModule):
-        TransformedModule = mdl
     else:
-        raise TypeError(f"mdl argument (type: {type(mdl)}) is not a supported type")
+        assert issubclass(type(mdl), CompiledModule)
+        TransformedModule = mdl
 
     session = Session()
     # There are some bugs with respect to Session/context interop that we
     # haven't squashed yet. For now, default everyone to round-tripping
     # via bytecode vs sharing the context between the importer/compiler.
     importer_uses_session = False and not _is_windows
     if importer_uses_session:
```

## shark_turbine/aot/params.py

```diff
@@ -2,19 +2,17 @@
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 from typing import Iterator, List, Optional, Set, Tuple, Union
 
-import json
+from dataclasses import dataclass
 from pathlib import Path
-import warnings
 
-import numpy as np
 import torch
 import torch.nn as nn
 
 from iree.runtime import (
     ParameterIndex,
     ParameterIndexEntry,
 )
@@ -24,15 +22,14 @@
 )
 
 
 __all__ = [
     "externalize_module_parameters",
     "save_module_parameters",
     "ParameterArchive",
-    "ParameterArchiveEntry",
     "ParameterArchiveBuilder",
 ]
 
 ################################################################################
 # Parameter externalization
 ################################################################################
 
@@ -46,84 +43,14 @@
         trait = ExternalTensorTrait(
             external_scope=external_scope, external_name=tensor_name
         )
         trait.set(tensor)
 
 
 ################################################################################
-# Metadata
-################################################################################
-
-_dtype_to_name: dict[torch.dtype, str] = {
-    torch.float32: "float32",
-    torch.float64: "float64",
-    torch.complex64: "complex64",
-    torch.complex128: "complex128",
-    torch.float16: "float16",
-    torch.bfloat16: "bfloat16",
-    torch.int8: "int8",
-    torch.int16: "int16",
-    torch.int32: "int32",
-    torch.int64: "int64",
-    torch.uint8: "uint8",
-    torch.bool: "bool",
-}
-
-
-# Deal with datatypes not yet added in all versions of Torch.
-def _add_optional_dtype(name: str):
-    try:
-        dtype = getattr(torch, name)
-    except AttributeError:
-        return
-    _dtype_to_name[dtype] = name
-
-
-_add_optional_dtype("float8_e4m3fn")
-_add_optional_dtype("float8_e4m3fnuz")
-_add_optional_dtype("float8_e5m2")
-_add_optional_dtype("float8_e5m2fnuz")
-_add_optional_dtype("uint16")
-_add_optional_dtype("uint32")
-_add_optional_dtype("uint64")
-
-
-_name_to_dtype: dict[str, torch.dtype] = {v: k for k, v in _dtype_to_name.items()}
-
-_metadata_prefix = "PYTORCH:"
-
-
-def _make_tensor_metadata(t: torch.Tensor) -> str:
-    """Makes a tensor metadata blob that can be used to reconstruct the tensor."""
-    dtype = t.dtype
-    try:
-        dtype_name = _dtype_to_name[dtype]
-    except KeyError:
-        dtype_name = "unknown"
-        warnings.warn(
-            f"Unknown dtype saving params: {dtype} (missing entry in params._dtype_to_name)"
-        )
-    dtype_desc = {
-        "class_name": type(dtype).__name__,
-        "is_complex": dtype.is_complex,
-        "is_floating_point": dtype.is_floating_point,
-        "is_signed": dtype.is_signed,
-        "itemsize": dtype.itemsize,
-    }
-    d = {
-        "type": "Tensor",
-        "dtype": dtype_name,
-        "shape": list(t.shape),
-        "dtype_desc": dtype_desc,
-    }
-    encoded = f"{_metadata_prefix}{json.dumps(d)}"
-    return encoded
-
-
-################################################################################
 # Parameter archives save/load
 ################################################################################
 
 
 def save_module_parameters(
     file_path: Union[str, Path], module: nn.Module, *, prefix: str = ""
 ):
@@ -132,99 +59,27 @@
     More options are available by using a ParameterArchiveBuilder.
     """
     builder = ParameterArchiveBuilder()
     builder.add_module(module, prefix=prefix)
     builder.save(file_path)
 
 
-class ParameterArchiveEntry:
-    """Wraps a raw ParameterIndexEntry with additional helpers."""
-
-    def __init__(self, raw: ParameterIndexEntry):
-        self.raw = raw
-
-    @property
-    def key(self) -> str:
-        return self.raw.key
-
-    def as_flat_tensor(self) -> torch.Tensor:
-        """Accesses the contents as a uint8 flat tensor.
-
-        If it is a splat, then the tensor will be a view of the splat pattern.
-
-        Raises a ValueError on unsupported entries.
-        """
-        if self.raw.is_file:
-            wrapper = np.array(self.raw.file_view, copy=False)
-        elif self.raw.is_splat:
-            wrapper = np.array(self.raw.splat_pattern, copy=True)
-        else:
-            raise ValueError(f"Unsupported ParameterIndexEntry: {self.raw}")
-
-        return torch.from_numpy(wrapper)
-
-    def as_tensor(self) -> torch.Tensor:
-        """Returns a tensor viewed with appropriate shape/dtype from metadata.
-
-        Raises a ValueError if unsupported.
-        """
-        # Decode metadata.
-        metadata = self.raw.metadata.decode()
-        if not metadata.startswith(_metadata_prefix):
-            raise ValueError(
-                f"No metadata for parameter entry {self.key}: Cannot convert to tensor"
-            )
-        metadata = metadata[len(_metadata_prefix) :]
-        d = json.loads(metadata)
-        try:
-            type_name = d["type"]
-            if d["type"] != "Tensor":
-                raise ValueError(
-                    f"Metadata for parameter entry {self.key} is not a Tensor ('{type_name}')"
-                )
-            dtype_name = d["dtype"]
-            shape = d["shape"]
-        except KeyError as e:
-            raise ValueError(f"Bad metadata for parameter entry {self.key}") from e
-
-        # Unpack/validate.
-        try:
-            dtype = _name_to_dtype[dtype_name]
-        except KeyError:
-            raise ValueError(f"Unknown dtype name '{dtype_name}'")
-        try:
-            shape = [int(d) for d in shape]
-        except ValueError as e:
-            raise ValueError(f"Illegal shape for parameter entry {self.key}") from e
-
-        t = self.as_flat_tensor()
-        return t.view(dtype=dtype).view(shape)
-
-    def __repr__(self):
-        return f"ParameterArchiveEntry({self.raw}, metadata={self.raw.metadata})"
-
-
 class ParameterArchive:
     """Allows access to a parameter archive as CPU tensors.
 
     TODO: Add more helpers for reading tensors once we get upstream versions that
     have that integrated.
     """
 
     def __init__(
-        self,
-        file_path: Optional[Union[str, Path]] = None,
-        *,
-        mmap: bool = True,
-        readable: bool = True,
-        writable: bool = False,
+        self, file_path: Optional[Union[str, Path]] = None, *, mmap: bool = True
     ):
         self._index = ParameterIndex()
         if file_path is not None:
-            self.load(file_path, mmap=mmap, readable=readable, writable=writable)
+            self.load(file_path, mmap=mmap)
 
     def load(
         self,
         file_path: Union[str, Path],
         *,
         mmap: bool = True,
         readable: bool = True,
@@ -235,20 +90,16 @@
             str(file_path), mmap=mmap, readable=readable, writable=writable
         )
 
     @property
     def index(self) -> ParameterIndex:
         return self._index
 
-    def items(self) -> List[Tuple[str, ParameterArchiveEntry]]:
-        """Returns the items in the archive.
-
-        Note that there can be duplicates if the archive was constructed that way.
-        """
-        return [(k, ParameterArchiveEntry(v)) for k, v in self._index.items()]
+    def items(self) -> List[Tuple[str, ParameterIndexEntry]]:
+        return self._index.items()
 
     def __repr__(self):
         return repr(self._index)
 
 
 class ParameterArchiveBuilder:
     """Helper for building parameter archives from live modules."""
@@ -258,30 +109,22 @@
 
     def save(self, file_path: Union[str, Path]):
         """Saves the archive."""
         self._index.create_archive_file(str(file_path))
 
     def add_tensor(self, name: str, tensor: torch.Tensor):
         """Adds an named tensor to the archive."""
-        flat_array = tensor.detach().flatten().contiguous().cpu().view(torch.uint8)
-        host_array = flat_array.numpy()
-        self._index.add_buffer(name, host_array, metadata=_make_tensor_metadata(tensor))
+        host_array = tensor.detach().cpu().contiguous().numpy()
+        self._index.add_buffer(name, host_array)
 
     def add_module(self, module: nn.Module, *, prefix: str = ""):
         """Adds all parameters and persistent buffers from a module hierarchy."""
         for name, t in _yield_saveable_tensors(module, prefix=prefix):
             self.add_tensor(name, t)
 
-    def add_blob(self, key: str, blob):
-        """Adds a raw blob to the index.
-
-        The blob must be interpretable as a buffer.
-        """
-        self._index.add_buffer(key, blob)
-
 
 def _yield_saveable_tensors(
     module: nn.Module, *, prefix: str = ""
 ) -> Iterator[Tuple[str, torch.Tensor]]:
     """Yields tuple of name/tensor for all saveable tensors in a module.
 
     This includes parameters and persistent buffers.
```

## shark_turbine/aot/builtins/__init__.py

```diff
@@ -32,10 +32,9 @@
     "AbstractIndex",
     "AbstractTensor",
     "IREE",
     "abstractify",
     "export_global",
     "export_global_tree",
     "export_parameters",
-    "export_buffers",
     "jittable",
 ]
```

## shark_turbine/aot/builtins/globals.py

```diff
@@ -25,22 +25,14 @@
 from torch.utils._pytree import (
     TreeSpec,
     tree_flatten,
     tree_map,
 )
 
 
-__all__ = [
-    "export_global",
-    "export_global_tree",
-    "export_parameters",
-    "export_buffers",
-]
-
-
 class export_global(GlobalsDef, Abstractifiable):
     """Exports a single global into a CompiledModule."""
 
     __slots__ = ["_name", "_value", "_schema"]
 
     def __init__(
         self,
@@ -168,68 +160,14 @@
         return self._tree[key]
 
     def __repr__(self):
         names = [name for name, _ in self._param_list]
         return f"<export_parameters {', '.join(names)}>"
 
 
-class export_buffers(GlobalsDef, TreeAbstractifiable):
-    """Exports buffers from an nn.Module.
-
-    These are exposed to procedural programs as a dictionary of param/values.
-    """
-
-    __slots__ = [
-        "_buffer_list",
-        "_schema",
-        "_tree",
-    ]
-
-    def __init__(
-        self,
-        nn_module: nn.Module,
-        *,
-        mutable: Optional[bool] = None,
-        external: Optional[bool] = None,
-        external_scope: Optional[str] = None,
-        name_mapper: Optional[NameMapCallback] = None,
-        uninitialized: Optional[bool] = None,
-        attrs: Optional[GlobalAttributes] = None,
-    ):
-        if attrs is None:
-            attrs = GlobalAttributes(
-                mutable=bool(mutable),
-                external=external,
-                external_scope=external_scope,
-                name_mapper=name_mapper,
-                uninitialized=uninitialized,
-            )
-        super().__init__(attrs)
-        self._buffer_list = list(nn_module.named_buffers())
-        self._tree = dict(self._buffer_list)
-        _, self._schema = tree_flatten(self._tree)
-
-    def items(self):
-        for name, value in self._buffer_list:
-            yield (name, value)
-
-    def schema(self) -> TreeSpec:
-        return self._schema
-
-    def abstractify_tree(self):
-        return tree_map(abstractify_single_value, self._tree)
-
-    def __getitem__(self, key):
-        return self._tree[key]
-
-    def __repr__(self):
-        names = [name for name, _ in self._param_list]
-        return f"<export_buffers {', '.join(names)}>"
-
-
 def _transform_tree_to_names(prefix: str, tree):
     """Produces a topologically similar tree but where each value is a fully qualified name."""
     join = lambda key: f"{prefix}.{key}" if prefix else key
     # No need to check for cycles as pytree already did something with it and
     # validates.
     if isinstance(tree, dict):
         return tree.__class__(
```

## shark_turbine/aot/builtins/jittable.py

```diff
@@ -222,15 +222,15 @@
             aten_graph=True,
             decomposition_table=self.decomposition_table,  # type: ignore
             assume_static_by_default=True,
             **export_kwargs,  # type: ignore
         )
         logger.debug("Invoking dynamo trace")
         gm, guards = exported_f(*flat_pytorch_args)
-        logger.debug("Dynamo trace complete")
+        logger.debug("Dyanmo trace complete")
 
         # TODO: Add debug logging for the exported graph module.
         # gm.print_readable()
 
         # We capture metadata about the results from the raw graph so that we can
         # pass it along in the trace (since the IREE type system is a partial erasure
         # of the PyTorch type system and we need the fidelity).
```

## shark_turbine/aot/support/ir_utils.py

```diff
@@ -21,15 +21,14 @@
 )
 
 from ...dynamo.type_conversion import (
     NativeTypeConverter,
 )
 
 from ...support.ir_imports import (
-    AsmState,
     Attribute,
     BF16Type,
     DenseElementsAttr,
     DenseResourceElementsAttr,
     F16Type,
     F32Type,
     F64Type,
@@ -152,32 +151,29 @@
     """Wrapper around module and IR accounting for a module being built."""
 
     __slots__ = [
         "body",
         "cache",
         "context",
         "fx_py_attr_tracker",
-        "last_global_op",
+        "global_ip",
         "ip",
         "module_op",
         "symbol_table",
         "global_ref_tracker",
         "native_type_converter",
         "_auto_symbol_counts",
     ]
 
     def __init__(self, module_op: Operation):
         self.module_op = module_op
         self.context = module_op.context
         self.body = module_op.regions[0].blocks[0]
         self.symbol_table = SymbolTable(module_op)
-        # We organize globals in order of declaration at the top of the module.
-        # To do so, record the last one emitted so that newly created ones
-        # can be ordered properly.
-        self.last_global_op: Optional[Operation] = None
+        self.global_ip = InsertionPoint.at_block_begin(self.body)
         self.ip = InsertionPoint(self.body)
         self.cache = ContextCache(self.context)
         # Tracks global references to a MaterializedGlobal.
         self.global_ref_tracker = RefTracker()
         # Usually the FxImporter makes a new ref tracker for each invocation,
         # but we want to preserve it across individual JIT evaluations so
         # as to better intern tensors to attributes.
@@ -197,15 +193,15 @@
         # TODO: Replace with a real dumping facility.
         # See: https://github.com/nod-ai/SHARK-Turbine/issues/136
         dump_path = Path(tempfile.gettempdir()) / "turbine_module_builder_error.mlir"
         logger.exception(f"{message} (dumping to {dump_path})")
         try:
             with open(dump_path, "wb") as f:
                 op.print(
-                    file=f,
+                    f,
                     binary=True,
                     print_generic_op_form=True,
                     large_elements_limit=100,
                 )
             logger.debug(f"Dump complete to {dump_path}")
         except Exception:
             logger.exception("Error generating dump file")
@@ -249,18 +245,15 @@
         *,
         attrs: GlobalAttributes,
         logical_name: Optional[str] = None,
     ) -> Tuple[str, Operation, IrType]:
         element_type = self.torch_dtype_to_iree_type(t.dtype)
         external, external_scope, external_name = attrs.infer_external_from_tensor(t)
 
-        # Always create globals at the top. Then after created, if there was
-        # a prior one, move the new one to after it to maintain declaration
-        # order.
-        with InsertionPoint.at_block_begin(self.body), Location.unknown():
+        with self.global_ip, Location.unknown():
             tensor_type = RankedTensorType.get(list(t.shape), element_type)
             ir_attrs = {
                 "sym_name": StringAttr.get(symbol_name),
                 "sym_visibility": StringAttr.get("private"),
                 "type": TypeAttr.get(tensor_type),
             }
             if attrs.noinline:
@@ -299,32 +292,26 @@
                 elements_attr = DenseResourceElementsAttr.get_from_buffer(
                     contents, blob_name, tensor_type
                 )
                 ir_attrs["initial_value"] = elements_attr
 
             global_op = Operation.create("util.global", attributes=ir_attrs)
             self.symbol_table.insert(global_op)
-            if self.last_global_op is not None:
-                global_op.move_after(self.last_global_op)
-            self.last_global_op = global_op
             actual_symbol_name = StringAttr(global_op.attributes["sym_name"]).value
             return actual_symbol_name, global_op, tensor_type
 
     def create_typed_global(
         self,
         symbol_name: str,
         global_type: IrType,
         *,
         attrs: GlobalAttributes,
         logical_name: Optional[str] = None,
     ) -> Tuple[str, Operation]:
-        # Always create globals at the top. Then after created, if there was
-        # a prior one, move the new one to after it to maintain declaration
-        # order.
-        with InsertionPoint.at_block_begin(self.body), Location.unknown():
+        with self.global_ip, Location.unknown():
             ir_attrs = {
                 "sym_name": StringAttr.get(symbol_name),
                 "sym_visibility": StringAttr.get("private"),
                 "type": TypeAttr.get(global_type),
             }
             if attrs.noinline:
                 ir_attrs["noinline"] = UnitAttr.get()
@@ -340,17 +327,14 @@
             else:
                 # Initialized by default.
                 ir_attrs["initial_value"] = self._create_initial_value_for_type(
                     global_type
                 )
             global_op = Operation.create("util.global", attributes=ir_attrs)
             self.symbol_table.insert(global_op)
-            if self.last_global_op is not None:
-                global_op.move_after(self.last_global_op)
-            self.last_global_op = global_op
             actual_symbol_name = StringAttr(global_op.attributes["sym_name"]).value
             return actual_symbol_name, global_op
 
     def _create_initial_value_for_type(self, t: IrType) -> Attribute:
         # TODO(#169): Implement something upstream for this (it exists in the C++ API)
         # and use it.
         if RankedTensorType.isinstance(t):
```

## shark_turbine/aot/support/procedural/exported_program.py

```diff
@@ -23,15 +23,14 @@
     # torch < 2.3 does not include this.
     treespec_pprint = lambda x: repr(x)  # type: ignore
 
 from iree.compiler.extras.fx_importer import (
     FxImporter,
     FxImporterHooks,
     GraphNodeImporter,
-    InputInfo,
 )
 
 from ....support.logging import aot_logger as logger
 
 from ....support.ir_imports import (
     func_d,
     util_d,
@@ -216,35 +215,14 @@
     )
 
 
 class _Hooks(FxImporterHooks):
     def __init__(self, module_builder: ModuleBuilder):
         self.module_builder = module_builder
 
-    def store_produced_value(
-        self,
-        gni: GraphNodeImporter,
-        py_value: Any,
-        produced_ir_value: Any,
-        info: InputInfo,
-    ):
-        module_builder = self.module_builder
-        # See if we know about it.
-        mapping = module_builder.global_ref_tracker.track(py_value)
-        if mapping.is_empty:
-            raise ValueError(f"Cannot store value to unmapped global for: {info}")
-        logger.debug("Resolved  global for store %r", mapping)
-        materialized_global: MaterializedGlobal = mapping.value  # type: ignore
-        converted_value = Operation.create(
-            "torch_c.to_builtin_tensor",
-            results=[materialized_global.ir_type],
-            operands=[produced_ir_value],
-        ).result
-        util_d.GlobalStoreOp(converted_value, materialized_global.symbol_name)
-
     def resolve_literal(self, gni: GraphNodeImporter, literal: Any) -> Optional[Value]:
         # We support resolution of tracked reference types. Currently this
         # only includes Tensors. All others we let the importer do what it
         # is going to do.
         if not isinstance(literal, torch.Tensor):
             return None
```

## shark_turbine/aot/support/procedural/globals.py

```diff
@@ -138,15 +138,18 @@
                     dtype=value.dtype,
                 )
                 logger.debug("TRACK NEW TENSOR(%s): %r", fq_name, mapping)
                 flat_globals.append(mapping.value)
                 continue
             elif isinstance(value, AbstractTensor):
                 global_type = value.get_ir_type(module_builder)
-                (actual_symbol_name, global_op,) = module_builder.create_typed_global(
+                (
+                    actual_symbol_name,
+                    global_op,
+                ) = module_builder.create_typed_global(
                     f"_{fq_name}",
                     global_type,
                     attrs=self._attrs,
                     logical_name=fq_name,
                 )
                 flat_globals.append(
                     IrGlobalTensor(
@@ -157,15 +160,18 @@
                         global_type=global_type,
                         dtype=value.dtype,
                     )
                 )
                 continue
             elif isinstance(value, AbstractScalar):
                 global_type = value.get_ir_type(module_builder)
-                (actual_symbol_name, global_op,) = module_builder.create_typed_global(
+                (
+                    actual_symbol_name,
+                    global_op,
+                ) = module_builder.create_typed_global(
                     f"_{fq_name}",
                     global_type,
                     attrs=self._attrs,
                     logical_name=fq_name,
                 )
                 flat_globals.append(
                     IrGlobalScalar(
```

## shark_turbine/dynamo/decompositions.py

```diff
@@ -111,14 +111,16 @@
         aten.nll_loss_forward,
         aten.nll_loss_backward,
         aten._to_copy,
         aten._log_softmax_backward_data,
         aten.lift_fresh_copy.default,
         aten._unsafe_index.Tensor,
         aten.unbind.int,
+        # decompositions added manually in this file
+        aten._scaled_dot_product_flash_attention.default,
     ]
 
 
 # Some older APIs still use an op list instead of a table.
 DEFAULT_DECOMPOSITIONS: DecompositionOpsList = _get_default_decomposition_ops()
 
 # The table of default decompositions.
```

## shark_turbine/dynamo/type_conversion.py

```diff
@@ -5,33 +5,31 @@
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Converters to/from torch types.
 
 Note that there are ad-hoc type conversions spread around a bit, and we
 should consolidate them here.
 """
-from typing import List, Optional
+from typing import List
 
 import functools
 import re
 
-from ..support.ir_imports import (
-    tensor_d,
+from iree.compiler.ir import (
     Context,
     F64Type,
     IntegerType,
     RankedTensorType,
     ShapedType,
-    IrType,
+    Type as IrType,
     Location,
     Operation,
     Value,
 )
 
-
 # Match an overall torch type declaration. Groups:
 #   1. Local name (int, float, vtensor)
 #   2. Parameter block ("<...>"), including the delimitters
 #   3. Inner parameter block (no delimitters)
 DECOMPOSE_TORCH_TYPE_PATTERN = re.compile(r"^!torch.([^<]+)(<([^>]*)>)?$")
 
 # Decomposes a vtensor parameter block into a dimension list and dtype. Groups:
@@ -101,23 +99,19 @@
         if signless:
             if IntegerType.isinstance(torch_type):
                 signed_int_type = IntegerType(torch_type)
                 return IntegerType.get_signless(signed_int_type.width)
         return torch_type
 
     def materialize_native_to_torch(
-        self, native_value: Value, torch_type: IrType, *, static_info_cast: bool = False
+        self, native_value: Value, torch_type: IrType
     ) -> Value:
         native_type = native_value.type
         if RankedTensorType.isinstance(native_type):
             # Convert to vtensor.
-            if static_info_cast:
-                required_native_type = self.torch_type_to_native(torch_type)
-                if required_native_type != native_type:
-                    native_value = tensor_d.cast(required_native_type, native_value)
             return Operation.create(
                 "torch_c.from_builtin_tensor",
                 results=[torch_type],
                 operands=[native_value],
             ).result
         elif IntegerType.isinstance(native_type):
             # Convert to !torch.int
@@ -140,31 +134,23 @@
                 "torch_c.from_f64", results=[torch_type], operands=[native_type]
             ).result
         else:
             raise TypeError(
                 f"Unsupported native->torch ABI type conversion: {native_type} -> {torch_type}"
             )
 
-    def materialize_torch_to_native(
-        self, torch_value: Value, *, static_info_cast_to: Optional[IrType] = None
-    ) -> Value:
+    def materialize_torch_to_native(self, torch_value: Value) -> Value:
         native_type = self.torch_type_to_native(torch_value.type)
         if RankedTensorType.isinstance(native_type):
             # Convert to vtensor.
-            builtin_tensor_value = Operation.create(
+            return Operation.create(
                 "torch_c.to_builtin_tensor",
                 results=[native_type],
                 operands=[torch_value],
             ).result
-            # Detect type difference and assume a static cast is needed.
-            if static_info_cast_to is not None and static_info_cast_to != native_type:
-                builtin_tensor_value = tensor_d.cast(
-                    static_info_cast_to, builtin_tensor_value
-                )
-            return builtin_tensor_value
         elif IntegerType.isinstance(native_type):
             # Convert to !torch.int
             int_type = IntegerType(native_type)
             width = int_type.width
             if width == 1:
                 op_name = "torch_c.to_i1"
             elif width == 64:
```

## shark_turbine/ops/iree.py

```diff
@@ -4,15 +4,14 @@
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Custom ops for built-in IREE functionality."""
 from typing import cast
 
 from ..support.ir_imports import (
-    Operation,
     RankedTensorType,
     StringAttr,
     Value,
     flow_d,
     tensor_d,
 )
 
@@ -57,28 +56,7 @@
         ksel.attr_str(0)
         ksel.arg_tensor(1, inplace_tied=True)
 
     def generate(self, ksel: KernelSelection, kb: KernelBuilder):
         key = cast(AttrArg, ksel.arg_descs[0])
         _emit_tensor_trace(kb, cast(str, key.v), [kb.arg_bindings[1]])
         kb.yield_results(kb.arg_bindings[1])
-
-
-@CustomOp.register(library=IREE_LIBRARY)
-class _test_add(CustomOp):
-    signature = "_test_add(Tensor t1, Tensor t2) -> (Tensor)"
-
-    def select(self, ksel: KernelSelection):
-        t1_desc = ksel.arg_tensor(0)
-        t1_desc.specialize_all_dims()
-        t2_desc = ksel.arg_tensor(1)
-        t2_desc.specialize_all_dims()
-        result_desc = ksel.return_new_tensor(list(t1_desc.t.shape), t1_desc.t.dtype)
-        result_desc.specialize_all_dims()
-
-    def generate(self, ksel: KernelSelection, kb: KernelBuilder):
-        t1, t2 = kb.arg_bindings
-        result_type = t1.type  # type: ignore
-        result = Operation.create(
-            "tosa.add", results=[result_type], operands=[t1, t2]
-        ).result
-        kb.yield_results(result)
```

## shark_turbine/runtime/device.py

```diff
@@ -3,15 +3,14 @@
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 from functools import lru_cache
 from typing import Callable, Optional, Union
 from threading import local, Lock
-import warnings
 
 import torch
 
 from iree.runtime import (
     BufferUsage,
     HalBufferView,
     HalDevice,
@@ -70,56 +69,26 @@
     standard named-access (not custom-constructed) drivers.
     """
 
     __slots__ = [
         "device",
         "driver",
         "instance",
-        "enumerated_info",
-        "torch_device",
-        "dlpack_device_type_code",
     ]
 
     def __init__(
         self,
         *,
         driver: Union[str, HalDriver],
         device: Optional[HalDevice] = None,
         vm_instance: Optional[VmInstance] = None,
-        enumerated_info: Optional[dict] = None,
-        torch_device: Optional[torch.device] = None,
-        dlpack_device_type_code: int = 0,
     ):
         self.instance = vm_instance or get_vm_instance()
         self.driver = driver if isinstance(driver, HalDriver) else get_driver(driver)
         self.device = device if device else self.driver.create_default_device()
-        self.enumerated_info = enumerated_info or {}
-        self.torch_device = torch_device
-        self.dlpack_device_type_code = dlpack_device_type_code
-
-    @property
-    def enumerated_device_id(self) -> int:
-        try:
-            return self.enumerated_info["device_id"]
-        except KeyError as e:
-            raise RuntimeError("No enumerated device_id for device") from e
-
-    @property
-    def enumerated_path(self) -> str:
-        try:
-            return self.enumerated_info["path"]
-        except KeyError as e:
-            raise RuntimeError("No enumerated path for device") from e
-
-    @property
-    def enumerated_name(self) -> str:
-        try:
-            return self.enumerated_info["name"]
-        except KeyError as e:
-            raise RuntimeError("No enumerated name for device") from e
 
     @staticmethod
     @lru_cache(maxsize=None)
     def from_uri(uri: str) -> "DeviceState":
         driver = get_driver(uri)
         return DeviceState(driver=driver, device=driver.create_device_by_uri(uri))
 
@@ -166,18 +135,15 @@
 
     # Compiler flags to use to target this device.
     # TODO: We should replace this with a target attribute but need an API
     # to derive that.
     compile_target_flags: tuple[str, ...]
 
     def __new__(
-        cls,
-        uri: Optional[str] = None,
-        *,
-        device_state: Optional[DeviceState] = None,
+        cls, uri: Optional[str] = None, *, device_state: Optional[DeviceState] = None
     ):
         if uri is not None:
             # Construction by URI is cached on the thread.
             assert not device_state, "device_state= cannot be given with explicit URI"
             try:
                 existing = _CURRENT_THREAD.device_by_uri[uri]
             except (AttributeError, KeyError):
@@ -273,35 +239,27 @@
             if _CURRENT_THREAD.stack[-1] is self:
                 _CURRENT_THREAD.stack.pop()
                 return
         except (AttributeError, IndexError):
             ...
         raise MismatchedDeviceSetClearError()
 
-    def dump_device_info(self) -> str:
-        return self._s.driver.dump_device_info(self._s.enumerated_device_id)
-
     def __repr__(self):
         return f"<Turbine Device: {self._s.device}>"
 
     def __enter__(self):
         try:
             _CURRENT_THREAD.stack.append(self)
         except AttributeError:
             _CURRENT_THREAD.stack = [self]
 
     def __exit__(self, type, value, traceback):
         _CURRENT_THREAD.stack.pop()
 
 
-################################################################################
-# CPU import/export
-################################################################################
-
-
 def _device_import_torch_tensor_cpu(device: Device, t: torch.Tensor) -> HalBufferView:
     hal_device = device.hal_device
     element_type = dtype_to_element_type(t.dtype)
     # TODO: In this case, we should be importing the raw buffer, but this is not
     # generically exposed to Python in the IREE runtime.
     bv = device.hal_device.allocator.allocate_buffer_copy(
         memory_type=MemoryType.DEVICE_LOCAL,
@@ -322,77 +280,29 @@
     mapped_memory = bv.map()
     shape = list(like.shape)
     np_dtype = torch_dtype_to_numpy(like.dtype)
     mapped_array = mapped_memory.asarray(shape, np_dtype)
     return torch.from_numpy(mapped_array)
 
 
-################################################################################
-# CUDA and HIP import/export
-################################################################################
-
-
-def _device_import_torch_tensor_cuda_hip(
-    device: Device, t: torch.Tensor
-) -> HalBufferView:
-    # We currently only support contiguous, so ensure that.
-    if not t.is_contiguous():
-        t = t.contiguous()
-    # TODO: The 'None' here tells the producer to synchronize on the default
-    # stream. For async, we should advance our timeline and signal when an
-    # event is raised on Torch's stream at the current position.
-    capsule = t.__dlpack__(None)
-    bv = device.hal_device.from_dlpack_capsule(capsule)
-    return bv
-
-
-def _device_export_torch_tensor_cuda_hip(
-    device: Device, bv: HalBufferView, like: torch.Tensor
-) -> torch.Tensor:
-    state = device._s
-    device_type_code = state.dlpack_device_type_code
-    assert device_type_code > 0
-    torch_device = state.torch_device
-    assert torch_device is not None
-    device_index = torch_device.index
-    t = torch.from_dlpack(
-        device.hal_device.create_dlpack_capsule(bv, device_type_code, device_index)
-    )
-    if t.dtype != like.dtype:
-        t = t.view(like.dtype)
-    # TODO: For async, we should enqueue an event on Torch's stream which will
-    # signal when this tensor is produced (i.e. at the current point in our
-    # timeline).
-    return t
-
-
 # Mapping of torch tensor importers keyed by driver name.
 TORCH_TENSOR_IMPORTERS: dict[str, Callable[[Device, torch.Tensor], HalBufferView]] = {
-    "cuda": _device_import_torch_tensor_cuda_hip,
-    "hip": _device_import_torch_tensor_cuda_hip,
     "local-sync": _device_import_torch_tensor_cpu,
     "local-task": _device_import_torch_tensor_cpu,
 }
 
 TORCH_TENSOR_EXPORTERS: dict[
     str, Callable[[Device, HalBufferView, torch.Tensor], torch.Tensor]
 ] = {
-    "cuda": _device_export_torch_tensor_cuda_hip,
-    "hip": _device_export_torch_tensor_cuda_hip,
     "local-sync": _device_export_torch_tensor_cpu,
     "local-task": _device_export_torch_tensor_cpu,
 }
 
 DEVICE_TARGET_COMPILE_FLAGS: dict[str, tuple[str, ...]] = {
-    "cuda": ("--iree-hal-target-backends=cuda",),
-    "hip": ("--iree-hal-target-backends=rocm",),
-    "local-task": (
-        "--iree-hal-target-backends=llvm-cpu",
-        "--iree-llvmcpu-target-cpu-features=host",
-    ),
+    "local-task": ("--iree-hal-target-backends=llvm-cpu",),
 }
 
 # Aliases.
 DEVICE_TARGET_COMPILE_FLAGS["local-sync"] = DEVICE_TARGET_COMPILE_FLAGS["local-task"]
 
 # Make sure all tables have the same keys.
 assert (
@@ -440,87 +350,22 @@
     if device is None:
         raise UnsupportedTorchDeviceError(torch_device)
     return device
 
 
 def _create_device_from_torch(torch_device: torch.device) -> Optional[Device]:
     torch_type = torch_device.type
+    uri = None
     if torch_type == "cpu":
-        cpu_driver = get_driver("local-task")
-        cpu_enumerated = cpu_driver.query_available_devices()
-        assert len(cpu_enumerated) >= 1
-        cpu_default = cpu_enumerated[0]
-        cpu_device_state = DeviceState(
-            driver=cpu_driver,
-            device=cpu_driver.create_default_device(),
-            enumerated_info=cpu_default,
-            torch_device=torch_device,
-            dlpack_device_type_code=1,
-        )
-        return Device(device_state=cpu_device_state)
-    elif torch_type == "cuda":
-        # Fork based on HIP or real CUDA.
-        props = torch.cuda.get_device_properties(torch_device)
-        if not hasattr(props, "gcnArchName"):
-            # Real CUDA.
-            return _create_cuda_device(torch_device, props)
-        else:
-            # HIP as CUDA.
-            return _create_hip_device(torch_device, props)
-
-    return None
-
-
-def _create_cuda_device(torch_device: torch.device, props) -> Optional[Device]:
-    # Note that the dlpack device type code for real CUDA ROCM is 2.
-    device = _create_cuda_like_device(torch_device, props, "hip", 2)
-    if device:
-        device.compile_target_flags = device.compile_target_flags + (
-            f"--iree-hal-cuda-llvm-target-arch=sm_{props.major}{props.minor}",
-        )
-    return device
+        uri = "local-task"
 
-
-def _create_hip_device(torch_device: torch.device, props) -> Optional[Device]:
-    # Note that the dlpack device type code for ROCM is 10.
-    device = _create_cuda_like_device(torch_device, props, "hip", 10)
-    if device:
-        gcn_arch_name = props.gcnArchName
-        device.compile_target_flags = device.compile_target_flags + (
-            f"--iree-rocm-target-chip={gcn_arch_name}",
-        )
-    return device
-
-
-def _create_cuda_like_device(
-    torch_device: torch.device, props, driver_name: str, dlpack_device_type_code: int
-) -> Optional[Device]:
-    if torch.cuda.device_count() > 1:
-        warnings.warn(
-            f"Multiple {driver_name} devices detected: Turbine does not yet "
-            f"guarantee stable device mapping"
-        )
-
-    requested_index = torch_device.index
-    driver = get_driver(driver_name)
-    available_infos = driver.query_available_devices()
-    if requested_index >= len(available_infos):
+    if uri is None:
         return None
-    device_info = available_infos[requested_index]
-    hal_device = driver.create_device(device_info)
-    device_state = DeviceState(
-        driver=driver,
-        device=hal_device,
-        vm_instance=get_vm_instance(),
-        enumerated_info=device_info,
-        torch_device=torch_device,
-        dlpack_device_type_code=dlpack_device_type_code,
-    )
-    device = Device(device_state=device_state)
-    return device
+
+    return Device(uri)
 
 
 ###############################################################################
 # Utilities
 ###############################################################################
 
 # The nanobind leak checker doesn't interop well with the way that
```

## shark_turbine/runtime/op_reg/base.py

```diff
@@ -4,17 +4,17 @@
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Base classes for registering custom operations with the PyTorch
 dispatcher.
 """
 
-from typing import Any, Callable, List, Optional, Sequence, Type, Union, cast
+from typing import Any, Callable, Optional, Sequence, Type, Union, cast
 
-from abc import ABC, abstractmethod
+from abc import ABC, abstractmethod, abstractproperty
 import functools
 import logging
 import re
 import textwrap
 import threading
 
 import torch
@@ -33,16 +33,14 @@
     IrType,
     Value,
     arith_d,
     builtin_d,
     func_d,
 )
 
-from ...support.logging import runtime_logger as logger
-
 from ...support.conversions import (
     TORCH_DTYPE_TO_IREE_TYPE_ASM,
 )
 
 __all__ = [
     "ArgDescriptor",
     "AttrArg",
@@ -51,14 +49,15 @@
     "IntArg",
     "KernelBuilder",
     "KernelSelection",
     "TensorArg",
     "def_library",
 ]
 
+logger = logging.getLogger("turbine.runtime.op_reg")
 
 ###############################################################################
 # Op library management
 ###############################################################################
 
 _CONFIG_LOCK = threading.Lock()
 
@@ -70,18 +69,19 @@
     the library is registered with the compiler in such a way that it can
     operate over all known custom ops.
     """
     return torch.library.Library(ns, "DEF")
 
 
 def default_dispatch_keys() -> list[str]:
-    keys = ["CPU"]
-    if torch.cuda.is_available():
-        keys.append("CUDA")
-    return keys
+    # TODO: Dynamically determine what devices to register against.
+    # Note that we have to register against specific keys instead of the
+    # fallback, as fallback is too broad and breaks certain elements of
+    # fx tracing.
+    return ["CPU"]
 
 
 # All such custom kernels are registered in the 'turbine' library/namespace.
 # We also allow extending existing libraries outside of this, but that is
 # the non default case.
 TURBINE_LIBRARY = def_library("turbine")
 
@@ -163,16 +163,15 @@
                 dispatch_key = [dispatch_key]
             for k in dispatch_key:
                 library.impl(name, _create_impl_trampoline(self), k)
 
         fq_name = f"{library.ns}.{name}"
         ALL_CUSTOM_OP_REGS[fq_name] = self
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def signature(self) -> str:
         """PyTorch function signature.
 
         This is in the normal PyTorch kernel registration form. For example:
 
         ```
         my_op(Tensor t) -> Tensor
@@ -345,22 +344,14 @@
 
         By default, it will be rank and dtype specialized but have completely dynamic
         dimensions. Dimensions can be further constrained by modifying the returned
         descriptor.
         """
         ...
 
-    def return_new_tensor(self, size: list, dtype: torch.dtype) -> "TensorArg":
-        """Constructs a new symbolic tensor and marks the next result as returning it.
-
-        This delegates to `return_tensor` but takes care of some easy to mess
-        up boiler plate for dynamic shapes.
-        """
-        return self.return_tensor(torch.empty(size, dtype=dtype, device="meta"))
-
 
 class EagerKernelSelection(KernelSelection):
     """Kernel selection specialized for eager arguments."""
 
     __slots__ = [
         "args",
     ]
@@ -481,49 +472,34 @@
     @property
     def mlir_type_asm(self) -> str:
         # TODO: We can have individual kernels constrain this to a narrower
         # type.
         return "i64"
 
 
-_NoneInt: Optional[int] = None
-
-
 class TensorArg:
     __slots__ = [
         "t",
         "spec_dims",
         "maybe_tensor_value",
     ]
 
     ir_arity: int = 1
     is_list: bool = False
 
     def __init__(self, t: Tensor):
         self.t = t
         # Any static dims that we are specializing. Defaults to all dynamic.
-        self.spec_dims = len(t.shape) * [_NoneInt]
+        self.spec_dims: Sequence[Optional[int]] = len(t.shape) * [None]
         # All descriptors have an attribute to indicate their value
         # as a tensor, and those that aren't are fixated to None.
         # This is to enable fast lookup in the hot path of determining
         # how to dispatch.
         self.maybe_tensor_value: Tensor = t
 
-    def specialize_all_dims(self):
-        """Marks all dimensions as specialized."""
-        self.spec_dims = list(self.t.shape)
-
-    def specialize_dims(self, *indices: int):
-        """Specializes individual dimensions.
-
-        `i` can have negative indexing.
-        """
-        for i in indices:
-            self.spec_dims[i] = self.t.size(i)
-
     def __repr__(self):
         return (
             f"TensorArg(shape={self.t.shape}, dtype={self.t.dtype}, "
             f"spec_dims={self.spec_dims})"
         )
 
     def generate_meta(self) -> Tensor:
@@ -636,15 +612,14 @@
         module_body: Block,
         symbol_table: SymbolTable,
     ):
         self.ksel = ksel
         self.arg_bindings = arg_bindings
         self.ip = ip
         self.module_body = module_body
-        self.context = module_body.owner.context
         self.symbol_table = symbol_table
         self.yielded = False
 
     def arg_value(self, index: int) -> Union[list[Value], Value]:
         """Gets the concrete IR `Value` for the argument at `index`.
 
         This will assert if the corresponding argument was set as `ir_arity=0`
```

## shark_turbine/runtime/op_reg/compiler.py

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 from dataclasses import dataclass
 from timeit import default_timer
-from typing import Any, Optional
+from typing import Any
 
 from iree.compiler.api import (
     Session,
     Source,
     Output,
 )
 
@@ -32,16 +32,14 @@
     runtime_logger as logger,
 )
 
 from ..device import (
     Device,
 )
 
-from ..tracing import tracer
-
 from .base import (
     FreeFuncKernelBuilder,
     KernelSelection,
 )
 
 
 @dataclass(slots=True)
@@ -67,18 +65,14 @@
     # NYI.
     layout_specialized: bool = False
 
     # Arbitrary objects to keep alive as part of this config. This can include
     # things like unbacked memory mappings, etc.
     keep_alive: Any = None
 
-    # If tracing is enabled, this may contain a sanitized key that can be
-    # used to log additional information against the kernel.
-    tracing_key: Optional[str] = None
-
 
 # TODO: The cache should be more than just a simple dict. Can be persistent
 KERNEL_CACHE: dict[str, tuple[VmContext, VmFunction, KernelCompileConfig]] = {}
 
 
 def _testing_get_cache_size() -> int:
     return len(KERNEL_CACHE)
@@ -96,18 +90,16 @@
     # Cache miss.
     start = default_timer()
     config = KernelCompileConfig(cache_key, list(device.compile_target_flags))
     kb = FreeFuncKernelBuilder.create_module(ksel, func_name=func_name)
     with kb.ip, Location.unknown():
         ksel.op.generate(ksel, kb)
     kb.module_op.verify()
-    # DO NOT SUBMIT: https://github.com/iree-org/iree/issues/17132
-    enable_debug_info = False
     module_asm = kb.module_op.get_asm(
-        binary=True, enable_debug_info=enable_debug_info, print_generic_op_form=False
+        binary=True, enable_debug_info=True, print_generic_op_form=True
     )
     generation_time = default_timer() - start
 
     if not config.in_process:
         raise NotImplementedError("Out-of-process compilation not yet supported")
 
     # TODO: We could be caching the session per device type key.
@@ -133,27 +125,18 @@
     vm_module = VmModule.copy_buffer(vm_instance, mapped_memory)
     # TODO: We should be able to wrap the buffer as below but there are some
     # subtle ref-counting/shutdown sequencing issues that need to be resolved.
     # vm_module = VmModule.wrap_buffer(vm_instance, mapped_memory)
     vm_context = VmContext(vm_instance, [device.create_hal_module(), vm_module])
     main_function = vm_module.lookup_function("main")
 
-    if tracer.enabled:
-        config.tracing_key = tracer.save_jit_kernel_artifacts(
-            cache_key=cache_key, module_asm=module_asm, binary=mapped_memory
-        )
-        tracer.log_structured(
-            tag="COMPILE",
-            msg=f"Compiled kernel {config.tracing_key}, cache_key={cache_key}",
-            columns=[
-                config.tracing_key,
-                main_function.name,
-                len(module_asm),
-                len(mapped_memory),
-                generation_time * 1000,
-                compilation_time * 1000,
-                " ".join(session.get_flags(non_default_only=True)),
-            ],
-        )
+    logger.debug(
+        "Compiled kernel %s: mlir=%d bytes, vmfb=%d bytes (generation: %sms, compilation: %sms)",
+        cache_key,
+        len(module_asm),
+        len(mapped_memory),
+        generation_time * 1000,
+        compilation_time * 1000,
+    )
     cache_hit = (vm_context, main_function, config)
     KERNEL_CACHE[cache_key] = cache_hit
     return cache_hit
```

## shark_turbine/runtime/op_reg/eager.py

```diff
@@ -9,16 +9,14 @@
 from timeit import default_timer
 from typing import Optional
 
 import torch
 
 from iree.runtime import (
     HalBufferView,
-    HalElementType,
-    VmRef,
     VmVariantList,
 )
 
 from ...support.exceptions import (
     UnsupportedTypeError,
 )
 
@@ -27,25 +25,22 @@
 )
 
 from ..device import (
     Device,
     lookup_device_from_torch,
 )
 
-from ..tracing import tracer
-
 from .base import (
     AttrArg,
     IntArg,
     KernelSelection,
 )
 
 from .compiler import (
     compile_standalone_kernel,
-    KernelCompileConfig,
 )
 
 __all__ = [
     "eager_dispatch",
 ]
 
 
@@ -154,16 +149,15 @@
         raise NotImplementedError("Async execution not yet implemented")
 
     # Invoke.
     ret_list = VmVariantList(len(ksel.result_descs))
     start = default_timer()
     vm_context.invoke(vm_f, arg_list, ret_list)
     invoke_time = default_timer() - start
-    if tracer.enabled:
-        _log_eager_dispatch(config, arg_list, invoke_time * 1000)
+    logger.debug("Kernel invocation %s: %sms", config.key, invoke_time * 1000)
 
     # Unpack results.
     results = []
     for i, result_desc in enumerate(ksel.result_descs):
         arity = result_desc.ir_arity
         meta_tensor_value = result_desc.maybe_tensor_value
         if meta_tensor_value is None:
@@ -181,66 +175,7 @@
 
     if len(results) == 1:
         return results[0]
     elif len(results) == 0:
         return None
     else:
         return tuple(results)
-
-
-def _log_eager_dispatch(
-    config: KernelCompileConfig, arg_list: VmVariantList, invoke_time_millis: float
-):
-    args = []
-    try:
-        for i in range(arg_list.size):
-            variant = arg_list.get_variant(i)
-            if isinstance(variant, VmRef):
-                if variant.isinstance(HalBufferView):
-                    args.append(_log_format_buffer_view(variant.deref(HalBufferView)))
-                    continue
-            args.append(variant)
-    except:
-        tracer.exception("Exception while pretty-printing arguments")
-
-    msg = ""
-    tracer.log_structured(
-        tag="INVOKE_KERNEL",
-        msg=msg,
-        columns=[config.tracing_key, invoke_time_millis] + args,
-    )
-
-
-def _log_format_buffer_view(bv: HalBufferView) -> str:
-    # TODO: We should expose this as a method on HalBufferView upstream instead
-    # of half doing it here.
-    shape = "x".join(str(i) for i in bv.shape)
-    dtype_desc = _LOG_HAL_ELEMENT_TYPE_DESC.get(bv.element_type)
-    if dtype_desc is None:
-        dtype_desc = f"<{bv.element_type}>"
-    return f"{shape}x{dtype_desc}"
-
-
-_LOG_HAL_ELEMENT_TYPE_DESC = {
-    HalElementType.BFLOAT_16: "bf16",
-    HalElementType.BOOL_8: "i1",
-    HalElementType.COMPLEX_64: "cf64",
-    HalElementType.COMPLEX_128: "cf128",
-    HalElementType.FLOAT_16: "f16",
-    HalElementType.FLOAT_32: "f32",
-    HalElementType.FLOAT_64: "f64",
-    HalElementType.INT_4: "i4",
-    HalElementType.INT_8: "i8",
-    HalElementType.INT_16: "i16",
-    HalElementType.INT_32: "i32",
-    HalElementType.INT_64: "i64",
-    HalElementType.SINT_4: "si4",
-    HalElementType.SINT_8: "si8",
-    HalElementType.SINT_16: "si16",
-    HalElementType.SINT_32: "si32",
-    HalElementType.SINT_64: "si64",
-    HalElementType.UINT_4: "ui4",
-    HalElementType.UINT_8: "ui8",
-    HalElementType.UINT_16: "ui16",
-    HalElementType.UINT_32: "ui32",
-    HalElementType.UINT_64: "ui64",
-}
```

## shark_turbine/support/__init__.py

```diff
@@ -1,9 +1,7 @@
 # Copyright 2023 Nod Labs, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-# Debugging must be loaded first as other low level things depend on it.
-from .debugging import *
 from .exceptions import *
```

## shark_turbine/support/ir_imports.py

```diff
@@ -4,15 +4,14 @@
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Unifies all imports of iree.compiler.ir into one place."""
 
 from iree.compiler.ir import (
-    AsmState,
     Attribute,
     Block,
     BlockArgument,
     Context,
     DenseElementsAttr,
     DenseResourceElementsAttr,
     FlatSymbolRefAttr,
```

## shark_turbine/support/logging.py

```diff
@@ -1,45 +1,10 @@
 # Copyright 2023 Advanced Micro Devices, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 import logging
-import sys
 
-from .debugging import flags
-
-
-class DefaultFormatter(logging.Formatter):
-    def __init__(self):
-        super().__init__(
-            "%(levelname)s %(asctime)s [%(filename)s:%(lineno)d] %(message)s",
-            "%m-%d %H:%M:%S",
-        )
-
-
-def _setup_logger():
-    root_logger = logging.getLogger("turbine")
-    root_logger.setLevel(flags.log_level)
-    default_handler = logging.StreamHandler(sys.stderr)
-    default_handler.flush = sys.stderr.flush
-    default_handler.setLevel(flags.log_level)
-    default_handler.setFormatter(DefaultFormatter())
-    root_logger.addHandler(default_handler)
-    root_logger.propagate = False
-    return root_logger, default_handler
-
-
-root_logger, default_handler = _setup_logger()
-
-
-def get_logger(name: str):
-    logger = logging.getLogger(name)
-    logger.setLevel(flags.log_level)
-    logger.addHandler(default_handler)
-    logger.propagate = False
-    return logger
-
-
-aot_logger = get_logger("turbine.aot")
-runtime_logger = get_logger("turbine.runtime")
+aot_logger = logging.getLogger("shark_turbine.aot")
+runtime_logger = logging.getLogger("shark_turbine.runtime")
```

## shark_turbine/transforms/merger.py

```diff
@@ -75,29 +75,24 @@
 
     def __init__(
         self,
         source_module: Operation,
         target_module: Operation,
         *,
         user_rename_map: Optional[Dict[str, str]] = None,
-        target_symbol_table: Optional[SymbolTable] = None,
         _logger=None,
     ):
         self._context = source_module.context
         self.source_module = source_module
         self.target_module = target_module
         self._target_body = self.target_module.regions[0].blocks[0]
         self.user_rename_map = user_rename_map if user_rename_map is not None else {}
         self._logger = _logger if _logger else null_logger
         self._source_symbol_table = SymbolTable(self.source_module)
-        self._target_symbol_table = (
-            target_symbol_table
-            if target_symbol_table is not None
-            else SymbolTable(self.target_module)
-        )
+        self._target_symbol_table = SymbolTable(self.target_module)
         self._rename_map: Dict[StringAttr, StringAttr] = {}
 
         self._nested_symbol_ops: List[Operation] = []
         self._nested_symbol_table_ops: List[Operation] = []
         self._top_ip = InsertionPoint.at_block_begin(self._target_body)
 
         # Map of value attributes to global operation.
@@ -141,15 +136,15 @@
         sources = get_top_level_ops(self.source_module, "hal.executable.source")
         for source in sources:
             source.detach_from_parent()
             self._nested_symbol_table_ops.append(source)
             self._target_body.append(source)
 
         # Merge functions.
-        funcs = get_top_level_ops(self.source_module, "func.func", "util.func")
+        funcs = get_top_level_ops(self.source_module, "func.func")
         for func_op in funcs:
             self._import_symbol_op(func_op)
             self._nested_symbol_table_ops.append(func_op)
 
         self._logger(f"The following symbol renames will be made: {self._rename_map}")
 
         # Go back through to nested symbol table ops and RAUW.
```

## shark_turbine/transforms/general/custom_op_expansion.py

```diff
@@ -1,19 +1,15 @@
 # Copyright 2023 Advanced Micro Devices, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from typing import Callable
-
 import torch
 from torch import Tensor
-from torch._subclasses.fake_tensor import FakeTensorMode
-from torch.fx.experimental.symbolic_shapes import ShapeEnv
 
 from ...dynamo.type_conversion import (
     NativeTypeConverter,
 )
 
 from ...runtime.op_reg.base import (
     ALL_CUSTOM_OP_REGS,
@@ -28,15 +24,14 @@
 
 from ...support.conversions import (
     MLIR_TYPE_ASM_TO_TORCH_DTYPE,
 )
 
 from ...support.ir_imports import (
     Block,
-    IrType,
     InsertionPoint,
     OpResult,
     Operation,
     RankedTensorType,
     StringAttr,
     SymbolTable,
     Value,
@@ -53,16 +48,14 @@
     ):
         super().__init__(root_op)
         self.reg = reg
         # Track pending deletions in a dict to preserve order and unique.
         self.ops_to_delete: dict[Operation, None] = {}
         self.type_converter = NativeTypeConverter(root_op.context)
         self.symbol_table = SymbolTable(root_op)
-        self.shape_env = ShapeEnv()
-        self.fake_mode = FakeTensorMode(shape_env=self.shape_env)
 
     def delete_op(self, op):
         self.ops_to_delete[op.operation] = None
 
     def run(self):
         for mr in self.funcs:
             self.expand_func(mr.op)
@@ -89,23 +82,17 @@
                         custom_op_reg = self.reg.get(local_name)
                         if custom_op_reg is not None:
                             self.expand_custom_op(custom_op_reg, op)
 
     def expand_custom_op(self, op_reg: CustomOp, op: Operation):
         original_operands: list[Value] = list(op.operands)
         ksel = AOTKernelSelection(
-            op_reg,
-            original_operands,
-            list(op.results),
-            self.type_converter,
-            self.shape_env,
+            op_reg, original_operands, list(op.results), self.type_converter
         )
-        with self.fake_mode:
-            op_reg.select(ksel)
-        ksel._run_validators()
+        op_reg.select(ksel)
 
         module_body = self.root_op.regions[0].blocks[0]
         kb = InlineKernelBuilder(
             ksel,
             op,
             type_converter=self.type_converter,
             module_body=module_body,
@@ -119,95 +106,60 @@
 
 
 class AOTKernelSelection(KernelSelection):
     __slots__ = [
         "operands",
         "results",
         "type_converter",
-        "shape_env",
-        "_validators",
     ]
 
     def __init__(
         self,
         op: CustomOp,
         operands: list[Value],
         results: list[Value],
         type_converter: NativeTypeConverter,
-        shape_env: ShapeEnv,
     ):
         super().__init__(op, len(operands))
         self.operands = operands
         self.results = results
         self.type_converter = type_converter
-        self.shape_env = shape_env
-        self._validators: list[Callable] = []
-
-    def _run_validators(self):
-        for v in self._validators:
-            v()
 
     def arg_tensor(self, arg: int, *, inplace_tied: bool = False) -> TensorArg:
         # This is annoying: We have to go from the Torch MLIR type system to the
         # original torch.tensor Python type system. We do this by way of the native
         # type converter because it has the mapping pathway we need. This is one of the
         # only places in the code where we have to go this way to preserve the facade.
         # Everywhere else is going from Torch -> IREE native.
         arg_descs = self.arg_descs
         assert arg_descs[arg] is None, f"Already constrained argument {arg}"
         operand = self.operands[arg]
-        signed_native_type = self.type_converter.torch_type_to_native(
-            operand.type, signless=False
-        )
+        signed_native_type = self.type_converter.torch_type_to_native(operand.type)
         try:
             rtt = RankedTensorType(signed_native_type)
+            # TODO: We need to do the FakeMode/ShapeEnv dance to create a symbolic
+            # fake tensor here.
         except TypeError as e:
             raise TypeError(
                 f"Argument type mismatch from Torch IR for arg {arg}: Expected ranked tensor, got {signed_native_type}"
             ) from e
+        assert not any(
+            rtt.is_dynamic_dim(i) for i in range(rtt.rank)
+        ), "NYI: Dynamic shape tensors in custom op AOT mode"
         element_type_asm = str(rtt.element_type)
         try:
             dtype = MLIR_TYPE_ASM_TO_TORCH_DTYPE[element_type_asm]
         except KeyError as e:
             raise AssertionError(
                 f"Could not find dtype mapping for {element_type_asm} in MLIR_TYPE_ASM_TO_TORCH_DTYPE"
             )
-
-        # Because we are operating in fake_mode, replace MLIR dyn dims with
-        # symints for the PyTorch type system.
-        shape_env = self.shape_env
-        sym_shape = [
-            d if d >= 0 else shape_env.create_unbacked_symint() for d in rtt.shape
-        ]
-        t = torch.empty(sym_shape, dtype=dtype)
+        t = torch.empty(rtt.shape, dtype=dtype, device="meta")
         arg_descs[arg] = desc = TensorArg(t)
         if inplace_tied:
             self.inplace_tied_arg_descs.append(desc)
-
-        def validator():
-            rank = rtt.rank
-            for i in range(rank):
-                spec_dim = desc.spec_dims[i]
-                if rtt.is_dynamic_dim(i):
-                    # Make sure that it wasn't specialized.
-                    if spec_dim is not None:
-                        raise ValueError(
-                            f"Custom op {self.op}, arg {arg} requires a static dim "
-                            f"at index {i} but it is dynamic: {rtt}"
-                        )
-                else:
-                    # Make sure specialized dim matches.
-                    actual_dim = rtt.get_dim_size(i)
-                    if spec_dim is not None and actual_dim != spec_dim:
-                        raise ValueError(
-                            f"Custom op {self.op}, arg {arg} has a mismatched static "
-                            f"dim at index {i}: actual = {actual_dim}, expected = {spec_dim}"
-                        )
-
-        self._validators.append(validator)
         return desc
 
     def arg_tensor_list(self, arg: int) -> TensorListArg:
         raise NotImplementedError("NYI: AOT arg_tensor_list")
 
     def arg_int(self, arg: int) -> IntArg:
         raise NotImplementedError("NYI: AOT arg_int")
@@ -259,18 +211,15 @@
             arg_bindings = []
             for desc, operand in zip(ksel.arg_descs, operands):
                 assert desc is not None, "NYI: None arguments"
                 arity = desc.ir_arity
                 if not desc.is_list:
                     if arity == 1:
                         arg_bindings.append(
-                            type_converter.materialize_torch_to_native(
-                                operand,
-                                static_info_cast_to=IrType.parse(desc.mlir_type_asm),
-                            )
+                            type_converter.materialize_torch_to_native(operand)
                         )
                     else:
                         arg_bindings.append(None)
                 else:
                     # arg_bindings.extend(native_operands)
                     raise NotImplementedError("NYI: AOT custom op list arguments")
 
@@ -297,13 +246,11 @@
             torch_op_results: list[Value] = list(self.torch_op.results)
             assert len(results) == len(
                 torch_op_results
             ), f"Mismatched yield_results with custom op results"
             for new_result, old_result in zip(results, torch_op_results):
                 torch_type = old_result.type
                 new_result = self.type_converter.materialize_native_to_torch(
-                    new_result,
-                    torch_type,
-                    static_info_cast=True,
+                    new_result, torch_type
                 )
                 old_result.replace_all_uses_with(new_result)
         self.yielded = True
```

## shark_turbine/transforms/quantization/mm_group_quant.py

```diff
@@ -71,32 +71,32 @@
 GROUP_MATMUL_TEMPLATE = r"""
 module {{
   util.global private @{param_name} {{noinline}} = #stream.parameter.named<"model"::"{param_name}"> : tensor<{k}x{n_div}xi8>
   util.global private @{param_name}.quant.scale {{noinline}} = #stream.parameter.named<"model"::"{param_name}_scale"> : tensor<{k}x{group0}x{element_type}>
   util.global private @{param_name}.quant.zero_point {{noinline}} = #stream.parameter.named<"model"::"{param_name}_zp"> : tensor<{k}x{group0}x{element_type}>
 
   func.func private @compute_mm_group_quant(%a : tensor<{m}x{n}x{element_type}>) -> tensor<{m}x{k}x{element_type}> {{
-    %c0 = arith.constant 0 : index
+    %c0 = arith.constant 0 : index        
     %weight_raw = util.global.load @{param_name} : tensor<{k}x{n_div}xi8>
     %m = tensor.dim %a, %c0 : tensor<{m}x{n}x{element_type}>
     %k = tensor.dim %weight_raw, %c0 : tensor<{k}x{n_div}xi8>
     %scale = util.global.load @{param_name}.quant.scale : tensor<{k}x{group0}x{element_type}>
     %zp = util.global.load @{param_name}.quant.zero_point : tensor<{k}x{group0}x{element_type}>
     %weight = flow.tensor.bitcast %weight_raw : tensor<{k}x{n_div}xi8> -> tensor<{k}x{n}x{lowp_type}>
     %a_exp = tensor.expand_shape %a [[0], [1, 2]] : tensor<{m}x{n}x{element_type}> into tensor<{m}x{group0}x{group1}x{element_type}>
     %weight_exp = tensor.expand_shape %weight [[0], [1, 2]] : tensor<{k}x{n}x{lowp_type}> into tensor<{k}x{group0}x{group1}x{lowp_type}>
     %empty_0 = tensor.empty() : tensor<{k}x{group0}x{group1}x{element_type}>
     %weight_cast = linalg.generic {{
         indexing_maps = [
-            affine_map<(d0, d1, d2) -> (d0, d1, d2)>,
-            affine_map<(d0, d1, d2) -> (d0, d1)>,
-            affine_map<(d0, d1, d2) -> (d0, d1)>,
-            affine_map<(d0, d1, d2) -> (d0, d1, d2)>],
-        iterator_types = ["parallel", "parallel", "parallel"] }}
-        ins(%weight_exp, %scale, %zp : tensor<{k}x{group0}x{group1}x{lowp_type}>, tensor<{k}x{group0}x{element_type}>, tensor<{k}x{group0}x{element_type}>)
+            affine_map<(d0, d1, d2) -> (d0, d1, d2)>, 
+            affine_map<(d0, d1, d2) -> (d0, d1)>, 
+            affine_map<(d0, d1, d2) -> (d0, d1)>, 
+            affine_map<(d0, d1, d2) -> (d0, d1, d2)>], 
+        iterator_types = ["parallel", "parallel", "parallel"] }} 
+        ins(%weight_exp, %scale, %zp : tensor<{k}x{group0}x{group1}x{lowp_type}>, tensor<{k}x{group0}x{element_type}>, tensor<{k}x{group0}x{element_type}>) 
         outs(%empty_0 : tensor<{k}x{group0}x{group1}x{element_type}>) {{
     ^bb0(%in: {lowp_type}, %in_1: {element_type}, %in_2: {element_type}, %out: {element_type}):
         %16 = arith.extui %in : {lowp_type} to i32
         %17 = arith.uitofp %16 : i32 to {element_type}
         %18 = arith.subf %17, %in_2 : {element_type}
         %19 = arith.mulf %18, %in_1 : {element_type}
         linalg.yield %19 : {element_type}
@@ -104,18 +104,18 @@
     %cst = arith.constant 0.000000e+00 : {element_type}
     %empty_1_dyn = tensor.empty(%m, %k) : tensor<?x?x{element_type}>
     %empty_1 = tensor.cast %empty_1_dyn : tensor<?x?x{element_type}> to tensor<{m}x{k}x{element_type}>
     %zero_init = linalg.fill ins(%cst : {element_type}) outs(%empty_1 : tensor<{m}x{k}x{element_type}>) -> tensor<{m}x{k}x{element_type}>
     %result = linalg.generic {{
         indexing_maps = [
             affine_map<(d0, d1, d2, d3) -> (d0, d2, d3)>,
-            affine_map<(d0, d1, d2, d3) -> (d1, d2, d3)>,
-            affine_map<(d0, d1, d2, d3) -> (d0, d1)>],
-        iterator_types = ["parallel", "parallel", "reduction", "reduction"] }}
-        ins(%a_exp, %weight_cast : tensor<{m}x{group0}x{group1}x{element_type}>, tensor<{k}x{group0}x{group1}x{element_type}>)
+            affine_map<(d0, d1, d2, d3) -> (d1, d2, d3)>, 
+            affine_map<(d0, d1, d2, d3) -> (d0, d1)>], 
+        iterator_types = ["parallel", "parallel", "reduction", "reduction"] }} 
+        ins(%a_exp, %weight_cast : tensor<{m}x{group0}x{group1}x{element_type}>, tensor<{k}x{group0}x{group1}x{element_type}>) 
         outs(%zero_init : tensor<{m}x{k}x{element_type}>) {{
     ^bb0(%in: {element_type}, %in_1: {element_type}, %out: {element_type}):
         %16 = arith.mulf %in, %in_1 : {element_type}
         %17 = arith.addf %16, %out : {element_type}
         linalg.yield %17 : {element_type}
     }} -> tensor<{m}x{k}x{element_type}>
     return %result : tensor<{m}x{k}x{element_type}>
```

## Comparing `iree_turbine-2.3.0.dist-info/METADATA` & `iree_turbine-2.3.0rc20240410.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,150 @@
 Metadata-Version: 2.1
 Name: iree-turbine
-Version: 2.3.0
+Version: 2.3.0rc20240410
 Summary: SHARK Turbine Machine Learning Deployment Tools
 Home-page: https://github.com/nod-ai/SHARK-Turbine
 Author: SHARK Authors
 Author-email: stella@nod.ai
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy >=1.26.3
-Requires-Dist: iree-compiler
-Requires-Dist: iree-runtime
-Requires-Dist: torch >=2.3.0
+Requires-Dist: numpy
+Requires-Dist: iree-compiler >=20240410.859
+Requires-Dist: iree-runtime >=20240410.859
+Requires-Dist: torch >=2.1.0
+Provides-Extra: onnx
+Requires-Dist: onnx ; extra == 'onnx'
 Provides-Extra: testing
-Requires-Dist: pytest >=8.0.0 ; extra == 'testing'
-Requires-Dist: pytest-xdist >=3.5.0 ; extra == 'testing'
-
-# IREE Turbine
+Requires-Dist: onnx ; extra == 'testing'
+Requires-Dist: pytest ; extra == 'testing'
+Requires-Dist: pytest-xdist ; extra == 'testing'
+Provides-Extra: torch-cpu-nightly
+Requires-Dist: torch ; extra == 'torch-cpu-nightly'
 
+# SHARK Turbine
 ![image](https://netl.doe.gov/sites/default/files/2020-11/Turbine-8412270026_83cfc8ee8f_c.jpg)
 
-Turbine is IREE's frontend for PyTorch.
+Turbine is the set of development tools that the [SHARK Team](https://github.com/nod-ai/SHARK)
+is building for deploying all of our models for deployment to the cloud and devices. We
+are building it as we transition from our TorchScript-era 1-off export and compilation 
+to a unified approach based on PyTorch 2 and Dynamo. While we use it heavily ourselves, it 
+is intended to be a general purpose model compilation and execution tool.
 
-Turbine provides a collection of tools:
+Turbine provides three primary tools:
 
 * *AOT Export*: For compiling one or more `nn.Module`s to compiled, deployment
   ready artifacts. This operates via both a simple one-shot export API (Already upstreamed to [torch-mlir](https://github.com/llvm/torch-mlir/blob/main/python/torch_mlir/extras/fx_importer.py))
-  for simple models and an underlying [advanced API](shark_turbine/aot/compiled_module.py) for complicated models
+  for simple models and an underlying [advanced API](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/shark_turbine/aot/compiled_module.py) for complicated models
   and accessing the full features of the runtime.
 * *Eager Execution*: A `torch.compile` backend is provided and a Turbine Tensor/Device
   is available for more native, interactive use within a PyTorch session.
-* *Custom Ops*: Integration for defining custom PyTorch ops and implementing them in
-  terms of IREE's backend IR or a Pythonic kernel language.
+* *Turbine Kernels*: (coming soon) A union of the [Triton](https://github.com/openai/triton) approach and
+  [Pallas](https://jax.readthedocs.io/en/latest/pallas/index.html) but based on
+  native PyTorch constructs and tracing. It is intended to complement for simple
+  cases where direct emission to the underlying, cross platform, vector programming model
+  is desirable.
+
+Under the covers, Turbine is based heavily on [IREE](https://github.com/openxla/iree) and
+[torch-mlir](https://github.com/llvm/torch-mlir) and we use it to drive evolution
+of both, upstreaming infrastructure as it becomes timely to do so.
+
+See [the roadmap](docs/roadmap.md) for upcoming work and places to contribute.
 
 ## Contact Us
 
-Turbine is under active development. Feel free to reach out on one of
-[IREE's communication channels](https://github.com/iree-org/iree?tab=readme-ov-file#communication-channels) (specifically, we monitor the
-#pytorch channel on the IREE Discord server).
+Turbine is under active development. If you would like to participate as it comes online,
+please reach out to us on the `#turbine` channel of the 
+[nod-ai Discord server](https://discord.gg/QMmR6f8rGb).
 
 ## Quick Start for Users
 
 1. Install from source:
 
 ```
-pip install iree-turbine
+pip install shark-turbine
 # Or for editable: see instructions under developers
 ```
 
 The above does install some unecessary cuda/cudnn packages for cpu use. To avoid this you
 can specify pytorch-cpu and install via:
 ```
-pip install -r pytorch-cpu-requirements.txt
-pip install iree-turbine
+pip install -r core/pytorch-cpu-requirements.txt
+pip install shark-turbine
 ```
 
 (or follow the "Developers" instructions below for installing from head/nightly)
 
 2. Try one of the samples:
 
-Generally, we use Turbine to produce valid, dynamic shaped Torch IR (from the
+Generally, we use Turbine to produce valid, dynamic shaped Torch IR (from the 
 [`torch-mlir torch` dialect](https://github.com/llvm/torch-mlir/tree/main/include/torch-mlir/Dialect/Torch/IR)
 with various approaches to handling globals). Depending on the use-case and status of the
 compiler, these should be compilable via IREE with `--iree-input-type=torch` for
 end to end execution. Dynamic shape support in torch-mlir is a work in progress,
 and not everything works at head with release binaries at present.
 
-  * [AOT MLP With Static Shapes](examples/aot_mlp/mlp_export_simple.py)
-  * [AOT MLP with a dynamic batch size](examples/aot_mlp/mlp_export_dynamic.py)
-  * [AOT llama2](examples/llama2_inference/llama2.ipynb):
+  * [AOT MLP With Static Shapes](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/aot_mlp/mlp_export_simple.py)
+  * [AOT MLP with a dynamic batch size](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/aot_mlp/mlp_export_dynamic.py)
+  * [AOT llama2](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/llama2_inference/llama2.ipynb):
     Dynamic sequence length custom compiled module with state management internal to the model.
-  * [Eager MNIST with `torch.compile`](examples/eager_mlp/mlp_eager_simple.py)
+  * [Eager MNIST with `torch.compile`](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/eager_mlp/mlp_eager_simple.py)
 
 ## Developers
 
-Use this as a guide to get started developing the project using pinned,
-pre-release dependencies. You are welcome to deviate as you see fit, but
-these canonical directions mirror what the CI does.
-
-### Setup a venv
+### Getting Up and Running
 
-We recommend setting up a virtual environment (venv). The project is configured
-to ignore `.venv` directories, and editors like VSCode pick them up by default.
+If only looking to develop against this project, then you need to install Python
+deps for the following:
 
-```
-python -m venv --prompt iree-turbine .venv
-source .venv/bin/activate
-```
+* PyTorch
+* iree-compiler (with Torch input support)
+* iree-runtime
 
-### Install PyTorch for Your System
+The pinned deps at HEAD require pre-release versions of all of the above, and
+therefore require additional pip flags to install. Therefore, to satisfy
+development, we provide a `requirements.txt` file which installs precise
+versions and has all flags. This can be installed prior to the package:
 
-If no explicit action is taken, the default PyTorch version will be installed.
-This will give you a current CUDA-based version. Install a different variant
-by doing so explicitly first:
-
-*CPU:*
+Installing into a venv is highly recommended.
 
 ```
-pip install -r pytorch-cpu-requirements.txt
+pip install -r core/pytorch-cpu-requirements.txt
+pip install --upgrade -r core/requirements.txt
+pip install --upgrade -e "core[torch-cpu-nightly,testing]"
 ```
 
-*ROCM:*
+Run tests:
 
 ```
-pip install -r pytorch-rocm-requirements.txt
+pytest core/
 ```
 
-### Install Development Packages
-
-```
-# Install editable local projects.
-pip install -r requirements.txt -e .
-```
-
-### Running Tests
-
-```
-pytest .
-```
-
-### Optional: Pre-commits and developer settings
-
-This project is set up to use the `pre-commit` tooling. To install it in
-your local repo, run: `pre-commit install`. After this point, when making
-commits locally, hooks will run. See https://pre-commit.com/
-
 ### Using a development compiler
 
 If doing native development of the compiler, it can be useful to switch to
 source builds for iree-compiler and iree-runtime.
 
 In order to do this, check out [IREE](https://github.com/openxla/iree) and
-follow the instructions to [build from source](https://iree.dev/building-from-source/getting-started/), making
-sure to specify [additional options for the Python bindings](https://iree.dev/building-from-source/getting-started/#building-with-cmake):
+follow the instructions to [build from source](https://openxla.github.io/iree/building-from-source/getting-started/#configuration-settings), making
+sure to specify [additional options](https://openxla.github.io/iree/building-from-source/getting-started/#building-with-cmake):
 
 ```
 -DIREE_BUILD_PYTHON_BINDINGS=ON -DPython3_EXECUTABLE="$(which python)"
 ```
 
 #### Configuring Python
 
 Uninstall existing packages:
 
 ```
 pip uninstall iree-compiler
 pip uninstall iree-runtime
 ```
-
 Copy the `.env` file from `iree/` to this source directory to get IDE
 support and add to your path for use from your shell:
 
 ```
 source .env && export PYTHONPATH
 ```
```

## Comparing `iree_turbine-2.3.0.dist-info/RECORD` & `iree_turbine-2.3.0rc20240410.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-iree/turbine/__init__.py,sha256=UQdKc1VCmcp1zMpbrFqFHcSSr1E5MjPpwNA6S2zD6fw,831
-shark_turbine/aot/__init__.py,sha256=HS96VEWDRqgxNGsV8XFBlexBGbBnFe_0zjYrVOv6zo8,515
+iree/turbine/__init__.py,sha256=aO-CTTyuCpkbBU7TwbF7t2hngKgFaLrFJYXOcZYjMCA,700
+shark_turbine/aot/__init__.py,sha256=adA_ZT60MsEFm9sCAMQHzpSZX6viiNODOS5HTzDGWkg,430
 shark_turbine/aot/compiled_module.py,sha256=uYIrK3lb-Jr4aiOrd5ljnMfkLc-qcFAgfXFrHoPwK4Y,23347
 shark_turbine/aot/decompositions.py,sha256=ouYk2ccigcWNtxo-oy3jSgJNBK1wG42fMJSQxZrqVo8,2815
-shark_turbine/aot/exporter.py,sha256=jedxPkmakeF2Wueb2YIl4cDPqt3e4gDID0sMbpkkdrQ,9877
+shark_turbine/aot/exporter.py,sha256=BueVZvHkAGcyrJiC6IgIaCo5WiwazaGhOFVwOD-4of4,9666
 shark_turbine/aot/fx_programs.py,sha256=jrRZqZDbCot8bu3L5JDn21bo8kf2ZGOWLr9RyjNp3AI,12219
-shark_turbine/aot/params.py,sha256=lYr05KfxGVjcZtZOLASIDCl-NW6qsgrxIV-vQR0RR6Q,9661
+shark_turbine/aot/params.py,sha256=afhJLynl0QFn5PzF7XfIGhUiu2oytnoHhlfubx_MHSU,4751
 shark_turbine/aot/tensor_traits.py,sha256=u_IuLi_SAJsh7BxCwiWueYbA0gxNIbdRRZCIFASnfP0,1023
-shark_turbine/aot/builtins/__init__.py,sha256=rDNDLuRqs_HmZE6QF1SJL1eszt-IhHivcraKqI7Pt9Q,906
-shark_turbine/aot/builtins/globals.py,sha256=v-SevLOve3je1IPUTDeHKreJm6-A9XQoCCmRyoqAPf0,7100
-shark_turbine/aot/builtins/jittable.py,sha256=I1nMrByxUxI_fBPsC5fYsY_KJtsVrzGllUBv8rLk8Kw,18037
+shark_turbine/aot/builtins/__init__.py,sha256=vx1VcMmc-yQidXaf1PPufmkrWX8RastJM1HYc_L_IlE,884
+shark_turbine/aot/builtins/globals.py,sha256=HxQcY2724-0bcuwvLObp-Xf2TCdCVG9s0OAzkPu5_Q4,5431
+shark_turbine/aot/builtins/jittable.py,sha256=w3XEtd_XcdqFrRr0Duwi5XfwS4hjga4Sxsemw00JxB0,18037
 shark_turbine/aot/passes/__init__.py,sha256=mkiANoenJUYzb2NsRgQV4sDfVPi-0b9VWotNDJ6ayHI,262
 shark_turbine/aot/passes/functorch.py,sha256=SwzWVkWLDq7ud_y-kODNEB1wPk_EaGsaHCdCqYQyr1w,3537
-shark_turbine/aot/support/ir_utils.py,sha256=Lqy2PV2viWfD5ZMT-d-ZlbgqrwODAPAhu2VpuhuBTMA,16691
+shark_turbine/aot/support/ir_utils.py,sha256=LMAsXEzNZpyHA5BvRJyyHTuNsibGSaWFIy9-AzWlpwQ,15795
 shark_turbine/aot/support/procedural/__init__.py,sha256=AAKJuYXBVmBbq-cClOOlzh3kbRiGW-Bkbwj982n8BiA,646
 shark_turbine/aot/support/procedural/base.py,sha256=2F5wdROfa75OQ96Y8by86FzoY5trK3C-fgrplWhC_ZQ,7507
-shark_turbine/aot/support/procedural/exported_program.py,sha256=A8eNKl9IYtBebQmX_Q8CrKo9iG9SDMT2WbNjpZE71Kg,12631
-shark_turbine/aot/support/procedural/globals.py,sha256=rmQoFOEsjDsLZZ7PtjSBu69E6rumHrW-Vpme34DmcqI,9222
+shark_turbine/aot/support/procedural/exported_program.py,sha256=sKjq22F4Yd1dR2qREZHTUgoeVagYyD1RaEiS7IhxDSY,11775
+shark_turbine/aot/support/procedural/globals.py,sha256=-clKFI0hGU6qfPfh0FjsXHYIWkW8cPllsuAkghpuBdw,9338
 shark_turbine/aot/support/procedural/iree_emitter.py,sha256=A0AU6KuE8r1A9HTfq6KHZkluO-ZAY3Dr8rwfB7GCGV4,12373
 shark_turbine/aot/support/procedural/primitives.py,sha256=O2xh2FdDg23cAbzUXMuH8uG1CzESwhH7sG85CXtsHNo,11744
 shark_turbine/aot/support/procedural/tracer.py,sha256=Eq6RVrl0wUVu1qUXxO5Aal6F-BUUuwspVWDRV3HeKcI,7211
 shark_turbine/dynamo/__init__.py,sha256=fsprbtYTtyX2jxbs8O8VZqutbrDJG87T1YkAGhwXisk,287
-shark_turbine/dynamo/decompositions.py,sha256=AI0kIYLvmw-WC7IMTqCihrQt2j5QkWLObFa39Om9w7U,3985
+shark_turbine/dynamo/decompositions.py,sha256=Omyu5TesiPAjYBqoZK9UG3Sv_rV_NrQnZx0US47VXu4,4096
 shark_turbine/dynamo/executor.py,sha256=vUTWn1czmZkrvoroXuYTtsWKyzCWeKtUx4FJW98A2Ss,8179
 shark_turbine/dynamo/passes.py,sha256=jFZdcVBL-fOaIJfjp2J66_iD1Hz2j5HRaM9JEo09WgE,814
 shark_turbine/dynamo/tensor.py,sha256=8DHnzqBoWCqCh7cxEaT1t3bNme6JpFR9deb9oB4YIF4,21970
-shark_turbine/dynamo/type_conversion.py,sha256=jKzPP1Z28FrUYRDEiqbeyQNj7r4Nbyc166CVF2lI5EM,7737
+shark_turbine/dynamo/type_conversion.py,sha256=LMctGCReXwZuXXjEBr6L21gRvq-co09nQPpf2MEbgTo,7017
 shark_turbine/dynamo/backends/cpu.py,sha256=i_1bYvn8tEisN32s9vJ2lDClK8h1bgtPEc59nNu5la8,2816
 shark_turbine/importers/ir.py,sha256=ufPQWLqroZ6Ul05k1RXLQHvstzAUD46IxABrIKtHaJM,857
 shark_turbine/importers/utils.py,sha256=9K8S7Wu7R3kqgiU8r_2hBET1VKGgQgTyv_0svK7Z_bw,1192
 shark_turbine/kernel/__init__.py,sha256=IontD5viYSNeQbAhKYpTDYyZVDIYV6zn98yXaL6GxWE,518
 shark_turbine/kernel/_support/context.py,sha256=7lr1iRE1YEJyYP8bBTHh5dyN_itoOpKUd7C0VK0LaBo,1484
 shark_turbine/kernel/_support/dtype.py,sha256=87HosOz7HNZovMptbpEPm_B3FkywlUaZPONMc4HQc8w,1157
 shark_turbine/kernel/_support/indexing.py,sha256=gss4gd2fsGcw8JCJBUBFOv5AZJcObI1Fpg0Jd152o08,12390
@@ -56,33 +56,30 @@
 shark_turbine/kernel/ops/control_flow.py,sha256=fHcTKIWB_0j75XM1Y_sFnB2RcmQ5pM8Zbrx2ovMZxDE,638
 shark_turbine/kernel/ops/core.py,sha256=N-gClns5wt9SKoYI_OAYVV9eH7sVa8vfrtBBHs3tgmU,581
 shark_turbine/kernel/ops/math.py,sha256=O7n8wXQHYvU9x00WN0J1xJeSdKd481JBhsBxkppwxQc,330
 shark_turbine/kernel/ops/memory.py,sha256=ZtyNLdWsDC_xkYyxqzs5bGp1wnQjCOGT0J7QfFRh4VI,577
 shark_turbine/kernel/ops/reduction.py,sha256=AfJHtJM6Iwy3dO6chdi4J1A04PZ6VkEwuSof8sgXY0s,487
 shark_turbine/kernel/ops/shape_manipulation.py,sha256=IswoyHQ1Zt6LHZrg4i0yI9CfW4v_0jxj2yrS4xmP5g0,555
 shark_turbine/ops/__init__.py,sha256=3ryhltgCM5UEUUBmn10xIn6RV0whheutIAgfK_QA_yg,248
-shark_turbine/ops/iree.py,sha256=TGZLdJ0ZbzFtloBQafZg4yX1skhJ4b9fhH-uPavtuQ4,2598
+shark_turbine/ops/iree.py,sha256=J3q-B_Mag_ArGhMqkdfe_mnZVQBC0yZvx1Do9smcUrM,1832
 shark_turbine/runtime/__init__.py,sha256=d5d9eGH_T80qOMPBSWC6vRw8EOKjBXx5gYYnGOAg65Y,272
-shark_turbine/runtime/device.py,sha256=h-NZ1zv9iwJnBH3ZIjtyvBM-vabVxcJqwdZf58dLKhQ,18221
-shark_turbine/runtime/tracing.py,sha256=gzTdCBXaC1gZj7ibFgwFVIk02-RSebU8DgIfblNnkx4,3453
+shark_turbine/runtime/device.py,sha256=58EAES0r517Q9u5NGfvjCT8z-o9GUNG41iNcEj0FDLI,12469
 shark_turbine/runtime/op_reg/__init__.py,sha256=Rg00q1Po-JFpWoHYcvqTqvNkVmwL7blhkKyxeIDZirU,249
-shark_turbine/runtime/op_reg/base.py,sha256=I7HhdjGOYu112URHJ_F66avgzhCoOkdhkJdqivdUrdU,28722
-shark_turbine/runtime/op_reg/compiler.py,sha256=PtoZhdhP1Ve1QbSlaPUtBB0XTTjVXxSCkQJJe0da_0Q,5156
-shark_turbine/runtime/op_reg/eager.py,sha256=0K8ohFvSkPUzrtnWQLqrMLXGbJ54bEtZLWqY-Mtk_ac,8341
-shark_turbine/support/__init__.py,sha256=4XzJ8ZeS0fbKqFsLXnyKOJ622sfrZZZiTWIRMFCyEw4,339
+shark_turbine/runtime/op_reg/base.py,sha256=nlRUci6NPHFhaATGY0aB6QxgWFicLNBfEF4WaAw-Adk,28076
+shark_turbine/runtime/op_reg/compiler.py,sha256=Rv2Fn8R_Sl0q3j_P8KW9ifDR86Ny4ECFxlOwOfJ-p7Y,4442
+shark_turbine/runtime/op_reg/eager.py,sha256=2BLuLG5biL8fqryqEos-OE46zzXCe97xV0netnHgjzc,6341
+shark_turbine/support/__init__.py,sha256=k_LVx8MyNLqne6v1i9ZryQgw_z5gOYiQXfhZ8cSC8cg,241
 shark_turbine/support/conversions.py,sha256=UngumsU4nDkJ1NgBOL8hWWHDRgJXNIGmoyZaPlawdJU,4118
-shark_turbine/support/debugging.py,sha256=Io3Z0K-KtA014PX1Hp8WJN_Acj8xAOX9OeIQfP6W2pM,3182
 shark_turbine/support/exceptions.py,sha256=EhMtpUEWT4wXo1ANF688oQP5H4ry2it9fjnEhJ9Nd24,1341
-shark_turbine/support/ir_imports.py,sha256=kMrMYO2dQx11vgv6bEbzHDvH0vSuKD2ovgOGtQAP0ow,1142
-shark_turbine/support/logging.py,sha256=2HkyMX1kF41yukyU7trjxaFzHmcoJ4CvWAJpNirzA6c,1255
+shark_turbine/support/ir_imports.py,sha256=rx7gwuMqvzxGCOCTXNj-4wypeJauOsq_lZ3N6pAajZU,1128
+shark_turbine/support/logging.py,sha256=Zk1eX0FE9ZO6MARJTLslUdYZUgPoszK251Z6bFncuAQ,357
 shark_turbine/transforms/builder.py,sha256=YDDfIZF28REmEUEyLRBRF5Y1oNyu9QKM59_snzgVI8w,2365
-shark_turbine/transforms/merger.py,sha256=yIEIaDZY1JaajN8TQoX8Vc7LWGVLWeUC7zl_fSYbHYY,8382
+shark_turbine/transforms/merger.py,sha256=trtv4JT9cIdRtw95lbqaBx5LvOvEaz28Kice6yTLp9g,8202
 shark_turbine/transforms/rewriter.py,sha256=UfTg26XJONA7dIipzyV6TMxq4Wgr2I7TxhqrWMwyktY,10997
-shark_turbine/transforms/general/custom_op_expansion.py,sha256=GfprwzNOXbCxlx5q93zsKVhvWpNGR2BYGFCNr3Ul_fY,10886
+shark_turbine/transforms/general/custom_op_expansion.py,sha256=rlStftau1NF9upIcUh3FUalGJM-OIHhg-AqCIQry9Sk,9012
 shark_turbine/transforms/general/rename_parameters.py,sha256=bPmDqRuCMJJFN5SjP8-b0ajcfDpIx5zpSKQZ_nB-jbg,4995
-shark_turbine/transforms/quantization/mm_group_quant.py,sha256=n72bd2XEJfTDVvlg6aYzZc_K3lBVIq4PmlTiC1Znp6c,7775
-iree_turbine-2.3.0.dist-info/LICENSE,sha256=nkXoVr7czun2clQILKEYUdlU3i_tdEjEvtGa2aq5mpE,12262
-iree_turbine-2.3.0.dist-info/METADATA,sha256=7LIjPiTMl8-QZLpof73jHiWSlG4NWynl-ObKiDXfOVM,5351
-iree_turbine-2.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-iree_turbine-2.3.0.dist-info/entry_points.txt,sha256=-bxFqt7ywvSixYOWlz1sZ8MXChj-5joPPR_gZfT3Kn4,80
-iree_turbine-2.3.0.dist-info/top_level.txt,sha256=HC8-angiduPf60mk4TnoHh0l6DedI5geRT925eyi6mc,19
-iree_turbine-2.3.0.dist-info/RECORD,,
+shark_turbine/transforms/quantization/mm_group_quant.py,sha256=DyqTvSJExiS2YlOajOO1Y8if7LBR_kslCc00BjJytTE,7793
+iree_turbine-2.3.0rc20240410.dist-info/METADATA,sha256=trjdTTVxwLPaIPh4FGeVWIGRl2kTSiKQpROhJbNiVIw,6262
+iree_turbine-2.3.0rc20240410.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+iree_turbine-2.3.0rc20240410.dist-info/entry_points.txt,sha256=-bxFqt7ywvSixYOWlz1sZ8MXChj-5joPPR_gZfT3Kn4,80
+iree_turbine-2.3.0rc20240410.dist-info/top_level.txt,sha256=HC8-angiduPf60mk4TnoHh0l6DedI5geRT925eyi6mc,19
+iree_turbine-2.3.0rc20240410.dist-info/RECORD,,
```

