# Comparing `tmp/danielutils-0.9.76.tar.gz` & `tmp/danielutils-0.9.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.76.tar", last modified: Sun Apr 21 21:50:41 2024, max compression
+gzip compressed data, was "danielutils-0.9.77.tar", last modified: Sat Apr 27 19:11:29 2024, max compression
```

## Comparing `danielutils-0.9.76.tar` & `danielutils-0.9.77.tar`

### file list

```diff
@@ -1,221 +1,224 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.537923 danielutils-0.9.76/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.76/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-21 21:50:40.000000 danielutils-0.9.76/MANIFEST.in
--rw-rw-rw-   0        0        0     4486 2024-04-21 21:50:41.536716 danielutils-0.9.76/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2024-04-21 19:23:37.000000 danielutils-0.9.76/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.430997 danielutils-0.9.76/danielutils/
--rw-rw-rw-   0        0        0     1364 2024-04-21 19:46:04.000000 danielutils-0.9.76/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.434997 danielutils-0.9.76/danielutils/abstractions/
--rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.76/danielutils/abstractions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.437508 danielutils-0.9.76/danielutils/abstractions/database/
--rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.76/danielutils/abstractions/database/__init__.py
--rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/abstractions/database/cached_database.py
--rw-rw-rw-   0        0        0     2616 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/abstractions/database/database.py
--rw-rw-rw-   0        0        0     1066 2024-04-21 19:46:04.000000 danielutils-0.9.76/danielutils/abstractions/database/redis_database.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.440018 danielutils-0.9.76/danielutils/abstractions/multiprogramming/
--rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.76/danielutils/abstractions/multiprogramming/__init__.py
--rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/abstractions/multiprogramming/multi_id.py
--rw-rw-rw-   0        0        0     2398 2024-04-21 19:22:23.000000 danielutils-0.9.76/danielutils/abstractions/multiprogramming/worker.py
--rw-rw-rw-   0        0        0     2426 2024-04-21 19:22:35.000000 danielutils-0.9.76/danielutils/abstractions/multiprogramming/worker_pool.py
--rw-rw-rw-   0        0        0     3162 2024-04-21 18:24:30.000000 danielutils-0.9.76/danielutils/abstractions/repl.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.442013 danielutils-0.9.76/danielutils/better_builtins/
--rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.76/danielutils/better_builtins/__init__.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/better_builtins/counter.py
--rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.76/danielutils/better_builtins/frange.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.446011 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4730 2024-04-09 22:20:09.000000 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/better_builtins/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5457 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/colors.py
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/convenience.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.448012 danielutils-0.9.76/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.450658 danielutils-0.9.76/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.76/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/conversions/specialized_conversions/to_int.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.453173 danielutils-0.9.76/danielutils/data_structures/
--rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/comparer.py
--rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.76/danielutils/data_structures/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.456845 danielutils-0.9.76/danielutils/data_structures/graph/
--rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/graph/__init__.py
--rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.76/danielutils/data_structures/graph/binary_node.py
--rw-rw-rw-   0        0        0     6917 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/graph/graph.py
--rw-rw-rw-   0        0        0     3149 2024-04-18 18:55:16.000000 danielutils-0.9.76/danielutils/data_structures/graph/multinode.py
--rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.76/danielutils/data_structures/graph/node.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.458851 danielutils-0.9.76/danielutils/data_structures/heap/
--rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.76/danielutils/data_structures/heap/__init__.py
--rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/heap/heap.py
--rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.76/danielutils/data_structures/heap/max_heap.py
--rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.76/danielutils/data_structures/heap/min_heap.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.461878 danielutils-0.9.76/danielutils/data_structures/queue/
--rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.76/danielutils/data_structures/queue/__init__.py
--rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.76/danielutils/data_structures/queue/atomic_queue.py
--rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.76/danielutils/data_structures/queue/priority_queue.py
--rw-rw-rw-   0        0        0     1621 2024-03-29 00:18:38.000000 danielutils-0.9.76/danielutils/data_structures/queue/queue.py
--rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/stack.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.463885 danielutils-0.9.76/danielutils/data_structures/trees/
--rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/data_structures/trees/__init__.py
--rw-rw-rw-   0        0        0     2507 2024-04-18 18:33:41.000000 danielutils-0.9.76/danielutils/data_structures/trees/binary_syntax_tree.py
--rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.76/danielutils/data_structures/trees/binary_tree.py
--rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.76/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.76/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.476995 danielutils-0.9.76/danielutils/decorators/
--rw-rw-rw-   0        0        0      446 2024-04-09 22:04:07.000000 danielutils-0.9.76/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.76/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1538 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.76/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1175 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1452 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1860 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0     1017 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7785 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0      995 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.76/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/singleton.py
--rw-rw-rw-   0        0        0      899 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     2157 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0     3741 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/decorators/total_ordering.py
--rw-rw-rw-   0        0        0    10004 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.482633 danielutils-0.9.76/danielutils/functions/
--rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.76/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.76/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.76/danielutils/functions/flatten.py
--rw-rw-rw-   0        0        0    10296 2024-04-21 18:21:37.000000 danielutils-0.9.76/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.76/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0     1286 2024-04-21 19:19:56.000000 danielutils-0.9.76/danielutils/functions/multiloop.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/functions/subseteq.py
--rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.76/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.485353 danielutils-0.9.76/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2869 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/internet.py
--rw-rw-rw-   0        0        0    12002 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/io_.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.488864 danielutils-0.9.76/danielutils/math_/
--rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.76/danielutils/math_/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/math_/constants.py
--rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/math_/functions.py
--rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.76/danielutils/math_/math_print.py
--rw-rw-rw-   0        0        0     4052 2024-04-21 18:05:24.000000 danielutils-0.9.76/danielutils/math_/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.489869 danielutils-0.9.76/danielutils/math_/polynomial/
--rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.76/danielutils/math_/polynomial/__init__.py
--rw-rw-rw-   0        0        0      653 2024-04-21 18:05:24.000000 danielutils-0.9.76/danielutils/math_/polynomial/polinomial.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.492751 danielutils-0.9.76/danielutils/metaclasses/
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.76/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0    10952 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/metaclasses/interface.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/metaclasses/overload_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.495756 danielutils-0.9.76/danielutils/mock_/
--rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.76/danielutils/mock_/__init__.py
--rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.76/danielutils/mock_/mock_database.py
--rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/mock_/mock_module.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/path.py
--rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.76/danielutils/print_.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.497753 danielutils-0.9.76/danielutils/protocols/
--rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/protocols/__init__.py
--rw-rw-rw-   0        0        0      311 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/protocols/dictable.py
--rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/protocols/evaluable.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.76/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.497753 danielutils-0.9.76/danielutils/reflection/
--rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.76/danielutils/reflection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.499769 danielutils-0.9.76/danielutils/reflection/class_/
--rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.76/danielutils/reflection/class_/__init__.py
--rw-rw-rw-   0        0        0     5271 2024-04-21 18:23:25.000000 danielutils-0.9.76/danielutils/reflection/class_/class_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.501079 danielutils-0.9.76/danielutils/reflection/file/
--rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.76/danielutils/reflection/file/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-04-21 18:22:59.000000 danielutils-0.9.76/danielutils/reflection/file/file_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.503085 danielutils-0.9.76/danielutils/reflection/function/
--rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.76/danielutils/reflection/function/__init__.py
--rw-rw-rw-   0        0        0     4459 2024-04-21 18:24:01.000000 danielutils-0.9.76/danielutils/reflection/function/function_reflections.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.508098 danielutils-0.9.76/danielutils/reflection/interpreter/
--rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.76/danielutils/reflection/interpreter/__init__.py
--rw-rw-rw-   0        0        0      714 2024-04-09 22:42:25.000000 danielutils-0.9.76/danielutils/reflection/interpreter/callstack.py
--rw-rw-rw-   0        0        0      447 2024-04-21 18:22:32.000000 danielutils-0.9.76/danielutils/reflection/interpreter/get_traceback.py
--rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/reflection/interpreter/os_.py
--rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/reflection/interpreter/packages.py
--rw-rw-rw-   0        0        0      627 2024-03-29 21:49:46.000000 danielutils-0.9.76/danielutils/reflection/interpreter/python_version.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/reflection/interpreter/signals.py
--rw-rw-rw-   0        0        0     5570 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/reflection/interpreter/tracer.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.509882 danielutils-0.9.76/danielutils/reflection/module/
--rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.76/danielutils/reflection/module/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/reflection/module/module_reflections.py
--rw-rw-rw-   0        0        0     4742 2024-04-21 18:27:13.000000 danielutils-0.9.76/danielutils/reflection/module/package_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.510803 danielutils-0.9.76/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.512848 danielutils-0.9.76/danielutils/system/
--rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.76/danielutils/system/independent.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.513847 danielutils-0.9.76/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.514847 danielutils-0.9.76/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/text.py
--rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/time.py
--rw-rw-rw-   0        0        0     1733 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/tqdm_.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.515847 danielutils-0.9.76/danielutils/university/
--rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.516848 danielutils-0.9.76/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.76/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.518848 danielutils-0.9.76/danielutils/university/oop/
--rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/oop/__init__.py
--rw-rw-rw-   0        0        0      802 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/oop/observer.py
--rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/oop/strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.522681 danielutils-0.9.76/danielutils/university/probability/
--rw-rw-rw-   0        0        0      190 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.523688 danielutils-0.9.76/danielutils/university/probability/conditional_variables/
--rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/__init__.py
--rw-rw-rw-   0        0        0     3191 2024-04-18 19:04:03.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/conditional_variable.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.524688 danielutils-0.9.76/danielutils/university/probability/conditional_variables/continuous/
--rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/continuous/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.530716 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/
--rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/__init__.py
--rw-rw-rw-   0        0        0      867 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/bernoulli.py
--rw-rw-rw-   0        0        0     1261 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/binomial.py
--rw-rw-rw-   0        0        0     1112 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/conditional_from_discrete_probability_func.py
--rw-rw-rw-   0        0        0     1378 2024-04-18 17:43:56.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/discrete.py
--rw-rw-rw-   0        0        0     1511 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/geometric.py
--rw-rw-rw-   0        0        0      996 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/poisson.py
--rw-rw-rw-   0        0        0     1034 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/uniform.py
--rw-rw-rw-   0        0        0      906 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/distributions.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.533718 danielutils-0.9.76/danielutils/university/probability/expressions/
--rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.76/danielutils/university/probability/expressions/__init__.py
--rw-rw-rw-   0        0        0     7463 2024-04-18 19:12:37.000000 danielutils-0.9.76/danielutils/university/probability/expressions/accumulation_expression.py
--rw-rw-rw-   0        0        0     4511 2024-04-18 19:12:09.000000 danielutils-0.9.76/danielutils/university/probability/expressions/probability_expression.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.536716 danielutils-0.9.76/danielutils/university/probability/funcs/
--rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/funcs/__init__.py
--rw-rw-rw-   0        0        0      293 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/funcs/covariance.py
--rw-rw-rw-   0        0        0     1174 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/funcs/expected_value.py
--rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/funcs/probability_function.py
--rw-rw-rw-   0        0        0      398 2024-04-17 20:37:10.000000 danielutils-0.9.76/danielutils/university/probability/funcs/variance.py
--rw-rw-rw-   0        0        0     1835 2024-04-17 23:39:30.000000 danielutils-0.9.76/danielutils/university/probability/operator.py
--rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.76/danielutils/university/probability/protocols.py
--rw-rw-rw-   0        0        0     1417 2024-04-21 18:13:57.000000 danielutils-0.9.76/danielutils/university/probability/supp.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:50:41.432998 danielutils-0.9.76/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4486 2024-04-21 21:50:41.000000 danielutils-0.9.76/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7582 2024-04-21 21:50:41.000000 danielutils-0.9.76/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 21:50:41.000000 danielutils-0.9.76/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-21 21:50:41.000000 danielutils-0.9.76/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      934 2024-04-21 21:48:25.000000 danielutils-0.9.76/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 21:50:41.537923 danielutils-0.9.76/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-21 21:43:33.000000 danielutils-0.9.76/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.469435 danielutils-0.9.77/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.77/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-27 19:11:28.000000 danielutils-0.9.77/MANIFEST.in
+-rw-rw-rw-   0        0        0     4593 2024-04-27 19:11:29.469435 danielutils-0.9.77/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2024-04-27 19:11:15.000000 danielutils-0.9.77/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.356810 danielutils-0.9.77/danielutils/
+-rw-rw-rw-   0        0        0     1364 2024-04-21 19:46:04.000000 danielutils-0.9.77/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.362027 danielutils-0.9.77/danielutils/abstractions/
+-rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.77/danielutils/abstractions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.364377 danielutils-0.9.77/danielutils/abstractions/database/
+-rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.77/danielutils/abstractions/database/__init__.py
+-rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/abstractions/database/cached_database.py
+-rw-rw-rw-   0        0        0     2616 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/abstractions/database/database.py
+-rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.77/danielutils/abstractions/database/redis_database.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.366375 danielutils-0.9.77/danielutils/abstractions/multiprogramming/
+-rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/__init__.py
+-rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/multi_id.py
+-rw-rw-rw-   0        0        0     2398 2024-04-21 19:22:23.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker.py
+-rw-rw-rw-   0        0        0     2426 2024-04-21 19:22:35.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker_pool.py
+-rw-rw-rw-   0        0        0     3162 2024-04-21 18:24:30.000000 danielutils-0.9.77/danielutils/abstractions/repl.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/aliases.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.368377 danielutils-0.9.77/danielutils/better_builtins/
+-rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.77/danielutils/better_builtins/__init__.py
+-rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/counter.py
+-rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.77/danielutils/better_builtins/frange.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.372391 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/
+-rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/__init__.py
+-rw-rw-rw-   0        0        0     4730 2024-04-09 22:20:09.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/factory.py
+-rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tdict.py
+-rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tset.py
+-rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/ttuple.py
+-rw-rw-rw-   0        0        0     5457 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/colors.py
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/convenience.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.373793 danielutils-0.9.77/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.375797 danielutils-0.9.77/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.77/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/specialized_conversions/to_int.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.378797 danielutils-0.9.77/danielutils/data_structures/
+-rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/comparer.py
+-rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.77/danielutils/data_structures/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.383273 danielutils-0.9.77/danielutils/data_structures/graph/
+-rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/graph/__init__.py
+-rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.77/danielutils/data_structures/graph/binary_node.py
+-rw-rw-rw-   0        0        0     6917 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/graph/graph.py
+-rw-rw-rw-   0        0        0     3149 2024-04-18 18:55:16.000000 danielutils-0.9.77/danielutils/data_structures/graph/multinode.py
+-rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.77/danielutils/data_structures/graph/node.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.386278 danielutils-0.9.77/danielutils/data_structures/heap/
+-rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.77/danielutils/data_structures/heap/__init__.py
+-rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/heap/heap.py
+-rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.77/danielutils/data_structures/heap/max_heap.py
+-rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.77/danielutils/data_structures/heap/min_heap.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.389278 danielutils-0.9.77/danielutils/data_structures/queue/
+-rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.77/danielutils/data_structures/queue/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.77/danielutils/data_structures/queue/atomic_queue.py
+-rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.77/danielutils/data_structures/queue/priority_queue.py
+-rw-rw-rw-   0        0        0     1621 2024-03-29 00:18:38.000000 danielutils-0.9.77/danielutils/data_structures/queue/queue.py
+-rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/stack.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.391782 danielutils-0.9.77/danielutils/data_structures/trees/
+-rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/trees/__init__.py
+-rw-rw-rw-   0        0        0     2644 2024-04-25 21:14:44.000000 danielutils-0.9.77/danielutils/data_structures/trees/binary_syntax_tree.py
+-rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.77/danielutils/data_structures/trees/binary_tree.py
+-rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.77/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.77/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.404279 danielutils-0.9.77/danielutils/decorators/
+-rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.77/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      741 2024-04-27 18:47:34.000000 danielutils-0.9.77/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1370 2024-04-27 18:47:49.000000 danielutils-0.9.77/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.77/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.77/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.77/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.77/danielutils/decorators/final.py
+-rw-rw-rw-   0        0        0     1681 2024-04-27 18:48:02.000000 danielutils-0.9.77/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      811 2024-04-27 18:48:25.000000 danielutils-0.9.77/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7571 2024-04-27 18:48:52.000000 danielutils-0.9.77/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0      822 2024-04-27 18:49:05.000000 danielutils-0.9.77/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.77/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/decorators/singleton.py
+-rw-rw-rw-   0        0        0      729 2024-04-27 18:49:28.000000 danielutils-0.9.77/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     1983 2024-04-27 18:49:18.000000 danielutils-0.9.77/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0     3741 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/decorators/total_ordering.py
+-rw-rw-rw-   0        0        0     9541 2024-04-27 18:40:42.000000 danielutils-0.9.77/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.411203 danielutils-0.9.77/danielutils/functions/
+-rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/functions/flatten.py
+-rw-rw-rw-   0        0        0    10081 2024-04-27 18:52:54.000000 danielutils-0.9.77/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0     1286 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/functions/multiloop.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/functions/subseteq.py
+-rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.414716 danielutils-0.9.77/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2869 2024-04-21 18:13:57.000000 danielutils-0.9.77/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/internet.py
+-rw-rw-rw-   0        0        0    12002 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/io_.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.417096 danielutils-0.9.77/danielutils/math_/
+-rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/__init__.py
+-rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/math_/constants.py
+-rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/math_/functions.py
+-rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/math_print.py
+-rw-rw-rw-   0        0        0     4052 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/math_symbols.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.419094 danielutils-0.9.77/danielutils/math_/polynomial/
+-rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/polynomial/__init__.py
+-rw-rw-rw-   0        0        0      849 2024-04-25 21:17:25.000000 danielutils-0.9.77/danielutils/math_/polynomial/polinomial.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.424070 danielutils-0.9.77/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.77/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.77/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0    10952 2024-04-21 18:13:57.000000 danielutils-0.9.77/danielutils/metaclasses/interface.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/metaclasses/overload_meta.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.426500 danielutils-0.9.77/danielutils/mock_/
+-rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.77/danielutils/mock_/__init__.py
+-rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.77/danielutils/mock_/mock_database.py
+-rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/mock_/mock_module.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/path.py
+-rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/print_.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.428878 danielutils-0.9.77/danielutils/protocols/
+-rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/protocols/__init__.py
+-rw-rw-rw-   0        0        0      454 2024-04-25 21:16:46.000000 danielutils-0.9.77/danielutils/protocols/dictable.py
+-rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/protocols/evaluable.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.77/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.428878 danielutils-0.9.77/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.429885 danielutils-0.9.77/danielutils/reflection/class_/
+-rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/class_/__init__.py
+-rw-rw-rw-   0        0        0     5529 2024-04-27 18:35:37.000000 danielutils-0.9.77/danielutils/reflection/class_/class_reflection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.431391 danielutils-0.9.77/danielutils/reflection/file/
+-rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/file/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.77/danielutils/reflection/file/file_reflection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.433265 danielutils-0.9.77/danielutils/reflection/function/
+-rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/function/__init__.py
+-rw-rw-rw-   0        0        0     4459 2024-04-21 18:24:01.000000 danielutils-0.9.77/danielutils/reflection/function/function_reflections.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.438928 danielutils-0.9.77/danielutils/reflection/interpreter/
+-rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/reflection/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.77/danielutils/reflection/interpreter/callstack.py
+-rw-rw-rw-   0        0        0      447 2024-04-21 18:22:32.000000 danielutils-0.9.77/danielutils/reflection/interpreter/get_traceback.py
+-rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/reflection/interpreter/os_.py
+-rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/reflection/interpreter/packages.py
+-rw-rw-rw-   0        0        0      627 2024-03-29 21:49:46.000000 danielutils-0.9.77/danielutils/reflection/interpreter/python_version.py
+-rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/reflection/interpreter/signals.py
+-rw-rw-rw-   0        0        0     5745 2024-04-25 21:09:28.000000 danielutils-0.9.77/danielutils/reflection/interpreter/tracer.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.439926 danielutils-0.9.77/danielutils/reflection/module/
+-rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.77/danielutils/reflection/module/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/reflection/module/module_reflections.py
+-rw-rw-rw-   0        0        0     4742 2024-04-21 18:27:13.000000 danielutils-0.9.77/danielutils/reflection/module/package_reflection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.441942 danielutils-0.9.77/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.443949 danielutils-0.9.77/danielutils/system/
+-rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/system/independent.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.445946 danielutils-0.9.77/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.447416 danielutils-0.9.77/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/text.py
+-rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.77/danielutils/time.py
+-rw-rw-rw-   0        0        0     1731 2024-04-25 20:10:37.000000 danielutils-0.9.77/danielutils/tqdm_.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.448884 danielutils-0.9.77/danielutils/university/
+-rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.449890 danielutils-0.9.77/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.451394 danielutils-0.9.77/danielutils/university/oop/
+-rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/oop/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/oop/observer.py
+-rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/oop/strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.456002 danielutils-0.9.77/danielutils/university/probability/
+-rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.457730 danielutils-0.9.77/danielutils/university/probability/conditional_variable/
+-rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/__init__.py
+-rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/conditional_variable.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.457730 danielutils-0.9.77/danielutils/university/probability/conditional_variable/continuous/
+-rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/continuous/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.463436 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/
+-rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/__init__.py
+-rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
+-rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/binomial.py
+-rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
+-rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/discrete.py
+-rw-rw-rw-   0        0        0     1658 2024-04-25 21:22:17.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/geometric.py
+-rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/poisson.py
+-rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/uniform.py
+-rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/distributions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.465435 danielutils-0.9.77/danielutils/university/probability/expressions/
+-rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.77/danielutils/university/probability/expressions/__init__.py
+-rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.77/danielutils/university/probability/expressions/accumulation_expression.py
+-rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.77/danielutils/university/probability/expressions/probability_expression.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.468436 danielutils-0.9.77/danielutils/university/probability/funcs/
+-rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/funcs/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/funcs/covariance.py
+-rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/funcs/expected_value.py
+-rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/funcs/probability_function.py
+-rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/funcs/variance.py
+-rw-rw-rw-   0        0        0     2005 2024-04-25 21:18:16.000000 danielutils-0.9.77/danielutils/university/probability/operator.py
+-rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.77/danielutils/university/probability/protocols.py
+-rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/supp.py
+-rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.77/danielutils/university/probability/transformation.py
+-rw-rw-rw-   0        0        0      605 2024-04-27 18:47:16.000000 danielutils-0.9.77/danielutils/versioned_imports.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.360487 danielutils-0.9.77/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4593 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7689 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-04-27 19:11:28.000000 danielutils-0.9.77/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 19:11:29.469435 danielutils-0.9.77/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-27 19:11:28.000000 danielutils-0.9.77/setup.py
```

### Comparing `danielutils-0.9.76/LICENSE` & `danielutils-0.9.77/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/PKG-INFO` & `danielutils-0.9.77/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.76
+Version: 0.9.77
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,17 @@
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
 # danielutils v=0.9.75
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
+**Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13` 
+
+Versions marked with * are partially working
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
 
 ### [`isoftype`](./READMES/isoftype.md)
 -- _"Boost your type checking game with `isoftype`: Effortlessly verify object types and subtypes, handle complex data structures, and tackle union types in Python!"_
 
 **Support for Parametrized Generics**
```

