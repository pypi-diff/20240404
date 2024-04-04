# Comparing `tmp/nodoc-1.0.5.tar.gz` & `tmp/nodoc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodoc-1.0.5.tar", last modified: Thu Apr  4 07:46:59 2024, max compression
+gzip compressed data, was "nodoc-1.0.6.tar", last modified: Thu Apr  4 08:04:22 2024, max compression
```

## Comparing `nodoc-1.0.5.tar` & `nodoc-1.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.785855 nodoc-1.0.5/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       36 2023-12-14 10:37:29.000000 nodoc-1.0.5/MANIFEST.in
--rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 07:46:59.785855 nodoc-1.0.5/PKG-INFO
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.782855 nodoc-1.0.5/nodoc/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      379 2024-04-04 07:45:42.000000 nodoc-1.0.5/nodoc/__init__.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.782855 nodoc-1.0.5/nodoc/nodoc/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      559 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      925 2024-02-19 12:14:58.000000 nodoc-1.0.5/nodoc/nodoc/const.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.783855 nodoc-1.0.5/nodoc/nodoc/database/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       74 2023-12-14 10:08:59.000000 nodoc-1.0.5/nodoc/nodoc/database/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     1936 2023-12-15 12:21:41.000000 nodoc-1.0.5/nodoc/nodoc/database/database.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     7786 2023-12-15 12:31:37.000000 nodoc-1.0.5/nodoc/nodoc/database/vectordb.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.783855 nodoc-1.0.5/nodoc/nodoc/debugger/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       89 2023-12-14 10:08:59.000000 nodoc-1.0.5/nodoc/nodoc/debugger/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     2748 2023-12-14 10:08:59.000000 nodoc-1.0.5/nodoc/nodoc/debugger/decorator.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.784855 nodoc-1.0.5/nodoc/nodoc/document/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      288 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/document/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8310 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/document/_base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     2824 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/document/base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     3490 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/document/flow_processing.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8050 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/document/markdown.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      348 2023-12-14 10:08:59.000000 nodoc-1.0.5/nodoc/nodoc/document/pdf.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.784855 nodoc-1.0.5/nodoc/nodoc/post_processing/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       55 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/post_processing/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      577 2024-03-26 11:56:53.000000 nodoc-1.0.5/nodoc/nodoc/post_processing/_base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     1924 2024-04-04 06:58:32.000000 nodoc-1.0.5/nodoc/nodoc/setup.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.784855 nodoc-1.0.5/nodoc/nodoc/structure/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      173 2023-12-14 10:08:59.000000 nodoc-1.0.5/nodoc/nodoc/structure/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8612 2024-02-19 12:29:29.000000 nodoc-1.0.5/nodoc/nodoc/structure/doc_tree.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)    11993 2023-12-15 12:06:54.000000 nodoc-1.0.5/nodoc/nodoc/structure/tree.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:46:59.784855 nodoc-1.0.5/nodoc.egg-info/
--rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 07:46:59.000000 nodoc-1.0.5/nodoc.egg-info/PKG-INFO
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      760 2024-04-04 07:46:59.000000 nodoc-1.0.5/nodoc.egg-info/SOURCES.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)        1 2024-04-04 07:46:59.000000 nodoc-1.0.5/nodoc.egg-info/dependency_links.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)        6 2024-04-04 07:46:59.000000 nodoc-1.0.5/nodoc.egg-info/top_level.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      469 2024-04-04 07:46:53.000000 nodoc-1.0.5/pyproject.toml
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       38 2024-04-04 07:46:59.785855 nodoc-1.0.5/setup.cfg
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.299902 nodoc-1.0.6/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       36 2023-12-14 10:37:29.000000 nodoc-1.0.6/MANIFEST.in
+-rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 08:04:22.299902 nodoc-1.0.6/PKG-INFO
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.296902 nodoc-1.0.6/nodoc/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      379 2024-04-04 07:45:42.000000 nodoc-1.0.6/nodoc/__init__.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.297902 nodoc-1.0.6/nodoc/nodoc/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      559 2024-03-26 11:56:53.000000 nodoc-1.0.6/nodoc/nodoc/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      925 2024-02-19 12:14:58.000000 nodoc-1.0.6/nodoc/nodoc/const.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.297902 nodoc-1.0.6/nodoc/nodoc/database/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       74 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/database/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     1936 2023-12-15 12:21:41.000000 nodoc-1.0.6/nodoc/nodoc/database/database.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     7786 2023-12-15 12:31:37.000000 nodoc-1.0.6/nodoc/nodoc/database/vectordb.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.297902 nodoc-1.0.6/nodoc/nodoc/debugger/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       89 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/debugger/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     2748 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/debugger/decorator.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.298902 nodoc-1.0.6/nodoc/nodoc/document/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      331 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8387 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/_base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     3068 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     3587 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/flow_processing.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)    10250 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/markdown.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      348 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/document/pdf.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.298902 nodoc-1.0.6/nodoc/nodoc/post_processing/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       55 2024-03-26 11:56:53.000000 nodoc-1.0.6/nodoc/nodoc/post_processing/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      577 2024-03-26 11:56:53.000000 nodoc-1.0.6/nodoc/nodoc/post_processing/_base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     1924 2024-04-04 06:58:32.000000 nodoc-1.0.6/nodoc/nodoc/setup.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.298902 nodoc-1.0.6/nodoc/nodoc/structure/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      173 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/structure/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8365 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/structure/doc_tree.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)    11993 2023-12-15 12:06:54.000000 nodoc-1.0.6/nodoc/nodoc/structure/tree.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.299902 nodoc-1.0.6/nodoc.egg-info/
+-rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/PKG-INFO
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      760 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)        1 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)        6 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/top_level.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      469 2024-04-04 08:04:09.000000 nodoc-1.0.6/pyproject.toml
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       38 2024-04-04 08:04:22.299902 nodoc-1.0.6/setup.cfg
```

### Comparing `nodoc-1.0.5/nodoc/nodoc/__init__.py` & `nodoc-1.0.6/nodoc/nodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/const.py` & `nodoc-1.0.6/nodoc/nodoc/const.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/database/database.py` & `nodoc-1.0.6/nodoc/nodoc/database/database.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/database/vectordb.py` & `nodoc-1.0.6/nodoc/nodoc/database/vectordb.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/debugger/decorator.py` & `nodoc-1.0.6/nodoc/nodoc/debugger/decorator.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/document/_base.py` & `nodoc-1.0.6/nodoc/nodoc/document/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,18 @@
         """
         self.content = content
         self.default = default
         pass
 
     def __rshift__(self, other):
         if self.content in other:
-            return other[self.content]
+            try:
+                return other[self.content]
+            except:
+                return self.default
         else:
             return self.default
 
 class MetaData(TypedDict):
     filename: str
     "文件名称"
     create: str
```

### Comparing `nodoc-1.0.5/nodoc/nodoc/document/base.py` & `nodoc-1.0.6/nodoc/nodoc/document/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import abc
 import time
 from typing import Literal, Self, Union
+
 from ._base import document_type
 from ._base import Message
 from ._base import Data
 from ._base import Checker
 from ._base import MessageInit
 from ._base import MetaData
 generalProperty = MessageInit.generalProperty
 fontStyleProperty = MessageInit.fontStyleProperty
 
-import pandas as pd
+def __import():
+    global docTree
+    from nodoc import docTree
+
 
 
 
 class Document(metaclass=abc.ABCMeta):
 
     def __init__(self, data: str = "", metadata: MetaData = None) -> None:
         if metadata is None:
@@ -42,14 +46,18 @@
     def content(self) -> str:
         return self.__data.content
 
     @property
     def message(self) -> Message:
         return self.__message
 
+    @message.setter
+    def message(self, message: Message) -> None:
+        self.__message = message
+
     @abc.abstractmethod
     def __document__(self):
         ...
 
     @abc.abstractmethod
     def normalize(self) -> Message:
         "文档标准化为消息。"
@@ -63,15 +71,15 @@
     def load(path: str) -> 'Document':
         "文档的导入方法。"
 
     @staticmethod
     @abc.abstractmethod
     def load_from_message(message: Message) -> 'Document':
         """
