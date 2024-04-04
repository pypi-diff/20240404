# Comparing `tmp/aibridge_test-0.2.2.tar.gz` & `tmp/aibridge_test-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.2.tar", last modified: Tue Apr  2 05:22:15 2024, max compression
+gzip compressed data, was "aibridge_test-0.2.3.tar", last modified: Thu Apr  4 10:17:38 2024, max compression
```

## Comparing `aibridge_test-0.2.2.tar` & `aibridge_test-0.2.3.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.657930 aibridge_test-0.2.2/
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.227931 aibridge_test-0.2.2/AIBridge/
--rw-rw-rw-   0        0        0     1486 2024-03-22 06:03:11.000000 aibridge_test-0.2.2/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.302930 aibridge_test-0.2.2/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.2/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0     8851 2024-04-02 05:11:27.000000 aibridge_test-0.2.2/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14075 2024-04-02 05:20:23.000000 aibridge_test-0.2.2/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.2/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11582 2024-04-02 05:11:24.000000 aibridge_test-0.2.2/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.2/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.2/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     1849 2024-03-22 05:14:23.000000 aibridge_test-0.2.2/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.321935 aibridge_test-0.2.2/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     3644 2024-03-22 05:49:31.000000 aibridge_test-0.2.2/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      711 2024-03-22 08:02:44.000000 aibridge_test-0.2.2/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.344930 aibridge_test-0.2.2/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.403930 aibridge_test-0.2.2/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1100 2024-03-22 04:53:56.000000 aibridge_test-0.2.2/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.427929 aibridge_test-0.2.2/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1505 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5468 2024-03-22 07:59:34.000000 aibridge_test-0.2.2/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.454939 aibridge_test-0.2.2/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.484930 aibridge_test-0.2.2/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6194 2024-04-01 09:25:14.000000 aibridge_test-0.2.2/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    21499 2024-04-02 05:22:15.653931 aibridge_test-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 05:22:15.648935 aibridge_test-0.2.2/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21499 2024-04-02 05:22:15.000000 aibridge_test-0.2.2/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1731 2024-04-02 05:22:15.000000 aibridge_test-0.2.2/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 05:22:15.000000 aibridge_test-0.2.2/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2024-04-02 05:22:15.000000 aibridge_test-0.2.2/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 05:22:15.000000 aibridge_test-0.2.2/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 05:22:15.657930 aibridge_test-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2836 2024-04-02 05:21:19.000000 aibridge_test-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.496682 aibridge_test-0.2.3/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.029679 aibridge_test-0.2.3/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.3/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.145686 aibridge_test-0.2.3/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.3/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    12767 2024-04-04 09:54:43.000000 aibridge_test-0.2.3/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0     8851 2024-04-02 05:11:27.000000 aibridge_test-0.2.3/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14015 2024-04-04 09:41:59.000000 aibridge_test-0.2.3/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.3/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.3/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.3/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.3/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.3/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.166685 aibridge_test-0.2.3/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     6650 2024-04-04 09:20:56.000000 aibridge_test-0.2.3/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      729 2024-04-04 03:51:54.000000 aibridge_test-0.2.3/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.209686 aibridge_test-0.2.3/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.261679 aibridge_test-0.2.3/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.3/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.280681 aibridge_test-0.2.3/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.3/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.3/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.297694 aibridge_test-0.2.3/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.367681 aibridge_test-0.2.3/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.3/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    21533 2024-04-04 10:17:38.494685 aibridge_test-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:17:38.490682 aibridge_test-0.2.3/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21533 2024-04-04 10:17:37.000000 aibridge_test-0.2.3/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-04 10:17:37.000000 aibridge_test-0.2.3/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:17:37.000000 aibridge_test-0.2.3/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      227 2024-04-04 10:17:37.000000 aibridge_test-0.2.3/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-04 10:17:37.000000 aibridge_test-0.2.3/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:17:38.497681 aibridge_test-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2862 2024-04-04 10:15:10.000000 aibridge_test-0.2.3/setup.py
```

### Comparing `aibridge_test-0.2.2/AIBridge/__init__.py` & `aibridge_test-0.2.3/AIBridge/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from AIBridge.ai_services.openai_images import OpenAIImage
 from AIBridge.ai_services.palm_text import PalmText
 from AIBridge.ai_services.palm_chat import PalmChat
 from AIBridge.ai_services.stable_diffusion_image import StableDiffusion
 from AIBridge.ai_services.cohere_llm import CohereApi
 from AIBridge.ai_services.ai21labs_text import JurasicText
 from AIBridge.ai_services.geminin_services import GeminiAIService
+from AIBridge.ai_services.anthropic_ai import AnthropicService
 
 
 __all__ = [
     "OpenAIService",
     "SetConfig",
     "COnfigException",
     "OpenAIException",
@@ -32,10 +33,11 @@
     "OpenAIImage",
     "PalmText",
     "PalmChat",
     "StableDiffusion",
     "CohereApi",
     "JurasicText",
     "GeminiAIService",
+    "AnthropicService",
 ]
 
 __version__ = "0.0.0"
