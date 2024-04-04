# Comparing `tmp/cao-lang-0.2.1.tar.gz` & `tmp/cao-lang-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cao-lang-0.2.1.tar", last modified: Fri Feb  9 23:05:52 2024, max compression
+gzip compressed data, was "cao-lang-0.2.2.tar", last modified: Thu Apr  4 20:52:07 2024, max compression
```

## Comparing `cao-lang-0.2.1.tar` & `cao-lang-0.2.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.798110 cao-lang-0.2.1/
--rw-r--r--   0 runner     (501) staff       (20)     1068 2024-02-09 23:05:35.000000 cao-lang-0.2.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      123 2024-02-09 23:05:35.000000 cao-lang-0.2.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-02-09 23:05:52.797502 cao-lang-0.2.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1098 2024-02-09 23:05:35.000000 cao-lang-0.2.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.776409 cao-lang-0.2.1/cao-lang/
--rw-r--r--   0 runner     (501) staff       (20)     1317 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/Cargo.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.776891 cao-lang-0.2.1/cao-lang/benches/
--rw-r--r--   0 runner     (501) staff       (20)     4146 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/benches/cao_lang_benches.rs
--rw-r--r--   0 runner     (501) staff       (20)     1246 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/build.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.781418 cao-lang-0.2.1/cao-lang/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.781850 cao-lang-0.2.1/cao-lang/src/alloc/
--rw-r--r--   0 runner     (501) staff       (20)     3168 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/alloc/caolang_alloc.rs
--rw-r--r--   0 runner     (501) staff       (20)      999 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/alloc.rs
--rw-r--r--   0 runner     (501) staff       (20)     1115 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/bytecode.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.783751 cao-lang-0.2.1/cao-lang/src/collections/
--rw-r--r--   0 runner     (501) staff       (20)     3084 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/bounded_stack.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.784385 cao-lang-0.2.1/cao-lang/src/collections/handle_table/
--rw-r--r--   0 runner     (501) staff       (20)     3731 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/handle_table/serde_impl.rs
--rw-r--r--   0 runner     (501) staff       (20)     2316 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/handle_table/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    16573 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/handle_table.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.784976 cao-lang-0.2.1/cao-lang/src/collections/hash_map/
--rw-r--r--   0 runner     (501) staff       (20)     3774 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/hash_map/serde_impl.rs
--rw-r--r--   0 runner     (501) staff       (20)     3547 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/hash_map/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    15603 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/hash_map.rs
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/mod.rs
--rw-r--r--   0 runner     (501) staff       (20)     5147 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/collections/value_stack.rs
--rw-r--r--   0 runner     (501) staff       (20)     6726 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiled_program.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.787399 cao-lang-0.2.1/cao-lang/src/compiler/
--rw-r--r--   0 runner     (501) staff       (20)    21154 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/card.rs
--rw-r--r--   0 runner     (501) staff       (20)     2273 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/compilation_error.rs
--rw-r--r--   0 runner     (501) staff       (20)      423 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/compile_options.rs
--rw-r--r--   0 runner     (501) staff       (20)      790 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/function.rs
--rw-r--r--   0 runner     (501) staff       (20)      793 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/function_ir.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.787709 cao-lang-0.2.1/cao-lang/src/compiler/module/
--rw-r--r--   0 runner     (501) staff       (20)     8441 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/module/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    16993 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/module.rs
--rw-r--r--   0 runner     (501) staff       (20)     3103 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    39021 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/compiler.rs
--rw-r--r--   0 runner     (501) staff       (20)     5505 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/instruction.rs
--rw-r--r--   0 runner     (501) staff       (20)     1606 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/lib.rs
--rw-r--r--   0 runner     (501) staff       (20)      403 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/prelude.rs
--rw-r--r--   0 runner     (501) staff       (20)     2992 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/procedures.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.788028 cao-lang-0.2.1/cao-lang/src/stdlib/
--rw-r--r--   0 runner     (501) staff       (20)    12839 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/stdlib/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    11742 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/stdlib.rs
--rw-r--r--   0 runner     (501) staff       (20)     5028 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/traits.rs
--rw-r--r--   0 runner     (501) staff       (20)    12013 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/value.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.789185 cao-lang-0.2.1/cao-lang/src/vm/
--rw-r--r--   0 runner     (501) staff       (20)    17984 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/instr_execution.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.790942 cao-lang-0.2.1/cao-lang/src/vm/runtime/
--rw-r--r--   0 runner     (501) staff       (20)     1006 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_function.rs
--rw-r--r--   0 runner     (501) staff       (20)     6511 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_object.rs
--rw-r--r--   0 runner     (501) staff       (20)     1105 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_string.rs
--rw-r--r--   0 runner     (501) staff       (20)     3729 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_table.rs
--rw-r--r--   0 runner     (501) staff       (20)    13858 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/runtime.rs
--rw-r--r--   0 runner     (501) staff       (20)     1882 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    33219 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/src/vm.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.792509 cao-lang-0.2.1/cao-lang/tests/
--rw-r--r--   0 runner     (501) staff       (20)    46718 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/tests/integration_tests.rs
--rw-r--r--   0 runner     (501) staff       (20)     1820 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/tests/test_fibonacci.rs
--rw-r--r--   0 runner     (501) staff       (20)     1146 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/tests/test_for_each.rs
--rw-r--r--   0 runner     (501) staff       (20)     3227 2024-02-09 23:05:35.000000 cao-lang-0.2.1/cao-lang/tests/test_tables.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.792917 cao-lang-0.2.1/py/
--rw-r--r--   0 runner     (501) staff       (20)      420 2024-02-09 23:05:35.000000 cao-lang-0.2.1/py/Cargo.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.794527 cao-lang-0.2.1/py/cao_lang/
--rw-r--r--   0 runner     (501) staff       (20)       27 2024-02-09 23:05:35.000000 cao-lang-0.2.1/py/cao_lang/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.797018 cao-lang-0.2.1/py/cao_lang.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-02-09 23:05:52.000000 cao-lang-0.2.1/py/cao_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1917 2024-02-09 23:05:52.000000 cao-lang-0.2.1/py/cao_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-09 23:05:52.000000 cao-lang-0.2.1/py/cao_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-09 23:05:52.000000 cao-lang-0.2.1/py/cao_lang.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-02-09 23:05:52.000000 cao-lang-0.2.1/py/cao_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.793721 cao-lang-0.2.1/py/src/
--rw-r--r--   0 runner     (501) staff       (20)     2664 2024-02-09 23:05:35.000000 cao-lang-0.2.1/py/src/lib.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-09 23:05:52.794078 cao-lang-0.2.1/py/tests/
--rw-r--r--   0 runner     (501) staff       (20)     2713 2024-02-09 23:05:35.000000 cao-lang-0.2.1/py/tests/test_cao_lang.py
--rw-r--r--   0 runner     (501) staff       (20)      117 2024-02-09 23:05:35.000000 cao-lang-0.2.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-02-09 23:05:52.798205 cao-lang-0.2.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1430 2024-02-09 23:05:35.000000 cao-lang-0.2.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.530055 cao-lang-0.2.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2024-04-04 20:51:56.000000 cao-lang-0.2.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      123 2024-04-04 20:51:56.000000 cao-lang-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 20:52:07.529639 cao-lang-0.2.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1098 2024-04-04 20:51:56.000000 cao-lang-0.2.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.510831 cao-lang-0.2.2/cao-lang/
+-rw-r--r--   0 runner     (501) staff       (20)     1317 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/Cargo.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.511165 cao-lang-0.2.2/cao-lang/benches/
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/benches/cao_lang_benches.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1246 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/build.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.515131 cao-lang-0.2.2/cao-lang/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.515492 cao-lang-0.2.2/cao-lang/src/alloc/
+-rw-r--r--   0 runner     (501) staff       (20)     3168 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/alloc/caolang_alloc.rs
+-rw-r--r--   0 runner     (501) staff       (20)      999 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/alloc.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1115 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/bytecode.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.517474 cao-lang-0.2.2/cao-lang/src/collections/
+-rw-r--r--   0 runner     (501) staff       (20)     3084 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/bounded_stack.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.518156 cao-lang-0.2.2/cao-lang/src/collections/handle_table/
+-rw-r--r--   0 runner     (501) staff       (20)     3731 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/handle_table/serde_impl.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2316 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/handle_table/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    16517 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/handle_table.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.518778 cao-lang-0.2.2/cao-lang/src/collections/hash_map/
+-rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/hash_map/serde_impl.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3547 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/hash_map/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    15603 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/hash_map.rs
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/mod.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/value_stack.rs
+-rw-r--r--   0 runner     (501) staff       (20)     6726 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiled_program.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.521377 cao-lang-0.2.2/cao-lang/src/compiler/
+-rw-r--r--   0 runner     (501) staff       (20)    21154 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/card.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2273 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/compilation_error.rs
+-rw-r--r--   0 runner     (501) staff       (20)      423 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/compile_options.rs
+-rw-r--r--   0 runner     (501) staff       (20)      790 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/function.rs
+-rw-r--r--   0 runner     (501) staff       (20)      793 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/function_ir.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.521673 cao-lang-0.2.2/cao-lang/src/compiler/module/
+-rw-r--r--   0 runner     (501) staff       (20)     8441 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/module/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    17167 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/module.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3103 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    39021 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5505 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/instruction.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1606 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/lib.rs
+-rw-r--r--   0 runner     (501) staff       (20)      403 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/prelude.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2992 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/procedures.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.522006 cao-lang-0.2.2/cao-lang/src/stdlib/
+-rw-r--r--   0 runner     (501) staff       (20)    12839 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/stdlib/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    11742 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/stdlib.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5028 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/traits.rs
+-rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/value.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.523089 cao-lang-0.2.2/cao-lang/src/vm/
+-rw-r--r--   0 runner     (501) staff       (20)    17984 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/instr_execution.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.524438 cao-lang-0.2.2/cao-lang/src/vm/runtime/
+-rw-r--r--   0 runner     (501) staff       (20)     1006 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_function.rs
+-rw-r--r--   0 runner     (501) staff       (20)     6511 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_object.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_string.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3729 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_table.rs
+-rw-r--r--   0 runner     (501) staff       (20)    13858 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1882 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    33219 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.525717 cao-lang-0.2.2/cao-lang/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    46718 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/integration_tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1820 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/test_fibonacci.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1146 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/test_for_each.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3227 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/test_tables.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.526056 cao-lang-0.2.2/py/
+-rw-r--r--   0 runner     (501) staff       (20)      420 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/Cargo.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.527479 cao-lang-0.2.2/py/cao_lang/
+-rw-r--r--   0 runner     (501) staff       (20)       27 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/cao_lang/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.529224 cao-lang-0.2.2/py/cao_lang.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1917 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.526690 cao-lang-0.2.2/py/src/
+-rw-r--r--   0 runner     (501) staff       (20)     2664 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/src/lib.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.526998 cao-lang-0.2.2/py/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     2713 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/tests/test_cao_lang.py
+-rw-r--r--   0 runner     (501) staff       (20)      117 2024-04-04 20:51:56.000000 cao-lang-0.2.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-04 20:52:07.530135 cao-lang-0.2.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1430 2024-04-04 20:51:56.000000 cao-lang-0.2.2/setup.py
```

### Comparing `cao-lang-0.2.1/LICENSE` & `cao-lang-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/PKG-INFO` & `cao-lang-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cao-lang
-Version: 0.2.1
+Version: 0.2.2
 Summary: The node based 'language' that governs the actors of the game Cao-Lo
 Home-page: https://github.com/caolo-game/cao-lang
 Author: Daniel Kiss
 Author-email: littlesnorrboy@gmail.com
 Project-URL: Bug Tracker, https://github.com/caolo-game/cao-lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cao-lang-0.2.1/README.md` & `cao-lang-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/Cargo.toml` & `cao-lang-0.2.2/cao-lang/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 default-features = false
 features = ["release_max_level_info"]
 version = "^0.1"
 
 [dev-dependencies]
 bincode = "1"
 ciborium = "0.2"
