# Comparing `tmp/paperinquirer-0.0.7-py3-none-any.whl.zip` & `tmp/paperinquirer-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7533 bytes, number of entries: 11
+Zip file size: 6018 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      106 b- defN 24-Mar-08 17:05 paperinquierer/__init__.py
 -rw-r--r--  2.0 unx     3721 b- defN 24-Mar-08 08:33 paperinquierer/paperinquirer.py
 -rw-r--r--  2.0 unx      106 b- defN 24-Mar-08 17:05 paperinquirer/__init__.py
--rw-r--r--  2.0 unx     4516 b- defN 24-Mar-08 20:58 paperinquirer/paperinquirer.py
--rwxr-xr-x  2.0 unx      265 b- defN 24-Mar-08 18:40 paperinquirer-0.0.7.data/scripts/more_features.py
--rwxr-xr-x  2.0 unx      165 b- defN 24-Mar-08 18:40 paperinquirer-0.0.7.data/scripts/simple.py
--rw-r--r--  2.0 unx     1084 b- defN 24-Mar-09 00:21 paperinquirer-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6829 b- defN 24-Mar-09 00:21 paperinquirer-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-09 00:21 paperinquirer-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-09 00:21 paperinquirer-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      957 b- defN 24-Mar-09 00:21 paperinquirer-0.0.7.dist-info/RECORD
-11 files, 17855 bytes uncompressed, 5891 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     5322 b- defN 24-Mar-27 20:40 paperinquirer/paperinquirer.py
+-rwxr-xr-x  2.0 unx      227 b- defN 24-Mar-27 20:28 paperinquirer-0.0.9.data/scripts/more_features.py
+-rwxr-xr-x  2.0 unx      191 b- defN 24-Mar-27 20:28 paperinquirer-0.0.9.data/scripts/simple.py
+-rw-r--r--  2.0 unx     1084 b- defN 24-Apr-04 07:32 paperinquirer-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      665 b- defN 24-Apr-04 07:32 paperinquirer-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 07:32 paperinquirer-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-04 07:32 paperinquirer-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      956 b- defN 24-Apr-04 07:32 paperinquirer-0.0.9.dist-info/RECORD
+11 files, 12484 bytes uncompressed, 4376 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: paperinquirer/__init__.py
 Comment: 
 
 Filename: paperinquirer/paperinquirer.py
 Comment: 
 
-Filename: paperinquirer-0.0.7.data/scripts/more_features.py
+Filename: paperinquirer-0.0.9.data/scripts/more_features.py
 Comment: 
 
-Filename: paperinquirer-0.0.7.data/scripts/simple.py
+Filename: paperinquirer-0.0.9.data/scripts/simple.py
 Comment: 
 
-Filename: paperinquirer-0.0.7.dist-info/LICENSE
+Filename: paperinquirer-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: paperinquirer-0.0.7.dist-info/METADATA
+Filename: paperinquirer-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: paperinquirer-0.0.7.dist-info/WHEEL
+Filename: paperinquirer-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: paperinquirer-0.0.7.dist-info/top_level.txt
+Filename: paperinquirer-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: paperinquirer-0.0.7.dist-info/RECORD
+Filename: paperinquirer-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paperinquirer/paperinquirer.py

