# Comparing `tmp/financial_datasets-0.1.1.tar.gz` & `tmp/financial_datasets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.1.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.2.tar", max compression
```

## Comparing `financial_datasets-0.1.1.tar` & `financial_datasets-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.1/LICENSE
--rw-r--r--   0        0        0     2700 2024-03-30 23:21:00.793310 financial_datasets-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.1/financial_datasets/__init__.py
--rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.1/financial_datasets/dataset.py
--rw-r--r--   0        0        0     3435 2024-04-03 12:46:57.792263 financial_datasets-0.1.1/financial_datasets/generator.py
--rw-r--r--   0        0        0      282 2024-03-30 22:53:11.228502 financial_datasets-0.1.1/financial_datasets/model.py
--rw-r--r--   0        0        0      602 2024-04-03 12:48:21.832604 financial_datasets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3472 1970-01-01 00:00:00.000000 financial_datasets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2700 2024-03-30 23:21:00.793310 financial_datasets-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.2/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.2/financial_datasets/dataset.py
+-rw-r--r--   0        0        0     3763 2024-04-03 18:32:20.963494 financial_datasets-0.1.2/financial_datasets/generator.py
+-rw-r--r--   0        0        0      282 2024-03-30 22:53:11.228502 financial_datasets-0.1.2/financial_datasets/model.py
+-rw-r--r--   0        0        0      619 2024-04-03 22:15:32.555865 financial_datasets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 financial_datasets-0.1.2/PKG-INFO
```

### Comparing `financial_datasets-0.1.1/LICENSE` & `financial_datasets-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.1/README.md` & `financial_datasets-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.1/financial_datasets/generator.py` & `financial_datasets-0.1.2/financial_datasets/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from typing import List
+from tqdm import tqdm
 
 from instructor import patch
 from openai import OpenAI
 
 from financial_datasets.dataset import DatasetItem, Dataset
 from financial_datasets.model import ModelConfig, ModelProvider
 
@@ -36,14 +37,16 @@
 
     def generate_from_texts(self, texts: List[str], max_questions=10) -> Dataset:
         items: List[DatasetItem] = []
         num_texts = len(texts)
         questions_per_text = max_questions // num_texts
         remaining_questions = max_questions % num_texts
 
+        progress_bar = tqdm(total=max_questions, desc="Generating questions", colour='green')
+
         for index, text in enumerate(texts):
             try:
                 # Determine the number of questions to generate for the current text
                 current_max_questions = questions_per_text
                 if index < remaining_questions:
                     current_max_questions += 1
 
@@ -55,17 +58,23 @@
                         {"role": "system", "content": system_prompt},
                         {"role": "user", "content": f"Generate {current_max_questions} questions for the following block of text: {text}"}
                     ],
                 )
 
                 # Add the generated items to our total list of questions
                 items.extend(response.items)
+
+                # Update the progress bar by the number of questions generated
+                progress_bar.update(len(response.items))
             except Exception as e:
                 print(f"Failed to generate questions for batch {index + 1}: {e}")
                 continue
 
             # Sleep for 1 second to avoid overloading the LLM
             time.sleep(1)
 
+        # Ensure the progress bar is closed
+        progress_bar.close()
+
         return Dataset(
             items=items,
         )
```

### Comparing `financial_datasets-0.1.1/PKG-INFO` & `financial_datasets-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financial-datasets
-Version: 0.1.1
+Version: 0.1.2
 Summary: Financial datasets for LLMs
 License: MIT
 Author: Virat Singh
 Author-email: virat@virat.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
 Requires-Dist: instructor (>=0.6.7,<0.7.0)
 Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # Financial Datasets
 
 Financial Datasets is an open-source Python library 
 that allows developers to create synthetic financial datasets
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: financial-datasets Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: financial-datasets Version: 0.1.2 Summary:
 Financial datasets for LLMs License: MIT Author: Virat Singh Author-email:
 virat@virat.ai Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist:
 chromadb (>=0.4.24,<0.5.0) Requires-Dist: datasets (>=2.18.0,<3.0.0) Requires-
 Dist: instructor (>=0.6.7,<0.7.0) Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0) Requires-Dist: tiktoken