-env_logger = "^0.10"
+env_logger = "^0.11"
 serde_json = "^1.0"
 serde_yaml = "^0.9"
 
 [dev-dependencies.criterion]
 features = ["html_reports"]
 version = "^0.5"
 
@@ -64,8 +64,8 @@
 build = "build.rs"
 description = "The back-end of cao-lang, a node based visual scripting language"
 edition = "2021"
 license = "MIT"
 name = "cao-lang"
 readme = "../README.md"
 repository = "https://github.com/caolo-game/cao-lang.git"
-version = "0.2.1"
+version = "0.2.2"
```

### Comparing `cao-lang-0.2.1/cao-lang/benches/cao_lang_benches.rs` & `cao-lang-0.2.2/cao-lang/benches/cao_lang_benches.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/build.rs` & `cao-lang-0.2.2/cao-lang/build.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/alloc/caolang_alloc.rs` & `cao-lang-0.2.2/cao-lang/src/alloc/caolang_alloc.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/alloc.rs` & `cao-lang-0.2.2/cao-lang/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/bytecode.rs` & `cao-lang-0.2.2/cao-lang/src/bytecode.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/bounded_stack.rs` & `cao-lang-0.2.2/cao-lang/src/collections/bounded_stack.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/handle_table/serde_impl.rs` & `cao-lang-0.2.2/cao-lang/src/collections/handle_table/serde_impl.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/handle_table/tests.rs` & `cao-lang-0.2.2/cao-lang/src/collections/handle_table/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/handle_table.rs` & `cao-lang-0.2.2/cao-lang/src/collections/handle_table.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 #[cfg(test)]
 mod tests;
 
 use bytemuck::{Pod, Zeroable};
 
 use crate::alloc::{Allocator, SysAllocator};
 
