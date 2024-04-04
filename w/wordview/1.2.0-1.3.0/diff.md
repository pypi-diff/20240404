# Comparing `tmp/wordview-1.2.0.tar.gz` & `tmp/wordview-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-1.2.0.tar", max compression
+gzip compressed data, was "wordview-1.3.0.tar", max compression
```

## Comparing `wordview-1.2.0.tar` & `wordview-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     3553 2023-12-19 10:23:25.130388 wordview-1.2.0/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-12-19 10:23:25.130388 wordview-1.2.0/LICENSE
--rw-r--r--   0        0        0     1027 2023-12-19 10:23:25.278388 wordview-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-12-19 10:23:25.298388 wordview-1.2.0/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-12-19 10:23:25.298388 wordview-1.2.0/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-12-19 10:23:25.298388 wordview-1.2.0/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4789 2023-12-19 10:23:25.298388 wordview-1.2.0/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       53 2023-12-19 10:23:25.298388 wordview-1.2.0/wordview/bias_analysis/__init__.py
--rw-r--r--   0        0        0    11136 2023-12-19 10:23:25.298388 wordview-1.2.0/wordview/bias_analysis/bias.py
--rw-r--r--   0        0        0     4131 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/bias_analysis/bias_terms.py
--rw-r--r--   0        0        0       48 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/clustering/cluster.py
--rw-r--r--   0        0        0     1416 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/io/dataframe_reader.py
--rw-r--r--   0        0        0       34 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     1764 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/mwes/association_measures.py
--rw-r--r--   0        0        0    11025 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     1967 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/mwes/patterns.py
--rw-r--r--   0        0        0      111 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3155 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0     3794 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/preprocessing/count.py
--rw-r--r--   0        0        0       75 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    14234 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/text_analysis/core.py
--rw-r--r--   0        0        0    13423 2023-12-19 10:23:25.302388 wordview-1.2.0/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 wordview-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3617 2024-04-04 11:52:47.999539 wordview-1.3.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2024-04-04 11:52:47.999539 wordview-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1061 2024-04-04 11:52:48.167539 wordview-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4789 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       53 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/bias_analysis/__init__.py
+-rw-r--r--   0        0        0    11136 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/bias_analysis/bias.py
+-rw-r--r--   0        0        0     4131 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/bias_analysis/bias_terms.py
+-rw-r--r--   0        0        0       48 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0     1416 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/io/dataframe_reader.py
+-rw-r--r--   0        0        0       34 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     1764 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/association_measures.py
+-rw-r--r--   0        0        0    10974 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     1967 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/patterns.py
+-rw-r--r--   0        0        0      111 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3155 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0     3794 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/preprocessing/count.py
+-rw-r--r--   0        0        0       75 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0     5809 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/chat/chat.html
+-rw-r--r--   0        0        0    14234 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0    16189 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 wordview-1.3.0/PKG-INFO
```

### Comparing `wordview-1.2.0/CHANGES.rst` & `wordview-1.3.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 1.3.0
+-------------
+- Chat feature for text analysis.
+
+
 Version 1.2.0
 -------------
 - Support for all Penn POS tags
 - Bar plots for POS tags (in addition to wordclouds)
 - Remove deprecated fasttext model.
