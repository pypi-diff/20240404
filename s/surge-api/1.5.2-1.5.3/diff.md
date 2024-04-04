# Comparing `tmp/surge_api-1.5.2-py3-none-any.whl.zip` & `tmp/surge_api-1.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18180 bytes, number of entries: 16
--rw-r--r--  2.0 unx      260 b- defN 24-Apr-01 21:14 surge/__init__.py
--rw-r--r--  2.0 unx     3066 b- defN 24-Mar-29 01:22 surge/api_resource.py
--rw-r--r--  2.0 unx      949 b- defN 23-Nov-30 19:24 surge/carousel.py
--rw-r--r--  2.0 unx     1606 b- defN 23-Jun-19 05:11 surge/errors.py
--rw-r--r--  2.0 unx    13792 b- defN 24-Mar-29 01:22 surge/projects.py
--rw-r--r--  2.0 unx    27971 b- defN 24-Mar-29 01:22 surge/questions.py
--rw-r--r--  2.0 unx     5481 b- defN 24-Mar-29 01:22 surge/reports.py
--rw-r--r--  2.0 unx      939 b- defN 23-Jun-19 05:11 surge/responses.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Mar-29 01:22 surge/tasks.py
--rw-r--r--  2.0 unx     4373 b- defN 24-Mar-29 01:22 surge/teams.py
--rw-r--r--  2.0 unx      442 b- defN 23-Jun-19 05:11 surge/utils.py
--rw-r--r--  2.0 unx     1062 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4402 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/RECORD
-16 files, 71695 bytes uncompressed, 16242 bytes compressed:  77.3%
+Zip file size: 18679 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      260 b- defN 24-Mar-13 18:58 surge/__init__.py
+-rw-r--r--  2.0 unx     3363 b- defN 24-Apr-04 21:46 surge/api_resource.py
+-rw-r--r--  2.0 unx      949 b- defN 24-Mar-13 18:58 surge/carousel.py
+-rw-r--r--  2.0 unx     1606 b- defN 24-Mar-13 18:58 surge/errors.py
+-rw-r--r--  2.0 unx    14523 b- defN 24-Apr-04 21:46 surge/projects.py
+-rw-r--r--  2.0 unx    32290 b- defN 24-Apr-04 21:46 surge/questions.py
+-rw-r--r--  2.0 unx     5551 b- defN 24-Apr-04 21:46 surge/reports.py
+-rw-r--r--  2.0 unx      939 b- defN 24-Mar-13 18:58 surge/responses.py
+-rw-r--r--  2.0 unx     6185 b- defN 24-Apr-04 21:46 surge/tasks.py
+-rw-r--r--  2.0 unx     4433 b- defN 24-Apr-04 21:46 surge/teams.py
+-rw-r--r--  2.0 unx      442 b- defN 24-Mar-13 18:58 surge/utils.py
+-rw-r--r--  2.0 unx     1062 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4402 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/RECORD
+16 files, 77304 bytes uncompressed, 16741 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: surge/teams.py
 Comment: 
 
 Filename: surge/utils.py
 Comment: 
 
-Filename: surge_api-1.5.2.dist-info/LICENSE
+Filename: surge_api-1.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: surge_api-1.5.2.dist-info/METADATA
+Filename: surge_api-1.5.3.dist-info/METADATA
 Comment: 
 
-Filename: surge_api-1.5.2.dist-info/WHEEL
+Filename: surge_api-1.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: surge_api-1.5.2.dist-info/top_level.txt
+Filename: surge_api-1.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: surge_api-1.5.2.dist-info/RECORD
+Filename: surge_api-1.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## surge/api_resource.py