-#[cfg(feature = "serde")]
-pub use self::serde_impl::*;
-
 use std::{
     alloc::Layout,
     mem::{align_of, size_of, swap, MaybeUninit},
     num::Wrapping,
     ops::{Index, IndexMut},
     ptr::NonNull,
     str::FromStr,
```

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/hash_map/serde_impl.rs` & `cao-lang-0.2.2/cao-lang/src/collections/hash_map/serde_impl.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/hash_map/tests.rs` & `cao-lang-0.2.2/cao-lang/src/collections/hash_map/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/hash_map.rs` & `cao-lang-0.2.2/cao-lang/src/collections/hash_map.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/collections/value_stack.rs` & `cao-lang-0.2.2/cao-lang/src/collections/value_stack.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiled_program.rs` & `cao-lang-0.2.2/cao-lang/src/compiled_program.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/card.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/card.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/compilation_error.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/compilation_error.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/function.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/function.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/function_ir.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/function_ir.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/module/tests.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/module/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/module.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/module.rs`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 #[derive(Debug, Clone, Default)]
 #[cfg_attr(feature = "serde", derive(serde::Serialize, serde::Deserialize))]
 pub struct Module {
     pub submodules: Submodules,
     pub functions: Functions,
     /// _functions_ to import from submodules
     ///
-    /// e.g. importing `foo.bar` allows you to use a `Jump("bar")` [[Card]]
+    /// e.g. importing `foo.bar` allows you to use a `Jump("bar")` [Card]
     pub imports: Imports,
 }
 
 /// Uniquely index a card in a module
 #[derive(Default, Debug, Clone, PartialEq, Eq, Hash)]
 #[cfg_attr(feature = "serde", derive(serde::Serialize, serde::Deserialize))]
 pub struct CardIndex {
@@ -181,42 +181,47 @@
 
 impl Module {
     pub fn get_card_mut<'a>(&'a mut self, idx: &CardIndex) -> Result<&'a mut Card, CardFetchError> {
         let (_, function) = self
             .functions
             .get_mut(idx.function)
             .ok_or(CardFetchError::FunctionNotFound)?;
+        let mut depth = 0;
         let mut card = function
             .cards
             .get_mut(idx.begin()?)
-            .ok_or(CardFetchError::CardNotFound { depth: 0 })?;
+            .ok_or(CardFetchError::CardNotFound { depth })?;
 
         for i in &idx.card_index.indices[1..] {
+            depth += 1;
             card = card
                 .get_child_mut(*i as usize)
-                .ok_or(CardFetchError::CardNotFound { depth: *i as usize })?;
+                .ok_or(CardFetchError::CardNotFound { depth })?;
         }
 
         Ok(card)
     }
 
     pub fn get_card<'a>(&'a self, idx: &CardIndex) -> Result<&'a Card, CardFetchError> {
         let (_, function) = self
             .functions
             .get(idx.function)
             .ok_or(CardFetchError::FunctionNotFound)?;
