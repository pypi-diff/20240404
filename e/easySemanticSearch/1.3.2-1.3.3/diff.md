# Comparing `tmp/easySemanticSearch-1.3.2.tar.gz` & `tmp/easySemanticSearch-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easySemanticSearch-1.3.2.tar", last modified: Mon Apr  1 23:15:43 2024, max compression
+gzip compressed data, was "easySemanticSearch-1.3.3.tar", last modified: Thu Apr  4 13:33:02 2024, max compression
```

## Comparing `easySemanticSearch-1.3.2.tar` & `easySemanticSearch-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:15:43.988158 easySemanticSearch-1.3.2/
--rw-rw-rw-   0        0        0     5153 2024-04-01 23:15:43.986158 easySemanticSearch-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4405 2024-04-01 22:01:58.000000 easySemanticSearch-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 23:15:43.963171 easySemanticSearch-1.3.2/easySemanticSearch/
--rw-rw-rw-   0        0        0       85 2024-04-01 21:09:48.000000 easySemanticSearch-1.3.2/easySemanticSearch/__init__.py
--rw-rw-rw-   0        0        0    10724 2024-04-01 23:15:36.000000 easySemanticSearch-1.3.2/easySemanticSearch/main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:15:43.984160 easySemanticSearch-1.3.2/easySemanticSearch.egg-info/
--rw-rw-rw-   0        0        0     5153 2024-04-01 23:15:43.000000 easySemanticSearch-1.3.2/easySemanticSearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-01 23:15:43.000000 easySemanticSearch-1.3.2/easySemanticSearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:15:43.000000 easySemanticSearch-1.3.2/easySemanticSearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-01 23:15:43.000000 easySemanticSearch-1.3.2/easySemanticSearch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 23:15:43.000000 easySemanticSearch-1.3.2/easySemanticSearch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 23:15:43.989158 easySemanticSearch-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      847 2024-04-01 22:40:01.000000 easySemanticSearch-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:33:02.896745 easySemanticSearch-1.3.3/
+-rw-rw-rw-   0        0        0     6982 2024-04-04 13:33:02.895688 easySemanticSearch-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6181 2024-04-04 13:05:30.000000 easySemanticSearch-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 13:33:02.863832 easySemanticSearch-1.3.3/easySemanticSearch/
+-rw-rw-rw-   0        0        0       85 2024-04-04 13:29:46.000000 easySemanticSearch-1.3.3/easySemanticSearch/__init__.py
+-rw-rw-rw-   0        0        0    12933 2024-04-04 13:32:44.000000 easySemanticSearch-1.3.3/easySemanticSearch/main.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:33:02.893689 easySemanticSearch-1.3.3/easySemanticSearch.egg-info/
+-rw-rw-rw-   0        0        0     6982 2024-04-04 13:33:02.000000 easySemanticSearch-1.3.3/easySemanticSearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-04 13:33:02.000000 easySemanticSearch-1.3.3/easySemanticSearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 13:33:02.000000 easySemanticSearch-1.3.3/easySemanticSearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-04 13:33:02.000000 easySemanticSearch-1.3.3/easySemanticSearch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-04 13:33:02.000000 easySemanticSearch-1.3.3/easySemanticSearch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 13:33:02.899284 easySemanticSearch-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-04-04 13:28:39.000000 easySemanticSearch-1.3.3/setup.py
```

### Comparing `easySemanticSearch-1.3.2/PKG-INFO` & `easySemanticSearch-1.3.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,55 @@
 Metadata-Version: 2.1
 Name: easySemanticSearch