```diff
@@ -71,23 +71,32 @@
         except Exception:
             # Generic exception handling
             raise SurgeRequestError
 
     @classmethod
     def get(cls, api_endpoint, params=None, api_key=None):
         method = "get"
-        return cls._base_request(method, api_endpoint, params=params, api_key=api_key)
+        return cls._base_request(method,
+                                 api_endpoint,
+                                 params=params,
+                                 api_key=api_key)
 
     @classmethod
     def post(cls, api_endpoint, params=None, api_key=None):
         method = "post"
-        return cls._base_request(method, api_endpoint, params=params, api_key=api_key)
+        return cls._base_request(method,
+                                 api_endpoint,
+                                 params=params,
+                                 api_key=api_key)
 
     @classmethod
     def put(cls, api_endpoint, params=None, api_key=None):
         method = "put"
-        return cls._base_request(method, api_endpoint, params=params, api_key=api_key)
+        return cls._base_request(method,
+                                 api_endpoint,
+                                 params=params,
+                                 api_key=api_key)
 
     @classmethod
     def delete_request(cls, api_endpoint, api_key=None):
         method = "delete"
         return cls._base_request(method, api_endpoint, api_key=api_key)
```

## surge/projects.py

```diff
@@ -1,8 +1,10 @@
 import dateutil.parser
+import datetime
+import json
 
 from surge.errors import SurgeMissingIDError, SurgeProjectQuestionError, SurgeMissingAttributeError
 from surge.api_resource import PROJECTS_ENDPOINT, APIResource
 from surge.questions import Question
 from surge.tasks import Task
 from surge import utils
 
@@ -36,14 +38,31 @@
     def attrs_repr(self):
         return self.print_attrs(forbid_list=["name", "id"])
 
     def _convert_questions_to_objects(self, questions_data):
         return list(
             map(lambda params: Question.from_params(params), questions_data))
 
+    def to_dict(self):
+        return {
+            key: self._to_dict_value(key, value)
+            for key, value in self.__dict__.items() if not key.startswith('_')
+        }
+
+    def _to_dict_value(self, key, value):
+        if key == 'questions':
+            return [item.to_dict() for item in value if item]
+        elif isinstance(value, datetime.datetime):
+            return value.isoformat()
+        else:
+            return value
+
+    def to_json(self):
+        return json.dumps(self.to_dict())
+
     @staticmethod
     def _validate_questions(questions):
         # Convert list of question objects into dicts in valid json format
         # If this isn't a list of Question objects, throw an exception
         if not all(isinstance(q, Question) for q in questions):
             raise SurgeProjectQuestionError
 
@@ -244,29 +263,38 @@
 
         Returns:
             {"success": True}
         '''
         endpoint = f"{PROJECTS_ENDPOINT}/{self.id}/delete"
         return self.get(endpoint, api_key=api_key)
 
-    def list_tasks(self, page: int = 1, per_page: int = 100, api_key: str = None):
+    def list_tasks(self,
+                   page: int = 1,
+                   per_page: int = 100,
+                   api_key: str = None):
         '''
         Lists all tasks belonging to this project.
         Tasks are returned in ascending order of created_at.
         Each page contains a maximum of 25 tasks.
 
         Arguments:
             page (int, optional): Page number to retrieve. Pages start at 1 (default value).
 
         Returns:
             tasks (list): list of Task objects.
         '''
-        return Task.list(self.id, page=page, per_page=per_page, api_key=api_key)
-
-    def create_tasks(self, tasks_data: list, launch=False, api_key: str = None):
+        return Task.list(self.id,
+                         page=page,
+                         per_page=per_page,
+                         api_key=api_key)
+
+    def create_tasks(self,
+                     tasks_data: list,
+                     launch=False,
+                     api_key: str = None):
         '''
         Creates new Task objects for this project.
 
         Arguments:
             tasks_data (list): list of dicts that map each task field to its value
                 e.g. [{"website": "surgehq.ai"}, {"website":"twitch.tv"}]
```

## surge/questions.py