+
+        let mut depth = 0;
         let mut card = function
             .cards
             .get(idx.begin()?)
-            .ok_or(CardFetchError::CardNotFound { depth: 0 })?;
+            .ok_or(CardFetchError::CardNotFound { depth })?;
 
         for i in &idx.card_index.indices[1..] {
+            depth += 1;
             card = card
                 .get_child(*i as usize)
-                .ok_or(CardFetchError::CardNotFound { depth: *i as usize })?;
+                .ok_or(CardFetchError::CardNotFound { depth })?;
         }
 
         Ok(card)
     }
 
     pub fn remove_card(&mut self, idx: &CardIndex) -> Result<Card, CardFetchError> {
         let (_, function) = self
@@ -225,25 +230,27 @@
             .ok_or(CardFetchError::FunctionNotFound)?;
         if idx.card_index.indices.len() == 1 {
             if function.cards.len() <= idx.card_index.indices[0] as usize {
                 return Err(CardFetchError::CardNotFound { depth: 0 });
             }
             return Ok(function.cards.remove(idx.card_index.indices[0] as usize));
         }
+        let mut depth = 0;
         let mut card = function
             .cards
             .get_mut(idx.begin()?)
-            .ok_or(CardFetchError::CardNotFound { depth: 0 })?;
+            .ok_or(CardFetchError::CardNotFound { depth })?;
 
         // len is at least 1
         let len = idx.card_index.indices.len();
         for i in &idx.card_index.indices[1..(len - 1).max(1)] {
+            depth += 1;
             card = card
                 .get_child_mut(*i as usize)
-                .ok_or(CardFetchError::CardNotFound { depth: *i as usize })?;
+                .ok_or(CardFetchError::CardNotFound { depth })?;
         }
         let i = *idx.card_index.indices.last().unwrap() as usize;
         card.remove_child(i)
             .ok_or(CardFetchError::CardNotFound { depth: len - 1 })
     }
 
     /// Return the old card
