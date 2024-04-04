# Comparing `tmp/macal-5.0rc8.tar.gz` & `tmp/macal-5.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macal-5.0rc8.tar", last modified: Mon Nov 13 18:05:18 2023, max compression
+gzip compressed data, was "macal-5.0rc9.tar", last modified: Mon Nov 13 20:39:07 2023, max compression
```

## Comparing `macal-5.0rc8.tar` & `macal-5.0rc9.tar`

### file list

```diff
@@ -1,187 +1,190 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.407198 macal-5.0rc8/
--rw-r--r--   0 marco     (1000) marco     (1000)     1121 2023-03-07 14:15:31.000000 macal-5.0rc8/LICENSE.txt
--rw-r--r--   0 marco     (1000) marco     (1000)      153 2023-11-13 10:28:47.000000 macal-5.0rc8/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)    32449 2023-11-13 18:05:18.407198 macal-5.0rc8/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)    31916 2023-11-10 01:04:08.000000 macal-5.0rc8/README.md
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.397198 macal-5.0rc8/documentation/
--rw-r--r--   0 marco     (1000) marco     (1000)     4950 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/General_Design_Interpreter_VM_Instructions_Opcodes_Etc.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     5119 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/ascii_art.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     3159 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/fib.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     2380 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/foreach.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     2121 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/function6_lex.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     7076 2023-10-24 20:15:07.000000 macal-5.0rc8/documentation/history.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-10-24 20:15:07.000000 macal-5.0rc8/documentation/links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1994 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/performance_bottlenecks.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     3385 2023-10-24 20:17:32.000000 macal-5.0rc8/documentation/register_flags.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1320 2023-10-24 20:15:07.000000 macal-5.0rc8/documentation/tests.md
--rw-r--r--   0 marco     (1000) marco     (1000)    10194 2023-10-24 20:15:07.000000 macal-5.0rc8/documentation/variables_and_scope.md
--rw-r--r--   0 marco     (1000) marco     (1000)      750 2023-11-13 18:03:28.000000 macal-5.0rc8/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-11-13 18:05:18.407198 macal-5.0rc8/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.387198 macal-5.0rc8/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.397198 macal-5.0rc8/src/macal/
--rw-r--r--   0 marco     (1000) marco     (1000)      345 2023-10-28 02:37:06.000000 macal-5.0rc8/src/macal/__about__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      170 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      629 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2148 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_assignment.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1193 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_binary_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)      919 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_block.py
--rw-r--r--   0 marco     (1000) marco     (1000)      790 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_break_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      922 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_case_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      807 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_continue_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      700 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_default_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1148 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_elif_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      828 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_else_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1013 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1132 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_foreach_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1157 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_function_call_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1653 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_function_call_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2061 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_function_definition.py
--rw-r--r--   0 marco     (1000) marco     (1000)      915 2023-11-10 19:10:31.000000 macal-5.0rc8/src/macal/ast_node_function_parameter.py
--rw-r--r--   0 marco     (1000) marco     (1000)      969 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_halt_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1518 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_if_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1091 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_include_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1066 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_indexed_variable_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1000 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_istype.py
--rw-r--r--   0 marco     (1000) marco     (1000)      908 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_library_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1109 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_literal_array_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1628 2023-11-10 18:26:22.000000 macal-5.0rc8/src/macal/ast_node_literal_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1144 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_literal_record_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1025 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_print_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      943 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_program.py
--rw-r--r--   0 marco     (1000) marco     (1000)      981 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_return_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1694 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_select_field.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1763 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_select_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1012 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      968 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_switch_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      872 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_type_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1107 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_unary_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1026 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_variable.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1059 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_variable_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1272 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_variable_function_call_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1219 2023-11-10 18:26:18.000000 macal-5.0rc8/src/macal/ast_node_while_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4528 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/ast_nodetype.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1078 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_address.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4789 2023-11-10 01:15:23.000000 macal-5.0rc8/src/macal/bytecode_debugger.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3805 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_flags_register.py
--rw-r--r--   0 marco     (1000) marco     (1000)      449 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_function.py
--rw-r--r--   0 marco     (1000) marco     (1000)      648 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_jump.py
--rw-r--r--   0 marco     (1000) marco     (1000)      687 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_label.py
--rw-r--r--   0 marco     (1000) marco     (1000)      656 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_library.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3281 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/bytecode_optimizer.py
--rw-r--r--   0 marco     (1000) marco     (1000)     7852 2023-11-10 19:13:39.000000 macal-5.0rc8/src/macal/bytecode_register.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5500 2023-11-10 19:13:35.000000 macal-5.0rc8/src/macal/bytecode_variable.py
--rw-r--r--   0 marco     (1000) marco     (1000)    36217 2023-11-13 18:01:19.000000 macal-5.0rc8/src/macal/cmacal_vm.pyx
--rw-r--r--   0 marco     (1000) marco     (1000)     7203 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/compiler_scope.py
--rw-r--r--   0 marco     (1000) marco     (1000)      401 2023-11-13 17:19:20.000000 macal-5.0rc8/src/macal/config.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5037 2023-11-10 17:15:05.000000 macal-5.0rc8/src/macal/conversion.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1341 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/ct_function.py
--rw-r--r--   0 marco     (1000) marco     (1000)      971 2023-11-10 17:14:16.000000 macal-5.0rc8/src/macal/ct_variable.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1186 2023-11-10 17:15:05.000000 macal-5.0rc8/src/macal/lex_token.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.397198 macal-5.0rc8/src/macal/lib/
--rw-r--r--   0 marco     (1000) marco     (1000)      284 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/csv.mcl
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.397198 macal-5.0rc8/src/macal/lib/ext/
--rw-r--r--   0 marco     (1000) marco     (1000)      682 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_csv.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1723 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_io.py
--rw-r--r--   0 marco     (1000) marco     (1000)      504 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_keyring.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1880 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_math.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2044 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_strings.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3723 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_syslog.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2429 2023-11-09 20:29:57.000000 macal-5.0rc8/src/macal/lib/ext/ext_system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1617 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/ext/ext_time.py
--rw-r--r--   0 marco     (1000) marco     (1000)    30467 2023-10-25 01:43:22.000000 macal-5.0rc8/src/macal/lib/ext/meraki_api_library_v1.py
--rw-r--r--   0 marco     (1000) marco     (1000)      544 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/io.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      383 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/keyring.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      916 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/math.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     4241 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/meraki_v1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1023 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/strings.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      302 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/syslog.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1116 2023-11-09 20:28:03.000000 macal-5.0rc8/src/macal/lib/system.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      620 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/lib/time.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    51453 2023-11-13 14:40:57.000000 macal-5.0rc8/src/macal/macal_compiler.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3248 2023-11-13 14:40:19.000000 macal-5.0rc8/src/macal/macal_decompiler.py
--rw-r--r--   0 marco     (1000) marco     (1000)    14513 2023-11-13 13:47:51.000000 macal-5.0rc8/src/macal/macal_instruction_emitter.py
--rw-r--r--   0 marco     (1000) marco     (1000)    12064 2023-11-13 13:45:27.000000 macal-5.0rc8/src/macal/macal_instructions.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2729 2023-11-10 01:15:23.000000 macal-5.0rc8/src/macal/macal_interactive.py
--rw-r--r--   0 marco     (1000) marco     (1000)    15971 2023-11-10 17:15:05.000000 macal-5.0rc8/src/macal/macal_lexer.py
--rw-r--r--   0 marco     (1000) marco     (1000)    35358 2023-11-13 11:01:52.000000 macal-5.0rc8/src/macal/macal_parser.py
--rw-r--r--   0 marco     (1000) marco     (1000)    30925 2023-11-13 18:02:55.000000 macal-5.0rc8/src/macal/macal_select_compiler.py
--rw-r--r--   0 marco     (1000) marco     (1000)    34334 2023-11-10 19:15:30.000000 macal-5.0rc8/src/macal/macal_vm.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3343 2023-11-09 23:58:00.000000 macal-5.0rc8/src/macal/mc.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2324 2023-11-09 20:53:14.000000 macal-5.0rc8/src/macal/md.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4927 2023-11-13 00:13:55.000000 macal-5.0rc8/src/macal/mi.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1984 2023-11-13 14:40:30.000000 macal-5.0rc8/src/macal/mr.py
--rw-r--r--   0 marco     (1000) marco     (1000)      781 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/python_module_info.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1394 2023-11-10 17:14:16.000000 macal-5.0rc8/src/macal/runtime_scope.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2316 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/statement_type_table.py
--rw-r--r--   0 marco     (1000) marco     (1000)      394 2023-10-24 20:17:32.000000 macal-5.0rc8/src/macal/switch_case_table.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.397198 macal-5.0rc8/src/macal.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)    32449 2023-11-13 18:05:18.000000 macal-5.0rc8/src/macal.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     4778 2023-11-13 18:05:18.000000 macal-5.0rc8/src/macal.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-11-13 18:05:18.000000 macal-5.0rc8/src/macal.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       90 2023-11-13 18:05:18.000000 macal-5.0rc8/src/macal.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       17 2023-11-13 18:05:18.000000 macal-5.0rc8/src/macal.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        6 2023-11-13 18:05:18.000000 macal-5.0rc8/src/macal.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 18:05:18.407198 macal-5.0rc8/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)      529 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/aor.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1486 2023-11-09 20:38:02.000000 macal-5.0rc8/tests/args.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)       32 2023-11-09 20:31:23.000000 macal-5.0rc8/tests/args.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      442 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/artest.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      255 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/bleed_test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      116 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/continue.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      334 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/fetest.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      172 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/fn_def.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      121 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/fnfnt.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      385 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/function.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       94 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/function2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      228 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/function3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      287 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/function4.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3559 2023-11-11 21:51:37.000000 macal-5.0rc8/tests/function5.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      541 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/function5.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      357 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/function6.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       51 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/halt_test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      475 2023-11-13 00:12:46.000000 macal-5.0rc8/tests/if.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      124 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/if.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      155 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/if2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      938 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/iftest.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      159 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/include_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      112 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/include_2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       96 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/indexed_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       89 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/indexed_2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/indexed_3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       54 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/indexed_4.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      172 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/indexed_5.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      550 2023-11-13 11:08:02.000000 macal-5.0rc8/tests/indexed_6.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      101 2023-11-13 11:06:52.000000 macal-5.0rc8/tests/indexed_6.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       27 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/interpolation_shorts.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1245 2023-11-09 20:24:45.000000 macal-5.0rc8/tests/libvar.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)       40 2023-11-09 20:24:22.000000 macal-5.0rc8/tests/libvar.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    46965 2023-11-13 14:46:31.000000 macal-5.0rc8/tests/mdi.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)     5722 2023-11-13 14:45:37.000000 macal-5.0rc8/tests/mdi.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3827 2023-11-13 11:07:54.000000 macal-5.0rc8/tests/meraki_firewall_dc.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3001 2023-11-13 11:30:59.000000 macal-5.0rc8/tests/meraki_firewall_sh.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     7301 2023-10-25 01:39:02.000000 macal-5.0rc8/tests/meraki_test.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      613 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/meraki_test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     6804 2023-11-10 01:30:08.000000 macal-5.0rc8/tests/mt.py
--rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/nested.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2198 2023-11-13 01:31:23.000000 macal-5.0rc8/tests/select_1.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/select_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      689 2023-11-13 10:01:28.000000 macal-5.0rc8/tests/select_2.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      160 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/select_2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2365 2023-11-13 10:01:37.000000 macal-5.0rc8/tests/select_3.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      557 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/select_3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      607 2023-11-13 10:01:40.000000 macal-5.0rc8/tests/select_4.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      264 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/select_4.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3954 2023-11-13 10:01:43.000000 macal-5.0rc8/tests/select_5.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      281 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/select_5.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      802 2023-11-13 14:16:57.000000 macal-5.0rc8/tests/select_7.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      196 2023-11-13 14:14:32.000000 macal-5.0rc8/tests/select_7.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1437 2023-11-13 18:03:42.000000 macal-5.0rc8/tests/select_8.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      611 2023-11-13 17:22:36.000000 macal-5.0rc8/tests/select_8.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      213 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/switch_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1011 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       96 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/test2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      139 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/test3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1052 2023-11-10 00:25:51.000000 macal-5.0rc8/tests/usereserved.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      798 2023-11-10 00:25:30.000000 macal-5.0rc8/tests/usereserved.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      131 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/variable.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      176 2023-10-24 20:17:32.000000 macal-5.0rc8/tests/whiletest.mcl
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1121 2023-03-07 14:15:31.000000 macal-5.0rc9/LICENSE.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)      153 2023-11-13 19:19:23.000000 macal-5.0rc9/MANIFEST.in
+-rw-r--r--   0 marco     (1000) marco     (1000)    32449 2023-11-13 20:39:07.615218 macal-5.0rc9/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)    31916 2023-11-13 19:19:23.000000 macal-5.0rc9/README.md
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.605218 macal-5.0rc9/documentation/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4950 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/General_Design_Interpreter_VM_Instructions_Opcodes_Etc.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     5119 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/ascii_art.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     3159 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/fib.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     2380 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/foreach.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     2121 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/function6_lex.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     7076 2023-10-24 20:15:07.000000 macal-5.0rc9/documentation/history.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1994 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/performance_bottlenecks.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     3385 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/register_flags.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1320 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/tests.md
+-rw-r--r--   0 marco     (1000) marco     (1000)    10194 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/variables_and_scope.md
+-rw-r--r--   0 marco     (1000) marco     (1000)      750 2023-11-13 20:37:36.000000 macal-5.0rc9/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-11-13 20:39:07.615218 macal-5.0rc9/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.605218 macal-5.0rc9/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal/
+-rw-r--r--   0 marco     (1000) marco     (1000)      345 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/__about__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      170 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      629 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2148 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_assignment.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1193 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_binary_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      919 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_block.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      790 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_break_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      922 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_case_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      807 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_continue_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      700 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_default_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1148 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_elif_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      828 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_else_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1013 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1132 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_foreach_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1157 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_call_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1653 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_call_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2061 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_definition.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      915 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_parameter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      969 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_halt_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1518 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_if_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1091 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_include_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1066 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_indexed_variable_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1000 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_istype.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      908 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_library_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1109 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_literal_array_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1628 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_literal_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1144 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_literal_record_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1025 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_print_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      943 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_program.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      981 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_return_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1694 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_select_field.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1763 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_select_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1012 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      968 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_switch_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      872 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_type_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1107 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_unary_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1026 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_variable.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1059 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_variable_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1272 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_variable_function_call_expression.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1219 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_while_statement.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4528 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_nodetype.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1078 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_address.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4789 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_debugger.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3805 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_flags_register.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      449 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_function.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      648 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_jump.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      687 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_label.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      656 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_library.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3320 2023-11-13 19:57:56.000000 macal-5.0rc9/src/macal/bytecode_optimizer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     7852 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_register.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5500 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_variable.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    36802 2023-11-13 20:06:30.000000 macal-5.0rc9/src/macal/cmacal_vm.pyx
+-rw-r--r--   0 marco     (1000) marco     (1000)     7203 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/compiler_scope.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      401 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/config.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5037 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/conversion.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1341 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ct_function.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      971 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ct_variable.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1186 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lex_token.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal/lib/
+-rw-r--r--   0 marco     (1000) marco     (1000)      284 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/csv.mcl
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal/lib/ext/
+-rw-r--r--   0 marco     (1000) marco     (1000)      682 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_csv.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1723 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_io.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      504 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_keyring.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1880 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_math.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2044 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_strings.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3723 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_syslog.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2429 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1617 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    30467 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/meraki_api_library_v1.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      544 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/io.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      383 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/keyring.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      916 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/math.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     4241 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/meraki_v1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1023 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/strings.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      302 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/syslog.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1116 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/system.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      620 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/time.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)    51453 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_compiler.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3248 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_decompiler.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    14642 2023-11-13 19:37:29.000000 macal-5.0rc9/src/macal/macal_instruction_emitter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    12185 2023-11-13 19:34:40.000000 macal-5.0rc9/src/macal/macal_instructions.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2729 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_interactive.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    15971 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_lexer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    35358 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_parser.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    32749 2023-11-13 20:15:04.000000 macal-5.0rc9/src/macal/macal_select_compiler.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3343 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/mc.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2324 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/md.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4927 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/mi.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1984 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/mr.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      781 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/python_module_info.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1394 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/runtime_scope.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2316 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/statement_type_table.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      394 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/switch_case_table.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)    32449 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     4832 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       90 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       17 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        6 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)      529 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/aor.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1486 2023-11-09 20:38:02.000000 macal-5.0rc9/tests/args.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)       32 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/args.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      442 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/artest.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      255 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/bleed_test.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      116 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/continue.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      334 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/fetest.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      172 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/fn_def.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      121 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/fnfnt.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      385 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       94 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function2.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      228 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function3.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      287 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function4.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     3559 2023-11-11 21:51:37.000000 macal-5.0rc9/tests/function5.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      541 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function5.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      357 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function6.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       51 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/halt_test.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      475 2023-11-13 00:12:46.000000 macal-5.0rc9/tests/if.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      124 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/if.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      155 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/if2.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      938 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/iftest.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      159 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/include_1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      112 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/include_2.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       96 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       89 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_2.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_3.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       54 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_4.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      172 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_5.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      550 2023-11-13 11:08:02.000000 macal-5.0rc9/tests/indexed_6.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      101 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_6.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       27 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/interpolation_shorts.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1245 2023-11-09 20:24:45.000000 macal-5.0rc9/tests/libvar.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)       40 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/libvar.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)    46965 2023-11-13 14:46:31.000000 macal-5.0rc9/tests/mdi.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)     5722 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/mdi.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     3827 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/meraki_firewall_dc.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     3001 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/meraki_firewall_sh.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     7301 2023-10-25 01:39:02.000000 macal-5.0rc9/tests/meraki_test.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      613 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/meraki_test.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     6804 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/mt.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/nested.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2198 2023-11-13 01:31:23.000000 macal-5.0rc9/tests/select_1.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      689 2023-11-13 10:01:28.000000 macal-5.0rc9/tests/select_2.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      160 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_2.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2365 2023-11-13 10:01:37.000000 macal-5.0rc9/tests/select_3.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      557 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_3.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      607 2023-11-13 10:01:40.000000 macal-5.0rc9/tests/select_4.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      264 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_4.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     4328 2023-11-13 20:08:24.000000 macal-5.0rc9/tests/select_5.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      583 2023-11-13 20:11:27.000000 macal-5.0rc9/tests/select_5.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     4586 2023-11-13 20:15:11.000000 macal-5.0rc9/tests/select_6.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      486 2023-11-13 20:14:09.000000 macal-5.0rc9/tests/select_6.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      955 2023-11-13 19:50:16.000000 macal-5.0rc9/tests/select_7.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      196 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_7.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1437 2023-11-13 18:03:42.000000 macal-5.0rc9/tests/select_8.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      611 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_8.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2956 2023-11-13 20:17:34.000000 macal-5.0rc9/tests/select_9.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      190 2023-11-13 20:17:18.000000 macal-5.0rc9/tests/select_9.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      213 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/switch_1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1011 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/test.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)       96 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/test2.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      139 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/test3.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1052 2023-11-10 00:25:51.000000 macal-5.0rc9/tests/usereserved.mbc
+-rw-r--r--   0 marco     (1000) marco     (1000)      798 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/usereserved.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      131 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/variable.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      176 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/whiletest.mcl
```

### Comparing `macal-5.0rc8/LICENSE.txt` & `macal-5.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/PKG-INFO` & `macal-5.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macal
-Version: 5.0rc8
+Version: 5.0rc9
 Summary: Macal is a DSL for collecting and transforming data from various sources.
 Author-email: Marco Caspers <SamaDevTeam@westcon.com>
 Project-URL: Homepage, https://github.com/Sama-Developer/macal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `macal-5.0rc8/README.md` & `macal-5.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/General_Design_Interpreter_VM_Instructions_Opcodes_Etc.txt` & `macal-5.0rc9/documentation/General_Design_Interpreter_VM_Instructions_Opcodes_Etc.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/ascii_art.txt` & `macal-5.0rc9/documentation/ascii_art.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/fib.txt` & `macal-5.0rc9/documentation/fib.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/foreach.txt` & `macal-5.0rc9/documentation/foreach.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/function6_lex.txt` & `macal-5.0rc9/documentation/function6_lex.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/history.txt` & `macal-5.0rc9/documentation/history.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/performance_bottlenecks.txt` & `macal-5.0rc9/documentation/performance_bottlenecks.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/register_flags.txt` & `macal-5.0rc9/documentation/register_flags.txt`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/tests.md` & `macal-5.0rc9/documentation/tests.md`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/documentation/variables_and_scope.md` & `macal-5.0rc9/documentation/variables_and_scope.md`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node.py` & `macal-5.0rc9/src/macal/ast_node.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_assignment.py` & `macal-5.0rc9/src/macal/ast_node_assignment.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_binary_expression.py` & `macal-5.0rc9/src/macal/ast_node_binary_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_block.py` & `macal-5.0rc9/src/macal/ast_node_block.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_break_statement.py` & `macal-5.0rc9/src/macal/ast_node_break_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_case_statement.py` & `macal-5.0rc9/src/macal/ast_node_case_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_continue_statement.py` & `macal-5.0rc9/src/macal/ast_node_continue_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_default_statement.py` & `macal-5.0rc9/src/macal/ast_node_default_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_elif_statement.py` & `macal-5.0rc9/src/macal/ast_node_elif_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_else_statement.py` & `macal-5.0rc9/src/macal/ast_node_else_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_expression.py` & `macal-5.0rc9/src/macal/ast_node_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_foreach_statement.py` & `macal-5.0rc9/src/macal/ast_node_foreach_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_function_call_expression.py` & `macal-5.0rc9/src/macal/ast_node_function_call_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_function_call_statement.py` & `macal-5.0rc9/src/macal/ast_node_function_call_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_function_definition.py` & `macal-5.0rc9/src/macal/ast_node_function_definition.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_function_parameter.py` & `macal-5.0rc9/src/macal/ast_node_function_parameter.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_halt_statement.py` & `macal-5.0rc9/src/macal/ast_node_halt_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_if_statement.py` & `macal-5.0rc9/src/macal/ast_node_if_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_include_statement.py` & `macal-5.0rc9/src/macal/ast_node_include_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_indexed_variable_expression.py` & `macal-5.0rc9/src/macal/ast_node_indexed_variable_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_istype.py` & `macal-5.0rc9/src/macal/ast_node_istype.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_library_expression.py` & `macal-5.0rc9/src/macal/ast_node_library_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_literal_array_expression.py` & `macal-5.0rc9/src/macal/ast_node_literal_array_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_literal_expression.py` & `macal-5.0rc9/src/macal/ast_node_literal_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_literal_record_expression.py` & `macal-5.0rc9/src/macal/ast_node_literal_record_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_print_statement.py` & `macal-5.0rc9/src/macal/ast_node_print_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_program.py` & `macal-5.0rc9/src/macal/ast_node_program.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_return_statement.py` & `macal-5.0rc9/src/macal/ast_node_return_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_select_field.py` & `macal-5.0rc9/src/macal/ast_node_select_field.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_select_statement.py` & `macal-5.0rc9/src/macal/ast_node_select_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_statement.py` & `macal-5.0rc9/src/macal/ast_node_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_switch_statement.py` & `macal-5.0rc9/src/macal/ast_node_switch_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_type_statement.py` & `macal-5.0rc9/src/macal/ast_node_type_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_unary_expression.py` & `macal-5.0rc9/src/macal/ast_node_unary_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_variable.py` & `macal-5.0rc9/src/macal/ast_node_variable.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_variable_expression.py` & `macal-5.0rc9/src/macal/ast_node_variable_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_variable_function_call_expression.py` & `macal-5.0rc9/src/macal/ast_node_variable_function_call_expression.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_node_while_statement.py` & `macal-5.0rc9/src/macal/ast_node_while_statement.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ast_nodetype.py` & `macal-5.0rc9/src/macal/ast_nodetype.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_address.py` & `macal-5.0rc9/src/macal/bytecode_address.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_debugger.py` & `macal-5.0rc9/src/macal/bytecode_debugger.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_flags_register.py` & `macal-5.0rc9/src/macal/bytecode_flags_register.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_jump.py` & `macal-5.0rc9/src/macal/bytecode_jump.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_label.py` & `macal-5.0rc9/src/macal/bytecode_label.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_library.py` & `macal-5.0rc9/src/macal/bytecode_library.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_optimizer.py` & `macal-5.0rc9/src/macal/bytecode_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 #
 
 # This is the bytecode optimizer.
 # The Optimizer will attempt to optimize the bytecode that was emitted by the compiler by the following strategies:
 # - remove push/pop pairs for the same register.
 
 from __future__ import annotations