```diff
@@ -3,22 +3,35 @@
 
 
 class Question(APIResource):
 
     def __init__(self,
                  id,
                  text,
+                 label,
                  type_=None,
                  required=True,
-                 column_header=None):
+                 column_header=None,
+                 question_category=None):
         self.id = id
         self.text = text
+        self.label = label
         self.type = type_
         self.required = required
         self.column_header = column_header
+        self.question_category = question_category
+
+    def __str__(self):
+        return f"<surge.{self.__class__.__name__}#{self.id} label=\"{self.label}\">"
+
+    def __repr__(self):
+        return f"<surge.{self.__class__.__name__}#{self.id} {self.attrs_repr()}>"
+
+    def attrs_repr(self):
+        return self.print_attrs(forbid_list=["text", "id"])
 
     def to_dict(self):
         return self.__dict__
 
     def to_json(self):
         return json.dumps(self.to_dict())
 
@@ -29,111 +42,129 @@
             for info in options_info:
                 # We don't need to provide created_at / updated_at.
                 info.pop("created_at", None)
                 info.pop("updated_at", None)
         if q["type"] == "free_response":
             return FreeResponseQuestion(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 required=q["required"],
                 preexisting_annotations=q["preexisting_annotations"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
         elif q["type"] == "multiple_choice":
             return MultipleChoiceQuestion(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 options=q["options"],
                 options_info=options_info,
                 required=q["required"],
                 preexisting_annotations=q["preexisting_annotations"],
                 require_tiebreaker=q["require_tie_breaker"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
 
         elif q["type"] == "checkbox":
             return CheckboxQuestion(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 options=q["options"],
                 options_info=options_info,
                 required=q["required"],
                 preexisting_annotations=q["preexisting_annotations"],
                 require_tiebreaker=q["require_tie_breaker"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
         elif q["type"] == "text_tagging":
             return TextTaggingQuestion(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 required=q["required"],
                 options=q["options"],
                 options_info=options_info,
                 preexisting_annotations=q["preexisting_annotations"],
                 token_granularity=q["ner_token_granularity"],
                 allow_relationship_tags=q["ner_allow_relationship_tags"],
                 allow_overlapping_tags=q["ner_allow_overlapping_tags"],
                 require_tiebreaker=q["require_tie_breaker"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
 
         elif q["type"] == "tree_selection":
             return TreeSelectionQuestion(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 options=q["options"],
                 options_info=options_info,
                 required=q["required"],
                 preexisting_annotations=q["preexisting_annotations"],
                 require_tiebreaker=q["require_tie_breaker"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
         elif q["type"] == "ranking":
             return RankingQuestion(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 options=q["options"],
                 options_info=options_info,
                 required=q["required"],
                 preexisting_annotations=q["preexisting_annotations"],
                 allow_ranking_ties=q["allow_ranking_ties"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
         elif q["type"] == "file_upload":
             return FileUpload(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 required=q["required"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
         elif q["type"] == "text":
             return TextArea(q["text"],
+                            q["label"],
                             id=q["id"],
                             shown_by_option_id=q["shown_by_item_option_id"],
                             hidden_by_option_id=q["hidden_by_item_option_id"],
-                            holistic=q["holistic"])
+                            holistic=q["holistic"],
+                            question_category=q.get("question_category"))
         elif q["type"] == "chat":
             return ChatBot(
                 q["text"],
+                q["label"],
                 id=q["id"],
                 options=q["options"],
                 options_info=options_info,
                 endpoint_url=q["endpoint_url"],
                 endpoint_headers=q["endpoint_headers"],
                 preexisting_annotations=q["preexisting_annotations"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
-                holistic=q["holistic"])
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
 
     def update(self,
                text: str = None,
                hidden_by_option_id: str = None,
                shown_by_option_id: str = None,
                api_key: str = None):
         params = {}
@@ -150,189 +181,213 @@
         return Question.from_params(response_json)
 
 
 class FreeResponseQuestion(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  required=True,
                  preexisting_annotations=None,
                  use_for_serial_collection=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create a free response question.
 
         Args:
             text (string): Required. The instructions above the free text box, e.g. "Please explain your reasoning".
+            label (string): Required. The label of the question being asked, e.g. "Overall Quality: Model A"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             required (boolean): Defaults to true. Whether or not workers must fill out this question before moving on to the next task.
             preexisting_annotations (string): You can use preexisting annotations to prepopulate text box an option specified in the task data.
                 The preexisting_annotations param should contain the task data key you are loading the default values from.
             use_for_serial_collection (boolean): Deprecated in favor of carousel. The free response question will not be shown to the user,
                 but will rather be used to collect the responses to a number of other items as a JSON string.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="free_response",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.preexisting_annotations = preexisting_annotations
         self.use_for_serial_collection = use_for_serial_collection
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class MultipleChoiceQuestion(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  options=[],
                  options_info=None,
                  descriptions=[],
                  required=True,
                  preexisting_annotations=None,
                  require_tiebreaker=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create a multiple choice radio question.
 
         Args:
             text (string): Required. The text of the question being asked, e.g. "Is the sentiment of this text positive or negative?"
+            label (string): Required. The label of the question being asked, e.g. "Overall Quality: Model A"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             options (list of strings): Required. A list of the options for the radios, e.g. ["Yes", "No"].
             options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
             descriptions(list of strings): Tooltip text for the options. This should have the same length as the options.
                 You can substitute in empty strings if one option doesn't have a tooltip.
             required (boolean): Defaults to true. Whether or not workers must fill out this question before moving on to the next task.
             preexisting_annotations (string): You can use preexisting annotations to prepopulate the radio selection with an option specified in the task data.
                 The preexisting_annotations param should contain the task data key you are loading the default values from.
             require_tiebreaker (boolean): If set to true, more workers will be assigned to this task if fewer than 50% agree on an answer.
                 For example, imagine you are using two workers per task. If one selects Option A and the second one selections Option B a third will be assigned to the task to break the tie.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="multiple_choice",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.descriptions = descriptions
         self.preexisting_annotations = preexisting_annotations
         self.require_tiebreaker = require_tiebreaker
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class CheckboxQuestion(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  options=[],
                  options_info=None,
                  descriptions=[],
                  required=True,
                  preexisting_annotations=None,
                  require_tiebreaker=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create a checkbox question. Unlike a multiple choice question, it's possible to select multiple checkboxes.
 
         Args:
             text (string): Required. The text of the question being asked, e.g. "Check all the apply."
+            label (string): Required. The label of the question being asked, e.g. "Model A - Factuality"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             options (list of strings): Required. A list of the options for the checkboxes.
             options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
             descriptions(list of strings): Tooltip text for the options. This should have the same length as the options.
                 You can substitute in empty strings if one option doesn't have a tooltip.
             required (boolean): Defaults to true. Whether or not workers must fill out this question before moving on to the next task.
             preexisting_annotations (string): You can use preexisting annotations to prepopulate the checkboxes with an options specified in the task data.
                 The preexisting_annotations param should contain the task data key you are loading the default values from.
             require_tiebreaker (boolean): If set to true, more workers will be assigned to this task if fewer than 50% agree on an answer.
                 For example, imagine you are using two workers per task. If one selects Option A and the second one selections Option B a third will be assigned to the task to break the tie.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="checkbox",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.descriptions = descriptions
         self.preexisting_annotations = preexisting_annotations
         self.require_tiebreaker = require_tiebreaker
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class TextTaggingQuestion(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  options=[],
                  options_info=None,
                  required=True,
                  preexisting_annotations=None,
                  token_granularity=True,
                  allow_relationship_tags=False,
                  allow_overlapping_tags=False,
                  require_tiebreaker=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create a text tagging (NER) question. Unlikely a multiple choice question, it's possible to select multiple checkboxes
 
         Args:
             text (string): Required. The text that needs to be tagged.
+            label (string): Required. "Model A - tags"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             required (boolean): If true, worker must tag at least element.
             options (list of strings): Required. A list of tags that can be used to tag spans of text, e.g. ["Person", "Place"].
             options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
             preexisting_annotations (string): You can use preexisting annotations to prepopulate the named entity tagger. This must contain serialized JSON data
                 in the same format outputted by the text tagging tool.
             token_granularity (boolean): If set to true, spans will snap to the nearest word to prevent workers from accidentally tagging parts of words.
             allow_relationship_tags (boolean): If true, enable relationship tagging.
             allow_overlapping_tags (boolean): If true, allow multiple tags to be assigned to the same span of text.
             require_tiebreaker (boolean): If set to true, more workers will be assigned to this task if fewer than 50% agree on an answer.
                 Workers must have the exact same set of tags to be considered in agreement.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="text_tagging",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.preexisting_annotations = preexisting_annotations
         self.token_granularity = token_granularity
         self.allow_relationship_tags = allow_relationship_tags
         self.allow_overlapping_tags = allow_overlapping_tags
         self.require_tiebreaker = require_tiebreaker
@@ -341,183 +396,214 @@
         self.holistic = holistic
 
 
 class TreeSelectionQuestion(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  options=[],
                  options_info=None,
                  descriptions=[],
                  required=True,
                  preexisting_annotations=None,
                  require_tiebreaker=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create a hierarchical multiple choice question. This is useful if you have a lot of options in a nested format.
 
         Args:
             text (string): Required. The text of the question being asked, e.g. "Which category does this example belong to?"
+            label (string): Required. The label of the question being asked, e.g. "Prompt Category"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             options (list of strings): Required. A list of the options for the tree. Each level of hierarchy should be separate by a " / ".
                 For example, one valid set of options would be ["1A / 2A", "1A / 2B", "1B / 2C", "1B / 2D"].
             options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
             descriptions(list of strings): Tooltip text for the options. This should have the same length as the options.
                 You can substitute in empty strings if one option doesn't have a tooltip.
             required (boolean): Defaults to true. Whether or not workers must fill out this question before moving on to the next task.
             preexisting_annotations (string): You can use preexisting annotations to prepopulate the radio selection with an option specified in the task data.
                 The preexisting_annotations param should contain the task data key you are loading the default values from.
             require_tiebreaker (boolean): If set to true, more workers will be assigned to this task if fewer than 50% agree on an answer.
                 For example, imagine you are using two workers per task. If one selects Option A and the second one selections Option B a third will be assigned to the task to break the tie.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="tree_selection",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.descriptions = descriptions
         self.preexisting_annotations = preexisting_annotations
         self.require_tiebreaker = require_tiebreaker
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class FileUpload(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  required=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Add a file upload widget where workers can upload images, documents, or other files.
 
         Args:
             text (string): This text will appear above the file upload and can be used to specify any instructions.
+            label (string): Required. The label of the question being asked, e.g. "Overall Quality: Model A"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             required (boolean): If true, Surgers will be required to upload a file before moving on to the next task.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="file_upload",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class RankingQuestion(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  options=[],
                  options_info=None,
                  required=False,
                  preexisting_annotations=None,
                  allow_ranking_ties=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create a ranking widget. Workers can drag and drop the option to specify their ranking.
 
         Args:
             required (boolean): If true, worker must rank at least one element.
             text (string): Required. The text of the question being asked, e.g. "Please rank these search results from best to worst"
+            label (string): Required. The label of the question being asked, e.g. "Overall Quality: Model A"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             options (list of strings): Required. A list of the options being ranked.
             options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
             preexisting_annotations (string): You can use preexisting annotations to prepopulate the named entity tagger.
                 This must contain serialized data in the same format outputted by the ranking tool.
             allow_ranking_ties (boolean): Optional. Whether or not to allow ties in the ranking. If ties are allowed, two options can be ranked in the same group.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="ranking",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.allow_ranking_ties = allow_ranking_ties
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class ChatBot(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  options=[],
                  options_info=None,
                  endpoint_url=None,
                  endpoint_headers=None,
                  preexisting_annotations=None,
                  required=False,
                  column_header=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
+                 holistic=False,
+                 question_category=None):
         '''
         Create an interactive chatbot on the labeling page. This is an advanced item type.
 
         Args:
             text (string): This text will appear above the chatbot and can be used to specify any instructions.
+            label (string): Required. The label of the question being asked, e.g. "Overall Quality: Model A"
             id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
             options (list of strings): Options for rating chatbot responses.
             options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
             endpoint_url (string): A URL to send chat responses to. It must include a "text" field in its response.
             endpoint_headers (string): Please provide a JSON string with any headers that need to be set when calling this URL.
             column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
             hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
             shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
         '''
         super().__init__(id,
                          text,
+                         label,
                          type_="chat",
                          required=required,
-                         column_header=column_header)
+                         column_header=column_header,
+                         question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.endpoint_url = endpoint_url
         self.endpoint_headers = endpoint_headers
         self.preexisting_annotations = preexisting_annotations
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class TextArea(Question):
 
     def __init__(self,
                  text,
+                 label,
                  id=None,
                  hidden_by_option_id=None,
                  shown_by_option_id=None,
-                 holistic=False):
-        super().__init__(id, text, type_="text", required=False)
+                 holistic=False,
+                 question_category=None):
+        super().__init__(id,
+                         text,
+                         label,
+                         type_="text",
+                         required=False,
+                         question_category=question_category)
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
```