-        从消息中加载markdown。
+        从消息中加载文档。
         - message: Message, 传入的消息。
         """
 
     @staticmethod
     def transform(source: 'Document', to: document_type) -> Union['Document', None]:
 
         match to:
@@ -89,13 +97,18 @@
             #     return Word.transform(source)
             # case 'ppt':
             #     from . import PPT
             #     return PPT.transform(source)
             # case 'excel':
             #     from . import Excel
             #     return Excel.transform(source)
+        
+    def treeify(self) -> 'docTree':
+        """
+        将文档树化。
+        """
 
     def __lshift__(self, other):
         return self.__data << other
 
     def __str__(self) -> str:
         return self.__data.content
```

### Comparing `nodoc-1.0.5/nodoc/nodoc/document/flow_processing.py` & `nodoc-1.0.6/nodoc/nodoc/document/flow_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from nodoc.post_processing import ocrData
 from nodoc.document import Message
+from nodoc.document import Checker
 
 """
 A special program which processing the last flow.
 """
 
 def parse(data: ocrData) -> Message:
     """
@@ -21,14 +22,16 @@
         for element in data 
         for unit in element['res']
         if element['type'] == 'title'
     ])
     fontSizes = list(fontSizes)
     fontSizes.sort()
     for element in data:
+        if element['type'] == 'figure': 
+            continue
         for unit in element['res']:
             if element['type'] == 'text':
 
                 fontHeight: str = unit['text_region'][2][1] - unit['text_region'][0][1] # 字符高度
                 textWidth: str = unit['text_region'][2][0] - unit['text_region'][0][0]  # 文本宽度
                 indent: float = unit['text_region'][0][0] - element['bbox'][0]          # 字符缩进（像素）
                 tailIndent: float = unit['text_region'][0][0] - element['bbox'][0]      # 文本尾部内边距（像素）
