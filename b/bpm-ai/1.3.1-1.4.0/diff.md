# Comparing `tmp/bpm_ai-1.3.1.tar.gz` & `tmp/bpm_ai-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.3.1.tar", max compression
+gzip compressed data, was "bpm_ai-1.4.0.tar", max compression
```

## Comparing `bpm_ai-1.3.1.tar` & `bpm_ai-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      932 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      143 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1034 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1509 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3575 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      738 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     3316 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     3385 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     4082 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     1986 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7210 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      616 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1486 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      160 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/schema.py
--rw-r--r--   0        0        0      576 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     3004 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0     1407 2024-04-04 10:58:06.146568 bpm_ai-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 bpm_ai-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      932 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1034 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1509 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     3575 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      738 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     3385 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     4082 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     1986 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-04 14:00:11.649153 bpm_ai-1.4.0/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     7294 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0     1486 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/translate/schema.py
+-rw-r--r--   0        0        0      576 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0     3004 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0     1407 2024-04-04 14:00:11.653153 bpm_ai-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 bpm_ai-1.4.0/PKG-INFO
```

### Comparing `bpm_ai-1.3.1/README.md` & `bpm_ai-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/common/multimodal.py` & `bpm_ai-1.4.0/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.4.0/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.4.0/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/compose/compose.py` & `bpm_ai-1.4.0/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/compose/util.py` & `bpm_ai-1.4.0/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.4.0/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.4.0/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/decide/decide.py` & `bpm_ai-1.4.0/bpm_ai/decide/decide.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/decide/schema.py` & `bpm_ai-1.4.0/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.4.0/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.4.0/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/extract/extract.py` & `bpm_ai-1.4.0/bpm_ai/extract/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import itertools
 import re
 from typing import Callable, Any
 
 from bpm_ai_core.classification.zero_shot_classifier import ZeroShotClassifier
+from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.token_classification.zero_shot_token_classifier import ZeroShotTokenClassifier
 from bpm_ai_core.tracing.decorators import trace
+from bpm_ai_core.util.file import is_supported_img_file
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
+from bpm_ai.extract.util import merge_dicts, strip_non_numeric_chars, create_json_object
 
 
 @trace("bpm-ai-extract", ["llm"])
 async def extract_llm(
     llm: LLM,
     input_data: dict[str, str | dict | None],
     output_schema: dict[str, str | dict],
@@ -66,78 +70,63 @@
     return transform_result(message.content or {})
 
 
 @trace("bpm-ai-extract", ["extractive-qa"])
 async def extract_qa(
     qa: QuestionAnswering,
     classifier: ZeroShotClassifier,
-    token_classifier: ZeroShotTokenClassifier,
     input_data: dict[str, str | dict | None],
     output_schema: dict[str, str | dict],
     multiple: bool = False,
     multiple_description: str = "",
     ocr: OCR | None = None,
+    vqa: QuestionAnswering | None = None,
+    token_classifier: ZeroShotTokenClassifier | None = None,
     asr: ASRModel | None = None
 ) -> dict | list[dict]:
     if all(value is None for value in input_data.values()):
         return input_data
 
-    input_data = await ocr_documents(input_data, ocr)
+    if vqa:
+        input_img_data = {k: v for k, v in input_data.items() if (isinstance(v, str) and is_supported_img_file(v))}
+        input_data = {k: v for k, v in input_data.items() if k not in input_img_data.keys()}
+    else:
+        input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
 
     if not output_schema:
         return input_data
 
     input_md = dict_to_md(input_data).strip()
     output_schema = expand_simplified_json_schema(output_schema)["properties"]
 
-    def strip_non_numeric_chars(s):
-        while len(s) > 0 and not s[0].isdigit():
-            s = s[1:]
-        while len(s) > 0 and not s[-1].isdigit():
-            s = s[:-1]
-        return s
-
-    async def create_json_object(target: str, schema, get_value: Callable, current_obj=None, root_obj=None, parent_key='', prefix=''):
-        if current_obj is None:
-            current_obj = {}
-            root_obj = {}
-
-        for name, properties in schema.items():
-            full_key = f'{parent_key}.{name}' if parent_key else name
-            if properties['type'] == 'object':
-                current_obj[name] = await create_json_object(target, properties['properties'], get_value, {}, root_obj, full_key)
-            else:
-                description = properties.get('description')
-                enum = properties.get('enum', None)
-                if prefix:
-                    description = prefix + (description[:1].lower() + description[1:])
-                value = await get_value(target, full_key, properties['type'], description, enum, root_obj)
-                current_obj[name] = value
-                root_obj[full_key] = value
-
-        return current_obj
-
     async def extract_value(text: str, field_name: str, field_type: str, description: str, enum: list, existing_values: dict) -> Any:
         """
         Extract value of type `field_type` from `text` based on `description`.
         `{}` placeholders in `description` will be formatted using `existing_values` dict which has flat dot notation keys
         (e.g. person.age if there is a person object with an age field).
         """
         if enum:
             # if an enum of values is given for the field, perform a classification instead of extraction
             return (await classifier.classify(text, enum)).max_label
 
         question = description + "?" if not description.endswith("?") else description
         question = question.format(**existing_values)
         question = question[:1].upper() + question[1:]  # capitalize first word
 
-        qa_result = await qa.answer(text, question, confidence_threshold=0.01)
+        if vqa and is_supported_img_file(text):
+            model = vqa
+            context = Blob.from_path_or_url(text)
+        else:
+            model = qa
+            context = text
+
+        qa_result = await model.answer(context, question, confidence_threshold=0.01 if not vqa else 0.1)
 
-        if qa_result is None:
+        if qa_result is None or qa_result.answer is None:
             return None
 
         if field_type == "integer":
             try:
                 return int(strip_non_numeric_chars(qa_result.answer))
             except ValueError:
                 return None
@@ -146,15 +135,24 @@
                 return float(strip_non_numeric_chars(qa_result.answer))
             except ValueError:
                 return None
         else:
             return qa_result.answer.strip(" .,;:!?")
 
     if not multiple:
-        return await create_json_object(input_md, output_schema, extract_value)
+        result_dict = await create_json_object(input_md, output_schema, extract_value)
+        if vqa:
+            img_result_dicts = [
+                await create_json_object(img, output_schema, extract_value) for img in input_img_data.values()
+            ]
+            # visual models can't process text and text models can't process documents, so if both modalities
+            # are present we use crude merging of multiple result dicts, giving precedence to visual results
+            return merge_dicts([result_dict], precedence_dicts=img_result_dicts)
+        else:
+            return result_dict
     else:
         if not multiple_description or multiple_description.isspace():
             raise MissingParameterError("Description for entity type is required.")
 
         result = await token_classifier.classify(input_md, classes=[multiple_description], confidence_threshold=0.75)
         entities = [s.word for s in result.spans]
```

### Comparing `bpm_ai-1.3.1/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.4.0/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.4.0/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/generic/generic.py` & `bpm_ai-1.4.0/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.4.0/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.4.0/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/bpm_ai/translate/translate.py` & `bpm_ai-1.4.0/bpm_ai/translate/translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.1/pyproject.toml` & `bpm_ai-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.3.1"
+version = "1.4.0"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai-1.3.1/PKG-INFO` & `bpm_ai-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.3.1
+Version: 1.4.0
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