@@ -256,25 +263,27 @@
             let c = function
                 .cards
                 .get_mut(idx.card_index.indices[0] as usize)
                 .ok_or(CardFetchError::CardNotFound { depth: 0 })?;
             let res = std::mem::replace(c, child);
             return Ok(res);
         }
+        let mut depth = 0;
         let mut card = function
             .cards
             .get_mut(idx.begin()?)
-            .ok_or(CardFetchError::CardNotFound { depth: 0 })?;
+            .ok_or(CardFetchError::CardNotFound { depth })?;
 
         // len is at least 1
         let len = idx.card_index.indices.len();
         for i in &idx.card_index.indices[1..(len - 1).max(1)] {
+            depth += 1;
             card = card
                 .get_child_mut(*i as usize)
-                .ok_or(CardFetchError::CardNotFound { depth: *i as usize })?;
+                .ok_or(CardFetchError::CardNotFound { depth })?;
         }
         let i = *idx.card_index.indices.last().unwrap() as usize;
         card.replace_child(i, child)
             .map_err(|_| CardFetchError::CardNotFound { depth: len - 1 })
     }
 
     pub fn insert_card(&mut self, idx: &CardIndex, child: Card) -> Result<(), CardFetchError> {
@@ -287,25 +296,27 @@
                 return Err(CardFetchError::CardNotFound { depth: 0 });
             }
             function
                 .cards
                 .insert(idx.card_index.indices[0] as usize, child);
             return Ok(());
         }
