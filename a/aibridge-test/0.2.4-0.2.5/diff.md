# Comparing `tmp/aibridge_test-0.2.4.tar.gz` & `tmp/aibridge_test-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.4.tar", last modified: Thu Apr  4 10:40:10 2024, max compression
+gzip compressed data, was "aibridge_test-0.2.5.tar", last modified: Thu Apr  4 10:55:31 2024, max compression
```

## Comparing `aibridge_test-0.2.4.tar` & `aibridge_test-0.2.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.441914 aibridge_test-0.2.4/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.104932 aibridge_test-0.2.4/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.4/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.191914 aibridge_test-0.2.4/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.4/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    12767 2024-04-04 09:54:43.000000 aibridge_test-0.2.4/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0     8851 2024-04-02 05:11:27.000000 aibridge_test-0.2.4/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14015 2024-04-04 09:41:59.000000 aibridge_test-0.2.4/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.4/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.4/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.4/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.4/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.4/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.208912 aibridge_test-0.2.4/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     6650 2024-04-04 09:20:56.000000 aibridge_test-0.2.4/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      729 2024-04-04 03:51:54.000000 aibridge_test-0.2.4/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.257914 aibridge_test-0.2.4/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.283923 aibridge_test-0.2.4/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.4/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.306913 aibridge_test-0.2.4/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.4/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.4/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.334915 aibridge_test-0.2.4/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.354912 aibridge_test-0.2.4/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.4/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    21574 2024-04-04 10:40:10.435915 aibridge_test-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:40:10.432912 aibridge_test-0.2.4/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21574 2024-04-04 10:40:09.000000 aibridge_test-0.2.4/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-04-04 10:40:10.000000 aibridge_test-0.2.4/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:40:09.000000 aibridge_test-0.2.4/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2024-04-04 10:40:09.000000 aibridge_test-0.2.4/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-04 10:40:09.000000 aibridge_test-0.2.4/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 10:40:10.442913 aibridge_test-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2895 2024-04-04 10:39:22.000000 aibridge_test-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.662554 aibridge_test-0.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.408557 aibridge_test-0.2.5/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.5/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.474555 aibridge_test-0.2.5/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.5/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    12767 2024-04-04 09:54:43.000000 aibridge_test-0.2.5/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0     8851 2024-04-02 05:11:27.000000 aibridge_test-0.2.5/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14015 2024-04-04 09:41:59.000000 aibridge_test-0.2.5/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.5/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.5/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.5/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.5/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.5/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.490559 aibridge_test-0.2.5/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     6650 2024-04-04 09:20:56.000000 aibridge_test-0.2.5/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      729 2024-04-04 03:51:54.000000 aibridge_test-0.2.5/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.533559 aibridge_test-0.2.5/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.547556 aibridge_test-0.2.5/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.5/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.563569 aibridge_test-0.2.5/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.5/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.5/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.578555 aibridge_test-0.2.5/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.598634 aibridge_test-0.2.5/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.5/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    21533 2024-04-04 10:55:31.657553 aibridge_test-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:55:31.655569 aibridge_test-0.2.5/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21533 2024-04-04 10:55:31.000000 aibridge_test-0.2.5/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-04 10:55:31.000000 aibridge_test-0.2.5/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:55:31.000000 aibridge_test-0.2.5/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      227 2024-04-04 10:55:31.000000 aibridge_test-0.2.5/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-04 10:55:31.000000 aibridge_test-0.2.5/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:55:31.668602 aibridge_test-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2862 2024-04-04 10:54:38.000000 aibridge_test-0.2.5/setup.py
```

### Comparing `aibridge_test-0.2.4/AIBridge/__init__.py` & `aibridge_test-0.2.5/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.2.5/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.2.5/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.2.5/AIBridge/ai_services/anthropic_ai.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.2.5/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.2.5/AIBridge/ai_services/geminin_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.2.5/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.2.5/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.2.5/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.2.5/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.2.5/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.2.5/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.2.5/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/constant/common.py` & `aibridge_test-0.2.5/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/constant/constant.py` & `aibridge_test-0.2.5/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/database/db_layer.py` & `aibridge_test-0.2.5/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/database/no_sql_service.py` & `aibridge_test-0.2.5/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/database/session.py` & `aibridge_test-0.2.5/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/database/sql_service.py` & `aibridge_test-0.2.5/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/exceptions.py` & `aibridge_test-0.2.5/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/output_validation/convertors.py` & `aibridge_test-0.2.5/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/output_validation/validations.py` & `aibridge_test-0.2.5/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.2.5/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.2.5/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.2.5/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.2.5/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.2.5/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.2.5/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/AIBridge/setconfig.py` & `aibridge_test-0.2.5/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/LICENSE` & `aibridge_test-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/PKG-INFO` & `aibridge_test-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.4
+Version: 0.2.5
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing_extensions>=4.7.0
 Requires-Dist: openai<=1.7.1
 Requires-Dist: SQLAlchemy>=2.0.19
 Requires-Dist: redis>=4.6.0
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: pymongo>=4.4.1
 Requires-Dist: sqlparse>=0.4.4
```

### Comparing `aibridge_test-0.2.4/README.md` & `aibridge_test-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.2.5/aibridge_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.4
+Version: 0.2.5
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing_extensions>=4.7.0
 Requires-Dist: openai<=1.7.1
 Requires-Dist: SQLAlchemy>=2.0.19
 Requires-Dist: redis>=4.6.0
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: pymongo>=4.4.1
 Requires-Dist: sqlparse>=0.4.4
```

### Comparing `aibridge_test-0.2.4/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.2.5/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.4/setup.py` & `aibridge_test-0.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.4"
+VERSION = "0.2.5"
 REQUIRED = [
-    "typing_extensions>=4.7.0",
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
     "sqlparse>=0.4.4",
```