```

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.2.3/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.2.3/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.2.3/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.2.3/AIBridge/ai_services/geminin_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
                         "parts": [content],
                     }
                 )
                 tokens = exe_model.count_tokens(str(message_data)).total_tokens
                 print(tokens, type(tokens))
                 token_used = token_used + tokens
                 for res in response.candidates:
-                    index = response.candidates.index(res)
                     if response.candidates[0].content.parts[0].text:
                         content = response.candidates[0].content.parts[0].text
                     else:
                         content = response.candidates[0].content.parts[0].function_call
                         content = json.dumps(type(content).to_dict(content))
                         content = json.loads(content)
                         content = content["args"]
```

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.2.3/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.2.3/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.2.3/AIBridge/ai_services/openai_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,14 @@
                             else response.choices[0].message.function_call.arguments
                         ),
                     }
                 )
                 tokens = response.usage.total_tokens
                 token_used = token_used + tokens
                 for res in response.choices:
-                    index = response.choices.index(res)
                     content = (
                         res.message.content
                         if res.message.content
                         else res.message.function_call.arguments
                     )
                     if output_format:
                         try:
```

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.2.3/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.2.3/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.2.3/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/constant/constant.py` & `aibridge_test-0.2.3/AIBridge/constant/constant.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 AI_SERVICES = [
     "open_ai",
     "palm_api",
     "stable_diffusion",
     "cohere_api",
     "ai21_api",
     "gemini_ai",
+    "anthropic",
 ]
 DB_TYPES = ["sql", "nosql"]
 CUSTOM_CONFIG_PATH = "AIBRIDGE_CONFIG"
 LINUX_MACOS_PATH = "/etc/aibridge/aibridge_config.yaml"
 OPENAI_IMAGE_TYPE = ["create", "variation", "edit"]
 OPENAI_IMAGE_SIZES = ["256x256", "512x512", "1024x1024"]
 STABLE_DIFFUSION_TYPES = [
```

### Comparing `aibridge_test-0.2.2/AIBridge/database/db_layer.py` & `aibridge_test-0.2.3/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/database/no_sql_service.py` & `aibridge_test-0.2.3/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/database/session.py` & `aibridge_test-0.2.3/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/database/sql_service.py` & `aibridge_test-0.2.3/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/exceptions.py` & `aibridge_test-0.2.3/AIBridge/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,7 +69,11 @@
 
 class Ai21Exception(AIBridgeException):
     pass
 
 
 class GeminiException(AIBridgeException):
     pass
+
+
+class AnthropicsException(AIBridgeException):
+    pass
```

### Comparing `aibridge_test-0.2.2/AIBridge/output_validation/convertors.py` & `aibridge_test-0.2.3/AIBridge/output_validation/convertors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import csv
 import xmltodict
 import io
+import re
 
 
 class IntoJson:
     @classmethod
     def csv_to_json(self, csv_data):
         csv_data = csv_data.replace("\n", "")
         csv_list = csv_data.split(",")
@@ -18,15 +19,17 @@
 
     @classmethod
     def xml_to_json(self, xml_data):
         if """<?xml version="1.0" encoding="UTF-8"?>""" in xml_data:
             xml_data = xml_data.replace(
                 """<?xml version="1.0" encoding="UTF-8"?>""", ""
             )
-        json_data = xmltodict.parse(xml_data)
+
+        cleaned_xml_data = re.sub(r"^.*?(<[^>]*>)", r"\1", xml_data, flags=re.DOTALL)
+        json_data = xmltodict.parse(cleaned_xml_data)
         new_json = {}
         for key, value in json_data.items():
             new_json[key] = [value]
             break
         return new_json
```

### Comparing `aibridge_test-0.2.2/AIBridge/output_validation/validations.py` & `aibridge_test-0.2.3/AIBridge/output_validation/validations.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,34 @@
 class Validation(ABC):
     @abstractmethod
     def validate(self, output_string, schema):
         pass
 
 
 class JsonSchema(Validation):
+    @classmethod
+    def compare_dict_types(self, dict1, dict2):
+        if len(dict1) != len(dict2):
+            return False
+        for k1, v1 in dict1.items():
+            if k1 not in dict2:
+                return False
+            v2 = dict2[k1]
+            if not isinstance(v1, type(v2)):
+                return False
+            if isinstance(v1, dict) and isinstance(v2, dict):
+                if not self.compare_dict_types(v1, v2):
+                    return False
+            elif not isinstance(v1, type(v2)):
+                return False
+        return True
+
     def validate(self, output_string, schema=None):
         try:
