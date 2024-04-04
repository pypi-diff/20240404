# Comparing `tmp/esbmc_ai-0.5.0.dev9.tar.gz` & `tmp/esbmc_ai-0.5.0rc0.tar.gz`

## Comparing `esbmc_ai-0.5.0.dev9.tar` & `esbmc_ai-0.5.0rc0.tar`

### file list

```diff
@@ -1,139 +1,27 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/build.sh
--rw-r--r--   0        0        0   126731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/cartpole_60_safe.c-amalgamation-89.c
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/clean.sh
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/config.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/CMakeLists.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/verifier_functions.h
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/verifier_stubs.c
--rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_activations.c
--rw-r--r--   0        0        0    16892 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_convolution_layers.c
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_core_layers.c
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_embedding_layers.c
--rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_helper_functions.c
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_include.h
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_merge_layers.c
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_normalization_layers.c
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_pooling_layers.c
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_recurrent_layers.c
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_tensor_include.h
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__cosdf.c
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__expo2f.c
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__fpclassifyf.c
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__invtrigl.c
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__invtrigl.h
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_divzerof.c
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_invalidf.c
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_oflowf.c
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_uflowf.c
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_xflowf.c
--rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__rem_pio2_large.c
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__rem_pio2f.c
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__signbitf.c
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__sindf.c
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__tandf.c
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/acosf.c
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/alltypes.h
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/asinf.c
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/atanhf.c
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/atomic.h
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/cosf.c
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/endian.h
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/erff.c
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/exp2f_data.c
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/exp2f_data.h
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/exp_data.h
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/expf.c
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/expm1f.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/fabsf.c
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/fmaxf.c
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/libm.h
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log1pf.c
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log2_data.h
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log2f_data.c
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log2f_data.h
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log_data.h
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/logf.c
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/logf_data.c
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/logf_data.h
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/pow_data.h
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/powf_data.c
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/powf_data.h
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sinf.c
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sqrt_data.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sqrt_data.h
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sqrtf.c
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/tanhf.c
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/threading.c
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/threading_broken.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_ai_models.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_config.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_esbmc_util.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_solution.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_solution_generator.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
--rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
--rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
--rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
--rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/config.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/config.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/esbmc_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,14 +63,33 @@
     line: Optional[int] = get_source_code_err_line(esbmc_output)
     if line:
         return line - 1
     else:
         return None
 
 
+def get_clang_err_line(clang_output: str) -> Optional[int]:
+    """For when the code does not compile, gets the error line reported in the clang
+    output. This is useful for `esbmc_output_type single`"""
+    # TODO Test me
+    lines: list[str] = clang_output.splitlines()
+    for line in lines:
+        # Find the first line containing a filename along with error.
+        line_split: list[str] = line.split(":")
+        # Check for the filename
+        if line_split[0].endswith(".c") and " error" in line_split[3]:
+            return int(line_split[1])
+
+    return None
+
+
+def get_clang_err_line_index(clang_output: str) -> Optional[int]:
+    return get_clang_err_line(clang_output)
+
+
 def esbmc(path: str, esbmc_params: list, timeout: Optional[float] = None):
     """Exit code will be 0 if verification successful, 1 if verification
     failed. And any other number for compilation error/general errors."""
     # Build parameters
     esbmc_cmd = [config.esbmc_path]
     esbmc_cmd.extend(esbmc_params)
     esbmc_cmd.append(path)
```

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/logging.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 def printvvv(m) -> None:
     """Level 3 verbose printing."""
     if _verbose > 2:
         print(m)
 
 
 def print_horizontal_line(verbosity: int) -> None:
-    if verbosity >= _verbose:
+    if _verbose >= verbosity:
         try:
-            printvv("-" * get_terminal_size().columns)
+            print("-" * get_terminal_size().columns)
         except OSError:
             pass