```

### Comparing `wordview-1.2.0/LICENSE` & `wordview-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/pyproject.toml` & `wordview-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "1.2.0"
+version = "1.3.0"
 description = """Wordview is a Python package for Exploratory Data Analysis of text and provides many statistics about your data in the form of plots, tables, and descriptions allowing you to have both a high-level and detailed overview of your data."""
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 include = ["CHANGES.rst"]
 exclude = ["notebooks/", "tests/", "data/"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
@@ -16,14 +16,16 @@
 scipy = "1.10.0"
 nltk = "3.6.6"
 tqdm = "4.62.3"
 wordcloud = "1.9.1.1"
 plotly = "5.5.0"
 tabulate = "0.9.0"
 sentence-transformers = "2.2.2"
+openai = "1.14.3"
+Flask = "3.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3.0.0"
 pytest = ">=7.1"
 pytest-cov = ">=3.0.0"
 ipython = ">=8.4.0"
 sphinx = ">=v6.1.3"
```

### Comparing `wordview-1.2.0/wordview/anomaly/gaussianize.py` & `wordview-1.3.0/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/anomaly/normaldist.py` & `wordview-1.3.0/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/bias_analysis/bias.py` & `wordview-1.3.0/wordview/bias_analysis/bias.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/bias_analysis/bias_terms.py` & `wordview-1.3.0/wordview/bias_analysis/bias_terms.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/clustering/cluster.py` & `wordview-1.3.0/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/io/dataframe_reader.py` & `wordview-1.3.0/wordview/io/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/mwes/association_measures.py` & `wordview-1.3.0/wordview/mwes/association_measures.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/mwes/mwe.py` & `wordview-1.3.0/wordview/mwes/mwe.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
             ngram_count_file_path: A path to a json file containing ngram counts.
             language: The language of the corpus. Currently only 'EN' and 'DE' are supported. Defaults = 'EN'.
             custom_pattern: A string pattern to match against the tokens. The pattern must be a string of the following form.
                 Examples of user-defined patterns:
                 NP: {<DT>?<JJ>*<NN>} # Noun phrase
                 You can use multiple and/or nested patterns, separated by a newline character e.g.:
                 custom_pattern = '''
-                NP: {<DT>?<JJ>*<NN>} # Noun phrase
                 VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
                 PROPN: {<NNP>+} # Proper noun
                 ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
                 ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase'''
             only_custom_pattern: If True, only the custom pattern will be used to extract MWEs, otherwise, the default patterns will be used as well.
 
             Returns:
```

### Comparing `wordview-1.2.0/wordview/mwes/patterns.py` & `wordview-1.3.0/wordview/mwes/patterns.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/preprocessing/cleaning.py` & `wordview-1.3.0/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/preprocessing/count.py` & `wordview-1.3.0/wordview/preprocessing/count.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/text_analysis/core.py` & `wordview-1.3.0/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-1.2.0/wordview/text_analysis/wrapper.py` & `wordview-1.3.0/wordview/text_analysis/wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import threading
 from typing import Any, Tuple
 
 import pandas
 import plotly.figure_factory as ff
 import plotly.graph_objs as go
+from flask import Flask, jsonify, request, send_from_directory
+from openai import OpenAI
 from tabulate import tabulate  # type: ignore
 
 from wordview.text_analysis.core import (
     do_txt_analysis,
     generate_label_plots,
     plotly_barplot,
     plotly_wordcloud,
@@ -92,14 +95,65 @@
         self.token_count = self.analysis.token_count
         self.num_docs = self.analysis.doc_count
         self.median_doc_len = self.analysis.median_doc_len
         self.pos_counts = {
             k: len(v) for k, v in self.analysis.word_count_by_pos.items()
         }
 
+    def chat(self, api_key: str = ""):
+        """Chat with OpenAI's latest model about the results of Wordview's text analysis.
+        Access the chat UI in your localhost under http://127.0.0.1:5000/
+
+        Args:
+            api_key: OpenAI API key.
+
+        Returns:
+            None
+        """
+        self.api_key = api_key
+        self.chat_client = OpenAI(api_key=api_key)
+        base_content = f"""Answer any questions about text and corpus analysis based on the following dictionary of Wordview Analysis.
+        \n\n
+        ------------------------------
+        Wordview Analysis:
+        ------------------------------
+        {self.return_stats()}
+        \n\n
+        Answer the questions without adding According to or Based on to the Wordview Analysis dictionary.
+        """
+        chat_history = [
+            {"role": "system", "content": base_content},
+        ]
+        app = Flask(__name__, static_folder="path_to_your_ui_folder")
+
+        @app.route("/")
+        def index():
+            return send_from_directory("chat", "chat.html")
+
+        @app.route("/chat", methods=["POST"])
+        def chat():
+            user_input = request.json["message"]
+            chat_history.append({"role": "user", "content": user_input})
+            response = (
+                self.chat_client.chat.completions.create(
+                    model="gpt-3.5-turbo",
+                    messages=chat_history,
+                )
+                .choices[0]
+                .message.content
+            )
+            chat_history.append({"role": "assistant", "content": response})
+            return jsonify({"reply": response})
+
+        def run():
+            app.run(port=5000)
+
+        flask_thread = threading.Thread(target=run)
+        flask_thread.start()
+
     def show_distplot(
         self,
         distribution: str,
         layout_settings: dict[str, str] = {},
         plot_settings: dict[str, str] = {},
     ) -> None:
         """Shows distribution plots for `distribution`.
@@ -322,14 +376,38 @@
                 ["Proper Nouns", f"{self.pos_counts['NNP']:,d}"],
                 ["Adverbs", f"{self.pos_counts['RB']:,d}"],
             ],
             tablefmt="simple_grid",
         )
         print(table)
 
+    def return_stats(self) -> dict[str, Any]:
+        """Returns dataset statistics, including:
+        Language/s
+        Number of unique words
+        Number of all words
+        Number of documents
+        Median document length
+        Number of nouns
+        Number of adjectives
+        Number of verbs.
+        """
+        return {
+            "Language/s": ", ".join(self.languages),
+            "Unique Words": f"{self.type_count:,d}",
+            "All Words": f"{self.token_count:,d}",
+            "Documents": f"{self.num_docs:,d}",
+            "Median Doc Length": self.median_doc_len,
+            "Nouns": f"{self.pos_counts['NN']:,d}",
+            "Adjectives": f"{self.pos_counts['JJ']:,d}",
+            "Verbs": f"{self.pos_counts['VB']:,d}",
+            "Proper Nouns": f"{self.pos_counts['NNP']:,d}",
+            "Adverbs": f"{self.pos_counts['RB']:,d}",
+        }
+
     def show_insights(self):
         """Prints insights about the dataset."""
         raise NotImplementedError
 
 
 class LabelStatsPlots:
     """
```

### Comparing `wordview-1.2.0/PKG-INFO` & `wordview-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 1.2.0
+Version: 1.3.0
 Summary: Wordview is a Python package for Exploratory Data Analysis of text and provides many statistics about your data in the form of plots, tables, and descriptions allowing you to have both a high-level and detailed overview of your data.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: Flask (==3.0.2)
 Requires-Dist: langdetect (>=1.0.9)
 Requires-Dist: nltk (==3.6.6)
+Requires-Dist: openai (==1.14.3)
 Requires-Dist: pandas (==2.0.1)
 Requires-Dist: plotly (==5.5.0)
 Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: scipy (==1.10.0)
 Requires-Dist: sentence-transformers (==2.2.2)
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: tqdm (==4.62.3)
```