-from .macal_vm import MacalVm
+import pyximport; pyximport.install()
+from .cmacal_vm import MacalVm
 from .compiler_scope import CompilerScope
 from .macal_instructions import MacalInstructionList
 from .bytecode_address import Address
 
 class BytecodeOptimizer:
     def __init__(self, vm: MacalVm, scope: CompilerScope):
         self.vm = vm
```

### Comparing `macal-5.0rc8/src/macal/bytecode_register.py` & `macal-5.0rc9/src/macal/bytecode_register.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/bytecode_variable.py` & `macal-5.0rc9/src/macal/bytecode_variable.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/cmacal_vm.pyx` & `macal-5.0rc9/src/macal/cmacal_vm.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                         res = reg.value - value
                         self.flags._zero = res == 0
                         self.flags._carry = res < 0
                     else:
                         self.flags._zero = reg.value == value
                         self.flags._carry = reg.value < value
             elif opCode[0] ==  3: # JMPNZ addr
-                if self.flags._zero == False:
+                if self.flags._zero is False:
                     self.rip.value = opCode[1]
             elif opCode[0] == 21: # SUBRR reg, reg
                 reg1: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
                 reg2: BytecodeRegister = self.opcode_to_register_map[opCode[2]]
                 if reg1.value_type == reg2.value_type:
                     if reg1.value_type == AstNodetype.INTEGER:
                         self.flags._zero = reg1.value - reg2.value == 0