```

### Comparing `nodoc-1.0.5/nodoc/nodoc/document/markdown.py` & `nodoc-1.0.6/nodoc/nodoc/document/markdown.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 import re
 from time import strftime
 from typing import Self, Union, Unpack
+from uuid import uuid4
+
+def __import():
+    from nodoc import docTree
 
 
 from .base import Data, Document, Message, Checker
 from .base import generalProperty, fontStyleProperty
 from .base import MetaData, time
 # Use a pipeline as a high-level helper
 INDENT = '\t'
@@ -27,14 +31,18 @@
     (r'^(\x20*)(>)(.*)',  r'\1\\\2\3'),            # 引用
     (r'^(\x20*)(\*{3,}|-{3,}|_{3,})(\x20*)$',  r'\1\\\2\3'),    # 分隔线
     (r'^\s*$',  ''),
 )
 
 RECOGNIZE_FORMATTER = ()
 
+def __import():
+    global docTree
+    from nodoc import docTree
+
 class Markdown(Document):
     
     def __init__(self, data: str = "", metadata: MetaData = None) -> None:
         super().__init__(data, metadata)
 
     @staticmethod
     def escape(text: Union['Markdown', str]):
@@ -109,14 +117,60 @@
         ...
 
     def export(self, name: str, directory: str = './'):
         directory = os.path.abspath(directory)
         with open(directory + '/' + name + '.md', 'w+', encoding='utf-8') as file:
             file.write(self.__str__())
 
