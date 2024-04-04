# Comparing `tmp/superagent_py-0.2.24.tar.gz` & `tmp/superagent_py-0.2.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.2.24.tar", max compression
+gzip compressed data, was "superagent_py-0.2.25.tar", max compression
```

## Comparing `superagent_py-0.2.24.tar` & `superagent_py-0.2.25.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     1073 2024-03-31 07:49:11.139535 superagent_py-0.2.24/LICENSE
--rw-r--r--   0        0        0     3946 2024-03-31 07:49:11.139535 superagent_py-0.2.24/README.md
--rw-r--r--   0        0        0      434 2024-03-31 07:49:11.139535 superagent_py-0.2.24/pyproject.toml
--rw-r--r--   0        0        0     3944 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/__init__.py
--rw-r--r--   0        0        0     6143 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/client.py
--rw-r--r--   0        0        0      790 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1732 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/file.py
--rw-r--r--   0        0        0     4882 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/core/request_options.py
--rw-r--r--   0        0        0      166 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/environment.py
--rw-r--r--   0        0        0      170 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/py.typed
--rw-r--r--   0        0        0      333 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    71006 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/api_key/__init__.py
--rw-r--r--   0        0        0    17585 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/api_key/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/api_user/__init__.py
--rw-r--r--   0        0        0    17007 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/api_user/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/datasource/__init__.py
--rw-r--r--   0        0        0    23365 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/datasource/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/llm/__init__.py
--rw-r--r--   0        0        0    17465 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/llm/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/tool/__init__.py
--rw-r--r--   0        0        0    26029 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/tool/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/vector_database/__init__.py
--rw-r--r--   0        0        0    18052 2024-03-31 07:49:11.139535 superagent_py-0.2.24/src/superagent/resources/vector_database/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/resources/workflow/__init__.py
--rw-r--r--   0        0        0    42138 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/resources/workflow/client.py
--rw-r--r--   0        0        0       65 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/resources/workflow_config/__init__.py
--rw-r--r--   0        0        0     8456 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/resources/workflow_config/client.py
--rw-r--r--   0        0        0     5337 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/__init__.py
--rw-r--r--   0        0        0     1028 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/agent_datasosurce_list.py
--rw-r--r--   0        0        0     1007 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/agent_list.py
--rw-r--r--   0        0        0     1003 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/agent_tool_list.py
--rw-r--r--   0        0        0      708 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/agent_type.py
--rw-r--r--   0        0        0      977 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/api_key_create.py
--rw-r--r--   0        0        0     1435 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/api_key_create_model.py
--rw-r--r--   0        0        0      991 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/api_key_list.py
--rw-r--r--   0        0        0      879 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_api_key.py
--rw-r--r--   0        0        0     1231 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_api_user.py
--rw-r--r--   0        0        0     1436 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_datasource.py
--rw-r--r--   0        0        0     1042 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_llm.py
--rw-r--r--   0        0        0      989 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_vector_db.py
--rw-r--r--   0        0        0      902 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_workflow.py
--rw-r--r--   0        0        0      984 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_request_workflow_step.py
--rw-r--r--   0        0        0      986 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_agent.py
--rw-r--r--   0        0        0      934 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_agent_invoke.py
--rw-r--r--   0        0        0      991 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_api_key.py
--rw-r--r--   0        0        0      995 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_api_user.py
--rw-r--r--   0        0        0     1006 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_datasource.py
--rw-r--r--   0        0        0      978 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_llm.py
--rw-r--r--   0        0        0      982 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_tool.py
--rw-r--r--   0        0        0      999 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_vector_db.py
--rw-r--r--   0        0        0      998 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_workflow.py
--rw-r--r--   0        0        0     1015 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/app_models_response_workflow_step.py
--rw-r--r--   0        0        0     1027 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/datasource_list.py
--rw-r--r--   0        0        0      696 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/datasource_status.py
--rw-r--r--   0        0        0     2649 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/datasource_type.py
--rw-r--r--   0        0        0      560 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/embeddings_model_provider.py
--rw-r--r--   0        0        0     1013 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/function_definition.py
--rw-r--r--   0        0        0      973 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      978 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/llm_list.py
--rw-r--r--   0        0        0     2237 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/llm_model.py
--rw-r--r--   0        0        0      943 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/llm_params.py
--rw-r--r--   0        0        0     1184 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/llm_provider.py
--rw-r--r--   0        0        0     1248 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/open_ai_assistant_parameters.py
--rw-r--r--   0        0        0     1240 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/open_ai_assistant_parameters_tools_item.py
--rw-r--r--   0        0        0     2565 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_agent.py
--rw-r--r--   0        0        0     1560 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_agent_datasource.py
--rw-r--r--   0        0        0     1497 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_agent_llm.py
--rw-r--r--   0        0        0     1506 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_agent_tool.py
--rw-r--r--   0        0        0     1480 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_api_key.py
--rw-r--r--   0        0        0     2497 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_api_user.py
--rw-r--r--   0        0        0     2170 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_datasource.py
--rw-r--r--   0        0        0     1696 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_llm.py
--rw-r--r--   0        0        0     1826 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_tool.py
--rw-r--r--   0        0        0     1687 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_vector_db.py
--rw-r--r--   0        0        0     1814 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_workflow.py
--rw-r--r--   0        0        0     1645 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/prisma_models_workflow_step.py
--rw-r--r--   0        0        0      864 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/tool_assistant_tools_code.py
--rw-r--r--   0        0        0      978 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/tool_assistant_tools_function.py
--rw-r--r--   0        0        0      869 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/tool_assistant_tools_retrieval.py
--rw-r--r--   0        0        0     1003 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/tool_list.py
--rw-r--r--   0        0        0     3416 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/tool_type.py
--rw-r--r--   0        0        0      992 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      999 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/vector_db_list.py
--rw-r--r--   0        0        0     1003 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/vector_db_provider.py
--rw-r--r--   0        0        0     1667 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/workflow_config.py
--rw-r--r--   0        0        0     1019 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/workflow_list.py
--rw-r--r--   0        0        0     1015 2024-03-31 07:49:11.143535 superagent_py-0.2.24/src/superagent/types/workflow_step_list.py
--rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 superagent_py-0.2.24/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-04 21:16:59.879193 superagent_py-0.2.25/LICENSE
+-rw-r--r--   0        0        0     3946 2024-04-04 21:16:59.879193 superagent_py-0.2.25/README.md
+-rw-r--r--   0        0        0      434 2024-04-04 21:16:59.879193 superagent_py-0.2.25/pyproject.toml
+-rw-r--r--   0        0        0     3944 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/__init__.py
+-rw-r--r--   0        0        0     6143 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/client.py
+-rw-r--r--   0        0        0      790 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1732 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/core/request_options.py
+-rw-r--r--   0        0        0      166 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/environment.py
+-rw-r--r--   0        0        0      170 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/py.typed
+-rw-r--r--   0        0        0      333 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    71786 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/api_key/__init__.py
+-rw-r--r--   0        0        0    17585 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/api_key/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/api_user/__init__.py
+-rw-r--r--   0        0        0    17007 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/api_user/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/datasource/__init__.py
+-rw-r--r--   0        0        0    23365 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/datasource/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/llm/__init__.py
+-rw-r--r--   0        0        0    17465 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/llm/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/tool/__init__.py
+-rw-r--r--   0        0        0    26029 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/tool/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/vector_database/__init__.py
+-rw-r--r--   0        0        0    18052 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/vector_database/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/workflow/__init__.py
+-rw-r--r--   0        0        0    42610 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/workflow/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/workflow_config/__init__.py
+-rw-r--r--   0        0        0     8456 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/resources/workflow_config/client.py
+-rw-r--r--   0        0        0     5337 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0     1028 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/agent_datasosurce_list.py
+-rw-r--r--   0        0        0     1007 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/agent_list.py
+-rw-r--r--   0        0        0     1003 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/agent_tool_list.py
+-rw-r--r--   0        0        0      708 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/agent_type.py
+-rw-r--r--   0        0        0      977 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/api_key_create.py
+-rw-r--r--   0        0        0     1435 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/api_key_create_model.py
+-rw-r--r--   0        0        0      991 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/api_key_list.py
+-rw-r--r--   0        0        0      879 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_api_key.py
+-rw-r--r--   0        0        0     1231 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_api_user.py
+-rw-r--r--   0        0        0     1436 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_datasource.py
+-rw-r--r--   0        0        0     1042 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_llm.py
+-rw-r--r--   0        0        0      989 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_vector_db.py
+-rw-r--r--   0        0        0      902 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_workflow.py
+-rw-r--r--   0        0        0      984 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_request_workflow_step.py
+-rw-r--r--   0        0        0      986 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_agent.py
+-rw-r--r--   0        0        0      934 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_agent_invoke.py
+-rw-r--r--   0        0        0      991 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_api_key.py
+-rw-r--r--   0        0        0      995 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_api_user.py
+-rw-r--r--   0        0        0     1006 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_datasource.py
+-rw-r--r--   0        0        0      978 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_llm.py
+-rw-r--r--   0        0        0      982 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_tool.py
+-rw-r--r--   0        0        0      999 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_vector_db.py
+-rw-r--r--   0        0        0      998 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_workflow.py
+-rw-r--r--   0        0        0     1015 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/app_models_response_workflow_step.py
+-rw-r--r--   0        0        0     1027 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/datasource_list.py
+-rw-r--r--   0        0        0      696 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/datasource_status.py
+-rw-r--r--   0        0        0     2649 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/datasource_type.py
+-rw-r--r--   0        0        0      560 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/embeddings_model_provider.py
+-rw-r--r--   0        0        0     1013 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/function_definition.py
+-rw-r--r--   0        0        0      973 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      978 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/llm_list.py
+-rw-r--r--   0        0        0     2237 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/llm_model.py
+-rw-r--r--   0        0        0      943 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/llm_params.py
+-rw-r--r--   0        0        0     1184 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/llm_provider.py
+-rw-r--r--   0        0        0     1248 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/open_ai_assistant_parameters.py
+-rw-r--r--   0        0        0     1240 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/open_ai_assistant_parameters_tools_item.py
+-rw-r--r--   0        0        0     2658 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_agent.py
+-rw-r--r--   0        0        0     1560 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_agent_datasource.py
+-rw-r--r--   0        0        0     1497 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_agent_llm.py
+-rw-r--r--   0        0        0     1506 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_agent_tool.py
+-rw-r--r--   0        0        0     1480 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_api_key.py
+-rw-r--r--   0        0        0     2497 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_api_user.py
+-rw-r--r--   0        0        0     2170 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_datasource.py
+-rw-r--r--   0        0        0     1696 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_llm.py
+-rw-r--r--   0        0        0     1826 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_tool.py
+-rw-r--r--   0        0        0     1687 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_vector_db.py
+-rw-r--r--   0        0        0     1814 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_workflow.py
+-rw-r--r--   0        0        0     1645 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/prisma_models_workflow_step.py
+-rw-r--r--   0        0        0      864 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/tool_assistant_tools_code.py
+-rw-r--r--   0        0        0      978 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/tool_assistant_tools_function.py
+-rw-r--r--   0        0        0      869 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/tool_assistant_tools_retrieval.py
+-rw-r--r--   0        0        0     1003 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/tool_list.py
+-rw-r--r--   0        0        0     3584 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/tool_type.py
+-rw-r--r--   0        0        0      992 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      999 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/vector_db_list.py
+-rw-r--r--   0        0        0     1003 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/vector_db_provider.py
+-rw-r--r--   0        0        0     1667 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/workflow_config.py
+-rw-r--r--   0        0        0     1019 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/workflow_list.py
+-rw-r--r--   0        0        0     1015 2024-04-04 21:16:59.879193 superagent_py-0.2.25/src/superagent/types/workflow_step_list.py
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 superagent_py-0.2.25/PKG-INFO
```

### Comparing `superagent_py-0.2.24/LICENSE` & `superagent_py-0.2.25/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/README.md` & `superagent_py-0.2.25/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/__init__.py` & `superagent_py-0.2.25/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/client.py` & `superagent_py-0.2.25/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/core/__init__.py` & `superagent_py-0.2.25/src/superagent/core/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/core/client_wrapper.py` & `superagent_py-0.2.25/src/superagent/core/client_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "superagent-py",
-            "X-Fern-SDK-Version": "v0.2.24",
+            "X-Fern-SDK-Version": "v0.2.25",
         }
         token = self._get_token()
         if token is not None:
             headers["Authorization"] = f"Bearer {token}"
         return headers
 
     def _get_token(self) -> typing.Optional[str]:
```

### Comparing `superagent_py-0.2.24/src/superagent/core/datetime_utils.py` & `superagent_py-0.2.25/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/core/file.py` & `superagent_py-0.2.25/src/superagent/core/file.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/core/http_client.py` & `superagent_py-0.2.25/src/superagent/core/http_client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.2.25/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/core/request_options.py` & `superagent_py-0.2.25/src/superagent/core/request_options.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/agent/client.py` & `superagent_py-0.2.25/src/superagent/resources/agent/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         llm_model: typing.Optional[str] = OMIT,
         llm_provider: typing.Optional[LlmProvider] = OMIT,
         description: typing.Optional[str] = OMIT,
         avatar: typing.Optional[str] = OMIT,
         type: typing.Optional[AgentType] = OMIT,
         parameters: typing.Optional[OpenAiAssistantParameters] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Create a new agent
 
         Parameters:
             - is_active: typing.Optional[bool].
@@ -129,14 +130,16 @@
 
             - type: typing.Optional[AgentType].
 
             - parameters: typing.Optional[OpenAiAssistantParameters].
 
             - metadata: typing.Optional[typing.Dict[str, typing.Any]].
 
+            - output_schema: typing.Optional[str].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if initial_message is not OMIT:
             _request["initialMessage"] = initial_message