@@ -567,14 +567,18 @@
             elif opCode[0] == 62: # SETRTI reg, type
                 reg: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
                 reg.value_type = opCode[2]
             elif opCode[0] == 72: # MOVRTOA
                 reg: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
                 reg.value = [reg.value]
                 reg.value_type = AstNodetype.ARRAY
+            elif opCode[0] == 83: # MOVATOR
+                reg: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
+                reg.value = reg.value[0]
+                reg.value_type = typeFromValue(reg.value)
             elif opCode[0] == 71: # HASFLDRR record has field function
                 reg1: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
                 reg2: BytecodeRegister = self.opcode_to_register_map[opCode[2]]
                 self.flags._zero = reg2.value in reg1.value.keys()
             elif opCode[0] == 73: # TYPE reg gets the type of the value of a register, basically puts reg.value_type in reg.value.
                 reg: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
                 reg.value = reg.value_type
@@ -600,30 +604,37 @@
                 print(f"{reg.name} {value} ({reg.value_type.name})")
             elif opCode[0] == 77: # DATASEG metadata
                 pass
             elif opCode[0] == 78: # MERGE reg1, reg2, reg3
                 reg1: BytecodeRegister = self.opcode_to_register_map[opCode[1]]
                 reg2: BytecodeRegister = self.opcode_to_register_map[opCode[2]]
                 reg3: BytecodeRegister = self.opcode_to_register_map[opCode[3]]
-                # just a single record in each but with the same set of fields, then merge them.
+                if reg2.value_type == AstNodetype.RECORD:
+                    reg2.value = [reg2.value]
+                    reg2.value_type = AstNodetype.ARRAY
+                if reg3.value_type == AstNodetype.RECORD:
+                    reg3.value = [reg3.value]
+                    reg3.value_type = AstNodetype.ARRAY
+                # just a single record in eachwith the same set of fields, then merge them.
                 if len(reg2.value) == 1 and len(reg3.value) == 1 and set(reg2.value[0].keys()) == set(reg3.value[0].keys()):
                     reg1.value = [reg2.value[0], reg3.value[0]]
                 # just a single record in each, but with different fields, then merge them but also the fields,
                 # overwriting any existing in the source (reg2).
                 elif len(reg2.value) == 1 and len(reg3.value) == 1:
                     keys = set().union(reg2.value[0].keys(), reg3.value[0].keys())
                     reg1.value = [{k: reg2.value[0].get(k, reg3.value[0].get(k, None)) for k in keys}]
-                # multiple records in each, but with the same set of fields, then just append them both.
+                # multiple records in each, with the same set of fields, then just append them both.
                 elif set(reg2.value[0].keys()) == set(reg3.value[0].keys()):
                     reg1.value = reg2.value.copy()
                     reg1.value.extend(reg3.value)
                 # multiple records in each, but with the or different fields, then merge the records and fields.
                 else:
                     keys = set().union(*(d.keys() for d in reg2.value + reg3.value))
                     reg1.value = [{k: d.get(k, None) for k in keys} for d in reg2.value + reg3.value]
+                reg1.value_type = AstNodetype.ARRAY
             elif opCode[0] == 79: # JMP R
                 self.rip.value = self.opcode_to_register_map[opCode[1]].value
             elif opCode[0] == 80: # RESERVE size
                 self.rsp.value += opCode[1]
                 while len(self.stack) < self.rsp.value:
                     self.stack.append((AstNodetype.NIL, AstNodetype.NIL))
                 for var in self.scope.variables:
```

### Comparing `macal-5.0rc8/src/macal/compiler_scope.py` & `macal-5.0rc9/src/macal/compiler_scope.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/conversion.py` & `macal-5.0rc9/src/macal/conversion.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ct_function.py` & `macal-5.0rc9/src/macal/ct_function.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/ct_variable.py` & `macal-5.0rc9/src/macal/ct_variable.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lex_token.py` & `macal-5.0rc9/src/macal/lex_token.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_csv.py` & `macal-5.0rc9/src/macal/lib/ext/ext_csv.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_io.py` & `macal-5.0rc9/src/macal/lib/ext/ext_io.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_math.py` & `macal-5.0rc9/src/macal/lib/ext/ext_math.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_strings.py` & `macal-5.0rc9/src/macal/lib/ext/ext_strings.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_syslog.py` & `macal-5.0rc9/src/macal/lib/ext/ext_syslog.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_system.py` & `macal-5.0rc9/src/macal/lib/ext/ext_system.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/ext_time.py` & `macal-5.0rc9/src/macal/lib/ext/ext_time.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/ext/meraki_api_library_v1.py` & `macal-5.0rc9/src/macal/lib/ext/meraki_api_library_v1.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/io.mcl` & `macal-5.0rc9/src/macal/lib/io.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/math.mcl` & `macal-5.0rc9/src/macal/lib/math.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/meraki_v1.mcl` & `macal-5.0rc9/src/macal/lib/meraki_v1.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/strings.mcl` & `macal-5.0rc9/src/macal/lib/strings.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/system.mcl` & `macal-5.0rc9/src/macal/lib/system.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/lib/time.mcl` & `macal-5.0rc9/src/macal/lib/time.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/macal_compiler.py` & `macal-5.0rc9/src/macal/macal_compiler.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/macal_decompiler.py` & `macal-5.0rc9/src/macal/macal_decompiler.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/macal_instruction_emitter.py` & `macal-5.0rc9/src/macal/macal_instruction_emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,7 +378,10 @@
         self.memory[self.rip.value] = (81, metadata)
         self.rip.value += 1
     
     def LOADIR(self, reg1: BytecodeRegister, reg2: BytecodeRegister):
         self.memory[self.rip.value] = (82, reg1.opcode, reg2.opcode)
         self.rip.value += 1
 
+    def MOVATOR(self, reg: BytecodeRegister):
+        self.memory[self.rip.value] = (83, reg.opcode)
+        self.rip.value += 1
```

### Comparing `macal-5.0rc8/src/macal/macal_instructions.py` & `macal-5.0rc9/src/macal/macal_instructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         self.add("PRNTR",    ["reg"],           "print reg, debug printing register name, value, type")
         self.add("DATASEG",  ["metadata"],      "set metadata for debugging")
         self.add("MERGE",    ["reg1", "reg2", "reg3"],  "merge reg2 and reg3 into reg1 reg1 = [reg2] + [reg3]")
         self.add("JMPR",     ["reg"],           "jump to reg")
         self.add("RESERVE",  ["imm"],           "reserve imm entries on the stack")
         self.add("RESERVEDS", ["metadata"],     "datasegment with metadata for variables that are reserved on the stack")
         self.add("LOADIR",   ["reg1", "reg2"],  "reg1 = stack[reg2]")
+        self.add("MOVATOR",  ["reg"],           "reg = reg[0], the first record in the array in reg is moved into reg.")
 
     def add(self, name: str, operands: Optional[List[str]] = None, description: Optional[str] = None):
         opcode = len(self.instructions)
         instruction = MacalInstruction(name, opcode, operands, description)
         self.instructions[opcode] = instruction
         self.named_instructions[name] = instruction
```

### Comparing `macal-5.0rc8/src/macal/macal_interactive.py` & `macal-5.0rc9/src/macal/macal_interactive.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/macal_lexer.py` & `macal-5.0rc9/src/macal/macal_lexer.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/macal_parser.py` & `macal-5.0rc9/src/macal/macal_parser.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/macal_select_compiler.py` & `macal-5.0rc9/src/macal/macal_select_compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,14 +239,15 @@
         # We can now release the registers that we used.
         self.cs.ReleaseRegister(source_register)
         self.cs.ReleaseRegister(index_register)
         self.cs.ReleaseRegister(result_register)
         self.cs.ReleaseRegister(record_register)
 
 
+
     def compile_select_fields(self, select: AstNodeSelectStatement, scope: CompilerScope) -> None:
         """
             This function compiles the code that will apply the field selection to the result of the from clause.
             (or the where clause if that exists)
         """
         self.parent.emit_new_label("fields", scope)
         # Compile the select fields
@@ -322,14 +323,16 @@
         self.cs.ReleaseRegister(array_register)
         self.cs.ReleaseRegister(result_array_register)
         self.cs.ReleaseRegister(result_record_register)
         self.cs.ReleaseRegister(current_record_register)
         self.cs.ReleaseRegister(index_register)
         self.cs.ReleaseRegister(field_value_register)
 
+
+
     def compile_field(self, field: AstNodeSelectField, record_register: BytecodeRegister,
                       result_record_register: BytecodeRegister, field_value_register: BytecodeRegister, scope: CompilerScope) -> None:
         new_record_field = self.cs.GetFreeRegister()
         self.emitter.MOVRI(new_record_field, AstNodetype.NIL, 'nil')
         has_fld_lbl = scope.root.get_new_label("has_fld")
         self.emitter.MOVRR(self.cs.rax, record_register) # rax is the current record
         self.emitter.MOVRI(self.cs.rbx, AstNodetype.STRING, field.fieldname) # rbx is the original name of the field
@@ -345,19 +348,50 @@
         self.emitter.MOVRI(self.cs.rbx, AstNodetype.STRING, field.altfieldname) # rbx is now the new field name.
         self.emitter.MOVRR(field_value_register, self.cs.rax) # field_value_register is now a "copy" of the field value in rax.
         self.emitter.MOVRR(self.cs.rax, result_record_register) # rax is now the result record.
         self.emitter.INDEXR(field_value_register) # # rax[rbx] = field_value_register so we add the current new field to the resulting record.
         self.emitter.MOVRR(result_record_register, self.cs.rax) # result_record_register is now a "copy" of the result record in rax.
         self.cs.ReleaseRegister(new_record_field)
 
+
+
     def compile_into(self, select: AstNodeSelectStatement, scope: CompilerScope) -> None:
         # Get the into variable if it exists, or create a new one, put the result on the stack.
-        into: CTVariable = scope.find_variable(select.Into.name)
-        
+        into: CTVariable = scope.find_variable(select.Into.name)       
         self.emitter.POP(self.cs.rax) # pop rax # rax has the value.
+        reg = self.cs.GetFreeRegister()
+
+        # process distinct to always return a record.
+        lbl = scope.root.get_new_label("into_skip_1")
+        self.emitter.LENR(reg, self.cs.rax)
+        self.emitter.CMPRI(reg, AstNodetype.INTEGER, 0)
+        self.parent.emit_jump(Opcode.JMPZ, lbl, scope) # if nothing here skip to lbl
+        self.emitter.CMPRTI(self.cs.rax, AstNodetype.RECORD)
+        self.parent.emit_jump(Opcode.JMPZ, lbl, scope) # if record here skip to lbl
+        self.emitter.MOVRI(reg, AstNodetype.BOOLEAN, select.distinct)
+        self.emitter.CMPRI(reg, AstNodetype.BOOLEAN, False)
+        self.parent.emit_jump(Opcode.JMPZ, lbl, scope) # not distinct, so we skip this
+        self.emitter.MOVATOR(self.cs.rax) # rax = rax[0] # we only need the first record.
+        scope.set_label_address(lbl, self.cs.rip.value)
+
+        # If the output is a single record, and it has only one field, and this is not * then the result is a single value.
+        lbl2 = scope.root.get_new_label("into_skip_2")
+        self.emitter.CMPRTI(self.cs.rax, AstNodetype.RECORD)
+        self.parent.emit_jump(Opcode.JMPNZ, lbl2, scope) # if not a record here skip to lbl2
+        self.emitter.MOVRI(reg, AstNodetype.INTEGER, len(select.Fields))
+        self.emitter.CMPRI(reg, AstNodetype.INTEGER, 1)
+        self.parent.emit_jump(Opcode.JMPNZ, lbl2, scope) # if not a single field, skip to lbl2
+        self.emitter.MOVRI(reg, AstNodetype.STRING, select.Fields[0].fieldname)
+        self.emitter.CMPRI(reg, AstNodetype.STRING, '*')
+        self.parent.emit_jump(Opcode.JMPZ, lbl2, scope) # if it's "all" fields, then skip to lbl2
+        self.emitter.MOVRR(self.cs.rbx, reg)
+        self.emitter.INDEX() # RAX = RAX[RBX]
+        scope.set_label_address(lbl2, self.cs.rip.value)
+        self.cs.ReleaseRegister(reg)
+
         if into is None:
             self.parent.emit_new_label("into need a new var", scope)
             # it doesn't exist so we make one.
             reg = self.cs.GetFreeRegister()
             self.emitter.XOR(reg, reg)
             into = scope.define_variable(select.Into.name, self.cs.rsp.value)
             self.emitter.MOVRR(self.cs.rbx,self.cs.rsp) # rbx is now the absolute index of the new variable in the stack.
```

### Comparing `macal-5.0rc8/src/macal/mc.py` & `macal-5.0rc9/src/macal/mc.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/md.py` & `macal-5.0rc9/src/macal/md.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/mi.py` & `macal-5.0rc9/src/macal/mi.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/mr.py` & `macal-5.0rc9/src/macal/mr.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/python_module_info.py` & `macal-5.0rc9/src/macal/python_module_info.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/runtime_scope.py` & `macal-5.0rc9/src/macal/runtime_scope.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal/statement_type_table.py` & `macal-5.0rc9/src/macal/statement_type_table.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/src/macal.egg-info/PKG-INFO` & `macal-5.0rc9/src/macal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macal
-Version: 5.0rc8
+Version: 5.0rc9
 Summary: Macal is a DSL for collecting and transforming data from various sources.
 Author-email: Marco Caspers <SamaDevTeam@westcon.com>
 Project-URL: Homepage, https://github.com/Sama-Developer/macal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `macal-5.0rc8/src/macal.egg-info/SOURCES.txt` & `macal-5.0rc9/src/macal.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 src/macal/macal_decompiler.py
 src/macal/macal_instruction_emitter.py
 src/macal/macal_instructions.py
 src/macal/macal_interactive.py
 src/macal/macal_lexer.py
 src/macal/macal_parser.py
 src/macal/macal_select_compiler.py