```diff
@@ -1,61 +1,87 @@
 import os
 from llama_index.core import (SimpleDirectoryReader, VectorStoreIndex, StorageContext, load_index_from_storage)
 from llama_index.core.tools import QueryEngineTool, ToolMetadata
 from llama_index.core.agent import ReActAgent
 from llama_index.llms.openai import OpenAI
 
 class PaperInquirer:
-    def __init__(self, pdf_dir, description_dir="", storage_dir=""):
+    def __init__(self, resource_dirs, storage_dir=""):
+        self._agent = None
         self.query_engine_tools = None
-        self.load(pdf_dir, description_dir, storage_dir)
+        self.file_list = []
+        self.load(resource_dirs, storage_dir)
 
-    def load(self, pdf_dir, description_dir="", storage_dir=""):
-        pdf_dir = self._get_valid_dir(pdf_dir)
-        if pdf_dir:
-            query_indices_info = self._create_query_indices_info(pdf_dir, description_dir, storage_dir)
-            query_engines_info = self._create_query_engines_info(query_indices_info)
-            self.query_engine_tools = self._create_query_engine_tools(query_engines_info)
+    def load(self, resource_dirs, storage_dir=""):
+        if not isinstance(resource_dirs, list):
+            resource_dirs = [resource_dirs]
+        query_indices_info = self._create_query_indices_info(resource_dirs, storage_dir)
+        query_engines_info = self._create_query_engines_info(query_indices_info)
+        self.query_engine_tools = self._create_query_engine_tools(query_engines_info)
 
     def inquire(self, question):
         response = ""
         if self.query_engine_tools is not None:
             agent = self._get_agent(self.query_engine_tools)
-            response = agent.chat(question)
+            response = agent.chat(self._embellish_question(question))
         else:
             raise ValueError("No query engine tools loaded")
         return str(response)
 
-    @staticmethod
-    def _get_agent(query_engine_tools):
-        llm = OpenAI(model="gpt-3.5-turbo-0613")
-        agent = ReActAgent.from_tools(
-            query_engine_tools,
-            llm=llm
-        )
-        return agent
-
-    def _create_query_indices_info(self, pdf_dir, description_dir, storage_dir):
-        indices_list =[]
-        for file in os.listdir(pdf_dir):
-            if file.endswith(".pdf"):
-                doc_index = self._load_index(storage_dir + file.split(".pdf")[0])
-                if doc_index is None:
-                    doc = SimpleDirectoryReader(
-                        input_files=[pdf_dir + file]
-                    ).load_data()
-                    doc_index = VectorStoreIndex.from_documents(doc)
-                    if storage_dir:
-                        storage_dir = self._get_valid_dir(storage_dir)
-                        doc_index.storage_context.persist(persist_dir=storage_dir + file.split(".pdf")[0])
-                doc_index_info = {'name': self._remove_hyphen(file.split(".pdf")[0]), 'index': doc_index,
-                                  'description': self._get_description_info(description_dir, file.split(".pdf")[0])}
-                indices_list.append(doc_index_info)
+    def _get_agent(self, query_engine_tools):
+        if self._agent is None:
+            llm = OpenAI(model="gpt-3.5-turbo-0613")
+            self._agent = ReActAgent.from_tools(
+                query_engine_tools,
+                llm=llm,
+                verbose=True
+            )
+
+        return self._agent
+
+    def _create_query_indices_info(self, resource_dirs, storage_dir):
+        indices_list = []
+        for resource_dir in resource_dirs:
+            resource_dir = self._get_valid_dir(resource_dir)
+            for file in os.listdir(resource_dir):
+                suffix = file.split(".")[-1]
+                if self.is_valid_suffix(suffix):
+                    self.file_list.append(file)
+                    doc_index = self._load_index(storage_dir + file.split("." + suffix)[0])
+                    if doc_index is None:
+                        doc = SimpleDirectoryReader(
+                            input_files=[resource_dir + file]
+                        ).load_data()
+                        doc_index = VectorStoreIndex.from_documents(doc)
+                        if storage_dir:
+                            storage_dir = self._get_valid_dir(storage_dir)
+                            doc_index.storage_context.persist(persist_dir=storage_dir + file.split("." + suffix)[0])
+                    doc_index_info = {'name': self.remove_space(self._remove_hyphen(file.split("." + suffix)[0])),
+                                      'index': doc_index}
+                    indices_list.append(doc_index_info)
+
         return indices_list
 
+    def _embellish_question(self, question):
+        embellished_question = ""
+        if len(self.file_list):
+            embellished_question += "You have to use "
+            for file_index in range(len(self.file_list)):
+                embellished_question += self.file_list[file_index].split(".")[0]
+                if file_index < len(self.file_list) - 1:
+                    if file_index == len(self.file_list) - 2:
+                        embellished_question += " and "
+                    else:
+                        embellished_question += ", "
+            embellished_question += " resources to answer the following question: " + question
+        else:
+            embellished_question = question
+
+        return embellished_question + " Think step by step."
+
     @staticmethod
     def _load_index(file_name):
         try:
             storage_context = StorageContext.from_defaults(
                 persist_dir=file_name
             )
             return load_index_from_storage(storage_context)
@@ -63,50 +89,46 @@
             return None
 
     @staticmethod
     def _create_query_engines_info(indices_info):
         engines_info_list = []
         for index_info in indices_info:
             engine = index_info['index'].as_query_engine(similarity_top_k=3)
-            engine_info = {'name': index_info['name'], 'description': index_info['description'], 'engine': engine}
+            engine_info = {'name': index_info['name'], 'engine': engine}
             engines_info_list.append(engine_info)
         return engines_info_list
 
     @staticmethod
     def _create_query_engine_tools(query_engines_info):
         tools_info_list = []
         for query_engine_info in query_engines_info:
             tools_info_list.append(
                 QueryEngineTool(
                     query_engine=query_engine_info['engine'],
                     metadata=ToolMetadata(
                     name=query_engine_info['name'],
-                    description=query_engine_info['description']
+                    description=query_engine_info['name']
                     ),
                 )
             )
         return tools_info_list
 
-    def _get_description_info(self, description_dir, file):
-        description_info = ""
-        if description_dir:
-            description_dir = self._get_valid_dir(description_dir)
-            abstract_file = description_dir + file + ".txt"
-            try:
-                with open(abstract_file, 'r') as file_name:
-                    return file_name.read()
-            except:
-                description_info = ""
-        return description_info
-
     @staticmethod
     def _get_valid_dir(directory):
         if not os.path.isdir(directory):
             raise ValueError(f'{directory} is not a directory')
             return ""
         if not directory.endswith(os.path.sep):
             directory += os.path.sep
         return directory
 
     @staticmethod
+    def is_valid_suffix(suffix):
+        return suffix in ["pdf", "txt", "sbml"]
+
+    @staticmethod
     def _remove_hyphen(file_name):
         return file_name.replace("-", "_")
+
+    @staticmethod
+    def remove_space(file_name):
+        return file_name.replace(" ", "_")
```

