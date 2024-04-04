# Comparing `tmp/cao-lang-0.2.2.tar.gz` & `tmp/cao-lang-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cao-lang-0.2.2.tar", last modified: Thu Apr  4 20:52:07 2024, max compression
+gzip compressed data, was "cao-lang-0.2.3.tar", last modified: Thu Apr  4 21:06:25 2024, max compression
```

## Comparing `cao-lang-0.2.2.tar` & `cao-lang-0.2.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.530055 cao-lang-0.2.2/
--rw-r--r--   0 runner     (501) staff       (20)     1068 2024-04-04 20:51:56.000000 cao-lang-0.2.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      123 2024-04-04 20:51:56.000000 cao-lang-0.2.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 20:52:07.529639 cao-lang-0.2.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1098 2024-04-04 20:51:56.000000 cao-lang-0.2.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.510831 cao-lang-0.2.2/cao-lang/
--rw-r--r--   0 runner     (501) staff       (20)     1317 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/Cargo.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.511165 cao-lang-0.2.2/cao-lang/benches/
--rw-r--r--   0 runner     (501) staff       (20)     4146 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/benches/cao_lang_benches.rs
--rw-r--r--   0 runner     (501) staff       (20)     1246 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/build.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.515131 cao-lang-0.2.2/cao-lang/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.515492 cao-lang-0.2.2/cao-lang/src/alloc/
--rw-r--r--   0 runner     (501) staff       (20)     3168 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/alloc/caolang_alloc.rs
--rw-r--r--   0 runner     (501) staff       (20)      999 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/alloc.rs
--rw-r--r--   0 runner     (501) staff       (20)     1115 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/bytecode.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.517474 cao-lang-0.2.2/cao-lang/src/collections/
--rw-r--r--   0 runner     (501) staff       (20)     3084 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/bounded_stack.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.518156 cao-lang-0.2.2/cao-lang/src/collections/handle_table/
--rw-r--r--   0 runner     (501) staff       (20)     3731 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/handle_table/serde_impl.rs
--rw-r--r--   0 runner     (501) staff       (20)     2316 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/handle_table/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    16517 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/handle_table.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.518778 cao-lang-0.2.2/cao-lang/src/collections/hash_map/
--rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/hash_map/serde_impl.rs
--rw-r--r--   0 runner     (501) staff       (20)     3547 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/hash_map/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    15603 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/hash_map.rs
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/mod.rs
--rw-r--r--   0 runner     (501) staff       (20)     5147 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/collections/value_stack.rs
--rw-r--r--   0 runner     (501) staff       (20)     6726 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiled_program.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.521377 cao-lang-0.2.2/cao-lang/src/compiler/
--rw-r--r--   0 runner     (501) staff       (20)    21154 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/card.rs
--rw-r--r--   0 runner     (501) staff       (20)     2273 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/compilation_error.rs
--rw-r--r--   0 runner     (501) staff       (20)      423 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/compile_options.rs
--rw-r--r--   0 runner     (501) staff       (20)      790 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/function.rs
--rw-r--r--   0 runner     (501) staff       (20)      793 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/function_ir.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.521673 cao-lang-0.2.2/cao-lang/src/compiler/module/
--rw-r--r--   0 runner     (501) staff       (20)     8441 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/module/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    17167 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/module.rs
--rw-r--r--   0 runner     (501) staff       (20)     3103 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    39021 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/compiler.rs
--rw-r--r--   0 runner     (501) staff       (20)     5505 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/instruction.rs
--rw-r--r--   0 runner     (501) staff       (20)     1606 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/lib.rs
--rw-r--r--   0 runner     (501) staff       (20)      403 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/prelude.rs
--rw-r--r--   0 runner     (501) staff       (20)     2992 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/procedures.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.522006 cao-lang-0.2.2/cao-lang/src/stdlib/
--rw-r--r--   0 runner     (501) staff       (20)    12839 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/stdlib/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    11742 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/stdlib.rs
--rw-r--r--   0 runner     (501) staff       (20)     5028 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/traits.rs
--rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/value.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.523089 cao-lang-0.2.2/cao-lang/src/vm/
--rw-r--r--   0 runner     (501) staff       (20)    17984 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/instr_execution.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.524438 cao-lang-0.2.2/cao-lang/src/vm/runtime/
--rw-r--r--   0 runner     (501) staff       (20)     1006 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_function.rs
--rw-r--r--   0 runner     (501) staff       (20)     6511 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_object.rs
--rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_string.rs
--rw-r--r--   0 runner     (501) staff       (20)     3729 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_table.rs
--rw-r--r--   0 runner     (501) staff       (20)    13858 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/runtime.rs
--rw-r--r--   0 runner     (501) staff       (20)     1882 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    33219 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/src/vm.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.525717 cao-lang-0.2.2/cao-lang/tests/
--rw-r--r--   0 runner     (501) staff       (20)    46718 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/integration_tests.rs
--rw-r--r--   0 runner     (501) staff       (20)     1820 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/test_fibonacci.rs
--rw-r--r--   0 runner     (501) staff       (20)     1146 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/test_for_each.rs
--rw-r--r--   0 runner     (501) staff       (20)     3227 2024-04-04 20:51:56.000000 cao-lang-0.2.2/cao-lang/tests/test_tables.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.526056 cao-lang-0.2.2/py/
--rw-r--r--   0 runner     (501) staff       (20)      420 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/Cargo.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.527479 cao-lang-0.2.2/py/cao_lang/
--rw-r--r--   0 runner     (501) staff       (20)       27 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/cao_lang/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.529224 cao-lang-0.2.2/py/cao_lang.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1917 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-04 20:52:07.000000 cao-lang-0.2.2/py/cao_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.526690 cao-lang-0.2.2/py/src/
--rw-r--r--   0 runner     (501) staff       (20)     2664 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/src/lib.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 20:52:07.526998 cao-lang-0.2.2/py/tests/
--rw-r--r--   0 runner     (501) staff       (20)     2713 2024-04-04 20:51:56.000000 cao-lang-0.2.2/py/tests/test_cao_lang.py
--rw-r--r--   0 runner     (501) staff       (20)      117 2024-04-04 20:51:56.000000 cao-lang-0.2.2/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-04 20:52:07.530135 cao-lang-0.2.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1430 2024-04-04 20:51:56.000000 cao-lang-0.2.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.705870 cao-lang-0.2.3/
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2024-04-04 21:06:14.000000 cao-lang-0.2.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      123 2024-04-04 21:06:14.000000 cao-lang-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 21:06:25.705318 cao-lang-0.2.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1098 2024-04-04 21:06:14.000000 cao-lang-0.2.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.677245 cao-lang-0.2.3/cao-lang/
+-rw-r--r--   0 runner     (501) staff       (20)     1317 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/Cargo.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.678083 cao-lang-0.2.3/cao-lang/benches/
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/benches/cao_lang_benches.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1246 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/build.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.683150 cao-lang-0.2.3/cao-lang/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.683556 cao-lang-0.2.3/cao-lang/src/alloc/
+-rw-r--r--   0 runner     (501) staff       (20)     3168 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/alloc/caolang_alloc.rs
+-rw-r--r--   0 runner     (501) staff       (20)      999 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/alloc.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1115 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/bytecode.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.685886 cao-lang-0.2.3/cao-lang/src/collections/
+-rw-r--r--   0 runner     (501) staff       (20)     3084 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/bounded_stack.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.686679 cao-lang-0.2.3/cao-lang/src/collections/handle_table/
+-rw-r--r--   0 runner     (501) staff       (20)     3731 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/handle_table/serde_impl.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2316 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/handle_table/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    16517 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/handle_table.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.687484 cao-lang-0.2.3/cao-lang/src/collections/hash_map/
+-rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/hash_map/serde_impl.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3547 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/hash_map/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    15603 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/hash_map.rs
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/mod.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/value_stack.rs
+-rw-r--r--   0 runner     (501) staff       (20)     6726 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiled_program.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.691843 cao-lang-0.2.3/cao-lang/src/compiler/
+-rw-r--r--   0 runner     (501) staff       (20)    21508 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/card.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2273 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/compilation_error.rs
+-rw-r--r--   0 runner     (501) staff       (20)      423 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/compile_options.rs
+-rw-r--r--   0 runner     (501) staff       (20)      790 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/function.rs
+-rw-r--r--   0 runner     (501) staff       (20)      793 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/function_ir.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.692237 cao-lang-0.2.3/cao-lang/src/compiler/module/
+-rw-r--r--   0 runner     (501) staff       (20)     8441 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/module/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    17167 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/module.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3103 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    39021 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5505 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/instruction.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1606 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/lib.rs
+-rw-r--r--   0 runner     (501) staff       (20)      403 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/prelude.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2992 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/procedures.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.692589 cao-lang-0.2.3/cao-lang/src/stdlib/
+-rw-r--r--   0 runner     (501) staff       (20)    12839 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/stdlib/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    11742 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/stdlib.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5028 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/traits.rs
+-rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/value.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.694389 cao-lang-0.2.3/cao-lang/src/vm/
+-rw-r--r--   0 runner     (501) staff       (20)    17984 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/instr_execution.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.696543 cao-lang-0.2.3/cao-lang/src/vm/runtime/
+-rw-r--r--   0 runner     (501) staff       (20)     1006 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_function.rs
+-rw-r--r--   0 runner     (501) staff       (20)     6511 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_object.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_string.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3729 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_table.rs
+-rw-r--r--   0 runner     (501) staff       (20)    13858 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1882 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    33219 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.698609 cao-lang-0.2.3/cao-lang/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    46718 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/integration_tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1820 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/test_fibonacci.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1146 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/test_for_each.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3227 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/test_tables.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.699120 cao-lang-0.2.3/py/
+-rw-r--r--   0 runner     (501) staff       (20)      420 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/Cargo.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.701374 cao-lang-0.2.3/py/cao_lang/
+-rw-r--r--   0 runner     (501) staff       (20)       27 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/cao_lang/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.704645 cao-lang-0.2.3/py/cao_lang.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1917 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.700141 cao-lang-0.2.3/py/src/
+-rw-r--r--   0 runner     (501) staff       (20)     2664 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/src/lib.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.700600 cao-lang-0.2.3/py/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     2713 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/tests/test_cao_lang.py
+-rw-r--r--   0 runner     (501) staff       (20)      117 2024-04-04 21:06:14.000000 cao-lang-0.2.3/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-04 21:06:25.705990 cao-lang-0.2.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1430 2024-04-04 21:06:14.000000 cao-lang-0.2.3/setup.py
```

### Comparing `cao-lang-0.2.2/LICENSE` & `cao-lang-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/PKG-INFO` & `cao-lang-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cao-lang
-Version: 0.2.2
+Version: 0.2.3
 Summary: The node based 'language' that governs the actors of the game Cao-Lo
 Home-page: https://github.com/caolo-game/cao-lang
 Author: Daniel Kiss
 Author-email: littlesnorrboy@gmail.com
 Project-URL: Bug Tracker, https://github.com/caolo-game/cao-lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cao-lang-0.2.2/README.md` & `cao-lang-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/Cargo.toml` & `cao-lang-0.2.3/cao-lang/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,8 @@
 build = "build.rs"
 description = "The back-end of cao-lang, a node based visual scripting language"
 edition = "2021"
 license = "MIT"
 name = "cao-lang"
 readme = "../README.md"
 repository = "https://github.com/caolo-game/cao-lang.git"