## surge/reports.py

```diff
@@ -40,15 +40,17 @@
           * `export_csv`
           * `export_csv_aggregated`
           * `export_csv_flattened`
         filepath (string or None): Location to save the results file. If not specified, will save to "project_{project_id}_results.{csv/json}
         poll_time (int): Number of seconds to poll for the report
       '''
         for _ in range(poll_time // 2):
-            response = cls.request(project_id=project_id, type=type, api_key=api_key)
+            response = cls.request(project_id=project_id,
+                                   type=type,
+                                   api_key=api_key)
             # Download zipped project results if ready
             if response.status == "READY":
                 file_ext = "csv" if "csv" in type else "json"
                 default_file_name = "project_{project_id}_results.{file_ext}.gzip".format(
                     project_id=project_id, file_ext=file_ext)
                 with urllib.request.urlopen(response.url) as response:
                     with tempfile.NamedTemporaryFile() as tmp_file:
```

## surge/tasks.py

```diff
@@ -94,15 +94,19 @@
         '''
         endpoint = f"{PROJECTS_ENDPOINT}/{project_id}/{TASKS_ENDPOINT}"
         data = {"fields": params}
         response_json = cls.post(endpoint, data, api_key=api_key)
         return cls(**response_json)
 
     @classmethod
-    def create_many(cls, project_id: str, tasks_data: list, launch: bool, api_key: str = None):
+    def create_many(cls,
+                    project_id: str,
+                    tasks_data: list,
+                    launch: bool,
+                    api_key: str = None):
         '''
         Creates new Task objects for a given project.
 
         Arguments:
             project_id (str): ID of the project to which the tasks are added.
             tasks_data (list): list of dicts that map each task field to its value.
                 e.g. [{"website": "surgehq.ai"}, {"website":"twitch.tv"}]
@@ -119,15 +123,19 @@
         endpoint = f"{PROJECTS_ENDPOINT}/{project_id}/{TASKS_ENDPOINT}/create_tasks"
         data = {"tasks": tasks_data, "launch": launch}
         response_json = cls.post(endpoint, data, api_key=api_key)
         tasks = [cls(**task_json) for task_json in response_json]
         return tasks
 
     @classmethod
-    def list(cls, project_id: str, page: int = 1, per_page: int = 100, api_key: str = None):
+    def list(cls,
+             project_id: str,
+             page: int = 1,
+             per_page: int = 100,
+             api_key: str = None):
         '''
         Lists all tasks belonging to a given project.
         Tasks are returned in ascending order of created_at.
         Each page contains a maximum of 25 tasks.
 
         Arguments:
             project_id (str): ID of project.
```