```

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/solution_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Author: Yiannis Charalambous 2023
 
 from re import S
 from typing import Optional
 from typing_extensions import override
 from langchain.base_language import BaseLanguageModel
-from langchain.schema import BaseMessage
+from langchain.schema import BaseMessage, HumanMessage
 
 from esbmc_ai.chat_response import ChatResponse, FinishReason
 from esbmc_ai.config import ChatPromptSettings, DynamicAIModelAgent
 from esbmc_ai.frontend.solution import apply_line_patch
 
 from .ai_models import AIModel
 from .base_chat_interface import BaseChatInterface
 from esbmc_ai.esbmc_util import (
     esbmc_get_counter_example,
     esbmc_get_violated_property,
     get_source_code_err_line_idx,
+    get_clang_err_line_index,
 )
 
 
 class ESBMCTimedOutException(Exception):
     pass
 
 
@@ -28,19 +29,27 @@
 
 
 def get_source_code_formatted(
     source_code_format: str, source_code: str, esbmc_output: str
 ) -> str:
     match source_code_format:
         case "single":
+            # Get source code error line from esbmc output
             line: Optional[int] = get_source_code_err_line_idx(esbmc_output)
-            assert line, f"error line not found in esbmc output:\n{esbmc_output}"
-            # ESBMC reports errors starting from 1. To get the correct line, we need to use 0 based
-            # indexing.
-            return source_code.splitlines(True)[line]
+            if line:
+                return source_code.splitlines(True)[line]
+
+            # Check if it parses
+            line = get_clang_err_line_index(esbmc_output)
+            if line:
+                return source_code.splitlines(True)[line]
+
+            raise AssertionError(
+                f"error line not found in esbmc output:\n{esbmc_output}"
+            )
         case "full":
             return source_code
         case _:
             raise ValueError(
                 f"Not a valid format for source code: {source_code_format}"
             )
 
@@ -88,42 +97,39 @@
         )
 
         super().__init__(
             ai_model_agent=chat_prompt,
             ai_model=ai_model,
             llm=llm,
         )
+
         self.initial_prompt = ai_model_agent.initial_prompt
 
         self.esbmc_output_type: str = esbmc_output_type
         self.source_code_format: str = source_code_format
         self.source_code_raw: str = source_code
+        # Used for resetting state.
+        self._original_source_code: str = source_code
 
+        # Format ESBMC output
         try:
             self.esbmc_output = get_esbmc_output_formatted(
                 esbmc_output_type=self.esbmc_output_type,
                 esbmc_output=esbmc_output,
             )
         except SourceCodeParseError:
+            # When clang output is displayed, show it entirely as it doesn't get very
+            # big.
             self.esbmc_output = esbmc_output
 
-        source_code_formatted: str = get_source_code_formatted(
-            source_code_format=self.source_code_format,
-            source_code=self.source_code_raw,
-            esbmc_output=self.esbmc_output,
-        )
-        self.apply_template_value(
-            source_code=source_code_formatted,
-            esbmc_output=self.esbmc_output,
-        )
-
     @override
     def compress_message_stack(self) -> None:
         # Resets the conversation - cannot summarize code
         self.messages: list[BaseMessage] = []
+        self.source_code_raw = self._original_source_code
 
     @classmethod
     def get_code_from_solution(cls, solution: str) -> str:
         """Strip the source code of any leftover text as sometimes the AI model
         will generate text and formatting despite being told not to."""
         try:
             code_start: int = solution.index("```") + 3
@@ -143,15 +149,31 @@
 
             solution = solution[code_start:code_end]
         except (ValueError, AssertionError):
             pass
         return solution
 
     def generate_solution(self) -> tuple[str, FinishReason]:
-        response: ChatResponse = self.send_message(self.initial_prompt)
+        self.push_to_message_stack(HumanMessage(content=self.initial_prompt))
+
+        # Format source code
+        source_code_formatted: str = get_source_code_formatted(
+            source_code_format=self.source_code_format,
+            source_code=self.source_code_raw,
+            esbmc_output=self.esbmc_output,
+        )
+
+        # Apply template substitution to message stack
+        self.apply_template_value(
+            source_code=source_code_formatted,
+            esbmc_output=self.esbmc_output,
+        )
+
+        # Generate the solution
+        response: ChatResponse = self.send_message()
         solution: str = str(response.message.content)
 
         solution = SolutionGenerator.get_code_from_solution(solution)
 
         # If source code passed to LLM is formatted then we need to recombine to
         # full source code before giving to ESBMC
         match self.source_code_format:
@@ -162,8 +184,10 @@
                 assert (
                     err_line
                 ), "fix code command: error line could not be found to apply brutal patch replacement"
                 solution = apply_line_patch(
                     self.source_code_raw, solution, err_line, err_line
                 )
 
+        # Remember it for next cycle
+        self.source_code_raw = solution
         return solution, response.finish_reason