-version = "0.2.2"
+version = "0.2.3"
```

### Comparing `cao-lang-0.2.2/cao-lang/benches/cao_lang_benches.rs` & `cao-lang-0.2.3/cao-lang/benches/cao_lang_benches.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/build.rs` & `cao-lang-0.2.3/cao-lang/build.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/alloc/caolang_alloc.rs` & `cao-lang-0.2.3/cao-lang/src/alloc/caolang_alloc.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/alloc.rs` & `cao-lang-0.2.3/cao-lang/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/bytecode.rs` & `cao-lang-0.2.3/cao-lang/src/bytecode.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/bounded_stack.rs` & `cao-lang-0.2.3/cao-lang/src/collections/bounded_stack.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/handle_table/serde_impl.rs` & `cao-lang-0.2.3/cao-lang/src/collections/handle_table/serde_impl.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/handle_table/tests.rs` & `cao-lang-0.2.3/cao-lang/src/collections/handle_table/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/handle_table.rs` & `cao-lang-0.2.3/cao-lang/src/collections/handle_table.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/hash_map/serde_impl.rs` & `cao-lang-0.2.3/cao-lang/src/collections/hash_map/serde_impl.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/hash_map/tests.rs` & `cao-lang-0.2.3/cao-lang/src/collections/hash_map/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/hash_map.rs` & `cao-lang-0.2.3/cao-lang/src/collections/hash_map.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/collections/value_stack.rs` & `cao-lang-0.2.3/cao-lang/src/collections/value_stack.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiled_program.rs` & `cao-lang-0.2.3/cao-lang/src/compiled_program.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/card.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/card.rs`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
         Self::Function(s.into())
     }
 
     pub fn get_child_mut(&mut self, i: usize) -> Option<&mut Card> {
         let res;
         match self {
             Card::CompositeCard(c) => res = c.cards.get_mut(i)?,
+            Card::Closure(c) => res = c.cards.get_mut(i)?,
             Card::Repeat(rep) => match i {
                 0 => res = &mut rep.n,
                 1 => res = &mut rep.body,
                 _ => return None,
             },
             Card::IfTrue(c) | Card::IfFalse(c) => return c.get_mut(i),
             Card::ForEach(fe) => {
@@ -304,15 +305,14 @@
                 return (i == 0)
                     .then_some(&mut j.function)
                     .or_else(|| j.args.0.get_mut(i - 1))
             }
             Card::Array(cards) => return cards.get_mut(i),
             Card::Function(_)
             | Card::NativeFunction(_)
-            | Card::Closure(_)
             | Card::ReadVar(_)
             | Card::ScalarInt(_)
             | Card::ScalarFloat(_)
             | Card::StringLiteral(_)
             | Card::Comment(_)
             | Card::ScalarNil
             | Card::CreateTable
@@ -321,14 +321,15 @@
         Some(res)
     }
 
     pub fn get_child(&self, i: usize) -> Option<&Card> {
         let res;
         match self {
             Card::CompositeCard(c) => res = c.cards.get(i)?,
+            Card::Closure(c) => res = c.cards.get(i)?,
             Card::Repeat(rep) => match i {
                 0 => res = &rep.n,
                 1 => res = &rep.body,
                 _ => return None,
             },
             Card::IfTrue(c) | Card::IfFalse(c) => return c.get(i),
             Card::ForEach(fe) => {
@@ -380,15 +381,14 @@
                 return (i == 0)
                     .then_some(&j.function)
                     .or_else(|| j.args.0.get(i - 1))
             }
             Card::Array(cards) => return cards.get(i),
             Card::Function(_)
             | Card::NativeFunction(_)
-            | Card::Closure(_)
             | Card::ReadVar(_)
             | Card::ScalarInt(_)
             | Card::ScalarFloat(_)
             | Card::StringLiteral(_)
             | Card::Comment(_)
             | Card::ScalarNil
             | Card::CreateTable
@@ -402,14 +402,20 @@
         match self {
             Card::CompositeCard(c) => {
                 if c.cards.len() <= i {
                     return None;
                 }
                 res = c.cards.remove(i);
             }
+            Card::Closure(c) => {
+                if c.cards.len() <= i {
+                    return None;
+                }
+                res = c.cards.remove(i);
+            }
             Card::Repeat(rep) => match i {
                 0 => res = std::mem::replace(&mut rep.n, Card::ScalarInt(0)),
                 1 => res = std::mem::replace(&mut rep.body, Card::ScalarNil),
                 _ => return None,
             },
             Card::IfTrue(_) | Card::IfFalse(_) => match self.get_child_mut(i) {
                 Some(c) => {
@@ -479,15 +485,14 @@
             Card::Function(_)
             | Card::NativeFunction(_)
             | Card::ReadVar(_)
             | Card::ScalarInt(_)
             | Card::ScalarFloat(_)
             | Card::StringLiteral(_)
             | Card::Comment(_)
-            | Card::Closure(_)
             | Card::ScalarNil
             | Card::CreateTable
             | Card::Abort => return None,
         }
         Some(res)
     }
 
@@ -499,14 +504,20 @@
         match self {
             Card::CompositeCard(c) => {
                 if c.cards.len() < i {
                     return Err(card);
                 }
                 c.cards.insert(i, card);
             }
+            Card::Closure(c) => {
+                if c.cards.len() < i {
+                    return Err(card);
+                }
+                c.cards.insert(i, card);
+            }
 
             Card::ForEach(fe) => {
                 let ForEach {
                     i: _,
                     k: _,
                     v: _,
                     iterable: a,
@@ -574,15 +585,14 @@
                 } else {
                     return Err(card);
                 }
             }
             Card::Function(_)
             | Card::NativeFunction(_)
             | Card::ReadVar(_)
-            | Card::Closure(_)
             | Card::ScalarInt(_)
             | Card::ScalarFloat(_)
             | Card::StringLiteral(_)
             | Card::Comment(_)
             | Card::ScalarNil
             | Card::CreateTable
             | Card::Abort => return Err(card),
```

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/compilation_error.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/compilation_error.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/function.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/function.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/function_ir.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/function_ir.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/module/tests.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/module/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/module.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/module.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler/tests.rs` & `cao-lang-0.2.3/cao-lang/src/compiler/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/compiler.rs` & `cao-lang-0.2.3/cao-lang/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/instruction.rs` & `cao-lang-0.2.3/cao-lang/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/lib.rs` & `cao-lang-0.2.3/cao-lang/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/procedures.rs` & `cao-lang-0.2.3/cao-lang/src/procedures.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/stdlib/tests.rs` & `cao-lang-0.2.3/cao-lang/src/stdlib/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/stdlib.rs` & `cao-lang-0.2.3/cao-lang/src/stdlib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/traits.rs` & `cao-lang-0.2.3/cao-lang/src/traits.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/value.rs` & `cao-lang-0.2.3/cao-lang/src/value.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/instr_execution.rs` & `cao-lang-0.2.3/cao-lang/src/vm/instr_execution.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_function.rs` & `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_function.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_object.rs` & `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_object.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_string.rs` & `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_string.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/runtime/cao_lang_table.rs` & `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_table.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/runtime.rs` & `cao-lang-0.2.3/cao-lang/src/vm/runtime.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm/tests.rs` & `cao-lang-0.2.3/cao-lang/src/vm/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/src/vm.rs` & `cao-lang-0.2.3/cao-lang/src/vm.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/tests/integration_tests.rs` & `cao-lang-0.2.3/cao-lang/tests/integration_tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/tests/test_fibonacci.rs` & `cao-lang-0.2.3/cao-lang/tests/test_fibonacci.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/tests/test_for_each.rs` & `cao-lang-0.2.3/cao-lang/tests/test_for_each.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/cao-lang/tests/test_tables.rs` & `cao-lang-0.2.3/cao-lang/tests/test_tables.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/py/cao_lang.egg-info/PKG-INFO` & `cao-lang-0.2.3/py/cao_lang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cao-lang
-Version: 0.2.2
+Version: 0.2.3
 Summary: The node based 'language' that governs the actors of the game Cao-Lo
 Home-page: https://github.com/caolo-game/cao-lang
 Author: Daniel Kiss
 Author-email: littlesnorrboy@gmail.com
 Project-URL: Bug Tracker, https://github.com/caolo-game/cao-lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cao-lang-0.2.2/py/cao_lang.egg-info/SOURCES.txt` & `cao-lang-0.2.3/py/cao_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/py/src/lib.rs` & `cao-lang-0.2.3/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/py/tests/test_cao_lang.py` & `cao-lang-0.2.3/py/tests/test_cao_lang.py`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.2/setup.py` & `cao-lang-0.2.3/setup.py`

 * *Files identical despite different names*