+    def treeify(self) -> 'docTree':
+        from nodoc import docNode
+        from nodoc import docTree
+        node = docNode(kind = 'title', content = '')
+        node.level = -1
+        uuid = uuid4()
+        tree = docTree(node)
+        node @ tree
+        message = self.message
+        pipeline = message['pipeline']
+        for order, unit in enumerate(pipeline):
+            last_node: docNode = node
+            node.order = order
+            node: docNode = docNode(kind = unit('type'), content = unit['content'])
+            match unit['type']:
+                case 'text':
+                    if last_node.isText:
+                        self.message['pipeline'][node.order]['parent'] = uuid
+                        (node & last_node) @ last_node.parent
+                    elif last_node.isTitle:
+                        node @ last_node
+
+                case 'title':
+                    node.level = unit['property']['level']
+                    def bind_parent(nodeA: docNode, nodeB: docNode):
+                        if nodeA.level == nodeB.level - 1:
+                            self.message['pipeline'][nodeA.order]['parent'] = uuid
+                            nodeA @ nodeB
+                        elif nodeA.level == nodeB.level:
+                            self.message['pipeline'][nodeA.order]['parent'] = uuid
+                            nodeA @ nodeB.parent
+                        elif nodeB.level == -1:
+                            self.message['pipeline'][nodeA.order]['parent'] = uuid
+                            nodeA @ nodeB
+                        else:
+                            bind_parent(nodeA, nodeB.parent)
+                    if last_node.isText:
+                        self.message['pipeline'][order]['parent'] = uuid
+                        (node & last_node) @ last_node.parent
+                    elif last_node.isTitle:
+                        bind_parent(node, last_node)
+            uuid = uuid4()
+            self.message['pipeline'][order]['uuid'] = uuid
+        return tree
+
+
     @staticmethod
     def transform(source: Document) -> 'Markdown':
         """
         静态方法，将任意受支持的文档类型转换为Markdown文档。
         - source: Document, 传入的文档。
         """
         document = Markdown.load_from_message(source.message)
@@ -125,14 +179,15 @@
     @staticmethod
     def load_from_message(message: Message) -> 'Markdown':
         """
         从消息中加载markdown。
         - message: Message, 传入的消息。
         """
         document: Markdown = Markdown(metadata=message['metadata'])
+        document.message = message
         for unit in message['pipeline']:
             match unit['type']:
                 case 'title':
                     if 'inherited' in unit['property']:
                         if isinstance(unit['property']['inherited'], str):
                             document.data << f'<span class="{unit["property"]["inherited"]}" style="'
                         else:
@@ -184,14 +239,15 @@
                 case 'footer':
                     ...
                 case 'fontStyle':
                     ...
                 
         return document
 
+
     @staticmethod
     def load(path: str) -> 'Markdown':
         with open(path, 'r+', encoding='utf-8') as file:
             text = file.read()
         return Markdown(text)
 
     def __document__(self):
```

### Comparing `nodoc-1.0.5/nodoc/nodoc/post_processing/_base.py` & `nodoc-1.0.6/nodoc/nodoc/post_processing/_base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/setup.py` & `nodoc-1.0.6/nodoc/nodoc/setup.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc/nodoc/structure/doc_tree.py` & `nodoc-1.0.6/nodoc/nodoc/structure/doc_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,51 +68,51 @@
         self._parent: docNode
         self._children: docNodes
         self._right: docNode
         self._left: docNode
 
     @property
     def tree(self) -> 'docTree':
-        return type(docTree)(super().tree)
+        return super().tree
 
     @tree.setter
     def tree(self, value: 'docTree'):
-        type(docTree)(super(docNode, docNode).tree).__set__(self, value)
+        super(docTree, docTree).tree.__set__(self, value)
 
     @property
     def children(self) -> 'docNodes':
-        return type(docNodes)(super().children)
+        return super().children
 
     @children.setter
     def children(self, value: 'docNodes'):
-        type(docTree)(super(docNode, docNode).children).__set__(self, value)
+        super(docNode, docNode).children.__set__(self, value)
 
     @property
     def parent(self) -> 'docNode':