+            print(schema, type(schema))
             json_data = output_string
             if type(output_string) != dict:
                 if "}" not in output_string:
                     output_string += '"}'
                     output_string = output_string + "}"
                 json_string = output_string[
                     output_string.index("{") : len(output_string)
@@ -33,19 +51,15 @@
         except json.JSONDecodeError as e:
             raise AIBridgeException(f" Error in the AI output for the validation->{e}")
         if schema:
             try:
                 user_schema = json.loads(schema)
             except AIBridgeException as e:
                 raise JSONDecodeError(f"Error in the schema you entred {e}")
-            try:
-                jsonschema.Draft7Validator.check_schema(user_schema)
-                jsonschema.Draft7Validator.check_schema(json_data)
-            except jsonschema.exceptions.SchemaError as e:
-                raise ValidationException(f"Invalid output JSON schema: {e}")
+            self.compare_dict_types(user_schema, json_data)
         return json.dumps(json_data)
 
 
 class CSVSchema(Validation):
     def validate(self, output_string, schema=None):
         try:
             output_schema = []
```

### Comparing `aibridge_test-0.2.2/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.2.3/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.2.3/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.2.3/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.2.3/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.2.3/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.2.3/AIBridge/queue_integration/response_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,33 @@
             stop_subsequence=message_data["stop_subsequence"],
             stream=message_data["stream"],
             context=message_data["context"],
         )
         return data
 
 
+class AnthropicRes(Caller):
+    @classmethod
+    def get_response(self, service_obj, message_data):
+        data = service_obj.get_response(
+            prompts=json.loads(message_data["prompts"]),
+            model=message_data["model"],
+            variation_count=message_data["variation_count"],
+            max_tokens=message_data["max_tokens"],
+            temperature=message_data["temperature"],
+            output_format=message_data["output_format"],
+            format_structure=message_data["format_structure"],
+            api_key=message_data["api_key"],
+            stop_subsequence=message_data["stop_subsequence"],
+            stream=message_data["stream"],
+            context=message_data["context"],
+        )
+        return data
+
+
 class OpenAiImageRes(Caller):
     @classmethod
     def get_response(self, service_obj, message_data):
         data = service_obj.get_response(
             prompts=json.loads(message_data["prompts"]),
             image_data=json.loads(message_data["image_data"]),
             mask_image=json.loads(message_data["mask_image"]),
```

### Comparing `aibridge_test-0.2.2/AIBridge/setconfig.py` & `aibridge_test-0.2.3/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/LICENSE` & `aibridge_test-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/PKG-INFO` & `aibridge_test-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -24,14 +24,15 @@
 Requires-Dist: sqlparse>=0.4.4
 Requires-Dist: jsonschema>=4.18.4
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: google-generativeai>=0.4.1
 Requires-Dist: cohere>=4.24
 Requires-Dist: ai21>=1.2.8
 Requires-Dist: xmltodict>=0.13.0
+Requires-Dist: anthropic>=0.21.3
 
 
 ## AIBridge 0.0.1
 
 AIBridge is the python package with the support of the Multiple LLM's,User can utilised the Formatters ,prompts, varibales to get most of the LLM's Through the AIBridge
 
 ### Requirement
```

### Comparing `aibridge_test-0.2.2/README.md` & `aibridge_test-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.2/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.2.3/aibridge_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -24,14 +24,15 @@
 Requires-Dist: sqlparse>=0.4.4
 Requires-Dist: jsonschema>=4.18.4
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: google-generativeai>=0.4.1
 Requires-Dist: cohere>=4.24
 Requires-Dist: ai21>=1.2.8
 Requires-Dist: xmltodict>=0.13.0
+Requires-Dist: anthropic>=0.21.3
 
 
 ## AIBridge 0.0.1
 
 AIBridge is the python package with the support of the Multiple LLM's,User can utilised the Formatters ,prompts, varibales to get most of the LLM's Through the AIBridge
 
 ### Requirement
```

### Comparing `aibridge_test-0.2.2/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.2.3/aibridge_test.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 AIBridge/__init__.py
 AIBridge/exceptions.py
 AIBridge/setconfig.py
 AIBridge/ai_services/__init__.py
 AIBridge/ai_services/ai21labs_text.py
 AIBridge/ai_services/ai_abstraction.py
 AIBridge/ai_services/ai_services_response.py
+AIBridge/ai_services/anthropic_ai.py
 AIBridge/ai_services/cohere_llm.py
 AIBridge/ai_services/geminin_services.py
 AIBridge/ai_services/image_optimisaton.py
 AIBridge/ai_services/openai_images.py
 AIBridge/ai_services/openai_services.py
 AIBridge/ai_services/palm_chat.py
 AIBridge/ai_services/palm_text.py
```

### Comparing `aibridge_test-0.2.2/setup.py` & `aibridge_test-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
     "sqlparse>=0.4.4",
     "jsonschema>=4.18.4",
     "Pillow>=10.0.0",
     "google-generativeai>=0.4.1",
     "cohere>=4.24",
     "ai21>=1.2.8",
     "xmltodict>=0.13.0",
+    "anthropic>=0.21.3",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
```

