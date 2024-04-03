# Comparing `tmp/danielutils-0.9.71.tar.gz` & `tmp/danielutils-0.9.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.71.tar", last modified: Fri Mar 29 00:19:07 2024, max compression
+gzip compressed data, was "danielutils-0.9.72.tar", last modified: Wed Apr  3 22:26:23 2024, max compression
```

## Comparing `danielutils-0.9.71.tar` & `danielutils-0.9.72.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.044659 danielutils-0.9.71/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.71/LISENCE
--rw-rw-rw-   0        0        0     4476 2024-03-29 00:19:07.043630 danielutils-0.9.71/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2024-03-21 23:41:27.000000 danielutils-0.9.71/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.981042 danielutils-0.9.71/danielutils/
--rw-rw-rw-   0        0        0      879 2024-03-27 21:41:30.000000 danielutils-0.9.71/danielutils/__init__.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.988760 danielutils-0.9.71/danielutils/classes/
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/Convenience.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/Counter.py
--rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/Tree.py
--rw-rw-rw-   0        0        0      159 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/__init__.py
--rw-rw-rw-   0        0        0     1642 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/frange.py
--rw-rw-rw-   0        0        0     3045 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/classes/repl.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.989864 danielutils-0.9.71/danielutils/classes/sorted_builtins/
--rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/sorted_builtins/__init__.py
--rw-rw-rw-   0        0        0      112 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/sorted_builtins/sset.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.995344 danielutils-0.9.71/danielutils/classes/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4730 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/classes/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5443 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/colors.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.996435 danielutils-0.9.71/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.998493 danielutils-0.9.71/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.71/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/conversions/specialized_conversions/to_int.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.002323 danielutils-0.9.71/danielutils/data_structures/
--rw-rw-rw-   0        0        0     1228 2024-03-28 19:48:44.000000 danielutils-0.9.71/danielutils/data_structures/Comparer.py
--rw-rw-rw-   0        0        0     1860 2024-03-28 19:42:06.000000 danielutils-0.9.71/danielutils/data_structures/Stack.py
--rw-rw-rw-   0        0        0      139 2024-03-28 19:25:52.000000 danielutils-0.9.71/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0      261 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.71/danielutils/data_structures/functions.py
--rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.71/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.71/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.013293 danielutils-0.9.71/danielutils/decorators/
--rw-rw-rw-   0        0        0      413 2024-03-27 18:54:28.000000 danielutils-0.9.71/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1555 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1016 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1192 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1469 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1877 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      997 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7511 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0     1012 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1753 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      916 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     2088 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0    10013 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/exceptions.py
--rw-rw-rw-   0        0        0    11820 2024-03-14 21:24:08.000000 danielutils-0.9.71/danielutils/files_and_folders.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.018660 danielutils-0.9.71/danielutils/functions/
--rw-rw-rw-   0        0        0      160 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0     9027 2024-03-29 00:10:11.000000 danielutils-0.9.71/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.020718 danielutils-0.9.71/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2827 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/internet.py
--rw-rw-rw-   0        0        0     2005 2024-02-19 17:33:20.000000 danielutils-0.9.71/danielutils/loops.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.024881 danielutils-0.9.71/danielutils/math/
--rw-rw-rw-   0        0        0       80 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/math/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/math/constants.py
--rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/math/functions.py
--rw-rw-rw-   0        0        0     1062 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/math/math_print.py
--rw-rw-rw-   0        0        0     4051 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/math/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.028380 danielutils-0.9.71/danielutils/metaclasses/
--rw-rw-rw-   0        0        0    10944 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/metaclasses/Interface.py
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.71/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1487 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/metaclasses/overload_meta.py
--rw-rw-rw-   0        0        0      202 2024-03-10 17:39:29.000000 danielutils-0.9.71/danielutils/multi_x.py
--rw-rw-rw-   0        0        0     1419 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/my_tqdm.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/path.py
--rw-rw-rw-   0        0        0     2800 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/print.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.71/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.033491 danielutils-0.9.71/danielutils/reflection/
--rw-rw-rw-   0        0        0     1627 2024-03-27 21:40:59.000000 danielutils-0.9.71/danielutils/reflection/__init__.py
--rw-rw-rw-   0        0        0      736 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/reflection/class_reflection.py
--rw-rw-rw-   0        0        0     1133 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/reflection/file_reflection.py
--rw-rw-rw-   0        0        0     5055 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/reflection/function_reflections.py
--rw-rw-rw-   0        0        0      748 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/reflection/get_prev_frame.py
--rw-rw-rw-   0        0        0      444 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/reflection/get_traceback.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/reflection/module_reflections.py
--rw-rw-rw-   0        0        0     1229 2024-03-27 18:56:28.000000 danielutils-0.9.71/danielutils/reflection/system_reflections.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/relations.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/signals.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.034516 danielutils-0.9.71/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.035562 danielutils-0.9.71/danielutils/system/
--rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/system/independent.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.037624 danielutils-0.9.71/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.039114 danielutils-0.9.71/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      477 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/text.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.041185 danielutils-0.9.71/danielutils/threads/
--rw-rw-rw-   0        0        0       51 2023-08-15 21:20:20.000000 danielutils-0.9.71/danielutils/threads/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/threads/worker.py
--rw-rw-rw-   0        0        0     2319 2024-03-27 18:52:27.000000 danielutils-0.9.71/danielutils/threads/worker_pool.py
--rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/time.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.042221 danielutils-0.9.71/danielutils/university/
--rw-rw-rw-   0        0        0       26 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:07.042221 danielutils-0.9.71/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.71/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:19:06.984557 danielutils-0.9.71/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4476 2024-03-29 00:19:06.000000 danielutils-0.9.71/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4167 2024-03-29 00:19:06.000000 danielutils-0.9.71/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 00:19:06.000000 danielutils-0.9.71/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-29 00:19:06.000000 danielutils-0.9.71/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-29 00:19:06.000000 danielutils-0.9.71/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      930 2024-03-29 00:19:06.000000 danielutils-0.9.71/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 00:19:07.044659 danielutils-0.9.71/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-03-29 00:19:06.000000 danielutils-0.9.71/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.940152 danielutils-0.9.72/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.72/LICENSE
+-rw-rw-rw-   0        0        0     4499 2024-04-03 22:26:23.937017 danielutils-0.9.72/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2024-03-21 23:41:27.000000 danielutils-0.9.72/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.825463 danielutils-0.9.72/danielutils/
+-rw-rw-rw-   0        0        0     1423 2024-03-30 13:12:04.000000 danielutils-0.9.72/danielutils/__init__.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/aliases.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.840384 danielutils-0.9.72/danielutils/classes/
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/Convenience.py
+-rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/Counter.py
+-rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/Tree.py
+-rw-rw-rw-   0        0        0      159 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/__init__.py
+-rw-rw-rw-   0        0        0     3776 2024-04-03 22:23:41.000000 danielutils-0.9.72/danielutils/classes/frange.py
+-rw-rw-rw-   0        0        0     3045 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/classes/repl.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.842325 danielutils-0.9.72/danielutils/classes/sorted_builtins/
+-rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/sorted_builtins/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/sorted_builtins/sset.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.849092 danielutils-0.9.72/danielutils/classes/typed_builtins/
+-rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/__init__.py
+-rw-rw-rw-   0        0        0     4730 2024-03-29 00:29:43.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/factory.py
+-rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/tdict.py
+-rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/tset.py
+-rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/ttuple.py
+-rw-rw-rw-   0        0        0     5434 2024-03-29 22:03:21.000000 danielutils-0.9.72/danielutils/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.851163 danielutils-0.9.72/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.854164 danielutils-0.9.72/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.72/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/specialized_conversions/to_int.py
+-rw-rw-rw-   0        0        0     2800 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/d_print.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.862272 danielutils-0.9.72/danielutils/data_structures/
+-rw-rw-rw-   0        0        0     1228 2024-03-28 19:48:44.000000 danielutils-0.9.72/danielutils/data_structures/Comparer.py
+-rw-rw-rw-   0        0        0     1860 2024-03-28 19:42:06.000000 danielutils-0.9.72/danielutils/data_structures/Stack.py
+-rw-rw-rw-   0        0        0      161 2024-03-30 20:21:37.000000 danielutils-0.9.72/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      261 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.72/danielutils/data_structures/functions.py
+-rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.72/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.72/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.881632 danielutils-0.9.72/danielutils/decorators/
+-rw-rw-rw-   0        0        0      413 2024-03-27 18:54:28.000000 danielutils-0.9.72/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1555 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1016 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1192 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1469 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1877 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0     1034 2024-03-29 21:27:58.000000 danielutils-0.9.72/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7511 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0     1012 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1753 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      916 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     2131 2024-04-03 22:25:29.000000 danielutils-0.9.72/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0    10013 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/exceptions.py
+-rw-rw-rw-   0        0        0    11820 2024-03-14 21:24:08.000000 danielutils-0.9.72/danielutils/files_and_folders.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.889164 danielutils-0.9.72/danielutils/functions/
+-rw-rw-rw-   0        0        0      160 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0     9027 2024-03-29 00:10:11.000000 danielutils-0.9.72/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.895523 danielutils-0.9.72/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2827 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/internet.py
+-rw-rw-rw-   0        0        0     2005 2024-02-19 17:33:20.000000 danielutils-0.9.72/danielutils/loops.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.901722 danielutils-0.9.72/danielutils/math/
+-rw-rw-rw-   0        0        0       80 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/__init__.py
+-rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/constants.py
+-rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/functions.py
+-rw-rw-rw-   0        0        0     1062 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/math_print.py
+-rw-rw-rw-   0        0        0     4051 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/math/math_symbols.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.910246 danielutils-0.9.72/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0    10944 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/metaclasses/Interface.py
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.72/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1487 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/overload_meta.py
+-rw-rw-rw-   0        0        0      202 2024-03-10 17:39:29.000000 danielutils-0.9.72/danielutils/multi_x.py
+-rw-rw-rw-   0        0        0     1419 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/my_tqdm.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/path.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.72/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.919207 danielutils-0.9.72/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1655 2024-03-29 21:36:20.000000 danielutils-0.9.72/danielutils/reflection/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-03-29 21:51:07.000000 danielutils-0.9.72/danielutils/reflection/class_reflection.py
+-rw-rw-rw-   0        0        0     1133 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/reflection/file_reflection.py
+-rw-rw-rw-   0        0        0     5055 2024-03-29 21:50:42.000000 danielutils-0.9.72/danielutils/reflection/function_reflections.py
+-rw-rw-rw-   0        0        0      748 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/reflection/get_prev_frame.py
+-rw-rw-rw-   0        0        0      444 2024-03-29 21:51:07.000000 danielutils-0.9.72/danielutils/reflection/get_traceback.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/reflection/module_reflections.py
+-rw-rw-rw-   0        0        0      639 2024-03-29 21:49:46.000000 danielutils-0.9.72/danielutils/reflection/system_reflections.py
+-rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/relations.py
+-rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.922437 danielutils-0.9.72/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.924440 danielutils-0.9.72/danielutils/system/
+-rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/system/independent.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.926852 danielutils-0.9.72/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.930339 danielutils-0.9.72/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/text.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.932925 danielutils-0.9.72/danielutils/threads/
+-rw-rw-rw-   0        0        0       51 2023-08-15 21:20:20.000000 danielutils-0.9.72/danielutils/threads/__init__.py
+-rw-rw-rw-   0        0        0     2416 2024-03-29 22:01:24.000000 danielutils-0.9.72/danielutils/threads/worker.py
+-rw-rw-rw-   0        0        0     2319 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/threads/worker_pool.py
+-rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/time.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.933925 danielutils-0.9.72/danielutils/university/
+-rw-rw-rw-   0        0        0       54 2024-03-30 12:00:49.000000 danielutils-0.9.72/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.935975 danielutils-0.9.72/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.831342 danielutils-0.9.72/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4499 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4191 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      934 2024-04-03 22:26:22.000000 danielutils-0.9.72/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 22:26:23.941071 danielutils-0.9.72/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-03 22:26:22.000000 danielutils-0.9.72/setup.py
```

### Comparing `danielutils-0.9.71/LISENCE` & `danielutils-0.9.72/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/PKG-INFO` & `danielutils-0.9.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.71
+Version: 0.9.72
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Keywords: functions,decorators,methods,classes,metaclasses
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: tqdm
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
```

### Comparing `danielutils-0.9.71/README.md` & `danielutils-0.9.72/README.md`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/aliases.py` & `danielutils-0.9.72/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/classes/Counter.py` & `danielutils-0.9.72/danielutils/classes/Counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/classes/frange.py` & `danielutils-0.9.72/danielutils/classes/frange.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,114 @@
-from typing import Iterable, Callable, Optional
+from typing import Iterable, Callable, Optional, Iterator
 
 
-class frange:
+class frange(Iterable[float]):
     """this class is the same like builtin range but with float values
     """
 
     def __init__(self, start: float, stop: Optional[float] = None,
                  step: float = 1, round_method: Callable[[float], float] = lambda f: round(f, 3)):
         if stop is None:
             stop = start
             start = 0
         self.start = start
         self.stop = stop
         self.step = step
         self.method = round_method
 
+    def __eq__(self, other):
+        if not isinstance(other, frange):
+            raise NotImplementedError
+        return self.start == other.start and self.stop == other.stop and self.step == other.step
+
     def __iter__(self) -> Iterable:
         if self.stop < self.start:
             return
         if self.start > self.stop:
             return
-        if abs(self.stop-self.start) < abs(self.step):
+        if abs(self.stop - self.start) < abs(self.step):
             return
         if self.stop > 0 and self.step < 0:
             return
         if self.stop < 0 and self.step > 0:
             return
 
         cur = self.start
         while cur < self.stop:
             yield self.method(cur)
             cur += self.step
 
     def __len__(self) -> int:
-        return int((self.stop-self.start)//self.step)
+        return int((self.stop - self.start) // self.step)
 
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.start}, {self.stop}, {self.step})"
 
+    @property
+    def _is_whole_step(self) -> bool:
+        return self.step - int(self.step) == 0
+
+    def __contains__(self, item):
+        if item < self.start:
+            return False
+        if item >= self.stop:
+            return False
+
+        if self._is_whole_step:
+            if not item - int(item) == 0:
+                return False
+
+        return item / self.step - item // self.step == 0
+
+    def normalize(self) -> 'frange':
+        return frange(self.start / self.step, self.stop / self.step, 1)
+
+    def intersect(self, other: 'frange') -> 'frange':
+        a, b = self.normalize(), other.normalize()
+        start1, stop1 = a.start, a.stop
+        start2, stop2 = b.start, b.stop
+        remainder1, remainder2 = start1 - int(start1), start2 - int(start2)
+        if remainder1 == remainder2:
+            if stop1 == float("inf") or stop2 == float("inf"):
+                return frange(max(start1, start2), float("inf"))
+            return frange(max(start1, start2), min(stop1, stop2))
+        raise NotImplementedError("this part is not implemented yet")
+        if remainder1 != 0 and remainder2 / remainder1 - remainder2 // remainder1 == 0:
+            pass
+
+        pass
+
+
+class frange_iterator(Iterator[float]):
+    def __init__(self, obj: frange):
+        self.r = obj
+
+    def __next__(self):
+        if self.r.stop < self.r.start:
+            return
+        if self.r.start > self.r.stop:
+            return
+        if abs(self.r.stop - self.r.start) < abs(self.r.step):
+            return
+        if self.r.stop > 0 and self.r.step < 0:
+            return
+        if self.r.stop < 0 and self.r.step > 0:
+            return
+
+        cur = self.r.start
+        while cur < self.r.stop:
+            yield self.r.method(cur)
+            cur += self.r.step
+
+    def __iter__(self):
+        return self
+
 
 class brange(frange):
     """like frange but with tqdm
     """
 
     def __iter__(self):
         itr = super().__iter__()
```