## Comparing `paperinquirer-0.0.7.dist-info/LICENSE` & `paperinquirer-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `paperinquirer-0.0.7.dist-info/RECORD` & `paperinquirer-0.0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 paperinquierer/__init__.py,sha256=lxDpvzFpwwUf5mgaCTQM6BtzaFizBO7UtXzvGR0sFT4,106
 paperinquierer/paperinquirer.py,sha256=DWQ24ojVvDizUjhiM1EHYZ10uXPsDWh1nq08iUu7K3I,3721
 paperinquirer/__init__.py,sha256=lxDpvzFpwwUf5mgaCTQM6BtzaFizBO7UtXzvGR0sFT4,106
-paperinquirer/paperinquirer.py,sha256=Y3eY18aK_H625nDDDGtj9tAm4sVQlj91Svg1linSVuY,4516
-paperinquirer-0.0.7.data/scripts/more_features.py,sha256=Y7G-TTDzLaysLx5t506PfBuzjrIfmuv9OmzTENFscbI,265
-paperinquirer-0.0.7.data/scripts/simple.py,sha256=PQ3rGpamOYYSNLu0kLWtXWWHlz4QV7bli4WotQP_2a8,165
-paperinquirer-0.0.7.dist-info/LICENSE,sha256=gGnkw4gXz_FZnTTWOhvH4kGG_w3jDFAHlIE8ESRa-b4,1084
-paperinquirer-0.0.7.dist-info/METADATA,sha256=AMQwFBNFbXxuK6wEEv_2PW5UJ7_P1CPgokAPQxB26Zg,6829
-paperinquirer-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-paperinquirer-0.0.7.dist-info/top_level.txt,sha256=sfwhUGrpOURQ3auFWgrbvIn9YVF3SWXeVQRM2_uJePY,14
-paperinquirer-0.0.7.dist-info/RECORD,,
+paperinquirer/paperinquirer.py,sha256=DpCIh8GJIJ5z9Xpt4GAi9fZ5ADnuGDqfe3ZIjZlzW6M,5322
+paperinquirer-0.0.9.data/scripts/more_features.py,sha256=PNeD6717r7cjrq7h5D2Zg0TjyU8ndQ4CfZEcmqKnnMQ,227
+paperinquirer-0.0.9.data/scripts/simple.py,sha256=eQKGz0PqRe5MaOwiGPqCjbFQS7ND9PxbAtQTc6BDNFY,191
+paperinquirer-0.0.9.dist-info/LICENSE,sha256=gGnkw4gXz_FZnTTWOhvH4kGG_w3jDFAHlIE8ESRa-b4,1084
+paperinquirer-0.0.9.dist-info/METADATA,sha256=unTU11VZl_-PWNtHOr7oHtlfVbv_bffnHS95QK-DRw4,665
+paperinquirer-0.0.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+paperinquirer-0.0.9.dist-info/top_level.txt,sha256=sfwhUGrpOURQ3auFWgrbvIn9YVF3SWXeVQRM2_uJePY,14
+paperinquirer-0.0.9.dist-info/RECORD,,
```