-Version: 1.3.2
-Summary: An easy way to use advanced semantic search.
+Version: 1.3.3
+Summary: UserFriendly implementation of Highly optimized advanced semantic search.
 Author: Abhishek Venkatachalam
 Author-email: abhishek.venkatachalam06@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sentence-transformers
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 For more information about the author, visit [LinkedIn](https://www.linkedin.com/in/abhishek-venkatachalam-62121049/).
 
-# Semantic Search Python Package
+# Python Package - easySemanticSearch
 
 ## Overview
 
 This Python package provides utilities for quick, simple and efficient semantic search.
 This package leverages the SBERT capabilities of the SentenceTransformer. It allows users to perform semantic search on CSV files and pandas DataFrames.
 
+Getting started is incredibly easy, just input the "CSV file path"/ "dataframe" and the query.
+Advanced configurations are also possible, this can be achieved by inputting the correct arguments, a detailed guide is provided below.
+
+The first run takes longer as the NLU model is downloaded and the dataset is encoded and embedded. Subsequent runs will take less than a second even for large dataset comprising of 19,000 records.
+
+This package has been tested on a power restricted i7-4720hq (2015) running at 15 watts locked to ensure it will run on the majority of systems today with the best efficiency possible.
+
+
+## Release Notes
+
+### Version 1.3.3
+- Multi-Threaded and Asynchronous processing of chunks has been added to reduce processing times upto 30 percentage on a power restricted i7-4720hq (2015) running at 15 watts locked.
+- Enhanced output format - The result is now a List of Tuples where each Tuple consists of the result in JSON format output as a String. The Similarity scores still remain as Float.
+- The Semantic Search has undergone further optimizations as a result of optimizing the input which is now a string passed with JSON style formatting instead of just String.
+
+### Version 1.3.2
+- The first public release of easySemanticSearch
+- There are 2 methods of input, csv or dataframe.
+- The output is a list of Tuples, each Tuple consists of the response in Str format and a Similarity Score in Float format.
+- The initial processing times for 19000 records in a Job posting dataset (file size 97mb) take 47 minutes to encode with the default NLU model.
+- After the initial embedding, the subsequent retrievals take less than 2 seconds on most accounts.
+- If the embeddings are loaded into python and reused, it takes less than 1 second.
+
+
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 pip install easySemanticSearch
 ```
@@ -97,16 +121,16 @@
 max_results = 3    # The maximum number of search results to be retrieved.
 top_SearchResults = csv_SimpleSemanticSearch(csv_filepath_name, input_query, max_results=max_results)
 
 print("Knowledge Base:\n")
 knowledgeBase = ""
 for description, score in top_SearchResults:
     knowledgeBase = knowledgeBase + "\n" + description
-    print(f"Description: {description}")
-    print("-" * 50)
+    print(f"Search Results: {description}")
+    print("-" * 25)
 ```
 
 
 2. Below is an example of how to Semantically Search dataframes using the `dF_SimpleSemanticSearch` method:
 
 ```python
 #Import the libraries.
@@ -127,15 +151,15 @@
 max_results = 3    # The maximum number of search results to be retrieved.
 top_SearchResults = dF_SimpleSemanticSearch(sample_dataset, input_query, max_results=max_results)
 
 print("Knowledge Base:\n")
 knowledgeBase = ""
 for description, score in top_SearchResults:
     knowledgeBase = knowledgeBase + "\n" + description
-    print(f"Description: {description}")
-    print("-" * 50)
+    print(f"Search Results: {description}")
+    print("-" * 25)
 ```
 
 ## Note
 
 The first time this code is run on a dataset, the encoding is time-consuming. Performance improves dramatically after the first initialization.
 By default, the SentenceTransformer model used is "all-MiniLM-L6-v2", which can be changed based on user preference.
```

### Comparing `easySemanticSearch-1.3.2/easySemanticSearch/main.py` & `easySemanticSearch-1.3.3/easySemanticSearch/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,47 +4,57 @@
 import os   # Library to prevent or ignore warnings from being displayed.
 
 # 2) Library to store and retrieve embeddings.
 import pickle
 from pathlib import Path  # Library for file path - used to check if file exists.
 
 # 3) Libraries for processing the embeddings for better comprehension.
+import json           # To convert the embeded and output data to dataframes.
 import numpy as np    # To compute mean, etc for the embeddings
 import pandas as pd    # For the dataframe that stores the embeddings.
 
+# 4) Libraries to enable multcore processing for faster embeddings.
+from concurrent.futures import ThreadPoolExecutor
+from multiprocessing import Pool, cpu_count
+import psutil
+
+
+# This is initialized as false to identify if the module has already been initialized, this improves performance after initial initialization.
+is_model_initialized = False
+
 #__________________________
 
 def _load_csvDataset(csv_filepath_name):
     """
     Warning: Private method, NOT intended for use independently.
     Takes csv as Dataset and produces a pandas series output.
     The output combines all columns to 1 column.
     """
 
     # Read dataset from CSV file
-    dataset = pd.DataFrame()
-    dataset = pd.read_csv(csv_filepath_name)
+    user_dataframe = pd.DataFrame()
+    user_dataframe = pd.read_csv(csv_filepath_name)
 
     # Collating the values from all the other fields into a new field 'All_Data'.
-    FullData_AllColumns = dataset.apply(lambda row: '\n'.join([f"{col}: \"{row[col]}\"" for col in dataset.columns.tolist()]), axis=1)
+    FullData_AllColumns = user_dataframe.apply(lambda row: json.dumps({col: str(row[col]) for col in user_dataframe.columns.tolist()}, indent=4), axis=1)
 
     # Returning the combined pd.series.
     return FullData_AllColumns
 
 #__________________________
     
 def _process_DataFrame(user_dataframe):
     """
     Warning: Private method, NOT intended for use independently.
     Takes a dataframe and produces a pandas series output.
     The output combines all columns to 1 column.
     """
 
     # Collating the values from all the other fields into a new field 'All_Data'.
-    FullData_AllColumns = user_dataframe.apply(lambda row: '\n'.join([f"{col}: \"{row[col]}\"" for col in user_dataframe.columns.tolist()]), axis=1)
+    FullData_AllColumns = user_dataframe.apply(lambda row: json.dumps({col: str(row[col]) for col in user_dataframe.columns.tolist()}, indent=4), axis=1)
 
     # Returning the combined pd.series.
     return FullData_AllColumns
 
 #__________________________
 
 def _initiate_SemanticSearchModel(model_name, cache_folder):
@@ -69,14 +79,68 @@
 
     # Returning the model.
     return model
 
 
 #__________________________
 
+# Function to compute embeddings for a chunk of sentences
+def _compute_embeddings(chunk):
+    """
+    Warning: Private method, NOT intended for use independently.
+    This computes the embeddings.
+    """
+    return model.encode(chunk.tolist(), convert_to_tensor=True)
+
+
+def _multicore_embeddingsEncoding(FullData_AllColumns):
+    """
+    Warning: Private method, NOT intended for use independently.
+    Utilizes multi core processing to speed up encoding times.   
+    """
+
+    # Get the number of CPU cores
+    num_cores = cpu_count()  # Limiting to 4 CPU cores
+
+    # Get available memory
+    available_memory_bytes = psutil.virtual_memory().available
+
+    # Estimate embedding size
+    embedding_size = model.get_sentence_embedding_dimension()
+
+    # Convert pandas.Series to numpy array
+    sentences = FullData_AllColumns.values
+
+    # Compute the optimal chunk size based on available memory and dataset size
+    total_sentences = len(sentences)
+
+    # Estimate memory usage for embeddings of a single chunk
+    optimal_memory_usage = available_memory_bytes / num_cores
+    optimal_chunk_size = int(optimal_memory_usage / (embedding_size * 4))  # Assuming float32 for embeddings
+
+    # Adjust chunk size to a smaller value, such as 10 or 20
+    chunk_size = min(total_sentences/num_cores, optimal_chunk_size)  # Adjust this value based on trial and error
+
+    # Split the dataset into chunks based on chunk size
+    chunks = np.array_split(sentences, int(np.ceil(total_sentences / chunk_size)))
+
+    # Initialize a ThreadPoolExecutor
+    with ThreadPoolExecutor(max_workers= num_cores) as executor:
+        embeddings_list = list(executor.map(_compute_embeddings, chunks))
+
+    # Concatenate the embeddings
+    embeddings = np.concatenate(embeddings_list, axis=0)
+
+    # Return the encodings.
+    return embeddings
+
+
+#__________________________
+
+
 def _embeddings_create_reuse(csv_filepath_name, embeddings_Filename, model):
     """
     Warning: Private method, NOT intended for use independently.
     The default name for embeddings is "embeddings_SemanticSearch.pkl".
     To create new embeddings, rename or delete existing one.
     """
 
@@ -95,39 +159,38 @@
     else:
 
         # if csv_filepath_name is string, we use the methods for csvDataset loading.
         if isinstance(csv_filepath_name, str):
 
             # Compute embeddings for the FullData_AllColumns column
             FullData_AllColumns = _load_csvDataset(csv_filepath_name)
-            embeddings_FullData_AllColumns = model.encode(FullData_AllColumns.tolist(), convert_to_tensor=True)
+            embeddings_FullData_AllColumns = _multicore_embeddingsEncoding(FullData_AllColumns = FullData_AllColumns)
 
             # Store sentences & embeddings on storage
             with open(file_pathname, "wb") as fOut:
                 pickle.dump({"sentences": FullData_AllColumns, "embeddings": embeddings_FullData_AllColumns}, fOut, protocol=pickle.HIGHEST_PROTOCOL)
 
         # Else - when csv_filepath_name is NOT str, we assume it is a DataFrame.
         else:
 
             # Compute embeddings for the FullData_AllColumns column
             FullData_AllColumns = _process_DataFrame(csv_filepath_name)
-            embeddings_FullData_AllColumns = model.encode(FullData_AllColumns.tolist(), convert_to_tensor=True)
+            embeddings_FullData_AllColumns = _multicore_embeddingsEncoding(FullData_AllColumns = FullData_AllColumns)
 
             # Store sentences & embeddings on storage
             with open(file_pathname, "wb") as fOut:
                 pickle.dump({"sentences": FullData_AllColumns, "embeddings": embeddings_FullData_AllColumns}, fOut, protocol=pickle.HIGHEST_PROTOCOL)
 
 
     #Return the FullData_AllColumns, embeddings_FullData_AllColumns.
     return FullData_AllColumns, embeddings_FullData_AllColumns
 
 
 #__________________________
 
-
 def _get_top_semanticResults(query, data_embeddings, data_fromDataSet, model, top_k):
     """
     Warning: Private method, NOT intended for use independently.
     Fetches the top search results for the query.
     """
 
     # Encode the query
@@ -141,20 +204,16 @@
     
     # Retrieve top k descriptions
     top_results = [(data_fromDataSet[i], cosine_scores[i].item()) for i in sorted_indices[:top_k]]
     
     # Returning the top results.
     return top_results
 
-
 #__________________________
 
-# This is initialized as false to identify if the module has already been initialized, this improves performance after initial initialization.
-is_model_initialized = False
-
 def csv_SimpleSemanticSearch(csv_filepath_name, input_query = "Some text", max_results = 5, model_name = "all-MiniLM-L6-v2", embeddings_Filename = "embeddings_SemanticSearch.pkl", cache_folder = "default_folder"):
     """
     Takes (input_query, csv_filepath_name, max_results) as input and makes it queryable.
     First time encoding is time consuming. Performance improves after first time.
     The default SentenceTransformer model name from huggingface = "all-MiniLM-L6-v2", this can be changed.
     Please refer to the PyPi Package page for more detailed information.
     """
@@ -186,19 +245,18 @@
         FullData_AllColumns, embeddings_FullData_AllColumns = _embeddings_create_reuse(csv_filepath_name, embeddings_Filename, model = model)
 
         # Fetch the Semantic Search Results.
         top_Searchresults = _get_top_semanticResults(data_embeddings = embeddings_FullData_AllColumns, data_fromDataSet = FullData_AllColumns, model = model, query = input_query, top_k = max_results)
 
     
     # Return the search results.
-    return top_Searchresults        
-
+    return top_Searchresults    
 #__________________________
 
-def dF_SimpleSemanticSearch(user_dataframe, input_query = "Some text", max_results = 5, model_name = "all-MiniLM-L6-v2", embeddings_Filename = "embeddings_SemanticSearch.pkl", cache_folder = "default_folder"):
+def df_SimpleSemanticSearch(user_dataframe, input_query = "Some text", max_results = 5, model_name = "all-MiniLM-L6-v2", embeddings_Filename = "embeddings_SemanticSearch.pkl", cache_folder = "default_folder"):
     """
     Takes (input_query, csv_filepath_name, max_results) as input and makes it queryable.
     First time encoding is time consuming. Performance improves after first time.
     The default SentenceTransformer model name from huggingface = "all-MiniLM-L6-v2", this can be changed.
     Please refer to the PyPi Package page for more detailed information.
     """
 
@@ -229,10 +287,10 @@
         FullData_AllColumns, embeddings_FullData_AllColumns = _embeddings_create_reuse(user_dataframe, embeddings_Filename, model = model)
 
         # Fetch the Semantic Search Results.
         top_Searchresults = _get_top_semanticResults(data_embeddings = embeddings_FullData_AllColumns, data_fromDataSet = FullData_AllColumns, model = model, query = input_query, top_k = max_results)
 
     
     # Return the search results.
-    return top_Searchresults     
+    return top_Searchresults   
 
 #__________________________
```

### Comparing `easySemanticSearch-1.3.2/easySemanticSearch.egg-info/PKG-INFO` & `easySemanticSearch-1.3.3/easySemanticSearch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,55 @@
 Metadata-Version: 2.1
 Name: easySemanticSearch
-Version: 1.3.2
-Summary: An easy way to use advanced semantic search.
+Version: 1.3.3
+Summary: UserFriendly implementation of Highly optimized advanced semantic search.
 Author: Abhishek Venkatachalam
 Author-email: abhishek.venkatachalam06@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sentence-transformers
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 For more information about the author, visit [LinkedIn](https://www.linkedin.com/in/abhishek-venkatachalam-62121049/).
 
-# Semantic Search Python Package
+# Python Package - easySemanticSearch
 
 ## Overview
 
 This Python package provides utilities for quick, simple and efficient semantic search.
 This package leverages the SBERT capabilities of the SentenceTransformer. It allows users to perform semantic search on CSV files and pandas DataFrames.
 
+Getting started is incredibly easy, just input the "CSV file path"/ "dataframe" and the query.
+Advanced configurations are also possible, this can be achieved by inputting the correct arguments, a detailed guide is provided below.
+
+The first run takes longer as the NLU model is downloaded and the dataset is encoded and embedded. Subsequent runs will take less than a second even for large dataset comprising of 19,000 records.
+
+This package has been tested on a power restricted i7-4720hq (2015) running at 15 watts locked to ensure it will run on the majority of systems today with the best efficiency possible.
+
+
+## Release Notes
+
+### Version 1.3.3
+- Multi-Threaded and Asynchronous processing of chunks has been added to reduce processing times upto 30 percentage on a power restricted i7-4720hq (2015) running at 15 watts locked.
+- Enhanced output format - The result is now a List of Tuples where each Tuple consists of the result in JSON format output as a String. The Similarity scores still remain as Float.
+- The Semantic Search has undergone further optimizations as a result of optimizing the input which is now a string passed with JSON style formatting instead of just String.
+
+### Version 1.3.2
+- The first public release of easySemanticSearch
+- There are 2 methods of input, csv or dataframe.
+- The output is a list of Tuples, each Tuple consists of the response in Str format and a Similarity Score in Float format.
+- The initial processing times for 19000 records in a Job posting dataset (file size 97mb) take 47 minutes to encode with the default NLU model.
+- After the initial embedding, the subsequent retrievals take less than 2 seconds on most accounts.
+- If the embeddings are loaded into python and reused, it takes less than 1 second.
+
+
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 pip install easySemanticSearch
 ```
@@ -97,16 +121,16 @@
 max_results = 3    # The maximum number of search results to be retrieved.
 top_SearchResults = csv_SimpleSemanticSearch(csv_filepath_name, input_query, max_results=max_results)
 
 print("Knowledge Base:\n")
 knowledgeBase = ""
 for description, score in top_SearchResults:
     knowledgeBase = knowledgeBase + "\n" + description
-    print(f"Description: {description}")
-    print("-" * 50)
+    print(f"Search Results: {description}")
+    print("-" * 25)
 ```
 
 
 2. Below is an example of how to Semantically Search dataframes using the `dF_SimpleSemanticSearch` method:
 
 ```python
 #Import the libraries.
@@ -127,15 +151,15 @@
 max_results = 3    # The maximum number of search results to be retrieved.
 top_SearchResults = dF_SimpleSemanticSearch(sample_dataset, input_query, max_results=max_results)
 
 print("Knowledge Base:\n")
 knowledgeBase = ""
 for description, score in top_SearchResults:
     knowledgeBase = knowledgeBase + "\n" + description
-    print(f"Description: {description}")
-    print("-" * 50)
+    print(f"Search Results: {description}")
+    print("-" * 25)
 ```
 
 ## Note
 
 The first time this code is run on a dataset, the encoding is time-consuming. Performance improves dramatically after the first initialization.
 By default, the SentenceTransformer model used is "all-MiniLM-L6-v2", which can be changed based on user preference.
```

### Comparing `easySemanticSearch-1.3.2/setup.py` & `easySemanticSearch-1.3.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='easySemanticSearch',
-    version='1.3.2',
+    version='1.3.3',
     author='Abhishek Venkatachalam',
     author_email='abhishek.venkatachalam06@gmail.com',
-    description='An easy way to use advanced semantic search.',
+    description='UserFriendly implementation of Highly optimized advanced semantic search.',
     long_description=(
         "For more information about the author, visit [LinkedIn](https://www.linkedin.com/in/abhishek-venkatachalam-62121049/).\n\n"
         + open('README.md').read()
     ),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