### Comparing `danielutils-0.9.71/danielutils/classes/repl.py` & `danielutils-0.9.72/danielutils/classes/repl.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/classes/typed_builtins/factory.py` & `danielutils-0.9.72/danielutils/classes/typed_builtins/factory.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/classes/typed_builtins/tdict.py` & `danielutils-0.9.72/danielutils/classes/typed_builtins/tdict.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/classes/typed_builtins/tlist.py` & `danielutils-0.9.72/danielutils/classes/typed_builtins/tlist.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/classes/typed_builtins/tset.py` & `danielutils-0.9.72/danielutils/classes/typed_builtins/tset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/colors.py` & `danielutils-0.9.72/danielutils/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, IO
-from .decorators.validate import validate
+from .decorators import validate
 
 
 RESET = "\033[0m"
 
 
 class ColoredText:
     """static utility class with static functions:\n
```

### Comparing `danielutils-0.9.71/danielutils/conversions/main_conversions.py` & `danielutils-0.9.72/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.72/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/data_structures/Comparer.py` & `danielutils-0.9.72/danielutils/data_structures/Comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/data_structures/Stack.py` & `danielutils-0.9.72/danielutils/data_structures/Stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/data_structures/functions.py` & `danielutils-0.9.72/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/date.py` & `danielutils-0.9.72/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/atomic.py` & `danielutils-0.9.72/danielutils/decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/attach.py` & `danielutils-0.9.72/danielutils/decorators/attach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.72/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/decorate_conditionally.py` & `danielutils-0.9.72/danielutils/decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/delay_call.py` & `danielutils-0.9.72/danielutils/decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/deprecate.py` & `danielutils-0.9.72/danielutils/decorators/deprecate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/limit_recursion.py` & `danielutils-0.9.72/danielutils/decorators/limit_recursion.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/memo.py` & `danielutils-0.9.72/danielutils/decorators/memo.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
     from builtins import dict as t_dict
     from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+from copy import deepcopy
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 @validate
 def memo(func: FuncT) -> FuncT:
@@ -23,14 +24,14 @@
     """
     cache: t_dict[tuple, Any] = {}
 
     @ functools.wraps(func)
     def wrapper(*args, **kwargs):
         if (args, *kwargs.items()) not in cache:
             cache[(args, *kwargs.items())] = func(*args, **kwargs)