-src/macal/macal_vm.py
 src/macal/mc.py
 src/macal/md.py
 src/macal/mi.py
 src/macal/mr.py
 src/macal/python_module_info.py
 src/macal/runtime_scope.py
 src/macal/statement_type_table.py
@@ -159,18 +158,22 @@
 tests/select_2.mcl
 tests/select_3.mbc
 tests/select_3.mcl
 tests/select_4.mbc
 tests/select_4.mcl
 tests/select_5.mbc
 tests/select_5.mcl
+tests/select_6.mbc
+tests/select_6.mcl
 tests/select_7.mbc
 tests/select_7.mcl
 tests/select_8.mbc
 tests/select_8.mcl
+tests/select_9.mbc
+tests/select_9.mcl
 tests/switch_1.mcl
 tests/test.mcl
 tests/test2.mcl
 tests/test3.mcl
 tests/usereserved.mbc
 tests/usereserved.mcl
 tests/variable.mcl
```

### Comparing `macal-5.0rc8/tests/aor.mcl` & `macal-5.0rc9/tests/aor.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/args.mbc` & `macal-5.0rc9/tests/args.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/function5.mbc` & `macal-5.0rc9/tests/function5.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/function5.mcl` & `macal-5.0rc9/tests/function5.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/iftest.mcl` & `macal-5.0rc9/tests/iftest.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/indexed_6.mbc` & `macal-5.0rc9/tests/indexed_6.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/libvar.mbc` & `macal-5.0rc9/tests/libvar.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/mdi.mbc` & `macal-5.0rc9/tests/mdi.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/mdi.mcl` & `macal-5.0rc9/tests/mdi.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/meraki_firewall_dc.mcl` & `macal-5.0rc9/tests/meraki_firewall_dc.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/meraki_firewall_sh.mcl` & `macal-5.0rc9/tests/meraki_firewall_sh.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/meraki_test.mbc` & `macal-5.0rc9/tests/meraki_test.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/meraki_test.mcl` & `macal-5.0rc9/tests/meraki_test.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/mt.py` & `macal-5.0rc9/tests/mt.py`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_1.mbc` & `macal-5.0rc9/tests/select_1.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_1.mcl` & `macal-5.0rc9/tests/select_1.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_2.mbc` & `macal-5.0rc9/tests/select_2.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_3.mbc` & `macal-5.0rc9/tests/select_3.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_3.mcl` & `macal-5.0rc9/tests/select_3.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_4.mbc` & `macal-5.0rc9/tests/select_4.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_5.mbc` & `macal-5.0rc9/tests/select_5.mbc`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 424d 4301 0000 0067 0f00 0080 0495 5c0f  BMC....g......\.
+00000000: 424d 4301 0000 00dd 1000 0080 0495 d210  BMC.............
 00000010: 0000 0000 0000 5d94 284b 094b 0686 944b  ......].(K.K...K
 00000020: 0b4b 064b 0787 944b 234b 004b 0087 944b  .K.K...K#K.K...K
 00000030: 094b 0086 9428 4b0c 4b00 8c12 6d61 6361  .K...(K.K...maca
 00000040: 6c2e 6173 745f 6e6f 6465 7479 7065 948c  l.ast_nodetype..
 00000050: 0b41 7374 4e6f 6465 7479 7065 9493 944b  .AstNodetype...K
 00000060: 8485 9452 945d 9474 944b 094b 0086 944b  ...R.].t.K.K...K
 00000070: 0a4b 0086 944b 394b 034b 0087 9428 4b0c  .K...K9K.K...(K.
@@ -139,110 +139,133 @@
 000008a0: 944b 0b4b 004b 0c87 944b 0b4b 014b 0b87  .K.K.K...K.K.K..
 000008b0: 9468 354b 3d4b 0068 1087 944b 428c 3d45  .h5K=K.h...KB.=E
 000008c0: 7870 6563 7465 6420 6120 7265 636f 7264  xpected a record
 000008d0: 2069 6e20 7468 6520 4652 4f4d 2063 6c61   in the FROM cla
 000008e0: 7573 6520 6f66 2074 6865 2053 454c 4543  use of the SELEC
 000008f0: 5420 7374 6174 656d 656e 742e 9486 944b  T statement....K
 00000900: 0b4b 0e4b 0087 9428 4b0c 4b0f 6810 7d94  .K.K...(K.K.h.}.
-00000910: 7494 284b 0c4b 0968 074b 8985 9452 946a  t.(K.K.h.K...R.j
-00000920: 3401 0000 7494 4b0b 4b00 4b0e 8794 284b  4...t.K.K.K...(K
-00000930: 0c4b 0168 388c 0661 7574 686f 7294 7494  .K.h8..author.t.
-00000940: 4b47 4b00 4b01 8794 4b02 4d1b 0186 944b  KGK.K...K.M....K
-00000950: 464b 0986 944b 0b4b 0e4b 0087 9468 3528  FK...K.K.K...h5(
-00000960: 4b0c 4b01 6838 8c06 4175 7468 6f72 9474  K.K.h8..Author.t
-00000970: 944b 0b4b 0a4b 0087 944b 0b4b 004b 0f87  .K.K.K...K.K.K..
-00000980: 944b 464b 0a86 944b 0b4b 0f4b 0087 9428  .KFK...K.K.K...(
-00000990: 4b0c 4b09 6a34 0100 006a 3401 0000 7494  K.K.j4...j4...t.
-000009a0: 4b0b 4b00 4b0e 8794 284b 0c4b 0168 388c  K.K.K...(K.K.h8.
-000009b0: 0574 6974 6c65 9474 944b 474b 004b 0187  .title.t.KGK.K..
-000009c0: 944b 024d 2801 8694 4b46 4b09 8694 4b0b  .K.M(...KFK...K.
-000009d0: 4b0e 4b00 8794 6835 284b 0c4b 0168 386a  K.K...h5(K.K.h8j
-000009e0: 4501 0000 7494 4b0b 4b0a 4b00 8794 4b0b  E...t.K.K.K...K.
-000009f0: 4b00 4b0f 8794 4b46 4b0a 8694 4b0b 4b0f  K.K...KFK...K.K.
-00000a00: 4b00 8794 284b 0c4b 096a 3401 0000 6a34  K...(K.K.j4...j4
-00000a10: 0100 0074 944b 0b4b 004b 0e87 9428 4b0c  ...t.K.K.K...(K.
-00000a20: 4b01 6838 8c04 7465 7374 9474 944b 474b  K.h8..test.t.KGK
-00000a30: 004b 0187 944b 024d 3501 8694 4b46 4b09  .K...K.M5...KFK.
-00000a40: 8694 4b0b 4b0e 4b00 8794 6835 284b 0c4b  ..K.K.K...h5(K.K
-00000a50: 0168 388c 0554 6974 6c65 9474 944b 0b4b  .h8..Title.t.K.K
-00000a60: 0a4b 0087 944b 0b4b 004b 0f87 944b 464b  .K...K.K.K...KFK
-00000a70: 0a86 944b 0b4b 0f4b 0087 944b 0b4b 004b  ...K.K.K...K.K.K
-00000a80: 0d87 944b 3f4b 004b 0f87 944b 0b4b 0d4b  ...K?K.K...K.K.K
-00000a90: 0087 944b 334b 0b86 944b 094b 0d86 944b  ...K3K...K.K...K
-00000aa0: 0a4b 0086 944b 234b 0a4b 0a87 944b 0b4b  .K...K#K.K...K.K
-00000ab0: 014b 0787 944b 094b 0a86 944b 3c4b 014b  .K...K.K...K<K.K
-00000ac0: 0087 944b 384b 004b 0387 944b 094b 0086  ...K8K.K...K.K..
-00000ad0: 944b 0a4b 0086 944b 3d4b 0068 1087 944b  .K.K...K=K.h...K
-00000ae0: 034d 4b01 8694 4b48 4b00 8694 4b09 4b00  .MK...KHK...K.K.
-00000af0: 8694 4b0a 4b00 8694 4b36 4b02 4b00 8794  ..K.K...K6K.K...
-00000b00: 284b 104b 0268 304b 0074 944b 024d 6b01  (K.K.h0K.t.K.Mk.
-00000b10: 8694 4b23 4b0a 4b0a 8794 4b0b 4b0b 4b00  ..K#K.K...K.K.K.
-00000b20: 8794 284b 0c4b 0e68 095d 9474 944b 0b4b  ..(K.K.h.].t.K.K
-00000b30: 004b 0b87 944b 0b4b 014b 0a87 9468 354b  .K...K.K.K...h5K
-00000b40: 0b4b 0f4b 0087 944b 0b4b 004b 0f87 9428  .K.K...K.K.K...(
-00000b50: 4b0c 4b01 6838 8c06 6175 7468 6f72 9474  K.K.h8..author.t
-00000b60: 9468 354b 094b 0086 9428 4b0c 4b00 6838  .h5K.K...(K.K.h8
-00000b70: 8c0d 446f 7567 6c61 7320 4164 616d 7394  ..Douglas Adams.
-00000b80: 7494 4b09 4b00 8694 4b0a 4b01 8694 4b0a  t.K.K...K.K...K.
-00000b90: 4b00 8694 4b11 4b00 4b01 8794 4b26 4b00  K...K.K.K...K&K.
-00000ba0: 8694 4b09 4b00 8694 4b0a 4b00 8694 284b  ..K.K...K.K...(K
-00000bb0: 104b 006a 1a01 0000 8874 944b 034d 6901  .K.j.....t.K.Mi.
-00000bc0: 8694 4b3f 4b0e 4b0f 8794 284b 0c4b 006a  ..K?K.K...(K.K.j
-00000bd0: 1a01 0000 8874 9428 4b10 4b00 6a1a 0100  .....t.(K.K.j...
-00000be0: 0088 7494 4b02 4d6b 0186 944b 334b 0a86  ..t.K.Mk...K3K..
-00000bf0: 944b 084d 5301 8694 4b09 4b0e 8694 4b0a  .K.MS...K.K...K.
-00000c00: 4b00 8694 4b0b 4b0f 4b00 8794 284b 0c4b  K...K.K.K...(K.K
-00000c10: 0e68 095d 9474 944b 234b 014b 0187 944b  .h.].t.K#K.K...K
-00000c20: 0b4b 0d4b 0187 944b 364b 024b 0087 944b  .K.K...K6K.K...K
-00000c30: 0b4b 004b 0f87 944b 0b4b 014b 0d87 9468  .K.K...K.K.K...h
-00000c40: 354b 3d4b 0068 1087 944b 426a 2e01 0000  5K=K.h...KBj....
-00000c50: 8694 4b0b 4b0b 4b00 8794 284b 0c4b 0a68  ..K.K.K...(K.K.h
-00000c60: 107d 9474 9428 4b0c 4b09 6a34 0100 006a  .}.t.(K.K.j4...j
-00000c70: 3401 0000 7494 4b0b 4b00 4b0b 8794 284b  4...t.K.K.K...(K
-00000c80: 0c4b 0168 388c 0661 7574 686f 7294 7494  .K.h8..author.t.
-00000c90: 4b47 4b00 4b01 8794 4b02 4d80 0186 944b  KGK.K...K.M....K
-00000ca0: 464b 0986 944b 0b4b 0b4b 0087 9468 3528  FK...K.K.K...h5(
-00000cb0: 4b0c 4b01 6838 8c06 4175 7468 6f72 9474  K.K.h8..Author.t
-00000cc0: 944b 0b4b 0c4b 0087 944b 0b4b 004b 0a87  .K.K.K...K.K.K..
-00000cd0: 944b 464b 0c86 944b 0b4b 0a4b 0087 9428  .KFK...K.K.K...(
-00000ce0: 4b0c 4b09 6a34 0100 006a 3401 0000 7494  K.K.j4...j4...t.
-00000cf0: 4b0b 4b00 4b0b 8794 284b 0c4b 0168 388c  K.K.K...(K.K.h8.
-00000d00: 0574 6974 6c65 9474 944b 474b 004b 0187  .title.t.KGK.K..
-00000d10: 944b 024d 8d01 8694 4b46 4b09 8694 4b0b  .K.M....KFK...K.
-00000d20: 4b0b 4b00 8794 6835 284b 0c4b 0168 386a  K.K...h5(K.K.h8j
-00000d30: ae01 0000 7494 4b0b 4b0c 4b00 8794 4b0b  ....t.K.K.K...K.
-00000d40: 4b00 4b0a 8794 4b46 4b0c 8694 4b0b 4b0a  K.K...KFK...K.K.
-00000d50: 4b00 8794 284b 0c4b 096a 3401 0000 6a34  K...(K.K.j4...j4
-00000d60: 0100 0074 944b 0b4b 004b 0b87 9428 4b0c  ...t.K.K.K...(K.
-00000d70: 4b01 6838 8c04 7465 7374 9474 944b 474b  K.h8..test.t.KGK
-00000d80: 004b 0187 944b 024d 9a01 8694 4b46 4b09  .K...K.M....KFK.
-00000d90: 8694 4b0b 4b0b 4b00 8794 6835 284b 0c4b  ..K.K.K...h5(K.K
-00000da0: 0168 388c 0554 6974 6c65 9474 944b 0b4b  .h8..Title.t.K.K
-00000db0: 0c4b 0087 944b 0b4b 004b 0a87 944b 464b  .K...K.K.K...KFK
-00000dc0: 0c86 944b 0b4b 0a4b 0087 944b 0b4b 004b  ...K.K.K...K.K.K
-00000dd0: 0e87 944b 3f4b 004b 0a87 944b 0b4b 0e4b  ...K?K.K...K.K.K
-00000de0: 0087 944b 334b 0d86 944b 094b 0e86 944b  ...K3K...K.K...K
-00000df0: 384b 0c4b 0487 944b 0a4b 0d86 9428 4b0c  8K.K...K.K...(K.
-00000e00: 4b0b 6809 5d94 7494 284b 4e4b 0b4b 0c4b  K.h.].t.(KNK.K.K
-00000e10: 0d74 944b 094b 0b86 944b 0a4b 0086 9428  .t.K.K...K.K...(
-00000e20: 4b0c 4b01 6830 4b04 7494 4b3c 4b01 4b00  K.K.h0K.t.K<K.K.
-00000e30: 8794 4b09 4b06 8694 4b0b 4b06 4b07 8794  ..K.K...K.K.K...
-00000e40: 4b38 4b00 4b04 8794 4b09 4b00 8694 4b35  K8K.K...K.K...K5
-00000e50: 4b00 8694 4b09 4b00 8694 4b23 4b00 4b00  K...K.K...K#K.K.
-00000e60: 8794 4b09 4b00 8694 4b09 4b00 8694 4b38  ..K.K...K.K...K8
-00000e70: 4b00 4b07 8794 4b38 4b01 4b08 8794 4b11  K.K...K8K.K...K.
-00000e80: 4b00 4b01 8794 4b02 4dc7 0186 944b 384b  K.K...K.M....K8K
-00000e90: 004b 0687 944b 4585 944b 394b 094b 0087  .K...KE..K9K.K..
-00000ea0: 944b 384b 004b 0987 944b 094b 0086 944b  .K8K.K...K.K...K
-00000eb0: 0a4b 0086 944b 4385 9428 4b0c 4b00 6838  .K...KC..(K.K.h8
-00000ec0: 8c01 0a94 7494 6ae8 0100 004b 384b 004b  ....t.j....K8K.K
-00000ed0: 0887 944b 334b 0086 944b 394b 084b 0087  ...K3K...K9K.K..
-00000ee0: 944b 014d b601 8694 4b0b 4b07 4b06 8794  .K.M....K.K.K...
-00000ef0: 4b0a 4b06 8694 4b0b 4b07 4b06 8794 4b0a  K.K...K.K.K...K.
-00000f00: 4b06 8694 4b2f 8594 4b51 7d94 288c 0956  K...K/..KQ}.(..V
-00000f10: 4152 4941 424c 4553 945d 948c 0946 554e  ARIABLES.]...FUN
-00000f20: 4354 494f 4e53 945d 948c 094c 4942 5241  CTIONS.]...LIBRA
-00000f30: 5249 4553 945d 948c 064c 4142 454c 5394  RIES.]...LABELS.
-00000f40: 5d94 8c05 4a55 4d50 5394 5d94 8c08 5245  ]...JUMPS.]...RE
-00000f50: 5345 5256 4544 945d 9428 8c03 7661 7294  SERVED.].(..var.
-00000f60: 4b03 8694 8c01 7994 4b04 8694 6575 8694  K.....y.K...eu..
-00000f70: 652e                                     e.
+00000910: 7494 284b 0c4b 0968 074b 8985 9452 948c  t.(K.K.h.K...R..
+00000920: 036e 696c 9474 944b 0b4b 004b 0e87 9428  .nil.t.K.K.K...(
+00000930: 4b0c 4b01 6838 8c06 6175 7468 6f72 9474  K.K.h8..author.t
+00000940: 944b 474b 004b 0187 944b 024d 1b01 8694  .KGK.K...K.M....
+00000950: 4b46 4b09 8694 4b0b 4b0e 4b00 8794 6835  KFK...K.K.K...h5
+00000960: 284b 0c4b 0168 388c 0641 7574 686f 7294  (K.K.h8..Author.
+00000970: 7494 4b0b 4b0a 4b00 8794 4b0b 4b00 4b0f  t.K.K.K...K.K.K.
+00000980: 8794 4b46 4b0a 8694 4b0b 4b0f 4b00 8794  ..KFK...K.K.K...
+00000990: 284b 0c4b 096a 3401 0000 6a35 0100 0074  (K.K.j4...j5...t
+000009a0: 944b 0b4b 004b 0e87 9428 4b0c 4b01 6838  .K.K.K...(K.K.h8
+000009b0: 8c05 7469 746c 6594 7494 4b47 4b00 4b01  ..title.t.KGK.K.
+000009c0: 8794 4b02 4d28 0186 944b 464b 0986 944b  ..K.M(...KFK...K
+000009d0: 0b4b 0e4b 0087 9468 3528 4b0c 4b01 6838  .K.K...h5(K.K.h8
+000009e0: 6a46 0100 0074 944b 0b4b 0a4b 0087 944b  jF...t.K.K.K...K
+000009f0: 0b4b 004b 0f87 944b 464b 0a86 944b 0b4b  .K.K...KFK...K.K
+00000a00: 0f4b 0087 9428 4b0c 4b09 6a34 0100 006a  .K...(K.K.j4...j
+00000a10: 3501 0000 7494 4b0b 4b00 4b0e 8794 284b  5...t.K.K.K...(K
+00000a20: 0c4b 0168 388c 0474 6573 7494 7494 4b47  .K.h8..test.t.KG
+00000a30: 4b00 4b01 8794 4b02 4d35 0186 944b 464b  K.K...K.M5...KFK
+00000a40: 0986 944b 0b4b 0e4b 0087 9468 3528 4b0c  ...K.K.K...h5(K.
+00000a50: 4b01 6838 8c05 5469 746c 6594 7494 4b0b  K.h8..Title.t.K.
+00000a60: 4b0a 4b00 8794 4b0b 4b00 4b0f 8794 4b46  K.K...K.K.K...KF
+00000a70: 4b0a 8694 4b0b 4b0f 4b00 8794 4b0b 4b00  K...K.K.K...K.K.
+00000a80: 4b0d 8794 4b3f 4b00 4b0f 8794 4b0b 4b0d  K...K?K.K...K.K.
+00000a90: 4b00 8794 4b33 4b0b 8694 4b09 4b0d 8694  K...K3K...K.K...
+00000aa0: 4b0a 4b00 8694 4b4c 4b00 8694 4b36 4b0a  K.K...KLK...K6K.
+00000ab0: 4b00 8794 284b 104b 0a68 304b 0074 944b  K...(K.K.h0K.t.K
+00000ac0: 024d 4b01 8694 4b3d 4b00 6810 8794 4b02  .MK...K=K.h...K.
+00000ad0: 4d4b 0186 9428 4b0c 4b0a 6a1a 0100 0088  MK...(K.K.j.....
+00000ae0: 7494 284b 104b 0a6a 1a01 0000 8974 944b  t.(K.K.j.....t.K
+00000af0: 024d 4b01 8694 4b53 4b00 8694 4b4c 4b00  .MK...KSK...KLK.
+00000b00: 8694 4b3d 4b00 6810 8794 4b03 4d56 0186  ..K=K.h...K.MV..
+00000b10: 9428 4b0c 4b0a 6830 4b03 7494 284b 104b  .(K.K.h0K.t.(K.K
+00000b20: 0a68 304b 0174 944b 034d 5601 8694 284b  .h0K.t.K.MV...(K
+00000b30: 0c4b 0a68 386a 3801 0000 7494 284b 104b  .K.h8j8...t.(K.K
+00000b40: 0a68 388c 012a 9474 944b 024d 5601 8694  .h8..*.t.K.MV...
+00000b50: 4b0b 4b01 4b0a 8794 6835 4b4c 4b00 8694  K.K.K...h5KLK...
+00000b60: 4b23 4b0a 4b0a 8794 4b0b 4b01 4b07 8794  K#K.K...K.K.K...
+00000b70: 4b09 4b0a 8694 4b3c 4b01 4b00 8794 4b38  K.K...K<K.K...K8
+00000b80: 4b00 4b03 8794 4b09 4b00 8694 4b0a 4b00  K.K...K.K...K.K.
+00000b90: 8694 4b3d 4b00 6810 8794 4b03 4d61 0186  ..K=K.h...K.Ma..
+00000ba0: 944b 484b 0086 944b 094b 0086 944b 0a4b  .KHK...K.K...K.K
+00000bb0: 0086 944b 364b 024b 0087 9428 4b10 4b02  ...K6K.K...(K.K.
+00000bc0: 6830 4b00 7494 4b02 4d81 0186 944b 234b  h0K.t.K.M....K#K
+00000bd0: 0a4b 0a87 944b 0b4b 0b4b 0087 9428 4b0c  .K...K.K.K...(K.
+00000be0: 4b0e 6809 5d94 7494 4b0b 4b00 4b0b 8794  K.h.].t.K.K.K...
+00000bf0: 4b0b 4b01 4b0a 8794 6835 4b0b 4b0f 4b00  K.K.K...h5K.K.K.
+00000c00: 8794 4b0b 4b00 4b0f 8794 284b 0c4b 0168  ..K.K.K...(K.K.h
+00000c10: 388c 0661 7574 686f 7294 7494 6835 4b09  8..author.t.h5K.
+00000c20: 4b00 8694 284b 0c4b 0068 388c 0d44 6f75  K...(K.K.h8..Dou
+00000c30: 676c 6173 2041 6461 6d73 9474 944b 094b  glas Adams.t.K.K
+00000c40: 0086 944b 0a4b 0186 944b 0a4b 0086 944b  ...K.K...K.K...K
+00000c50: 114b 004b 0187 944b 264b 0086 944b 094b  .K.K...K&K...K.K
+00000c60: 0086 944b 0a4b 0086 9428 4b10 4b00 6a1a  ...K.K...(K.K.j.
+00000c70: 0100 0088 7494 4b03 4d7f 0186 944b 3f4b  ....t.K.M....K?K
+00000c80: 0e4b 0f87 9428 4b0c 4b00 6a1a 0100 0088  .K...(K.K.j.....
+00000c90: 7494 284b 104b 006a 1a01 0000 8874 944b  t.(K.K.j.....t.K
+00000ca0: 024d 8101 8694 4b33 4b0a 8694 4b08 4d69  .M....K3K...K.Mi
+00000cb0: 0186 944b 094b 0e86 944b 0a4b 0086 944b  ...K.K...K.K...K
+00000cc0: 0b4b 0f4b 0087 9428 4b0c 4b0e 6809 5d94  .K.K...(K.K.h.].
+00000cd0: 7494 4b23 4b01 4b01 8794 4b0b 4b0d 4b01  t.K#K.K...K.K.K.
+00000ce0: 8794 4b36 4b02 4b00 8794 4b0b 4b00 4b0f  ..K6K.K...K.K.K.
+00000cf0: 8794 4b0b 4b01 4b0d 8794 6835 4b3d 4b00  ..K.K.K...h5K=K.
+00000d00: 6810 8794 4b42 6a2e 0100 0086 944b 0b4b  h...KBj......K.K
+00000d10: 0b4b 0087 9428 4b0c 4b0a 6810 7d94 7494  .K...(K.K.h.}.t.
+00000d20: 284b 0c4b 096a 3401 0000 6a35 0100 0074  (K.K.j4...j5...t
+00000d30: 944b 0b4b 004b 0b87 9428 4b0c 4b01 6838  .K.K.K...(K.K.h8
+00000d40: 8c06 6175 7468 6f72 9474 944b 474b 004b  ..author.t.KGK.K
+00000d50: 0187 944b 024d 9601 8694 4b46 4b09 8694  ...K.M....KFK...
+00000d60: 4b0b 4b0b 4b00 8794 6835 284b 0c4b 0168  K.K.K...h5(K.K.h
+00000d70: 388c 0641 7574 686f 7294 7494 4b0b 4b0c  8..Author.t.K.K.
+00000d80: 4b00 8794 4b0b 4b00 4b0a 8794 4b46 4b0c  K...K.K.K...KFK.
+00000d90: 8694 4b0b 4b0a 4b00 8794 284b 0c4b 096a  ..K.K.K...(K.K.j
+00000da0: 3401 0000 6a35 0100 0074 944b 0b4b 004b  4...j5...t.K.K.K
+00000db0: 0b87 9428 4b0c 4b01 6838 8c05 7469 746c  ...(K.K.h8..titl
+00000dc0: 6594 7494 4b47 4b00 4b01 8794 4b02 4da3  e.t.KGK.K...K.M.
+00000dd0: 0186 944b 464b 0986 944b 0b4b 0b4b 0087  ...KFK...K.K.K..
+00000de0: 9468 3528 4b0c 4b01 6838 6ac5 0100 0074  .h5(K.K.h8j....t
+00000df0: 944b 0b4b 0c4b 0087 944b 0b4b 004b 0a87  .K.K.K...K.K.K..
+00000e00: 944b 464b 0c86 944b 0b4b 0a4b 0087 9428  .KFK...K.K.K...(
+00000e10: 4b0c 4b09 6a34 0100 006a 3501 0000 7494  K.K.j4...j5...t.
+00000e20: 4b0b 4b00 4b0b 8794 284b 0c4b 0168 388c  K.K.K...(K.K.h8.
+00000e30: 0474 6573 7494 7494 4b47 4b00 4b01 8794  .test.t.KGK.K...
+00000e40: 4b02 4db0 0186 944b 464b 0986 944b 0b4b  K.M....KFK...K.K
+00000e50: 0b4b 0087 9468 3528 4b0c 4b01 6838 8c05  .K...h5(K.K.h8..
+00000e60: 5469 746c 6594 7494 4b0b 4b0c 4b00 8794  Title.t.K.K.K...
+00000e70: 4b0b 4b00 4b0a 8794 4b46 4b0c 8694 4b0b  K.K.K...KFK...K.
+00000e80: 4b0a 4b00 8794 4b0b 4b00 4b0e 8794 4b3f  K.K...K.K.K...K?
+00000e90: 4b00 4b0a 8794 4b0b 4b0e 4b00 8794 4b33  K.K...K.K.K...K3
+00000ea0: 4b0d 8694 4b09 4b0e 8694 4b38 4b0c 4b04  K...K.K...K8K.K.
+00000eb0: 8794 4b0a 4b0d 8694 284b 0c4b 0b68 095d  ..K.K...(K.K.h.]
+00000ec0: 9474 9428 4b4e 4b0b 4b0c 4b0d 7494 4b09  .t.(KNK.K.K.t.K.
+00000ed0: 4b0b 8694 4b0a 4b00 8694 4b4c 4b00 8694  K...K.K...KLK...
+00000ee0: 4b36 4b0b 4b00 8794 284b 104b 0b68 304b  K6K.K...(K.K.h0K
+00000ef0: 0074 944b 024d cb01 8694 4b3d 4b00 6810  .t.K.M....K=K.h.
+00000f00: 8794 4b02 4dcb 0186 9428 4b0c 4b0b 6a1a  ..K.M....(K.K.j.
+00000f10: 0100 0088 7494 284b 104b 0b6a 1a01 0000  ....t.(K.K.j....
+00000f20: 8974 944b 024d cb01 8694 4b53 4b00 8694  .t.K.M....KSK...
+00000f30: 4b4c 4b00 8694 4b3d 4b00 6810 8794 4b03  KLK...K=K.h...K.
+00000f40: 4dd6 0186 9428 4b0c 4b0b 6830 4b03 7494  M....(K.K.h0K.t.
+00000f50: 284b 104b 0b68 304b 0174 944b 034d d601  (K.K.h0K.t.K.M..
+00000f60: 8694 284b 0c4b 0b68 386a b701 0000 7494  ..(K.K.h8j....t.
+00000f70: 284b 104b 0b68 386a 7601 0000 7494 4b02  (K.K.h8jv...t.K.
+00000f80: 4dd6 0186 944b 0b4b 014b 0b87 9468 354b  M....K.K.K...h5K
+00000f90: 4c4b 0086 9428 4b0c 4b01 6830 4b04 7494  LK...(K.K.h0K.t.
+00000fa0: 4b3c 4b01 4b00 8794 4b09 4b06 8694 4b0b  K<K.K...K.K...K.
+00000fb0: 4b06 4b07 8794 4b38 4b00 4b04 8794 4b09  K.K...K8K.K...K.
+00000fc0: 4b00 8694 4b35 4b00 8694 4b09 4b00 8694  K...K5K...K.K...
+00000fd0: 4b23 4b00 4b00 8794 4b09 4b00 8694 4b09  K#K.K...K.K...K.
+00000fe0: 4b00 8694 4b38 4b00 4b07 8794 4b38 4b01  K...K8K.K...K8K.
+00000ff0: 4b08 8794 4b11 4b00 4b01 8794 4b02 4df3  K...K.K.K...K.M.
+00001000: 0186 944b 384b 004b 0687 944b 4585 944b  ...K8K.K...KE..K
+00001010: 394b 094b 0087 944b 384b 004b 0987 944b  9K.K...K8K.K...K
+00001020: 094b 0086 944b 0a4b 0086 944b 4385 9428  .K...K.K...KC..(
+00001030: 4b0c 4b00 6838 8c01 0a94 7494 6a14 0200  K.K.h8....t.j...
+00001040: 004b 384b 004b 0887 944b 334b 0086 944b  .K8K.K...K3K...K
+00001050: 394b 084b 0087 944b 014d e201 8694 4b0b  9K.K...K.M....K.
+00001060: 4b07 4b06 8794 4b0a 4b06 8694 4b0b 4b07  K.K...K.K...K.K.
+00001070: 4b06 8794 4b0a 4b06 8694 4b2f 8594 4b51  K...K.K...K/..KQ
+00001080: 7d94 288c 0956 4152 4941 424c 4553 945d  }.(..VARIABLES.]
+00001090: 948c 0946 554e 4354 494f 4e53 945d 948c  ...FUNCTIONS.]..
+000010a0: 094c 4942 5241 5249 4553 945d 948c 064c  .LIBRARIES.]...L
+000010b0: 4142 454c 5394 5d94 8c05 4a55 4d50 5394  ABELS.]...JUMPS.
+000010c0: 5d94 8c08 5245 5345 5256 4544 945d 9428  ]...RESERVED.].(
+000010d0: 8c03 7661 7294 4b03 8694 8c01 7994 4b04  ..var.K.....y.K.
+000010e0: 8694 6575 8694 652e                      ..eu..e.
```

### Comparing `macal-5.0rc8/tests/select_7.mbc` & `macal-5.0rc9/tests/select_7.mbc`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 424d 4301 0000 0017 0300 0080 0495 0c03  BMC.............
+00000000: 424d 4301 0000 00b0 0300 0080 0495 a503  BMC.............
 00000010: 0000 0000 0000 5d94 284b 094b 0686 944b  ......].(K.K...K
 00000020: 0b4b 064b 0787 944b 234b 004b 0087 944b  .K.K...K#K.K...K
 00000030: 094b 0086 9428 4b0c 4b00 8c12 6d61 6361  .K...(K.K...maca
 00000040: 6c2e 6173 745f 6e6f 6465 7479 7065 948c  l.ast_nodetype..
 00000050: 0b41 7374 4e6f 6465 7479 7065 9493 944b  .AstNodetype...K
 00000060: 8485 9452 945d 9428 7d94 288c 0269 6494  ...R.].(}.(..id.
 00000070: 4b01 8c04 6e61 6d65 948c 0474 6573 7494  K...name...test.
@@ -29,23 +29,32 @@
 000001c0: 8694 4b0a 4b01 8694 4b0a 4b00 8694 4b11  ..K.K...K.K...K.
 000001d0: 4b00 4b01 8794 4b26 4b00 8694 4b09 4b00  K.K...K&K...K.K.
 000001e0: 8694 4b0a 4b00 8694 284b 104b 0068 074b  ..K.K...(K.K.h.K
 000001f0: 8385 9452 9488 7494 4b03 4b32 8694 4b3f  ...R..t.K.K2..K?
 00000200: 4b0d 4b0c 8794 284b 0c4b 0068 4989 7494  K.K...(K.K.hI.t.
 00000210: 284b 104b 0068 4988 7494 4b02 4b34 8694  (K.K.hI.t.K.K4..
 00000220: 4b33 4b0f 8694 4b08 4b1c 8694 4b09 4b0d  K3K...K.K...K.K.
-00000230: 8694 4b0a 4b00 8694 284b 0c4b 0168 2f4b  ..K.K...(K.K.h/K
-00000240: 0474 944b 0b4b 0c4b 0087 944b 524b 004b  .t.K.K.K...KRK.K
-00000250: 0187 944b 094b 0086 9428 4b0c 4b00 682f  ...K.K...(K.K.h/
-00000260: 4b01 7494 4b09 4b00 8694 4b0a 4b01 8694  K.t.K.K...K.K...
-00000270: 4b0a 4b00 8694 4b46 4b0c 8694 4b38 4b00  K.K...KFK...K8K.
-00000280: 4b04 8794 4b09 4b00 8694 4b0a 4b00 8694  K...K.K...K.K...
-00000290: 4b43 8594 284b 0c4b 0068 3c8c 010a 9474  KC..(K.K.h<....t
-000002a0: 9468 604b 0b4b 074b 0687 944b 0a4b 0686  .h`K.K.K...K.K..
-000002b0: 944b 2f85 944b 517d 9428 8c09 5641 5249  .K/..KQ}.(..VARI
-000002c0: 4142 4c45 5394 5d94 8c09 4655 4e43 5449  ABLES.]...FUNCTI
-000002d0: 4f4e 5394 5d94 8c09 4c49 4252 4152 4945  ONS.]...LIBRARIE
-000002e0: 5394 5d94 8c06 4c41 4245 4c53 945d 948c  S.]...LABELS.]..
-000002f0: 054a 554d 5053 945d 948c 0852 4553 4552  .JUMPS.]...RESER
-00000300: 5645 4494 5d94 288c 0376 6172 944b 0386  VED.].(..var.K..
-00000310: 948c 0476 6172 3294 4b04 8694 6575 8694  ...var2.K...eu..
-00000320: 652e                                     e.
+00000230: 8694 4b0a 4b00 8694 4b36 4b0c 4b00 8794  ..K.K...K6K.K...
+00000240: 284b 104b 0c68 2f4b 0074 944b 024b 3f86  (K.K.h/K.t.K.K?.
+00000250: 944b 3d4b 0068 2787 944b 024b 3f86 9428  .K=K.h'..K.K?..(
+00000260: 4b0c 4b0c 6849 8974 9428 4b10 4b0c 6849  K.K.hI.t.(K.K.hI
+00000270: 8974 944b 024b 3f86 944b 534b 0086 944b  .t.K.K?..KSK...K
+00000280: 3d4b 0068 2787 944b 034b 4986 9428 4b0c  =K.h'..K.KI..(K.
+00000290: 4b0c 682f 4b01 7494 284b 104b 0c68 2f4b  K.h/K.t.(K.K.h/K
+000002a0: 0174 944b 034b 4986 9428 4b0c 4b0c 683c  .t.K.KI..(K.K.h<
+000002b0: 8c01 2a94 7494 284b 104b 0c68 3c68 6274  ..*.t.(K.K.h<hbt
+000002c0: 944b 024b 4986 944b 0b4b 014b 0c87 9468  .K.KI..K.K.K...h
+000002d0: 3828 4b0c 4b01 682f 4b04 7494 4b0b 4b0c  8(K.K.h/K.t.K.K.
+000002e0: 4b00 8794 4b52 4b00 4b01 8794 4b09 4b00  K...KRK.K...K.K.
+000002f0: 8694 284b 0c4b 0068 2f4b 0174 944b 094b  ..(K.K.h/K.t.K.K
+00000300: 0086 944b 0a4b 0186 944b 0a4b 0086 944b  ...K.K...K.K...K
+00000310: 464b 0c86 944b 384b 004b 0487 944b 094b  FK...K8K.K...K.K
+00000320: 0086 944b 0a4b 0086 944b 4385 9428 4b0c  ...K.K...KC..(K.
+00000330: 4b00 683c 8c01 0a94 7494 6873 4b0b 4b07  K.h<....t.hsK.K.
+00000340: 4b06 8794 4b0a 4b06 8694 4b2f 8594 4b51  K...K.K...K/..KQ
+00000350: 7d94 288c 0956 4152 4941 424c 4553 945d  }.(..VARIABLES.]
+00000360: 948c 0946 554e 4354 494f 4e53 945d 948c  ...FUNCTIONS.]..
+00000370: 094c 4942 5241 5249 4553 945d 948c 064c  .LIBRARIES.]...L
+00000380: 4142 454c 5394 5d94 8c05 4a55 4d50 5394  ABELS.]...JUMPS.
+00000390: 5d94 8c08 5245 5345 5256 4544 945d 9428  ]...RESERVED.].(
+000003a0: 8c03 7661 7294 4b03 8694 8c04 7661 7232  ..var.K.....var2
+000003b0: 944b 0486 9465 7586 9465 2e              .K...eu..e.
```

### Comparing `macal-5.0rc8/tests/select_8.mbc` & `macal-5.0rc9/tests/select_8.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/select_8.mcl` & `macal-5.0rc9/tests/select_8.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/test.mcl` & `macal-5.0rc9/tests/test.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/usereserved.mbc` & `macal-5.0rc9/tests/usereserved.mbc`

 * *Files identical despite different names*

### Comparing `macal-5.0rc8/tests/usereserved.mcl` & `macal-5.0rc9/tests/usereserved.mcl`

 * *Files identical despite different names*