```

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/commands/fix_code_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Author: Yiannis Charalambous
 
-from os import get_terminal_size
 import sys
 from typing import Any, Tuple
 from typing_extensions import override
 from langchain.schema import AIMessage, HumanMessage
 
 from esbmc_ai.chat_response import FinishReason
 
@@ -36,20 +35,21 @@
             help_message="Generates a solution for this code, and reevaluates it with ESBMC.",
         )
         self.anim = create_loading_widget()
 
     @override
     def execute(self, **kwargs: Any) -> Tuple[bool, str]:
         def print_raw_conversation() -> None:
-            print("Notice: Printing raw conversation...")
+            print_horizontal_line(0)
+            print("ESBMC-AI Notice: Printing raw conversation...")
             all_messages = solution_generator._system_messages.copy()
             all_messages.extend(solution_generator.messages.copy())
             messages: list[str] = [f"{msg.type}: {msg.content}" for msg in all_messages]
             print("\n" + "\n\n".join(messages))
-            print("Notice: End of conversation")
+            print("ESBMC-AI Notice: End of raw conversation")
 
         file_name: str = kwargs["file_name"]
         source_code: str = kwargs["source_code"]
         esbmc_output: str = kwargs["esbmc_output"]
 
         # Parse the esbmc output here and determine what "Scenario" to use.
         scenario: str = esbmc_get_error_type(esbmc_output)
@@ -115,42 +115,46 @@
                 source_code=llm_solution,
                 esbmc_params=config.esbmc_params,
                 auto_clean=config.temp_auto_clean,
                 timeout=config.verifier_timeout,
             )
             self.anim.stop()
 
-            # TODO Move this process into Solution Generator since have (beginning) is done
-            # inside, and the other half is done here.
-            try:
-                esbmc_output = get_esbmc_output_formatted(
-                    esbmc_output_type=config.esbmc_output_type,
-                    esbmc_output=esbmc_output,
-                )
-            except SourceCodeParseError:
-                pass
-            except ESBMCTimedOutException:
-                print("error: ESBMC has timed out...")
-                sys.exit(1)
-
             # Print verbose lvl 2
             print_horizontal_line(2)
             printvv(esbmc_output)
             print_horizontal_line(2)
 
+            # Solution found
             if exit_code == 0:
                 self.on_solution_signal.emit(llm_solution)
 
                 if config.raw_conversation:
                     print_raw_conversation()
 
+                printv("ESBMC-AI Notice: Successfully verified code")
+
                 return False, llm_solution
 
+            # TODO Move this process into Solution Generator since have (beginning) is done
+            # inside, and the other half is done here.
+            # Get formatted ESBMC output
+            try:
+                esbmc_output = get_esbmc_output_formatted(
+                    esbmc_output_type=config.esbmc_output_type,
+                    esbmc_output=esbmc_output,
+                )
+            except SourceCodeParseError:
+                pass
+            except ESBMCTimedOutException:
+                print("error: ESBMC has timed out...")
+                sys.exit(1)
+
             # Failure case
-            print(f"Failure {idx+1}/{max_retries}: Retrying...")
+            print(f"ESBMC-AI Notice: Failure {idx+1}/{max_retries}: Retrying...")
             # If final iteration no need to sleep.
             if idx < max_retries - 1:
 
                 # Inform solution generator chat about the ESBMC response.
                 # TODO Add option to customize in config.
                 if exit_code != 1:
                     # The program did not compile.
@@ -168,8 +172,9 @@
 
                 solution_generator.push_to_message_stack(
                     AIMessage(content="Understood.")
                 )
 
         if config.raw_conversation:
             print_raw_conversation()
-        return True, "Failed all attempts..."
+
+        return True, "ESBMC-AI Notice: Failed all attempts..."
```

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0rc0/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/.gitignore` & `esbmc_ai-0.5.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/LICENSE` & `esbmc_ai-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/README.md` & `esbmc_ai-0.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev9/pyproject.toml` & `esbmc_ai-0.5.0rc0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -61,26 +61,18 @@
 "Source Code" = "https://github.com/Yiannis128/esbmc-ai"
 Documentation = "https://github.com/Yiannis128/esbmc-ai/wiki"
 Issues = "https://github.com/Yiannis128/esbmc-ai/issues"
 
 [tool.hatch.version]
 path = "esbmc_ai/__about__.py"
 
-# [tool.hatch.build.targets.esbmc_ai]
-# ignore-vcs = true
-# include = [
-#   "/esbmc_ai/**/*.py",
-#   "/esbmc_ai_config/**/*.py",
-# ]
-# exclude = [
-#  "/.github/*",
-#  "/.vscode",
-#  "/notebooks",
-#  "/samples",
-#  "/scripts",
-#  "/tests",
-#  "/env.example",
-#  "/.gitignore"
-# ]
+[tool.hatch.build.targets.sdist]
+ignore-vcs = false
+# include = ["esbmc-ai/**/*", "pyproject.toml", "README.md"]
+# exclude = ["**/*"]
+packages = ["esbmc_ai"]
 
-# [tool.hatch.build.targets.esbmc_ai.force-include]
-# "config.json" = "esbmc_ai_config/data/config.template.json"
+[tool.hatch.build.targets.wheel]
+ignore-vcs = false
+# include = ["esbmc-ai/**/*", "pyproject.toml", "README.md"]
+# exclude = ["**/*"]
+packages = ["esbmc_ai"]
```

### Comparing `esbmc_ai-0.5.0.dev9/PKG-INFO` & `esbmc_ai-0.5.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0.dev9
+Version: 0.5.0rc0
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