-        return cache[(args, *kwargs.items())]
+        return deepcopy(cache[(args, *kwargs.items())])
     return wrapper
 
 
 __all__ = [
     "memo"
 ]
```

### Comparing `danielutils-0.9.71/danielutils/decorators/overload.py` & `danielutils-0.9.72/danielutils/decorators/overload.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.72/danielutils/decorators/partially_implemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/processify.py` & `danielutils-0.9.72/danielutils/decorators/processify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/property.py` & `danielutils-0.9.72/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/threadify.py` & `danielutils-0.9.72/danielutils/decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/decorators/timeout.py` & `danielutils-0.9.72/danielutils/decorators/timeout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import threading
 import functools
 import platform
 from typing import Callable, TypeVar, Union
 from .validate import validate
 from ..reflection import get_python_version
+
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
@@ -25,14 +26,15 @@
     Raises:
         ValueError: if a function is not provided to be decorated
         Exception: any exception from within the function
 
     Returns:
         Callable: the result decorated function
     """
+
     # https://stackoverflow.com/a/21861599/6416556
     def timeout_deco(func: FuncT) -> FuncT:
         if not callable(func):
             raise ValueError("timeout must decorate a function")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
@@ -52,9 +54,16 @@
             except Exception as thread_error:
                 raise thread_error
             if isinstance(res[0], BaseException):
                 if not silent:
                     raise res[0]
                 return None
             return res[0]
+
         return wrapper
+
     return timeout_deco
+
+
+__all__ = [
+    "timeout"
+]
```

### Comparing `danielutils-0.9.71/danielutils/decorators/validate.py` & `danielutils-0.9.72/danielutils/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/exceptions.py` & `danielutils-0.9.72/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/files_and_folders.py` & `danielutils-0.9.72/danielutils/files_and_folders.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/functions/areoneof.py` & `danielutils-0.9.72/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/functions/check_foreach.py` & `danielutils-0.9.72/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/functions/isoftype.py` & `danielutils-0.9.72/danielutils/functions/isoftype.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/functions/isoneof.py` & `danielutils-0.9.72/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/functions/powerset.py` & `danielutils-0.9.72/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/functions/types_subseteq.py` & `danielutils-0.9.72/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/generators/conditional_generator.py` & `danielutils-0.9.72/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/generators/join_generators.py` & `danielutils-0.9.72/danielutils/generators/join_generators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/internet.py` & `danielutils-0.9.72/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/loops.py` & `danielutils-0.9.72/danielutils/loops.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/math/constants.py` & `danielutils-0.9.72/danielutils/math/constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/math/functions.py` & `danielutils-0.9.72/danielutils/math/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/math/math_print.py` & `danielutils-0.9.72/danielutils/math/math_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/math/math_symbols.py` & `danielutils-0.9.72/danielutils/math/math_symbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/metaclasses/Interface.py` & `danielutils-0.9.72/danielutils/metaclasses/Interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.72/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.72/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.72/danielutils/metaclasses/instance_cache_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.72/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/my_tqdm.py` & `danielutils-0.9.72/danielutils/my_tqdm.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/path.py` & `danielutils-0.9.72/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/print.py` & `danielutils-0.9.72/danielutils/d_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/reflection/__init__.py` & `danielutils-0.9.72/danielutils/reflection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .system_reflections import *  # this has to be first, the order matters!
 from .file_reflection import *
 from .function_reflections import *
 from .get_traceback import *
 from .module_reflections import *
 from .class_reflection import *
 from .get_prev_frame import *
+from .interpreter import *
 # def get_class(module_name: str, class_name: str) -> type:
 #     """dynammically loads the module and returns the class from this file
 
 #     Args:
 #         module_name (str): name of python module, (typically a file name without extention)
 #         class_name (str): the name of the wanted class