### Comparing `danielutils-0.9.76/README.md` & `danielutils-0.9.77/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
 # danielutils v=0.9.75
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
+**Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13` 
+
+Versions marked with * are partially working
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
 
 ### [`isoftype`](./READMES/isoftype.md)
 -- _"Boost your type checking game with `isoftype`: Effortlessly verify object types and subtypes, handle complex data structures, and tackle union types in Python!"_
 
 **Support for Parametrized Generics**
```

### Comparing `danielutils-0.9.76/danielutils/__init__.py` & `danielutils-0.9.77/danielutils/__init__.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/abstractions/database/cached_database.py` & `danielutils-0.9.77/danielutils/abstractions/database/cached_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/abstractions/database/database.py` & `danielutils-0.9.77/danielutils/abstractions/database/database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/abstractions/database/redis_database.py` & `danielutils-0.9.77/danielutils/abstractions/database/redis_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Optional, TypeVar
 
 try:
     import redis
 except ImportError:
-    from mock_ import MockImportObject
+    from ...mock_ import MockImportObject
 
     redis = MockImportObject("`redis` is not installed")
-from abstractions.database.database import Database
+from .database import Database
 
 K = TypeVar('K')
 V = TypeVar('V')
 
 
 class RedisDatabase(Database[K, V]):
     """
```

### Comparing `danielutils-0.9.76/danielutils/abstractions/multiprogramming/worker.py` & `danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/abstractions/multiprogramming/worker_pool.py` & `danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker_pool.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/abstractions/repl.py` & `danielutils-0.9.77/danielutils/abstractions/repl.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/aliases.py` & `danielutils-0.9.77/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/better_builtins/counter.py` & `danielutils-0.9.77/danielutils/better_builtins/counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/better_builtins/frange.py` & `danielutils-0.9.77/danielutils/better_builtins/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/better_builtins/typed_builtins/factory.py` & `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/factory.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/better_builtins/typed_builtins/tdict.py` & `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tdict.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/better_builtins/typed_builtins/tlist.py` & `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tlist.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/better_builtins/typed_builtins/tset.py` & `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/colors.py` & `danielutils-0.9.77/danielutils/colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/conversions/main_conversions.py` & `danielutils-0.9.77/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.77/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/comparer.py` & `danielutils-0.9.77/danielutils/data_structures/comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/functions.py` & `danielutils-0.9.77/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/graph/binary_node.py` & `danielutils-0.9.77/danielutils/data_structures/graph/binary_node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/graph/graph.py` & `danielutils-0.9.77/danielutils/data_structures/graph/graph.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/graph/multinode.py` & `danielutils-0.9.77/danielutils/data_structures/graph/multinode.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/graph/node.py` & `danielutils-0.9.77/danielutils/data_structures/graph/node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/heap/heap.py` & `danielutils-0.9.77/danielutils/data_structures/heap/heap.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/queue/priority_queue.py` & `danielutils-0.9.77/danielutils/data_structures/queue/priority_queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/queue/queue.py` & `danielutils-0.9.77/danielutils/data_structures/queue/queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/stack.py` & `danielutils-0.9.77/danielutils/data_structures/stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/data_structures/trees/binary_syntax_tree.py` & `danielutils-0.9.77/danielutils/data_structures/trees/binary_syntax_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Union, Any, Callable
+from typing import Union, Any, Callable,Dict as t_dict
 from .binary_tree import BinaryTree
 from ..graph import BinaryNode
-
+from ...reflection import get_python_version
+if get_python_version()>=(3,9):
+    from builtins import dict as t_dict
 
 class BinarySyntaxTree(BinaryTree):
     """
     Binary tree data structure to represent syntax of expressions
     """
 
     @staticmethod
-    def _evaluate_node(v: BinaryNode, operator_func_dict: dict[Any, Callable[[Any, Any], Any]]):
+    def _evaluate_node(v: BinaryNode, operator_func_dict: t_dict[Any, Callable[[Any, Any], Any]]):
         if not isinstance(v, BinaryNode) or v.left is None and v.right is None:
             return v
 
         lres = BinarySyntaxTree._evaluate_node(v.left, operator_func_dict)
         rres = BinarySyntaxTree._evaluate_node(v.right, operator_func_dict)
 
         return operator_func_dict[v.data](lres, rres)
@@ -68,15 +70,15 @@
 
     def reverse(self) -> "BinarySyntaxTree":
         return BinarySyntaxTree(self.root.reverse())
 
     def __reversed__(self) -> "BinarySyntaxTree":
         return self.reverse()
 
-    def evaluate(self, operator_func_dict: dict[Any, Callable[[Any, Any], Any]]) -> Any:
+    def evaluate(self, operator_func_dict: t_dict[Any, Callable[[Any, Any], Any]]) -> Any:
         return BinarySyntaxTree._evaluate_node(self.root, operator_func_dict)
 
 
 
 __all__ = [
     "BinarySyntaxTree"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/data_structures/trees/binary_tree.py` & `danielutils-0.9.77/danielutils/data_structures/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/date.py` & `danielutils-0.9.77/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/atomic.py` & `danielutils-0.9.77/danielutils/decorators/atomic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import functools
 from typing import Callable, Any, TypeVar
 import threading
 from .validate import validate
 
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+from ..versioned_imports import ParamSpec
+
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 @validate
 def atomic(func: FuncT) -> FuncT:
@@ -22,17 +19,18 @@
         func (Callable): function to make thread safe
 
     Returns:
         Callable: the thread safe function
     """
     lock = threading.Lock()
 