-        return type(docNode)(super().parent)
+        return super().parent
 
     @parent.setter
     def parent(self, value: 'docNode'):
-        type(docTree)(super(docNode, docNode).parent).__set__(self, value)
+        super(docNode, docNode).parent.__set__(self, value)
 
     @property
     def left(self) -> 'docNode':
-        return type(docNode)(super().left)
+        return super().left
 
     @left.setter
     def left(self, value: 'docNode'):
-        type(docTree)(super(docNode, docNode).left).__set__(self, value)
+        super(docNode, docNode).left.__set__(self, value)
 
     @property
     def right(self) -> 'docNode':
-        return type(docNode)(super().right)
+        return super().right
 
     @right.setter
     def right(self, value: 'docNode'):
-        type(docTree)(super(docNode, docNode).right).__set__(self, value)
+        super(docNode, docNode).right.__set__(self, value)
 
     @property
     def isText(self) -> bool:
         "是否是正文节点"
         return self._isText
 
     @isText.setter
@@ -163,36 +163,36 @@
             return len(self.children) == 0
         return super().__eq__(__value)
 
     def __rshift__(self, other: Union['docNode', None]):
         result = super().__rshift__(other)
         if result is None:
             return None
-        return type(docNodes)(result)
+        return result
 
     def __lshift__(self, other: Union['docNode', None]):
         result = super().__lshift__(other)
         if result is None:
             return None
-        return type(docNodes)(result)
+        return result
 
     def get_route(self, endpoint: 'docNode', condition: docnode_return_bool | None = None) -> Union['docNodes', None]:
         """
         获取子父节点的路由 -> 默认是从该节点到目标节点之间的所有标题节点（不包括该节点）。
         - endpoint: Node，该节点的目标节点。
         """
         if condition is None:
             def __condition(node: docNode):
                     return node.isTitle
         else:
             __condition = condition
         result = super().get_route(endpoint, __condition)
         if result is None:
             return None
-        return type(docNodes)(result)
+        return result
 
     def __matmul__(self, other):
         result = super().__matmul__(other)
         return result
 
     def __str__(self):
         return f"""
@@ -229,19 +229,19 @@
     def __init__(self, root: docNode, name: str = '文档树', **data: Unpack[docArg]) -> None:
         """
         实例化一个文档树对象。
         - root: docNode, 文档树的根节点。
         - name: str, 文档树的名称，用于查询。
         """
         data.setdefault('head', None)
-        data.setdefault('metadata', type(metadata)({
+        data.setdefault('metadata', {
             'create_time': time.strftime('%Y-%m-%d %H:%M:%S', time.localtime()),
             'modify_time': time.strftime('%Y-%m-%d %H:%M:%S', time.localtime()),
             'visit_time': time.strftime('%Y-%m-%d %H:%M:%S', time.localtime())
-        }))
+        })
 
         if not isinstance(root, docNode):
             raise TypeError(f'期望：docNode，实际：{type(root)}')
 
         super().__init__(root, name)
         self.data = data
         self.root: docNode
@@ -251,20 +251,20 @@
 
     def from_document(self, document: Document):
         self.document = document.content
 
     # @override
     def DFT(self, node=None, callback: Callable[[Node], bool] = lambda node: True) -> list[docNode] | None:
         result = super().DFT(node, callback)
-        return type(docNodes)(result)
+        return result
 
     # @override
     def BFT(self, callback: Callable[[Node], bool] = lambda node: True) -> list[docNode] | None:
         result = super().BFT(callback)
-        return type(docNodes)(result)
+        return result
 
     def __str__(self):
         document = None
         if hasattr(self, 'document'):
             if len(self.document) <= 12:
                 document = self.document.replace('\n', '')
             else:
```

### Comparing `nodoc-1.0.5/nodoc/nodoc/structure/tree.py` & `nodoc-1.0.6/nodoc/nodoc/structure/tree.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.5/nodoc.egg-info/SOURCES.txt` & `nodoc-1.0.6/nodoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