```

### Comparing `danielutils-0.9.71/danielutils/reflection/class_reflection.py` & `danielutils-0.9.72/danielutils/reflection/class_reflection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from ..reflection import get_python_version
+from .interpreter import get_python_version
 if get_python_version() >= (3, 9):
     from builtins import list as t_list  # type:ignore
 else:
     from typing import List as t_list
 
 
 def get_explicitly_declared_functions(cls: type) -> t_list[str]:
```

### Comparing `danielutils-0.9.71/danielutils/reflection/file_reflection.py` & `danielutils-0.9.72/danielutils/reflection/file_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/reflection/function_reflections.py` & `danielutils-0.9.72/danielutils/reflection/function_reflections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from typing import cast, Optional, Callable, Any
 from types import FrameType
 from .get_prev_frame import get_prev_frame_from, get_n_prev_frame
-from ..reflection import get_python_version
+from .interpreter import get_python_version
 
 if get_python_version() < (3, 9):
     from typing import List as t_list, Set as t_set  # pylint: disable=ungrouped-imports
 else:
     from builtins import list as t_list, set as t_set
```

### Comparing `danielutils-0.9.71/danielutils/reflection/get_prev_frame.py` & `danielutils-0.9.72/danielutils/reflection/get_prev_frame.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/system/independent.py` & `danielutils-0.9.72/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.72/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/system/windows/windows.py` & `danielutils-0.9.72/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/text.py` & `danielutils-0.9.72/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/threads/worker.py` & `danielutils-0.9.72/danielutils/threads/worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from threading import Thread
 from abc import ABC, abstractmethod
 from typing import Optional, Any
 from logging import error