@@ -152,14 +155,16 @@
             _request["avatar"] = avatar
         if type is not OMIT:
             _request["type"] = type
         if parameters is not OMIT:
             _request["parameters"] = parameters
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if output_schema is not OMIT:
+            _request["outputSchema"] = output_schema
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -283,14 +288,15 @@
         initial_message: typing.Optional[str] = OMIT,
         prompt: typing.Optional[str] = OMIT,
         llm_model: typing.Optional[str] = OMIT,
         description: typing.Optional[str] = OMIT,
         avatar: typing.Optional[str] = OMIT,
         type: typing.Optional[str] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Patch an agent
 
         Parameters:
             - agent_id: str.
@@ -309,14 +315,16 @@
 
             - avatar: typing.Optional[str].
 
             - type: typing.Optional[str].
 
             - metadata: typing.Optional[typing.Dict[str, typing.Any]].
 
+            - output_schema: typing.Optional[str].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         """
         _request: typing.Dict[str, typing.Any] = {}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if name is not OMIT:
             _request["name"] = name
@@ -330,14 +338,16 @@
             _request["description"] = description
         if avatar is not OMIT:
             _request["avatar"] = avatar
         if type is not OMIT:
             _request["type"] = type
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if output_schema is not OMIT:
+            _request["outputSchema"] = output_schema
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -893,14 +903,15 @@
         llm_model: typing.Optional[str] = OMIT,
         llm_provider: typing.Optional[LlmProvider] = OMIT,
         description: typing.Optional[str] = OMIT,
         avatar: typing.Optional[str] = OMIT,
         type: typing.Optional[AgentType] = OMIT,
         parameters: typing.Optional[OpenAiAssistantParameters] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Create a new agent
 
         Parameters:
             - is_active: typing.Optional[bool].
@@ -921,14 +932,16 @@
 
             - type: typing.Optional[AgentType].
 
             - parameters: typing.Optional[OpenAiAssistantParameters].
 
             - metadata: typing.Optional[typing.Dict[str, typing.Any]].
 
+            - output_schema: typing.Optional[str].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if initial_message is not OMIT:
             _request["initialMessage"] = initial_message
@@ -944,14 +957,16 @@
             _request["avatar"] = avatar
         if type is not OMIT:
             _request["type"] = type
         if parameters is not OMIT:
             _request["parameters"] = parameters
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if output_schema is not OMIT:
+            _request["outputSchema"] = output_schema
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -1077,14 +1092,15 @@
         initial_message: typing.Optional[str] = OMIT,
         prompt: typing.Optional[str] = OMIT,
         llm_model: typing.Optional[str] = OMIT,
         description: typing.Optional[str] = OMIT,
         avatar: typing.Optional[str] = OMIT,
         type: typing.Optional[str] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Patch an agent
 
         Parameters:
             - agent_id: str.
@@ -1103,14 +1119,16 @@
 
             - avatar: typing.Optional[str].
 
             - type: typing.Optional[str].
 
             - metadata: typing.Optional[typing.Dict[str, typing.Any]].
 
+            - output_schema: typing.Optional[str].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         """
         _request: typing.Dict[str, typing.Any] = {}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if name is not OMIT:
             _request["name"] = name