-(>=0.6.0,<0.7.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Description-
-Content-Type: text/markdown # Financial Datasets Financial Datasets is an open-
-source Python library that allows developers to create synthetic financial
-datasets using Large Language Models (LLMs). With this library, you can
-generate realistic financial datasets based on SEC filings such as 10-Ks, 10-
-Qs, and other financial reports. [![Twitter Follow](https://img.shields.io/
-twitter/follow/virattt?style=social)](https://twitter.com/virattt) ## Features
-- Generate synthetic financial datasets using LLMs - Supports various SEC
-filings (10-Ks, 10-Qs, etc.) - Easy integration with Python projects -
-Customizable data generation options Example dataset: ```json [ { "question":
-"What was Airbnb's revenue in 2023?", "answer": "$9.9 billion", "context": "In
-2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due
-to a 14% increase in Nights and Experiences Booked of 54.5 million combined
-with higher average daily rates driving a 16% increase in Gross Booking Value
-of $10.0 billion." }, { "question": "By what percentage did Airbnb's net income
-increase in 2023 compared to the prior year?", "answer": "153%", "context":
-"Net income in 2023 increased by 153% to $4.8 billion, compared to the prior
-year, driven by our revenue growth, increased interest income, discipline in
-managing our cost structure, and the release of a portion of our valuation
-allowance on deferred tax assets of $2.9 billion." } ] ``` ## Installation ###
-Using pip You can install the Financial Datasets library using pip: ``` pip
-install financial-datasets ``` ### Using Poetry If you prefer to use Poetry for
-dependency management, you can add Financial Datasets to your project: ```
-poetry add financial-datasets ``` ### From the Repository If you want to
-install the library directly from the repository, follow these steps: 1. Clone
-the repository: ``` git clone https://github.com/yourusername/financial-
-datasets.git ``` 2. Navigate to the project directory: ``` cd financial-
-datasets ``` 3. Install the dependencies using Poetry: ``` poetry install ```
-4. You can now use the library in your Python projects. ## Usage Here's a
-simple example of how to use the Financial Datasets library: ```python # TODO -
-coming soon ``` ## Contributing Contributions are welcome! If you find any
-issues or have suggestions for improvements, please open an issue or submit a
-pull request. ## License This project is licensed under the [MIT License](link-
-to-license-file). ## Contributors_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_i_r_a_t_t_t_/
-_f_i_n_a_n_c_i_a_l_-_d_a_t_a_s_e_t_s_]
+(>=0.6.0,<0.7.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0) Requires-Dist: xmltodict
+(>=0.13.0,<0.14.0) Description-Content-Type: text/markdown # Financial Datasets
+Financial Datasets is an open-source Python library that allows developers to
+create synthetic financial datasets using Large Language Models (LLMs). With
+this library, you can generate realistic financial datasets based on SEC
+filings such as 10-Ks, 10-Qs, and other financial reports. [![Twitter Follow]
+(https://img.shields.io/twitter/follow/virattt?style=social)](https://
+twitter.com/virattt) ## Features - Generate synthetic financial datasets using
+LLMs - Supports various SEC filings (10-Ks, 10-Qs, etc.) - Easy integration
+with Python projects - Customizable data generation options Example dataset:
+```json [ { "question": "What was Airbnb's revenue in 2023?", "answer": "$9.9
+billion", "context": "In 2023, revenue increased by 18% to $9.9 billion
+compared to 2022, primarily due to a 14% increase in Nights and Experiences
+Booked of 54.5 million combined with higher average daily rates driving a 16%
+increase in Gross Booking Value of $10.0 billion." }, { "question": "By what
+percentage did Airbnb's net income increase in 2023 compared to the prior
+year?", "answer": "153%", "context": "Net income in 2023 increased by 153% to
+$4.8 billion, compared to the prior year, driven by our revenue growth,
+increased interest income, discipline in managing our cost structure, and the
+release of a portion of our valuation allowance on deferred tax assets of $2.9
+billion." } ] ``` ## Installation ### Using pip You can install the Financial
+Datasets library using pip: ``` pip install financial-datasets ``` ### Using
+Poetry If you prefer to use Poetry for dependency management, you can add
+Financial Datasets to your project: ``` poetry add financial-datasets ``` ###
+From the Repository If you want to install the library directly from the
+repository, follow these steps: 1. Clone the repository: ``` git clone https://
+github.com/yourusername/financial-datasets.git ``` 2. Navigate to the project
+directory: ``` cd financial-datasets ``` 3. Install the dependencies using
+Poetry: ``` poetry install ``` 4. You can now use the library in your Python
+projects. ## Usage Here's a simple example of how to use the Financial Datasets
+library: ```python # TODO - coming soon ``` ## Contributing Contributions are
+welcome! If you find any issues or have suggestions for improvements, please
+open an issue or submit a pull request. ## License This project is licensed
+under the [MIT License](link-to-license-file). ## Contributors_[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_i_r_a_t_t_t_/_f_i_n_a_n_c_i_a_l_-_d_a_t_a_s_e_t_s_]
```