-import danielutils
+import danielutils # this is explicitly this way to prevent circular import
 from ..reflection import get_python_version
 if get_python_version() >= (3, 9):
     from builtins import tuple as t_tuple  # type:ignore
 else:
     from typing import Tuple as t_tuple
```

### Comparing `danielutils-0.9.71/danielutils/threads/worker_pool.py` & `danielutils-0.9.72/danielutils/threads/worker_pool.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/time.py` & `danielutils-0.9.72/danielutils/time.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils/university/databases/all.py` & `danielutils-0.9.72/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.71/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.72/danielutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.71
+Version: 0.9.72
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Keywords: functions,decorators,methods,classes,metaclasses
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: tqdm
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
```

### Comparing `danielutils-0.9.71/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.72/danielutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-LISENCE
+LICENSE
 README.md
 pyproject.toml
 setup.py
+./LICENSE
+./README.md
 danielutils/__init__.py
 danielutils/aliases.py
 danielutils/colors.py
+danielutils/d_print.py
 danielutils/date.py
 danielutils/date_time.py
 danielutils/exceptions.py
 danielutils/files_and_folders.py
 danielutils/internet.py
 danielutils/loops.py
 danielutils/multi_x.py
 danielutils/my_tqdm.py
 danielutils/path.py
-danielutils/print.py
 danielutils/py.typed
 danielutils/relations.py
 danielutils/signals.py
 danielutils/text.py
 danielutils/time.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
```

### Comparing `danielutils-0.9.71/pyproject.toml` & `danielutils-0.9.72/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.71"
+version = "0.9.72"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = ['tqdm']
 keywords = ['functions', 'decorators', 'methods', 'classes', 'metaclasses']
-license = { "file" = "LISENCE" }
+license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
-readme = "README.md"
+readme = "./README.md"
 requires-python = ">=3.8.0"
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
 	"Programming Language :: Python :: 3",
 	"Operating System :: Microsoft :: Windows"
 ]
```