+        let mut depth = 0;
         let mut card = function
             .cards
             .get_mut(idx.begin()?)
-            .ok_or(CardFetchError::CardNotFound { depth: 0 })?;
+            .ok_or(CardFetchError::CardNotFound { depth })?;
 
         // len is at least 1
         let len = idx.card_index.indices.len();
         for i in &idx.card_index.indices[1..(len - 1).max(1)] {
+            depth += 1;
             card = card
                 .get_child_mut(*i as usize)
-                .ok_or(CardFetchError::CardNotFound { depth: *i as usize })?;
+                .ok_or(CardFetchError::CardNotFound { depth })?;
         }
         let i = *idx.card_index.indices.last().unwrap() as usize;
         card.insert_child(i, child)
             .map_err(|_| CardFetchError::CardNotFound { depth: len - 1 })
     }
 
     /// flatten this program into a vec of functions
```

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler/tests.rs` & `cao-lang-0.2.2/cao-lang/src/compiler/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/compiler.rs` & `cao-lang-0.2.2/cao-lang/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/instruction.rs` & `cao-lang-0.2.2/cao-lang/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/lib.rs` & `cao-lang-0.2.2/cao-lang/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/procedures.rs` & `cao-lang-0.2.2/cao-lang/src/procedures.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/stdlib/tests.rs` & `cao-lang-0.2.2/cao-lang/src/stdlib/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/stdlib.rs` & `cao-lang-0.2.2/cao-lang/src/stdlib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/traits.rs` & `cao-lang-0.2.2/cao-lang/src/traits.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/value.rs` & `cao-lang-0.2.2/cao-lang/src/value.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/instr_execution.rs` & `cao-lang-0.2.2/cao-lang/src/vm/instr_execution.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_function.rs` & `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_function.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_object.rs` & `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_object.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_string.rs` & `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_string.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/runtime/cao_lang_table.rs` & `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_table.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/runtime.rs` & `cao-lang-0.2.2/cao-lang/src/vm/runtime.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm/tests.rs` & `cao-lang-0.2.2/cao-lang/src/vm/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/src/vm.rs` & `cao-lang-0.2.2/cao-lang/src/vm.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/tests/integration_tests.rs` & `cao-lang-0.2.2/cao-lang/tests/integration_tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/tests/test_fibonacci.rs` & `cao-lang-0.2.2/cao-lang/tests/test_fibonacci.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/tests/test_for_each.rs` & `cao-lang-0.2.2/cao-lang/tests/test_for_each.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/cao-lang/tests/test_tables.rs` & `cao-lang-0.2.2/cao-lang/tests/test_tables.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/py/cao_lang.egg-info/PKG-INFO` & `cao-lang-0.2.2/py/cao_lang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cao-lang
-Version: 0.2.1
+Version: 0.2.2
 Summary: The node based 'language' that governs the actors of the game Cao-Lo
 Home-page: https://github.com/caolo-game/cao-lang
 Author: Daniel Kiss
 Author-email: littlesnorrboy@gmail.com
 Project-URL: Bug Tracker, https://github.com/caolo-game/cao-lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cao-lang-0.2.1/py/cao_lang.egg-info/SOURCES.txt` & `cao-lang-0.2.2/py/cao_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/py/src/lib.rs` & `cao-lang-0.2.2/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/py/tests/test_cao_lang.py` & `cao-lang-0.2.2/py/tests/test_cao_lang.py`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.1/setup.py` & `cao-lang-0.2.2/setup.py`

 * *Files identical despite different names*