-    @ functools.wraps(func)
+    @functools.wraps(func)
     def wrapper(*args, **kwargs) -> Any:
         with lock:
             return func(*args, **kwargs)
+
     return wrapper
 
 
 __all__ = [
     "atomic"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/attach.py` & `danielutils-0.9.77/danielutils/decorators/attach.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import functools
 from typing import Callable, Optional, TypeVar
 from .validate import validate
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+from ..versioned_imports import ParamSpec
+
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 @validate(strict=False)
 def attach(before: Optional[Callable] = None, after: Optional[Callable] = None) -> Callable[[FuncT], FuncT]:
@@ -37,14 +34,16 @@
         def wrapper(*args, **kwargs):
             if before is not None:
                 before()
             res = func(*args, **kwargs)
             if after is not None:
                 after()
             return res
+
         return wrapper
+
     return attach_deco
 
 
 __all__ = [
     "attach"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.77/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/decorate_conditionally.py` & `danielutils-0.9.77/danielutils/decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/delay_call.py` & `danielutils-0.9.77/danielutils/decorators/limit_recursion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,51 @@
-from typing import Callable, TypeVar, Union
-import time
 import functools
-from .decorate_conditionally import decorate_conditionally
-from .threadify import threadify
+import re
+import traceback
+from typing import Any, Callable, TypeVar
+from .validate import validate
+from ..colors import warning
+from ..versioned_imports import ParamSpec
 
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore# pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
-def delay_call(seconds: Union[float, int], blocking: bool = True) -> Callable[[FuncT], FuncT]:
-    """will delay the call to a function by the given amount of seconds
+@validate
+def limit_recursion(max_depth: int, return_value: Any = None, quiet: bool = True) -> Callable[[FuncT], FuncT]:
+    """decorator to limit recursion of functions
 
     Args:
-        seconds (float | int): the amount of time to wait
-        blocking (bool, optional): whether to block the main thread
-        when waiting or to wait in a different thread. Defaults to True.
+        max_depth (int): max recursion depth which is allowed for this function
+        return_value (Any, optional): The value to return when the limit is reached. Defaults to None.
+            if is None, will return the last a tuple for the last args, kwargs given
+        quiet (bool, optional): whether to print a warning message. Defaults to True.
     """
+
     def deco(func: FuncT) -> FuncT:
-        @decorate_conditionally(threadify, not blocking)
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
-            time.sleep(seconds)
-            func(*args, **kwargs)
+            depth = functools.reduce(
+                lambda count, line:
+                count + 1 if re.search(rf"{func.__name__}\(.*\)$", line)
+                else count,
+                traceback.format_stack(), 0
+            )
+            if depth >= max_depth:
+                if not quiet:
+                    warning(
+                        "limit_recursion has limited the number of calls for "
+                        f"{func.__module__}.{func.__qualname__} to {max_depth}")
+                if return_value:
+                    return return_value
+                return args, kwargs
+            return func(*args, **kwargs)
+
         return wrapper
+
     return deco
 
 
 __all__ = [
-    "delay_call"
+    "limit_recursion"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/deprecate.py` & `danielutils-0.9.77/danielutils/decorators/deprecate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from typing import Callable, TypeVar
 from ..colors import warning, ColoredText
+from ..versioned_imports import ParamSpec
 
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 def deprecate_with(replacement_func) -> Callable[[FuncT], FuncT]:
     """will replace a deprecated function with the replacement func and will print a warning"""
+
     def deco(func: FuncT) -> FuncT:
         warning(f"{func.__module__}.{func.__qualname__} is deprecated,"
                 f" using {replacement_func.__module__}.{replacement_func.__qualname__} instead")
 
         def wrapper(*args, **kwargs):
             return replacement_func(*args, **kwargs)
+
         return wrapper
+
     return deco
 
 
 def deprecate(deprecation_message: str) -> Callable[[FuncT], FuncT]:
     """A decorator to print a deprecation message when using a deprecated function
 
     Args:
         deprecation_message (str): deprecation message
     """
+
     def deco(func: FuncT) -> FuncT:
         def wrapper(*args, **kwargs):
             print(ColoredText.orange("Deprecation Warning") +
                   ":", deprecation_message)
             return func(*args, **kwargs)
+
         return wrapper
+
     return deco
 
 
 __all__ = [
     "deprecate_with",
     "deprecate"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/memo.py` & `danielutils-0.9.77/danielutils/decorators/delay_call.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+from typing import Callable, TypeVar, Union
+import time
 import functools
-from typing import Callable, Any, TypeVar, Dict as t_dict
-from copy import deepcopy
-from .validate import validate
-
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from builtins import dict as t_dict
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+from .decorate_conditionally import decorate_conditionally
+from .threadify import threadify
+from ..versioned_imports import ParamSpec
+
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
-@validate
-def memo(func: FuncT) -> FuncT:
-    """decorator to memorize function calls in order to improve performance by using more memory
+def delay_call(seconds: Union[float, int], blocking: bool = True) -> Callable[[FuncT], FuncT]:
+    """will delay the call to a function by the given amount of seconds
 
     Args:
-        func (Callable): function to memorize
+        seconds (float | int): the amount of time to wait
+        blocking (bool, optional): whether to block the main thread
+        when waiting or to wait in a different thread. Defaults to True.
     """
-    cache: t_dict[tuple, Any] = {}
 
-    @ functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        if (args, *kwargs.items()) not in cache:
-            cache[(args, *kwargs.items())] = func(*args, **kwargs)
-        return deepcopy(cache[(args, *kwargs.items())])
-    return wrapper
+    def deco(func: FuncT) -> FuncT:
+        @decorate_conditionally(threadify, not blocking)
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            time.sleep(seconds)
+            func(*args, **kwargs)
+
+        return wrapper
+
+    return deco
 
 
 __all__ = [
-    "memo"
+    "delay_call"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/overload.py` & `danielutils-0.9.77/danielutils/decorators/overload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from typing import Callable, cast, Any, TypeVar, Dict as t_dict, List as t_list
 import inspect
 import functools
 from ..reflection import is_function_annotated_properly
 from ..functions import isoftype, isoneof, isoneof_strict
 from ..exceptions import OverloadDuplication, OverloadNotFound
 from .deprecate import deprecate
-from ..reflection import get_python_version
+from ..versioned_imports import ParamSpec, t_dict, t_list
 
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore# pylint: disable=ungrouped-imports
-    from builtins import dict as t_dict, list as t_list
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 T2 = TypeVar("T2")
 P2 = ParamSpec("P2")
 FuncT2 = Callable[P2, T2]  # type:ignore
```

### Comparing `danielutils-0.9.76/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.77/danielutils/decorators/partially_implemented.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from typing import Callable, Any, TypeVar
 import functools
 from .validate import validate
 from ..colors import warning
+from ..versioned_imports import ParamSpec
 
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 @validate
 def PartiallyImplemented(func: FuncT) -> FuncT:
     """decorator to mark function as not fully implemented for development purposes
 
     Args:
         func (Callable): the function to decorate
     """
 
-    @ functools.wraps(func)
+    @functools.wraps(func)
     def wrapper(*args, **kwargs) -> Any:
         warning(
             f"As marked by the developer, {func.__module__}.{func.__qualname__} "
             "may not be fully implemented and might not work properly.")
         return func(*args, **kwargs)
+
     return wrapper
 
 
 __all__ = [
     "PartiallyImplemented"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/processify.py` & `danielutils-0.9.77/danielutils/decorators/processify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/property.py` & `danielutils-0.9.77/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/singleton.py` & `danielutils-0.9.77/danielutils/decorators/singleton.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/threadify.py` & `danielutils-0.9.77/danielutils/decorators/threadify.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from typing import Callable, TypeVar
 import functools
 import threading
+from ..versioned_imports import ParamSpec
 
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 def threadify(func: FuncT) -> FuncT:
     """will modify the function that when calling it a new thread
@@ -18,16 +14,18 @@
 
     Args:
         func (Callable): the function to make a thread
 
     Returns:
         Callable: the modified function
     """
+
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         threading.Thread(target=func, args=args, kwargs=kwargs).start()
+
     return wrapper
 
 
 __all__ = [
     "threadify"
 ]
```

### Comparing `danielutils-0.9.76/danielutils/decorators/timeout.py` & `danielutils-0.9.77/danielutils/decorators/timeout.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import threading
 import functools
 from typing import Callable, TypeVar, Union
 from .validate import validate
-from ..reflection import get_python_version
+from ..versioned_imports import ParamSpec
 
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 @validate
 def timeout(duration: Union[int, float], silent: bool = False) -> Callable[[FuncT], FuncT]:
```

### Comparing `danielutils-0.9.76/danielutils/decorators/total_ordering.py` & `danielutils-0.9.77/danielutils/decorators/total_ordering.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/decorators/validate.py` & `danielutils-0.9.77/danielutils/decorators/validate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import functools
 import inspect
 from typing import Callable, get_type_hints, cast, TypeVar, Union
 from ..functions.isoftype import isoftype
 from ..reflection import get_function_return_type
-from ..exceptions import EmptyAnnotationException,\
+from ..exceptions import EmptyAnnotationException, \
     InvalidDefaultValueException, ValidationException, InvalidReturnValueException
-from ..reflection import get_python_version
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+from ..versioned_imports import ParamSpec
+
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 def validate(strict: Union[FuncT, bool] = True) -> FuncT:
     """A decorator that validates the annotations and types of the arguments and return
@@ -102,107 +99,109 @@
                 # why does this even happen?
                 return_type = get_type_hints(func)["return"]
             if return_type is not type(None) and not isoftype(result, return_type):
                 raise InvalidReturnValueException(
                     f"In function {func_name}, the return type is annotated as "
                     f"{return_type} but got '{result}' which is {type(result)}")
             return result
+
         return wrapper
+
     if callable(strict):
         func = strict
         strict = True
         return deco(func)
     return deco
 
 
 # def validate(func: Callable) -> Callable:
-    # """A decorator that validates the annotations and types of the arguments and return
-    # value of a function.
+# """A decorator that validates the annotations and types of the arguments and return
+# value of a function.
 
-    #     * 'None' is allowed as default value for everything
-    #     * Because of their use in better_builtins, the generally accepted keywords 'self' and 'cls'
-    #     are not validated to not break intellisense when using 'Any'
-
-    # Args:
-    #     func (Callable): The function to be decorated.
-
-    # Raises:
-    #     TypeError: if the decorated object is nto a Callable
-    #     EmptyAnnotationException: If an argument is not annotated.
-    #     InvalidDefaultValueException: If an argument's default value is not of the annotated type.
-    #     ValidationException: If an argument's value is not of the expected type.
-    #     InvalidReturnValueException: If the return value is not of the expected type.
-
-    # Returns:
-    #     Callable: A wrapper function that performs the validation and calls the original function.
-    # """
-    # SKIP_SET = {"self", "cls"}
-    # if not isinstance(func, Callable):
-    #     raise TypeError("The validate decorator must only decorate a function")
-    # func_name = f"{func.__module__}.{func.__qualname__}"
-    # # get the signature of the function
-    # signature = inspect.signature(func)
-    # for arg_name, arg_param in signature.parameters.items():
-    #     if arg_name not in SKIP_SET:
-    #         arg_type = arg_param.annotation
-    #         # check if an annotation is missing
-    #         if arg_type == inspect.Parameter.empty:
-    #             raise EmptyAnnotationException(
-    #                 f"In {func_name}, argument '{arg_name}' is not annotated")
-
-    #     # check if the argument has a default value
-    #     default_value = signature.parameters[arg_name].default
-    #     if default_value != inspect.Parameter.empty:
-    #         # allow everything to be set to None as default
-    #         if default_value is None:
-    #             continue
-    #         # if it does, check the type of the default value
-    #         if not isoftype(default_value, arg_type):
-    #             raise InvalidDefaultValueException(
-    #                 f"In {func_name}, argument '{arg_name}'s default value is annotated \
-    #                 as {arg_type} but got '{default_value}' which is {type(default_value)}")
-
-    # @functools.wraps(func)
-    # def wrapper(*args, **kwargs):
-    #     """wrapper function for the type validating - will run on each call independently
-    #     """
-    #     hints = None
-    #     # check all arguments
-    #     bound = signature.bind(*args, **kwargs)
-    #     for variable_name, variable_value in bound.arguments.items():
-    #         if variable_name in SKIP_SET:
-    #             continue
-    #         expected_type = func.__annotations__[variable_name]
-
-    #         if isinstance(expected_type, str):
-    #             # why does this even happen?
-    #             if hints is None:
-    #                 hints = get_type_hints(func)
-    #             expected_type = hints[variable_name]
-
-    #         if not isoftype(variable_value, expected_type):
-    #             raise ValidationException(
-    #                 f"In {func_name}, argument '{variable_name}' is annotated as \
-    #                     {expected_type} but got '{variable_value}' which is {type(variable_value)}")
-
-    #     # call the function
-    #     result = func(*args, **kwargs)
-
-    #     # check the return type
-    #     return_type = type(None) if ("inspect._empty" in str(signature.return_annotation)
-    #                                  or signature.return_annotation is None) else signature.return_annotation
-    #     if isinstance(return_type, str):
-    #         # why does this even happen?
-    #         return_type = get_type_hints(func)["return"]
-    #     if return_type is not type(None) and not isoftype(result, return_type):
-    #         raise InvalidReturnValueException(
-    #             f"In function {func_name}, the return type is annotated as "
-    #             f"{return_type} but got '{result}' which is {type(result)}")
-    #     return result
-    # return wrapper
+#     * 'None' is allowed as default value for everything
+#     * Because of their use in better_builtins, the generally accepted keywords 'self' and 'cls'
+#     are not validated to not break intellisense when using 'Any'
+
+# Args:
+#     func (Callable): The function to be decorated.
+
+# Raises:
+#     TypeError: if the decorated object is nto a Callable
+#     EmptyAnnotationException: If an argument is not annotated.
+#     InvalidDefaultValueException: If an argument's default value is not of the annotated type.
+#     ValidationException: If an argument's value is not of the expected type.
+#     InvalidReturnValueException: If the return value is not of the expected type.
+
+# Returns:
+#     Callable: A wrapper function that performs the validation and calls the original function.
+# """
+# SKIP_SET = {"self", "cls"}
+# if not isinstance(func, Callable):
+#     raise TypeError("The validate decorator must only decorate a function")
+# func_name = f"{func.__module__}.{func.__qualname__}"
+# # get the signature of the function
+# signature = inspect.signature(func)
+# for arg_name, arg_param in signature.parameters.items():
+#     if arg_name not in SKIP_SET:
+#         arg_type = arg_param.annotation
+#         # check if an annotation is missing
+#         if arg_type == inspect.Parameter.empty:
+#             raise EmptyAnnotationException(
+#                 f"In {func_name}, argument '{arg_name}' is not annotated")
+
+#     # check if the argument has a default value
+#     default_value = signature.parameters[arg_name].default
+#     if default_value != inspect.Parameter.empty:
+#         # allow everything to be set to None as default
+#         if default_value is None:
+#             continue
+#         # if it does, check the type of the default value
+#         if not isoftype(default_value, arg_type):
+#             raise InvalidDefaultValueException(
+#                 f"In {func_name}, argument '{arg_name}'s default value is annotated \
+#                 as {arg_type} but got '{default_value}' which is {type(default_value)}")
+
+# @functools.wraps(func)
+# def wrapper(*args, **kwargs):
+#     """wrapper function for the type validating - will run on each call independently
+#     """
+#     hints = None
+#     # check all arguments
+#     bound = signature.bind(*args, **kwargs)
+#     for variable_name, variable_value in bound.arguments.items():
+#         if variable_name in SKIP_SET:
+#             continue
+#         expected_type = func.__annotations__[variable_name]
+
+#         if isinstance(expected_type, str):
+#             # why does this even happen?
+#             if hints is None:
+#                 hints = get_type_hints(func)
+#             expected_type = hints[variable_name]
+
+#         if not isoftype(variable_value, expected_type):
+#             raise ValidationException(
+#                 f"In {func_name}, argument '{variable_name}' is annotated as \
+#                     {expected_type} but got '{variable_value}' which is {type(variable_value)}")
+
+#     # call the function
+#     result = func(*args, **kwargs)
+
+#     # check the return type
+#     return_type = type(None) if ("inspect._empty" in str(signature.return_annotation)
+#                                  or signature.return_annotation is None) else signature.return_annotation
+#     if isinstance(return_type, str):
+#         # why does this even happen?
+#         return_type = get_type_hints(func)["return"]
+#     if return_type is not type(None) and not isoftype(result, return_type):
+#         raise InvalidReturnValueException(
+#             f"In function {func_name}, the return type is annotated as "
+#             f"{return_type} but got '{result}' which is {type(result)}")
+#     return result
+# return wrapper
 
 # @validate
 # def NotImplemented(func: Callable) -> Callable:
 #     """decorator to mark function as not implemented for development purposes
 
 #     Args:
 #         func (Callable): the function to decorate
```

### Comparing `danielutils-0.9.76/danielutils/exceptions.py` & `danielutils-0.9.77/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/areoneof.py` & `danielutils-0.9.77/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/check_foreach.py` & `danielutils-0.9.77/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/flatten.py` & `danielutils-0.9.77/danielutils/functions/flatten.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/isoftype.py` & `danielutils-0.9.77/danielutils/functions/isoftype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from typing import get_args, get_origin, get_type_hints, Any, Union, TypeVar, \
-    ForwardRef, Literal, Optional, Tuple as t_tuple, Protocol
+    ForwardRef, Literal, Optional, Protocol
 from collections.abc import Callable, Generator, Iterable
 from ..reflection import get_python_version
+from ..versioned_imports import ParamSpec, Concatenate, t_tuple
 
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec, Concatenate
-else:
-
-    # pylint: disable=ungrouped-imports
-    from typing import ParamSpec, Concatenate  # type:ignore
-    from builtins import tuple as t_tuple  # type:ignore
 # implicit_union_type = type(int | str)
 concatenate_t = type(Concatenate[str, ParamSpec("P_")])
 ellipsis_ = ...
 
 
 def __isoftype_inquire(obj: Any) -> t_tuple[Optional[type], Optional[tuple], Optional[dict]]:
     """
@@ -170,15 +164,15 @@
         return not strict
 
     if t_args is None:
         return True
     if len(t_args) == 0:
         return True
 
-    if get_python_version() < (3, 9):
+    if get_python_version() < (3, 10):
         if isoftype(t_args[0][0], [ParamSpec, concatenate_t]):
             return True
     else:
         if isoftype(t_args[0], [ParamSpec, concatenate_t]):
             return True
 
     obj_return_type = obj_hints.get('return')
```

### Comparing `danielutils-0.9.76/danielutils/functions/isoneof.py` & `danielutils-0.9.77/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/multiloop.py` & `danielutils-0.9.77/danielutils/functions/multiloop.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/powerset.py` & `danielutils-0.9.77/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/functions/types_subseteq.py` & `danielutils-0.9.77/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/generators/conditional_generator.py` & `danielutils-0.9.77/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/generators/join_generators.py` & `danielutils-0.9.77/danielutils/generators/join_generators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/internet.py` & `danielutils-0.9.77/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/io_.py` & `danielutils-0.9.77/danielutils/io_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/math_/constants.py` & `danielutils-0.9.77/danielutils/math_/constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/math_/functions.py` & `danielutils-0.9.77/danielutils/math_/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/math_/math_print.py` & `danielutils-0.9.77/danielutils/math_/math_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/math_/math_symbols.py` & `danielutils-0.9.77/danielutils/math_/math_symbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/math_/polynomial/polinomial.py` & `danielutils-0.9.77/danielutils/math_/polynomial/polinomial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from typing import TypeVar
+from typing import TypeVar, List as t_list
 from copy import deepcopy
 from fractions import Fraction
+from ...reflection import get_python_version
 
+if get_python_version() >= (3, 9):
+    from builtins import list as t_list
+    from builtins import dict as t_dict
 from ...print_ import mprint
+
 Number = TypeVar("Number", int, float, Fraction, complex)
 
 
 class Polynomial:
-    def __init__(self, coefficients: list[Number], powers: list[Number]):
+    def __init__(self, coefficients: t_list[Number], powers: t_list[Number]):
         self._coefficients = coefficients
         self._powers = powers
 
     @property
-    def coefficients(self) -> list[Fraction]:
+    def coefficients(self) -> t_list[Fraction]:
         return deepcopy(self._coefficients)
 
     @property
-    def powers(self) -> list[Fraction]:
+    def powers(self) -> t_list[Fraction]:
         return deepcopy(self._powers)
 
     def __len__(self):
         return len(self.coefficients)
 
-__all__=[
+
+__all__ = [
     "Polynomial"
-]
+]
```

### Comparing `danielutils-0.9.76/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.77/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.77/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.77/danielutils/metaclasses/instance_cache_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/metaclasses/interface.py` & `danielutils-0.9.77/danielutils/metaclasses/interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.77/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/mock_/mock_database.py` & `danielutils-0.9.77/danielutils/mock_/mock_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/path.py` & `danielutils-0.9.77/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/print_.py` & `danielutils-0.9.77/danielutils/print_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/reflection/__init__.py` & `danielutils-0.9.77/danielutils/reflection/__init__.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/reflection/class_/class_reflection.py` & `danielutils-0.9.77/danielutils/reflection/class_/class_reflection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import inspect, re
-from typing import Any, List as t_list, Optional
+from typing import Any, List as t_list, Optional, Tuple as t_tuple
+from dataclasses import dataclass
 from ..interpreter import get_python_version
 
+argument_kwargs = dict(frozen=True)
+FunctionDeclaration_kwargs = dict(frozen=True)
 if get_python_version() >= (3, 9):
-    from builtins import list as t_list  # type:ignore
+    from builtins import list as t_list, tuple as t_tuple  # type:ignore
+
+elif get_python_version() >= (3, 10):
+    argument_kwargs.update(slots=True)
+    FunctionDeclaration_kwargs.update(slots=True)
 
 
 def get_explicitly_declared_functions(cls: type) -> t_list[str]:
     """
     Returns the names of the functions that are explicitly declared in a class.
 
     This function does not return inherited functions.
@@ -31,33 +38,30 @@
         list[type]: the resulting mro for the object
     """
     if isinstance(obj, type):
         return obj.mro()
     return get_mro(obj.__class__)
 
 
-from dataclasses import dataclass
-
-
-@dataclass(frozen=True, slots=True)
+@dataclass(**argument_kwargs)
 class Argument:
     name: str
     type: Optional[str]
     default: Optional[str]
 
 
 func_pattern = re.compile(
     r"(.*def[\s\\]*?(\w+)[\s\\]*?\(([\w\W]*?)\)(?:[\s\\]*?->[\s\\]*?([\w\(\)\[\]\,]+))?[\s\\]*?:)",
     flags=re.MULTILINE)
 not_whitespace_pattern = re.compile(r"\S+", flags=re.MULTILINE)
 arg_pattern = re.compile(r"([\w\*\/]+)(?:\s*?:\s*?([\w\[\]\(\)\,]+))?(?:\s*?=\s*?(.+))?")
 class_pattern = re.compile(r"\s*class\s+?\w+\s*?(?:\((.*)\))?\s*?:")
 
 
-def split_args(args: str) -> list[str]:
+def split_args(args: str) -> t_list[str]:
     from danielutils import Stack
     res = []
     s: Stack[str] = Stack()
     start = 0
     for i, c in enumerate(args):
         if c not in {'(', ')', '[', ']', ','}:
             continue
@@ -74,21 +78,21 @@
     return res
 
 
 def remove_whitespace(text: str) -> str:
     return "".join(not_whitespace_pattern.findall(text.strip())).replace("\\", "")
 
 
-@dataclass(frozen=True, slots=True)
+@dataclass(**FunctionDeclaration_kwargs)
 class FunctionDeclaration:
     name: str
-    arguments: tuple[Argument, ...]
+    arguments: t_tuple[Argument, ...]
     return_type: Optional[str]
-    decorators: Optional[list[str]] = None
-    generics: Optional[tuple[str]] = None
+    decorators: Optional[t_list[str]] = None
+    generics: Optional[t_tuple[str]] = None
 
     def duplicate(self, **override_kwargs) -> 'FunctionDeclaration':
         dct = dict(
             name=self.name,
             arguments=self.arguments,
             return_type=self.return_type,
             decorators=self.decorators,
@@ -98,15 +102,15 @@
         return FunctionDeclaration(**dct)
 
     @property
     def has_generics(self) -> bool:
         return self.generics is not None and len(self.generics) > 0
 
     @staticmethod
-    def get_declared_functions(cls) -> list['FunctionDeclaration']:
+    def get_declared_functions(cls) -> t_list['FunctionDeclaration']:
         """will yield the names of all the functions declared inside a class
 
         Yields:
             Generator[str, None, None]: yields str values which are names of declared functions
         """
         if not isinstance(cls, type):
             raise TypeError('cls must be a Class')
```

### Comparing `danielutils-0.9.76/danielutils/reflection/file/file_reflection.py` & `danielutils-0.9.77/danielutils/reflection/file/file_reflection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 import inspect
 import os
 from typing import Optional, cast
 from types import FrameType
 from ..interpreter.callstack import _get_prev_frame_from
 
 
-def get_filename() -> Optional[str]:
-    """returns the name of the file that this functions is called from
+def get_caller_file_name() -> Optional[str]:
+    """return the name of the file that the caller of the
+    function that's using this function is in
 
     Returns:
         Optional[str]: name of file
     """
-    frame = _get_prev_frame_from(inspect.currentframe())
+    frame = _get_prev_frame_from(_get_prev_frame_from(inspect.currentframe()))
     if frame is None:
         return None
     frame = cast(FrameType, frame)
     return frame.f_code.co_filename
 
 
-def get_caller_filename() -> Optional[str]:
-    """return the name of the file that the caller of the 
-    function that's using this function is in
+def get_current_file_path() -> Optional[str]:
+    """returns the name of the file that this functions is called from
 
     Returns:
         Optional[str]: name of file
     """
-    frame = _get_prev_frame_from(_get_prev_frame_from(inspect.currentframe()))
-    if frame is None:
-        return None
-    frame = cast(FrameType, frame)
-    return frame.f_code.co_filename
+    return get_caller_file_name()
+
+
+def get_current_file_name() -> Optional[str]:
+    if (filepath := get_caller_file_name()) is None: return None
+    return filepath.split('\\')[-1]
+
+
+def get_current_folder_path() -> Optional[str]:
+    if (filepath := get_caller_file_name()) is None: return None
+    return "\\".join(filepath.split("\\")[:-1])
+
+
+def get_current_folder_name() -> Optional[str]:
+    if (filepath := get_caller_file_name()) is None: return None
+    return filepath.split("\\")[-2]
 
 
 def get_current_directory() -> str:
     """returns the name of the directory of main script"""
-    return os.path.dirname(os.path.abspath(get_caller_filename()))  # type:ignore # noqa
+    return os.path.dirname(os.path.abspath(get_caller_file_name()))  # type:ignore # noqa
 
 
 __all__ = [
-    "get_filename",
-    "get_caller_filename",
+    "get_current_file_path",
+    "get_current_file_name",
+    "get_current_folder_path",
+    "get_current_folder_name",
+    "get_caller_file_name",
     'get_current_directory',
 ]
```

### Comparing `danielutils-0.9.76/danielutils/reflection/function/function_reflections.py` & `danielutils-0.9.77/danielutils/reflection/function/function_reflections.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/reflection/interpreter/os_.py` & `danielutils-0.9.77/danielutils/reflection/interpreter/os_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/reflection/interpreter/packages.py` & `danielutils-0.9.77/danielutils/reflection/interpreter/packages.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/reflection/interpreter/python_version.py` & `danielutils-0.9.77/danielutils/reflection/interpreter/python_version.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/reflection/interpreter/tracer.py` & `danielutils-0.9.77/danielutils/reflection/interpreter/tracer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import sys
 from abc import ABC, abstractmethod
 from enum import Enum
 from types import FrameType
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Set as t_set, Dict as t_dict
+from .python_version import get_python_version
+
+if get_python_version() >= (3, 9):
+    from builtins import set as t_set, dict as t_dict
 
 
 # from danielutils import singleton
 # @singleton
 class Tracer(ABC):
     """
     A class to trace (during runtime) the flow of the currently executing code
@@ -39,18 +43,18 @@
             skip_c_call: bool = True,
             skip_c_return: bool = True,
             functions: bool = True,
             classes: bool = True,
             instance_methods: bool = True,
             static_methods: bool = True,
             class_methods: bool = True,
-            exclude: Optional[set[str]] = None
+            exclude: Optional[t_set[str]] = None
     ) -> None:
 
-        self._call_dict: dict[Tracer.EventType, Callable] = {
+        self._call_dict: t_dict[Tracer.EventType, Callable] = {
             Tracer.EventType.CALL: self.on_call,
             Tracer.EventType.C_CALL: self.on_call_c,
             Tracer.EventType.RETURN: self.on_return,
             Tracer.EventType.C_RETURN: self.on_return_c,
         }
         self._skip_call = skip_call
         self._skip_return = skip_return
```

### Comparing `danielutils-0.9.76/danielutils/reflection/module/package_reflection.py` & `danielutils-0.9.77/danielutils/reflection/module/package_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/system/independent.py` & `danielutils-0.9.77/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.77/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/system/windows/windows.py` & `danielutils-0.9.77/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/text.py` & `danielutils-0.9.77/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/time.py` & `danielutils-0.9.77/danielutils/time.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import time
 from datetime import datetime
 from typing import Callable, TypeVar
-from .reflection import get_python_version
+from .versioned_imports import ParamSpec
 
-if get_python_version() < (3, 9):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def measure(func: Callable[P, T]) -> Callable[P, float]:
     """A function to measure the execution time of a function.
```

### Comparing `danielutils-0.9.76/danielutils/tqdm_.py` & `danielutils-0.9.77/danielutils/tqdm_.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .reflection import get_python_version
 
 if get_python_version() >= (3, 9):
     from builtins import list as t_list  # type:ignore
 try:
     from tqdm import tqdm
 except ImportError:
-    from .imports import MockImportObject
+    from .mock_ import MockImportObject
 
     tqdm = MockImportObject("`tqdm` is not installed")  # type:ignore
 
 
 class ProgressBarPool:
     """
     My attempt at creating a progress bar pool using tqdm
```

### Comparing `danielutils-0.9.76/danielutils/university/databases/all.py` & `danielutils-0.9.77/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/university/oop/observer.py` & `danielutils-0.9.77/danielutils/university/oop/observer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/conditional_variable.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/conditional_variable.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 from fractions import Fraction
 from typing import Callable, Any
 from ..expressions import ProbabilityExpression, AccumulationExpression
 from ..operator import Operator
 from ..supp import Supp
 from ..protocols import Evaluable
 
+def _create_operator(op: Operator, reverse: bool = False) -> Callable[['ConditionalVariable', Any], Evaluable]:
+    def operator(self, other) -> Evaluable:
+        lhs, rhs = self, other
+        if reverse:
+            lhs, rhs = rhs, lhs
+
+        if isinstance(other, (int, float, Fraction)):
+            return ProbabilityExpression(lhs, op, rhs)
+
+        if isinstance(rhs, ProbabilityExpression):
+            l = ProbabilityExpression(lhs, op, rhs.lhs)
+            r = ProbabilityExpression(rhs.rhs, None, None)
+            o = other.op
+            return AccumulationExpression(l, o, r)
 
-class ConditionalVariable(ABC):
-    OPERATOR_TYPE = Callable[['ConditionalVariable', Any], Evaluable]
+        # if isinstance(rhs, ConditionalVariable):
+        #     return AccumulationExpression(ProbabilityExpression(lhs), op, ProbabilityExpression(rhs))
 
-    @staticmethod
-    def _create_operator(op: Operator, reverse: bool = False) -> Callable[['ConditionalVariable', Any], Evaluable]:
-        def operator(self, other) -> Evaluable:
-            lhs, rhs = self, other
-            if reverse:
-                lhs, rhs = rhs, lhs
-
-            if isinstance(other, (int, float, Fraction)):
-                return ProbabilityExpression(lhs, op, rhs)
-
-            if isinstance(rhs, ProbabilityExpression):
-                l = ProbabilityExpression(lhs, op, rhs.lhs)
-                r = ProbabilityExpression(rhs.rhs, None, None)
-                o = other.op
-                return AccumulationExpression(l, o, r)
+        raise NotImplementedError("Not Implemented")
 
-            # if isinstance(rhs, ConditionalVariable):
-            #     return AccumulationExpression(ProbabilityExpression(lhs), op, ProbabilityExpression(rhs))
+    return operator
 
-            raise NotImplementedError("Not Implemented")
+class ConditionalVariable(ABC):
+    OPERATOR_TYPE = Callable[['ConditionalVariable', Any], Evaluable]
 
-        return operator
 
     __eq__: OPERATOR_TYPE = _create_operator(Operator.EQ)
     __ne__: OPERATOR_TYPE = _create_operator(Operator.NE)
     __gt__: OPERATOR_TYPE = _create_operator(Operator.GT)
     __ge__: OPERATOR_TYPE = _create_operator(Operator.GE)
     __lt__: OPERATOR_TYPE = _create_operator(Operator.LT)
     __le__: OPERATOR_TYPE = _create_operator(Operator.LE)
@@ -53,21 +52,44 @@
     __radd__: OPERATOR_TYPE = _create_operator(Operator.ADD, reverse=True)
     __sub__: OPERATOR_TYPE = _create_operator(Operator.SUB)
     __rsub__: OPERATOR_TYPE = _create_operator(Operator.SUB, reverse=True)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}"
 
-    def is_dependent(self, other) -> bool:
+    def is_identical(self, other) -> bool:
         if not isinstance(other, ConditionalVariable):
             return False
         return self is other
 
     def is_independent(self, other) -> bool:
-        return not self.is_dependent(other)
+        if not isinstance(other, ConditionalVariable):
+            return False
+        if not self.supp.is_finite and not other.supp.is_finite:
+            raise ValueError("Can't check if two variables are independent if their supp is not finite")
+
+        if self.supp != other.supp:
+            return False
+        from ..funcs import probability_function as P
+        for k in self.supp:
+            if not (P((self == k) & (other == k)) == P(self == k) * P(other == k)):
+                return False
+        return True
+
+    def is_dependent(self, other) -> bool:
+        return not self.is_independent(other)
+
+    def is_correlated(self, other) -> bool:
+        if not isinstance(other, ConditionalVariable):
+            return False
+        from ..funcs import covariance as cov
+        return cov(self, other) == 0
+
+    def is_uncorrelated(self, other) -> bool:
+        return not self.is_correlated(other)
 
     @abstractmethod
     def evaluate(self, other: Any, operator: Operator) -> Fraction:
         ...
 
     @abstractmethod
     def between(self, a, b, *args) -> Fraction:
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/bernoulli.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/uniform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from fractions import Fraction
 
-from .discrete import DiscreteConditionalVariable
-from ...supp import DiscreteSupp
+from ...supp import FrangeSupp
 from ...operator import Operator
+
+from .discrete import DiscreteConditionalVariable
 from ...protocols import ExpectedValueCalculable, VariableCalculable
 
 
-class Bernoulli(DiscreteConditionalVariable, ExpectedValueCalculable, VariableCalculable):
+class Uniform(DiscreteConditionalVariable, ExpectedValueCalculable, VariableCalculable):
     def evaluate(self, n: int, op: Operator) -> Fraction:
         if n not in self.supp:
-            return 0
+            return Fraction(0, 1)
 
         if op == Operator.EQ:
-            return self.p if n == 1 else 1 - self.p
-        assert False  # TODO
+            return self.p
 
-        return 1 - self.evaluate(n, op.inverse)
+        assert False  # TODO
+        return self.evaluate(n, op.inverse)
 
-    def __init__(self, p) -> None:
-        super().__init__(p, DiscreteSupp(range(0, 2)))
+    def __init__(self, size) -> None:
+        super().__init__(Fraction(1, size), FrangeSupp(range(1, size + 1)))
 
     def expected_value(self) -> Fraction:
-        return self.p
+        return Fraction(Fraction.from_float(self.supp.minimum + self.supp.maximum), 2)
 
     def variance(self) -> Fraction:
-        return self.p * (1 - self.p)
-
+        return Fraction(
+            Fraction.from_float((self.supp.maximum - self.supp.minimum - 1) ** 2 - 1),
+            12
+        )
 
-__all__ = ['Bernoulli']
+    __all__ = ['Uniform']
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/binomial.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/binomial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from fractions import Fraction
 from typing import Union
 from math import factorial
 from .discrete import DiscreteConditionalVariable
-from ...supp import DiscreteSupp
+from ...supp import FrangeSupp
 from ...operator import Operator
 from .....better_builtins import frange
 from ...protocols import ExpectedValueCalculable, VariableCalculable
 
 
 def choose(n: int, k: int) -> Fraction:
     return Fraction(factorial(n), (factorial(k) * factorial(n - k)))
 
 
 class Binomial(DiscreteConditionalVariable, ExpectedValueCalculable, VariableCalculable):
     def __init__(self, n: int, p: Union[float, Fraction]):
-        super().__init__(p, DiscreteSupp(frange(0, float("inf"))))
+        super().__init__(p, FrangeSupp(frange(0, float("inf"))))
         self._n = n
 
     @property
     def n(self) -> int:
         return self._n
 
     def evaluate(self, k: int, op: Operator) -> Fraction:
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/conditional_from_discrete_probability_func.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable
 from fractions import Fraction
 from .discrete import DiscreteConditionalVariable
-from ...supp import DiscreteSupp
+from ...supp import FrangeSupp
 from ...operator import Operator
 
 
 class ConditionalFromDiscreteProbabilityFunc(DiscreteConditionalVariable):
     def evaluate(self, n: int, op: Operator) -> Fraction:
         if op == Operator.EQ:
             return self.f(n)
@@ -15,15 +15,15 @@
                 res += self.evaluate(k, Operator.EQ)
             return res
         if op == Operator.LE:
             return self.evaluate(n, Operator.LT) + self.evaluate(n, Operator.EQ)
 
         return 1 - self.evaluate(n, op.inverse)
 
-    def __init__(self, p: Callable[[int], Fraction], supp: DiscreteSupp) -> None:
+    def __init__(self, p: Callable[[int], Fraction], supp: FrangeSupp) -> None:
         super().__init__(None, supp)
         self.f = p
 
     @property
     def p(self):
         raise AttributeError(f"{self.__class__.__name__} has no attribute 'p'")
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/discrete.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/discrete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from fractions import Fraction
 from typing import Union
 
 from ..conditional_variable import ConditionalVariable
-from ...supp import DiscreteSupp
+from ...supp import FrangeSupp
 from ...operator import Operator
 
 
 class DiscreteConditionalVariable(ConditionalVariable):
 
-    def __init__(self, p: Union[float, Fraction], supp: DiscreteSupp):
+    def __init__(self, p: Union[float, Fraction], supp: FrangeSupp):
         self._p: Fraction = p if isinstance(p, Fraction) else Fraction.from_float(p)
-        self._supp: DiscreteSupp = supp
+        self._supp: FrangeSupp = supp
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.p})"
 
     @property
-    def supp(self) -> DiscreteSupp:
+    def supp(self) -> FrangeSupp:
         return self._supp
 
     @property
     def p(self) -> Fraction:
         return self._p
 
     def between(self, a, b, op1: Operator, op2: Operator) -> Fraction:
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/geometric.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/geometric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from fractions import Fraction
-from typing import Union
+from typing import Union, Tuple as t_tuple
 
 from .discrete import DiscreteConditionalVariable
 from ...operator import Operator
 from .....better_builtins import frange
-from ...supp import DiscreteSupp
+from ...supp import FrangeSupp
 from ...protocols import ExpectedValueCalculable, VariableCalculable
+from .....reflection import get_python_version
+
+
+if get_python_version() >= (3, 9):
+    from builtins import tuple as t_tuple
 
 
 class Geometric(DiscreteConditionalVariable, ExpectedValueCalculable, VariableCalculable):
     def __init__(self, p: Union[float, Fraction]):
-        super().__init__(Fraction(p), DiscreteSupp(frange(1, float("inf"), 1)))
+        super().__init__(Fraction(p), FrangeSupp(frange(1, float("inf"), 1)))
 
-    def _is_edge_case(self, n: int, op: Operator) -> tuple[bool, Fraction]:
+    def _is_edge_case(self, n: int, op: Operator) -> t_tuple[bool, Fraction]:
         if n <= 0 and op in Operator.greater_than_inequalities():
             return True, Fraction(1, 1)
         if n <= 0 and op in Operator.less_than_inequalities():
             return True, Fraction(0, 1)
         return False, Fraction(0, 1)
 
     def evaluate(self, n: int, op: Operator) -> Fraction:
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/poisson.py` & `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/poisson.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from fractions import Fraction
 from typing import Union
 from math import e, factorial
 
 from .discrete import DiscreteConditionalVariable
-from ...supp import DiscreteSupp
+from ...supp import FrangeSupp
 from ...operator import Operator
 from .....better_builtins import frange
 from ...protocols import ExpectedValueCalculable, VariableCalculable
 
 
 class Poisson(DiscreteConditionalVariable, ExpectedValueCalculable, VariableCalculable):
     def __init__(self, p: Union[float, Fraction]):
-        super().__init__(p, DiscreteSupp(frange(1, float("inf"))))
+        super().__init__(p, FrangeSupp(frange(1, float("inf"))))
 
     def evaluate(self, n: int, op: Operator) -> Fraction:
         if n < 0:
             return Fraction(0, 1)
         if op == Operator.EQ:
             return Fraction((e ** (-self.p)) * (self.p ** n), factorial(n))
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/conditional_variables/discrete/uniform.py` & `danielutils-0.9.77/danielutils/university/probability/funcs/expected_value.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-from fractions import Fraction
-
-from ...supp import DiscreteSupp
-from ...operator import Operator
-
-from .discrete import DiscreteConditionalVariable
-from ...protocols import ExpectedValueCalculable, VariableCalculable
-
-
-class Uniform(DiscreteConditionalVariable, ExpectedValueCalculable, VariableCalculable):
-    def evaluate(self, n: int, op: Operator) -> Fraction:
-        if n not in self.supp:
-            return Fraction(0, 1)
+from typing import Union
 
-        if op == Operator.EQ:
-            return self.p
-
-        assert False  # TODO
-        return self.evaluate(n, op.inverse)
-
-    def __init__(self, size) -> None:
-        super().__init__(Fraction(1, size), DiscreteSupp(range(1, size + 1)))
-
-    def expected_value(self) -> Fraction:
-        return Fraction(Fraction.from_float(self.supp.start + self.supp.stop), 2)
+from fractions import Fraction
+from ..conditional_variable import ConditionalVariable
+from .probability_function import probability_function as P
+from ..expressions import ProbabilityExpression
+from ..operator import Operator
+from ..protocols import ExpectedValueCalculable
+
+
+def expected_value(obj: Union[ConditionalVariable, ProbabilityExpression]) -> Fraction:
+    if isinstance(obj, ExpectedValueCalculable):
+        return obj.expected_value()
+    res = Fraction(0, 1)
+    if isinstance(obj, ConditionalVariable):
+        X = obj
+        for n in X.supp:
+            res += n * P(X == n)
+        return res
+    if isinstance(obj.rhs, int):
+        const = obj.rhs
+        op = obj.op
+        X = obj.lhs
+
+        def f(n):
+            return {
+                Operator.POW: lambda n: n ** const,
+                Operator.MUL: lambda n: n * const,
+                Operator.DIV: lambda n: n / const,
+                Operator.MODULUS: lambda n: n & const,
+            }[op](n)
+
+        for n in X.supp:
+            res += f(n) * P(X == n)
+        return res
+    assert False
 
-    def variance(self) -> Fraction:
-        return Fraction(
-            Fraction.from_float((self.supp.stop - self.supp.start - 1) ** 2 - 1),
-            12
-        )
 
-    __all__ = ['Uniform']
+__all__ = ['expected_value']
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/distributions.py` & `danielutils-0.9.77/danielutils/university/probability/distributions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
-from .conditional_variables import ConditionalVariable
-from .conditional_variables.discrete import Bernoulli, Geometric, Uniform, Binomial, Poisson
+from .conditional_variable import ConditionalVariable
+from .conditional_variable.discrete import Bernoulli, Geometric, Uniform, Binomial, Poisson
 
 
 class DiscreteDistribution(Enum):
     Ber = Bernoulli
     Geo = Geometric
     Unif = Uniform
     Bin = Binomial
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/expressions/accumulation_expression.py` & `danielutils-0.9.77/danielutils/university/probability/expressions/accumulation_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 from fractions import Fraction
 from typing import Callable, Any, Union, Optional
 from .probability_expression import ProbabilityExpression
 from ..protocols import Evaluable, Equatable
 from ..operator import Operator
 from ....data_structures import BinarySyntaxTree as BST
 
-
-class AccumulationExpression(Evaluable):
-    @staticmethod
-    def _probability_expression_to_nodes(expr: ProbabilityExpression) -> BST.Node:
-        return BST.Node(expr.op, BST.Node(expr.lhs), BST.Node(expr.rhs))
-
-    @staticmethod
-    def _create_operator(op: Operator, reverse: bool = False) -> Callable[['AccumulationExpression', Any], Evaluable]:
+def _create_operator(op: Operator, reverse: bool = False) -> Callable[['AccumulationExpression', Any], Evaluable]:
         def operator(self, other) -> Evaluable:
             op
             lhs, rhs = self, other
             if reverse:
                 lhs, rhs = rhs, lhs
             raise NotImplementedError("Not Implemented")
 
         return operator
 
+class AccumulationExpression(Evaluable):
+    @staticmethod
+    def _probability_expression_to_nodes(expr: ProbabilityExpression) -> BST.Node:
+        return BST.Node(expr.op, BST.Node(expr.lhs), BST.Node(expr.rhs))
+
+
     @staticmethod
     def _expression_intersection(expr1: ProbabilityExpression, expr2: ProbabilityExpression) -> Fraction:
         if expr1.is_equal(expr2):
             return expr1.evaluate()
 
         a = expr1.rhs
         op1 = expr1.op
@@ -87,15 +86,15 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(lhs={self._tree.root.left}, op={self._tree.root.data}, rhs={self._tree.root.right})"
 
     def is_equal(self, other) -> bool:
         if not isinstance(other, AccumulationExpression):
             return False
-        from ..conditional_variables import ConditionalVariable
+        from ..conditional_variable import ConditionalVariable
         # I have to create a custom comparer because the BST can't (and shouldn't) know to compare using
         # ConditionalVariable.is_equal
         def are_nodes_equal(a: Any, b: Any) -> bool:
             if not (isinstance(a, BST.Node) and isinstance(b, BST.Node)):
                 if a is None and b is None:
                     return True
                 return False
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/expressions/probability_expression.py` & `danielutils-0.9.77/danielutils/university/probability/expressions/probability_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 from typing import Any, Callable, Optional
 from fractions import Fraction
 from ..protocols import Evaluable
 from ..operator import Operator
 
 
+def _create_operator(op: Operator, reverse: bool = False) -> Callable[['ConditionalVariable', Any], Evaluable]:
+    def operator(self: 'ProbabilityExpression', other: Any) -> Evaluable:
+        lhs, rhs = self, other
+        if reverse:
+            lhs, rhs = rhs, lhs
+        from .accumulation_expression import AccumulationExpression
+
+        if op in Operator.order_operators():
+            if isinstance(rhs, (int, float, Fraction)):
+                if op in Operator.inequalities():
+                    rhs = ProbabilityExpression(lhs.lhs, op, rhs)
+                    return AccumulationExpression(lhs, Operator.AND, rhs)
+                elif op == Operator.EQ:
+                    return AccumulationExpression(lhs, op, ProbabilityExpression(rhs))
+            elif isinstance(rhs, (ProbabilityExpression, AccumulationExpression)):
+                if isinstance(other, ProbabilityExpression):
+                    # TODO P((0<X)<(Y<5))
+                    # I think that this is the solution
+                    return AccumulationExpression(self, op, other)
+            raise NotImplementedError("Illegal state")
+        if op in {Operator.AND, Operator.GIVEN}:
+            if not isinstance(other, ProbabilityExpression):
+                raise NotImplementedError("Illegal state")
+            return AccumulationExpression(lhs, op, rhs)
+        raise NotImplementedError("Illegal state 2")
+
+    return operator
 class ProbabilityExpression(Evaluable):
     OPERATOR_TYPE = Callable[['ProbabilityExpression', Any], 'AccumulationExpression']
 
-    @staticmethod
-    def _create_operator(op: Operator, reverse: bool = False) -> Callable[['ConditionalVariable', Any], Evaluable]:
-        def operator(self: 'ProbabilityExpression', other: Any) -> Evaluable:
-            lhs, rhs = self, other
-            if reverse:
-                lhs, rhs = rhs, lhs
-            from .accumulation_expression import AccumulationExpression
-
-            if op in Operator.order_operators():
-                if isinstance(rhs, (int, float, Fraction)):
-                    if op in Operator.inequalities():
-                        rhs = ProbabilityExpression(lhs.lhs, op, rhs)
-                        return AccumulationExpression(lhs, Operator.AND, rhs)
-                    elif op == Operator.EQ:
-                        return AccumulationExpression(lhs, op, ProbabilityExpression(rhs))
-                elif isinstance(rhs, (ProbabilityExpression, AccumulationExpression)):
-                    if isinstance(other, ProbabilityExpression):
-                        # TODO P((0<X)<(Y<5))
-                        # I think that this is the solution
-                        return AccumulationExpression(self, op, other)
-                raise NotImplementedError("Illegal state")
-            if op in {Operator.AND, Operator.GIVEN}:
-                if not isinstance(other, ProbabilityExpression):
-                    raise NotImplementedError("Illegal state")
-                return AccumulationExpression(lhs, op, rhs)
-            raise NotImplementedError("Illegal state 2")
-
-        return operator
 
     def __init__(self, lhs: Evaluable, op: Optional[Operator] = None, rhs: Optional[Any] = None):
         self._lhs = lhs
         self._op = op
         self._rhs = rhs
 
     __eq__: OPERATOR_TYPE = _create_operator(Operator.EQ)
@@ -76,15 +75,15 @@
     def evaluate(self) -> Fraction:
         return self.lhs.evaluate(self.rhs, self.op)
 
     def is_equal(self, other) -> bool:
         if not isinstance(other, ProbabilityExpression):
             raise TypeError(
                 f"Cant compare equality between {self.__class__.__qualname__} and non ConditionalExpression")
-        from ..conditional_variables import ConditionalVariable
+        from ..conditional_variable import ConditionalVariable
         if isinstance(self.lhs, ConditionalVariable) and not isinstance(other.lhs, ConditionalVariable):
             return False
         if not isinstance(self.lhs, ConditionalVariable) and isinstance(other.lhs, ConditionalVariable):
             return False
         # We need this complicated thing instead of doing self.lhs == other.lhs (and same for rhs) because we
         # cant use __eq__
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/operator.py` & `danielutils-0.9.77/danielutils/university/probability/operator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 from enum import Enum
+from typing import Set as t_set
+from ...reflection import get_python_version
+
+if get_python_version() >= (3, 9):
+    from builtins import set as t_set
 
 
 class Operator(Enum):
     """
     Operator Enum to define the types of operators.
     """
     EQ = "=="
     NE = "!="
     GT = ">"
     GE = ">="
     LT = "<"
     LE = "<="
 
     @staticmethod
-    def strong_inequalities() -> set['Operator']:
+    def strong_inequalities() -> t_set['Operator']:
         return {Operator.GT, Operator.LT}
 
     @staticmethod
-    def weak_inequalities() -> set['Operator']:
+    def weak_inequalities() -> t_set['Operator']:
         return {Operator.GE, Operator.LE}
 
     @staticmethod
-    def inequalities() -> set['Operator']:
+    def inequalities() -> t_set['Operator']:
         return Operator.strong_inequalities().union(Operator.weak_inequalities())
 
     @staticmethod
-    def equalities() -> set['Operator']:
+    def equalities() -> t_set['Operator']:
         return {Operator.EQ, Operator.NE}
 
     @staticmethod
-    def greater_than_inequalities() -> set['Operator']:
+    def greater_than_inequalities() -> t_set['Operator']:
         return {Operator.GE, Operator.GT}
 
     @staticmethod
-    def less_than_inequalities() -> set['Operator']:
+    def less_than_inequalities() -> t_set['Operator']:
         return {Operator.LE, Operator.LT}
 
     @staticmethod
-    def order_operators() -> set['Operator']:
+    def order_operators() -> t_set['Operator']:
         return Operator.inequalities().union(Operator.equalities())
 
     MUL = "*"
     DIV = "/"
     MODULUS = "%"
     GIVEN = '|'
     AND = '&'
```

### Comparing `danielutils-0.9.76/danielutils/university/probability/protocols.py` & `danielutils-0.9.77/danielutils/university/probability/protocols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.76/danielutils/university/probability/supp.py` & `danielutils-0.9.77/danielutils/university/probability/supp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod, ABC
 from typing import Iterator, TypeVar, Union
 from ...better_builtins import frange
-
+from ...decorators import memo
 T = TypeVar('T')
 
 
 class Supp(ABC, Iterator[T]):
     @property
     @abstractmethod
     def is_finite(self) -> bool: ...
@@ -14,58 +14,87 @@
         return not self.is_finite
 
     @abstractmethod
     def __contains__(self, item) -> bool: ...
 
     @property
     @abstractmethod
-    def start(self) -> float: ...
+    def minimum(self) -> float: ...
 
     @property
     @abstractmethod
-    def stop(self) -> float: ...
+    def maximum(self) -> float: ...
 
 
 class DiscreteSupp(Supp[int]):
+    pass
+
+
+class FrangeSupp(DiscreteSupp):
     @property
     def is_finite(self) -> bool:
         if isinstance(self._r, frange):
             return self._r.is_finite
         return True
 
     def __next__(self):
         yield from self
 
     def __init__(self, r: Union[range, frange]):
-        self._r = r
+        self._r: frange = r if isinstance(r, frange) else frange.from_range(r)
 
     def __iter__(self) -> Iterator[int]:
         return iter(self._r)
 
     def __contains__(self, item) -> bool:
         return item in self._r
 
     @property
-    def start(self) -> float:
+    def minimum(self) -> float:
         return self._r.start
 
     @property
-    def stop(self) -> float:
+    def maximum(self) -> float:
         return self._r.stop
 
     @property
     def step(self) -> float:
         return self._r.step
 
 
+class SetSupp(DiscreteSupp):
+    @property
+    def is_finite(self) -> bool:
+        return True
+
+    @property
+    @memo
+    def minimum(self) -> float:
+        return min(self._s)
+
+    @property
+    @memo
+    def maximum(self) -> float:
+        return max(self._s)
+
+    def __init__(self, s: set) -> None:
+        self._s = s
+
+    def __iter__(self) -> Iterator:
+        return iter(self._s)
+
+    def __contains__(self, item) -> bool:
+        return item in self._s
+
+
 class ContinuseSupp(Supp[float]):
 
     @property
     def is_finite(self) -> bool:
         return False
 
 
 __all__ = [
     "Supp",
-    "DiscreteSupp",
+    "FrangeSupp",
     "ContinuseSupp",
 ]
```

### Comparing `danielutils-0.9.76/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.77/danielutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.76
+Version: 0.9.77
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,17 @@
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
 # danielutils v=0.9.75
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
+**Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13` 
+
+Versions marked with * are partially working
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
 
 ### [`isoftype`](./READMES/isoftype.md)
 -- _"Boost your type checking game with `isoftype`: Effortlessly verify object types and subtypes, handle complex data structures, and tackle union types in Python!"_
 
 **Support for Parametrized Generics**
```

### Comparing `danielutils-0.9.76/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.77/danielutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 danielutils/io_.py
 danielutils/path.py
 danielutils/print_.py
 danielutils/py.typed
 danielutils/text.py
 danielutils/time.py
 danielutils/tqdm_.py
+danielutils/versioned_imports.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
 danielutils.egg-info/top_level.txt
 danielutils/abstractions/__init__.py
 danielutils/abstractions/repl.py
 danielutils/abstractions/database/__init__.py
@@ -70,14 +71,15 @@
 danielutils/decorators/__init__.py
 danielutils/decorators/atomic.py
 danielutils/decorators/attach.py
 danielutils/decorators/chain_decorators.py
 danielutils/decorators/decorate_conditionally.py
 danielutils/decorators/delay_call.py
 danielutils/decorators/deprecate.py
+danielutils/decorators/final.py
 danielutils/decorators/limit_recursion.py
 danielutils/decorators/memo.py
 danielutils/decorators/overload.py
 danielutils/decorators/partially_implemented.py
 danielutils/decorators/processify.py
 danielutils/decorators/property.py
 danielutils/decorators/singleton.py
@@ -152,25 +154,26 @@
 danielutils/university/oop/observer.py
 danielutils/university/oop/strategy.py
 danielutils/university/probability/__init__.py
 danielutils/university/probability/distributions.py
 danielutils/university/probability/operator.py
 danielutils/university/probability/protocols.py
 danielutils/university/probability/supp.py
-danielutils/university/probability/conditional_variables/__init__.py
-danielutils/university/probability/conditional_variables/conditional_variable.py
-danielutils/university/probability/conditional_variables/continuous/__init__.py
-danielutils/university/probability/conditional_variables/discrete/__init__.py
-danielutils/university/probability/conditional_variables/discrete/bernoulli.py
-danielutils/university/probability/conditional_variables/discrete/binomial.py
-danielutils/university/probability/conditional_variables/discrete/conditional_from_discrete_probability_func.py
-danielutils/university/probability/conditional_variables/discrete/discrete.py
-danielutils/university/probability/conditional_variables/discrete/geometric.py
-danielutils/university/probability/conditional_variables/discrete/poisson.py
-danielutils/university/probability/conditional_variables/discrete/uniform.py
+danielutils/university/probability/transformation.py
+danielutils/university/probability/conditional_variable/__init__.py
+danielutils/university/probability/conditional_variable/conditional_variable.py
+danielutils/university/probability/conditional_variable/continuous/__init__.py
+danielutils/university/probability/conditional_variable/discrete/__init__.py
+danielutils/university/probability/conditional_variable/discrete/bernoulli.py
+danielutils/university/probability/conditional_variable/discrete/binomial.py
+danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
+danielutils/university/probability/conditional_variable/discrete/discrete.py
+danielutils/university/probability/conditional_variable/discrete/geometric.py
+danielutils/university/probability/conditional_variable/discrete/poisson.py
+danielutils/university/probability/conditional_variable/discrete/uniform.py
 danielutils/university/probability/expressions/__init__.py
 danielutils/university/probability/expressions/accumulation_expression.py
 danielutils/university/probability/expressions/probability_expression.py
 danielutils/university/probability/funcs/__init__.py
 danielutils/university/probability/funcs/covariance.py
 danielutils/university/probability/funcs/expected_value.py
 danielutils/university/probability/funcs/probability_function.py
```

### Comparing `danielutils-0.9.76/pyproject.toml` & `danielutils-0.9.77/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.76"
+version = "0.9.77"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = []
 keywords = ['functions', 'decorators', 'methods', 'better_builtins', 'metaclasses']
 license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
-readme = "./README.md"
+readme = {file = "./README.md", content-type = "text/markdown"}
 requires-python = ">=3.8.0"
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
 	"Programming Language :: Python :: 3",
 	"Operating System :: Microsoft :: Windows"
 ]
 
 [tool.setuptools]
-packages=["danielutils"]
+packages = ["danielutils"]
 [tool.setuptools.package-data]
 "danielutils" = ["py.typed"]
 
 [project.urls]
 "Homepage" = "https://github.com/danielnachumdev/danielutils"
 "Bug Tracker" = "https://github.com/danielnachumdev/danielutils/issues"
```