@@ -1124,14 +1142,16 @@
             _request["description"] = description
         if avatar is not OMIT:
             _request["avatar"] = avatar
         if type is not OMIT:
             _request["type"] = type
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if output_schema is not OMIT:
+            _request["outputSchema"] = output_schema
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
```

### Comparing `superagent_py-0.2.24/src/superagent/resources/api_key/client.py` & `superagent_py-0.2.25/src/superagent/resources/api_key/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/api_user/client.py` & `superagent_py-0.2.25/src/superagent/resources/api_user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/datasource/client.py` & `superagent_py-0.2.25/src/superagent/resources/datasource/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/llm/client.py` & `superagent_py-0.2.25/src/superagent/resources/llm/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/tool/client.py` & `superagent_py-0.2.25/src/superagent/resources/tool/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/vector_database/client.py` & `superagent_py-0.2.25/src/superagent/resources/vector_database/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/resources/workflow/client.py` & `superagent_py-0.2.25/src/superagent/resources/workflow/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,33 +281,38 @@
     def invoke(
         self,
         workflow_id: str,
         *,
         input: str,
         enable_streaming: bool,
         session_id: typing.Optional[str] = OMIT,
+        output_schemas: typing.Optional[typing.Dict[str, str]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Invoke a specific workflow
 
         Parameters:
             - workflow_id: str.
 
             - input: str.
 
             - enable_streaming: bool.
 
             - session_id: typing.Optional[str].
 
+            - output_schemas: typing.Optional[typing.Dict[str, str]].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         """
         _request: typing.Dict[str, typing.Any] = {"input": input, "enableStreaming": enable_streaming}
         if session_id is not OMIT:
             _request["sessionId"] = session_id
+        if output_schemas is not OMIT:
+            _request["outputSchemas"] = output_schemas
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/invoke"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -741,33 +746,38 @@
     async def invoke(
         self,
         workflow_id: str,
         *,
         input: str,
         enable_streaming: bool,
         session_id: typing.Optional[str] = OMIT,
+        output_schemas: typing.Optional[typing.Dict[str, str]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Invoke a specific workflow
 
         Parameters:
             - workflow_id: str.
 
             - input: str.
 
             - enable_streaming: bool.
 
             - session_id: typing.Optional[str].
 
+            - output_schemas: typing.Optional[typing.Dict[str, str]].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         """
         _request: typing.Dict[str, typing.Any] = {"input": input, "enableStreaming": enable_streaming}
         if session_id is not OMIT:
             _request["sessionId"] = session_id
+        if output_schemas is not OMIT:
+            _request["outputSchemas"] = output_schemas
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/invoke"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
```

### Comparing `superagent_py-0.2.24/src/superagent/resources/workflow_config/client.py` & `superagent_py-0.2.25/src/superagent/resources/workflow_config/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/__init__.py` & `superagent_py-0.2.25/src/superagent/types/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/agent_datasosurce_list.py` & `superagent_py-0.2.25/src/superagent/types/agent_datasosurce_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/agent_list.py` & `superagent_py-0.2.25/src/superagent/types/agent_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/agent_tool_list.py` & `superagent_py-0.2.25/src/superagent/types/agent_tool_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/agent_type.py` & `superagent_py-0.2.25/src/superagent/types/agent_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/api_key_create.py` & `superagent_py-0.2.25/src/superagent/types/api_key_create.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/api_key_create_model.py` & `superagent_py-0.2.25/src/superagent/types/api_key_create_model.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/api_key_list.py` & `superagent_py-0.2.25/src/superagent/types/api_key_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_api_key.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_api_key.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_api_user.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_api_user.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_datasource.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_llm.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_vector_db.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_vector_db.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_workflow.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_workflow.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_request_workflow_step.py` & `superagent_py-0.2.25/src/superagent/types/app_models_request_workflow_step.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_agent.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_agent.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_agent_invoke.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_agent_invoke.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_api_key.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_api_key.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_api_user.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_api_user.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_datasource.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_llm.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_tool.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_tool.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_vector_db.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_vector_db.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_workflow.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_workflow.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/app_models_response_workflow_step.py` & `superagent_py-0.2.25/src/superagent/types/app_models_response_workflow_step.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/datasource_list.py` & `superagent_py-0.2.25/src/superagent/types/datasource_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/datasource_status.py` & `superagent_py-0.2.25/src/superagent/types/datasource_status.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/datasource_type.py` & `superagent_py-0.2.25/src/superagent/types/datasource_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/embeddings_model_provider.py` & `superagent_py-0.2.25/src/superagent/types/embeddings_model_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/function_definition.py` & `superagent_py-0.2.25/src/superagent/types/function_definition.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/http_validation_error.py` & `superagent_py-0.2.25/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/llm_list.py` & `superagent_py-0.2.25/src/superagent/types/llm_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/llm_model.py` & `superagent_py-0.2.25/src/superagent/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/llm_params.py` & `superagent_py-0.2.25/src/superagent/types/llm_params.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/llm_provider.py` & `superagent_py-0.2.25/src/superagent/types/llm_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/open_ai_assistant_parameters.py` & `superagent_py-0.2.25/src/superagent/types/open_ai_assistant_parameters.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/open_ai_assistant_parameters_tools_item.py` & `superagent_py-0.2.25/src/superagent/types/open_ai_assistant_parameters_tools_item.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_agent.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
     datasources: typing.Optional[typing.List[PrismaModelsAgentDatasource]] = None
     tools: typing.Optional[typing.List[PrismaModelsAgentTool]] = None
     workflow_steps: typing.Optional[typing.List[PrismaModelsWorkflowStep]] = pydantic.Field(
         alias="workflowSteps", default=None
     )
     metadata: typing.Optional[typing.Any] = None
+    output_schema: typing.Optional[str] = pydantic.Field(alias="outputSchema", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_agent_datasource.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_agent_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_agent_llm.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_agent_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_agent_tool.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_agent_tool.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_api_key.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_api_key.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_api_user.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_api_user.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_datasource.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_llm.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_tool.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_tool.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_vector_db.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_vector_db.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_workflow.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_workflow.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/prisma_models_workflow_step.py` & `superagent_py-0.2.25/src/superagent/types/prisma_models_workflow_step.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/tool_assistant_tools_code.py` & `superagent_py-0.2.25/src/superagent/types/tool_assistant_tools_code.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/tool_assistant_tools_function.py` & `superagent_py-0.2.25/src/superagent/types/tool_assistant_tools_function.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/tool_assistant_tools_retrieval.py` & `superagent_py-0.2.25/src/superagent/types/tool_assistant_tools_retrieval.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/tool_list.py` & `superagent_py-0.2.25/src/superagent/types/tool_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/tool_type.py` & `superagent_py-0.2.25/src/superagent/types/tool_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     HAND_OFF = "HAND_OFF"
     FUNCTION = "FUNCTION"
     HTTP = "HTTP"
     SUPERRAG = "SUPERRAG"
     RESEARCH = "RESEARCH"
     GITHUB = "GITHUB"
     SCRAPER = "SCRAPER"
+    GOOGLE_SEARCH = "GOOGLE_SEARCH"
 
     def visit(
         self,
         algolia: typing.Callable[[], T_Result],
         browser: typing.Callable[[], T_Result],
         bing_search: typing.Callable[[], T_Result],
         replicate: typing.Callable[[], T_Result],
@@ -54,14 +55,15 @@
         hand_off: typing.Callable[[], T_Result],
         function: typing.Callable[[], T_Result],
         http: typing.Callable[[], T_Result],
         superrag: typing.Callable[[], T_Result],
         research: typing.Callable[[], T_Result],
         github: typing.Callable[[], T_Result],
         scraper: typing.Callable[[], T_Result],
+        google_search: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is ToolType.ALGOLIA:
             return algolia()
         if self is ToolType.BROWSER:
             return browser()
         if self is ToolType.BING_SEARCH:
             return bing_search()
@@ -99,7 +101,9 @@
             return superrag()
         if self is ToolType.RESEARCH:
             return research()
         if self is ToolType.GITHUB:
             return github()
         if self is ToolType.SCRAPER:
             return scraper()
+        if self is ToolType.GOOGLE_SEARCH:
+            return google_search()
```

### Comparing `superagent_py-0.2.24/src/superagent/types/validation_error.py` & `superagent_py-0.2.25/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/vector_db_list.py` & `superagent_py-0.2.25/src/superagent/types/vector_db_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/vector_db_provider.py` & `superagent_py-0.2.25/src/superagent/types/vector_db_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/workflow_config.py` & `superagent_py-0.2.25/src/superagent/types/workflow_config.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/workflow_list.py` & `superagent_py-0.2.25/src/superagent/types/workflow_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/src/superagent/types/workflow_step_list.py` & `superagent_py-0.2.25/src/superagent/types/workflow_step_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.24/PKG-INFO` & `superagent_py-0.2.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.2.24
+Version: 0.2.25
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