## surge/teams.py

```diff
@@ -79,15 +79,19 @@
         '''
         endpoint = f"{TEAMS_ENDPOINT}/{self.id}/remove_surgers"
         params = {"surger_ids": surger_ids}
         response_json = self.post(endpoint, params, api_key=api_key)
         return Team(**response_json)
 
     @classmethod
-    def create(cls, name: str, members: list, description=None, api_key: str = None):
+    def create(cls,
+               name: str,
+               members: list,
+               description=None,
+               api_key: str = None):
         '''
         Creates a new Team.
 
         Arguments:
             name (str): Team name.
             members (list): List of user IDs to add to the team.
             description (str): Optional, team description.
```

## Comparing `surge_api-1.5.2.dist-info/LICENSE` & `surge_api-1.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `surge_api-1.5.2.dist-info/METADATA` & `surge_api-1.5.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surge-api
-Version: 1.5.2
+Version: 1.5.3
 Summary: Surge Python SDK
 Home-page: https://github.com/surge-ai/surge-python
 Author: Surge
 Author-email: team@surgehq.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `surge_api-1.5.2.dist-info/RECORD` & `surge_api-1.5.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 surge/__init__.py,sha256=EbBXghvhL6SxEURWh2-92f0oM9vsw0sG3C82fHCI_ko,260
-surge/api_resource.py,sha256=CWoRluTsaBfjP4LakN4Au0wiq7MkEJQd33MMRZXaeFY,3066
+surge/api_resource.py,sha256=m89DCbbEo4zdLtoa5tUo1cg2RFGRCnuK5YTAC-KfEVI,3363
 surge/carousel.py,sha256=ZCYGVsgd8G2u-goTB49RuzbknV-s3v7hYgr9jQVYtv8,949
 surge/errors.py,sha256=N83WpLlqrRi_Y03-q8JUXlutgCUpUrMeL47TvbOv11c,1606
-surge/projects.py,sha256=X2iD67DRkaViGe6Mv5p169Rl5dQL_UyP7Bp8k5POzdA,13792
-surge/questions.py,sha256=0xNhWUIMJ3eJGLHrbL-tM3q2P37fydjxL0pTh1Umq98,27971
-surge/reports.py,sha256=BgbbcCEXF7haGBgZkdws2tRxnq8bwl1IJtdGAFgjwj4,5481
+surge/projects.py,sha256=y7uK5pLsf4EnJD9BCIhb9N-aZPcKXmIMGw5iMLmEuVI,14523
+surge/questions.py,sha256=gqs1C2gy3JXSUqzqknbDHH4QISS7-3f-XBVGwKp-Tio,32290
+surge/reports.py,sha256=pbBtaV3-MBvmZ8-FFpl2s9WY_LOakYhUtAdr43Nx1WE,5551
 surge/responses.py,sha256=uQIQj55KS2H334OBXIe59FFEerOnDuqk0MhTTUye-D4,939
-surge/tasks.py,sha256=Tpk5azp4qMwICc9RkUX-Cvdnljv1JmL7DHZxPlJGvP8,6053
-surge/teams.py,sha256=kH4_za61bwsJxwrM-N7kBd7bojiazuDOt-Auk3e3aYU,4373
+surge/tasks.py,sha256=sy8OU1Qh2Q504eEw7zC9PSmIs8sQARAysb4cURhNyp4,6185
+surge/teams.py,sha256=GbmonLJ_44UeG4Fr4KBGu9-pBgZPI_I1ovwyFnTC1po,4433
 surge/utils.py,sha256=4SO3vQVwOOgn-mrDFmUH0HipfRJwcU8v5eTXp4uoZag,442
-surge_api-1.5.2.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
-surge_api-1.5.2.dist-info/METADATA,sha256=-Cr5jvqLlshkKAcaAz0S8ETwWnvVUt7xjnsHl9NRoJ0,4402
-surge_api-1.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-surge_api-1.5.2.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
-surge_api-1.5.2.dist-info/RECORD,,
+surge_api-1.5.3.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
+surge_api-1.5.3.dist-info/METADATA,sha256=PnkIMq1KPmmtZ-187v7p4fiEsz-g3WIZIZ5lIxQHvxw,4402
+surge_api-1.5.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+surge_api-1.5.3.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
+surge_api-1.5.3.dist-info/RECORD,,
```

