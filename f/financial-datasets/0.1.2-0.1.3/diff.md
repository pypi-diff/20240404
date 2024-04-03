# Comparing `tmp/financial_datasets-0.1.2.tar.gz` & `tmp/financial_datasets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.2.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.3.tar", max compression
```

## Comparing `financial_datasets-0.1.2.tar` & `financial_datasets-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.2/LICENSE
--rw-r--r--   0        0        0     2700 2024-03-30 23:21:00.793310 financial_datasets-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.2/financial_datasets/__init__.py
--rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.2/financial_datasets/dataset.py
--rw-r--r--   0        0        0     3763 2024-04-03 18:32:20.963494 financial_datasets-0.1.2/financial_datasets/generator.py
--rw-r--r--   0        0        0      282 2024-03-30 22:53:11.228502 financial_datasets-0.1.2/financial_datasets/model.py
--rw-r--r--   0        0        0      619 2024-04-03 22:15:32.555865 financial_datasets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 financial_datasets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3089 2024-04-03 22:32:30.744861 financial_datasets-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.3/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.3/financial_datasets/dataset.py
+-rw-r--r--   0        0        0     3772 2024-04-03 22:24:59.390489 financial_datasets-0.1.3/financial_datasets/generator.py
+-rw-r--r--   0        0        0      619 2024-04-03 22:35:41.133840 financial_datasets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 financial_datasets-0.1.3/PKG-INFO
```

### Comparing `financial_datasets-0.1.2/LICENSE` & `financial_datasets-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.2/README.md` & `financial_datasets-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,30 @@
 ## Features
 
 - Generate synthetic financial datasets using LLMs
 - Supports various SEC filings (10-Ks, 10-Qs, etc.)
 - Easy integration with Python projects
 - Customizable data generation options
 
-Example dataset:
+## Usage
+
+**Example code:**
+```python
+import os
+from financial_datasets.generator import DatasetGenerator
+
+texts = ...  # List of texts from SEC filing
+generator = DatasetGenerator(
+   model="gpt-4-0125-preview",
+   api_key=os.environ["OPENAI_API_KEY"],
+)
+dataset = generator.generate_from_texts(texts, max_questions=100)
+```
+
+**Example generated dataset:**
 ```json
 [
   {
     "question": "What was Airbnb's revenue in 2023?",
     "answer": "$9.9 billion",
     "context": "In 2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due to a 14% increase in Nights and Experiences Booked of 54.5 million combined with higher average daily rates driving a 16% increase in Gross Booking Value of $10.0 billion."
   },
@@ -27,14 +42,15 @@
     "question": "By what percentage did Airbnb's net income increase in 2023 compared to the prior year?",
     "answer": "153%",
     "context": "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior year, driven by our revenue growth, increased interest income, discipline in managing our cost structure, and the release of a portion of our valuation allowance on deferred tax assets of $2.9 billion."
   }
 ]
 ```
 
+A full end-to-end code example can be found [here](https://colab.research.google.com/gist/virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb).
 ## Installation
 
 ### Using pip
 
 You can install the Financial Datasets library using pip:
 
 ```
@@ -65,21 +81,14 @@
    
 3. Install the dependencies using Poetry:
    ```
    poetry install
    ```
 
 4. You can now use the library in your Python projects.
-## Usage
-
-Here's a simple example of how to use the Financial Datasets library:
-
-```python
-# TODO - coming soon
-```
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements, 
 please open an issue or submit a pull request.
 
 ## License
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
 # Financial Datasets Financial Datasets is an open-source Python library that
 allows developers to create synthetic financial datasets using Large Language
 Models (LLMs). With this library, you can generate realistic financial datasets
 based on SEC filings such as 10-Ks, 10-Qs, and other financial reports. [!
 [Twitter Follow](https://img.shields.io/twitter/follow/virattt?style=social)]
 (https://twitter.com/virattt) ## Features - Generate synthetic financial
 datasets using LLMs - Supports various SEC filings (10-Ks, 10-Qs, etc.) - Easy
-integration with Python projects - Customizable data generation options Example
-dataset: ```json [ { "question": "What was Airbnb's revenue in 2023?",
-"answer": "$9.9 billion", "context": "In 2023, revenue increased by 18% to $9.9
-billion compared to 2022, primarily due to a 14% increase in Nights and
-Experiences Booked of 54.5 million combined with higher average daily rates
-driving a 16% increase in Gross Booking Value of $10.0 billion." },
-{ "question": "By what percentage did Airbnb's net income increase in 2023
-compared to the prior year?", "answer": "153%", "context": "Net income in 2023
-increased by 153% to $4.8 billion, compared to the prior year, driven by our
-revenue growth, increased interest income, discipline in managing our cost
-structure, and the release of a portion of our valuation allowance on deferred
-tax assets of $2.9 billion." } ] ``` ## Installation ### Using pip You can
-install the Financial Datasets library using pip: ``` pip install financial-
-datasets ``` ### Using Poetry If you prefer to use Poetry for dependency
-management, you can add Financial Datasets to your project: ``` poetry add
-financial-datasets ``` ### From the Repository If you want to install the
-library directly from the repository, follow these steps: 1. Clone the
-repository: ``` git clone https://github.com/yourusername/financial-
-datasets.git ``` 2. Navigate to the project directory: ``` cd financial-
-datasets ``` 3. Install the dependencies using Poetry: ``` poetry install ```
-4. You can now use the library in your Python projects. ## Usage Here's a
-simple example of how to use the Financial Datasets library: ```python # TODO -
-coming soon ``` ## Contributing Contributions are welcome! If you find any
-issues or have suggestions for improvements, please open an issue or submit a
-pull request. ## License This project is licensed under the [MIT License](link-
-to-license-file). ## Contributors_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_i_r_a_t_t_t_/
-_f_i_n_a_n_c_i_a_l_-_d_a_t_a_s_e_t_s_]
+integration with Python projects - Customizable data generation options ##
+Usage **Example code:** ```python import os from financial_datasets.generator
+import DatasetGenerator texts = ... # List of texts from SEC filing generator =
+DatasetGenerator( model="gpt-4-0125-preview", api_key=os.environ
+["OPENAI_API_KEY"], ) dataset = generator.generate_from_texts(texts,
+max_questions=100) ``` **Example generated dataset:** ```json [ { "question":
+"What was Airbnb's revenue in 2023?", "answer": "$9.9 billion", "context": "In
+2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due
+to a 14% increase in Nights and Experiences Booked of 54.5 million combined
+with higher average daily rates driving a 16% increase in Gross Booking Value
+of $10.0 billion." }, { "question": "By what percentage did Airbnb's net income
+increase in 2023 compared to the prior year?", "answer": "153%", "context":
+"Net income in 2023 increased by 153% to $4.8 billion, compared to the prior
+year, driven by our revenue growth, increased interest income, discipline in
+managing our cost structure, and the release of a portion of our valuation
+allowance on deferred tax assets of $2.9 billion." } ] ``` A full end-to-end
+code example can be found [here](https://colab.research.google.com/gist/
+virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb). ##
+Installation ### Using pip You can install the Financial Datasets library using
+pip: ``` pip install financial-datasets ``` ### Using Poetry If you prefer to
+use Poetry for dependency management, you can add Financial Datasets to your
+project: ``` poetry add financial-datasets ``` ### From the Repository If you
+want to install the library directly from the repository, follow these steps:
+1. Clone the repository: ``` git clone https://github.com/yourusername/
+financial-datasets.git ``` 2. Navigate to the project directory: ``` cd
+financial-datasets ``` 3. Install the dependencies using Poetry: ``` poetry
+install ``` 4. You can now use the library in your Python projects. ##
+Contributing Contributions are welcome! If you find any issues or have
+suggestions for improvements, please open an issue or submit a pull request. ##
+License This project is licensed under the [MIT License](link-to-license-file).
+## Contributors_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_i_r_a_t_t_t_/_f_i_n_a_n_c_i_a_l_-_d_a_t_a_s_e_t_s_]
```

### Comparing `financial_datasets-0.1.2/financial_datasets/generator.py` & `financial_datasets-0.1.3/financial_datasets/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import List
 from tqdm import tqdm
 
 from instructor import patch
 from openai import OpenAI
 
 from financial_datasets.dataset import DatasetItem, Dataset
-from financial_datasets.model import ModelConfig, ModelProvider
 
 system_prompt = """
 You are an expert at understanding and analyzing financial documents. 
 Your role is to generate question and ground truth answer pairs based on the provided financial text. 
 The types of texts you will be working with include 10-Ks, 10-Qs, earnings call transcripts, and other financial documents.
 
 When generating questions and answers, adhere to the following guidelines:
@@ -24,20 +23,24 @@
    Context: [Relevant paragraph from the text that supports the answer]
 
 Remember, your primary objective is to create accurate, grounded, and contextually relevant question-answer pairs while strictly avoiding any fabrication or speculation.
 """
 
 
 class DatasetGenerator:
-    def __init__(self, model_config: ModelConfig):
-        if model_config.provider != ModelProvider.OPEN_AI:
-            raise NotImplementedError(f'Provider {model_config.provider} is not supported yet.')
+    def __init__(self, model: str, api_key: str):
+        # Ensure model begins with gpt-
+        if not model.startswith('gpt-'):
+            raise NotImplementedError(f'Model {model} is not supported yet.')
 
-        self._client = patch(OpenAI())
-        self._model_name = model_config.name
+        if not api_key:
+            raise ValueError("API key is required.")
+
+        self._model = model
+        self._client = patch(OpenAI(api_key=api_key))
 
     def generate_from_texts(self, texts: List[str], max_questions=10) -> Dataset:
         items: List[DatasetItem] = []
         num_texts = len(texts)
         questions_per_text = max_questions // num_texts
         remaining_questions = max_questions % num_texts
 
@@ -48,15 +51,15 @@
                 # Determine the number of questions to generate for the current text
                 current_max_questions = questions_per_text
                 if index < remaining_questions:
                     current_max_questions += 1
 
                 # Generate questions
                 response = self._client.chat.completions.create(
-                    model=self._model_name,
+                    model=self._model,
                     response_model=Dataset,
                     messages=[
                         {"role": "system", "content": system_prompt},
                         {"role": "user", "content": f"Generate {current_max_questions} questions for the following block of text: {text}"}
                     ],
                 )
```

### Comparing `financial_datasets-0.1.2/PKG-INFO` & `financial_datasets-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financial-datasets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Financial datasets for LLMs
 License: MIT
 Author: Virat Singh
 Author-email: virat@virat.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,30 @@
 ## Features
 
 - Generate synthetic financial datasets using LLMs
 - Supports various SEC filings (10-Ks, 10-Qs, etc.)
 - Easy integration with Python projects
 - Customizable data generation options
 
-Example dataset:
+## Usage
+
+**Example code:**
+```python
+import os
+from financial_datasets.generator import DatasetGenerator
+
+texts = ...  # List of texts from SEC filing
+generator = DatasetGenerator(
+   model="gpt-4-0125-preview",
+   api_key=os.environ["OPENAI_API_KEY"],
+)
+dataset = generator.generate_from_texts(texts, max_questions=100)
+```
+
+**Example generated dataset:**
 ```json
 [
   {
     "question": "What was Airbnb's revenue in 2023?",
     "answer": "$9.9 billion",
     "context": "In 2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due to a 14% increase in Nights and Experiences Booked of 54.5 million combined with higher average daily rates driving a 16% increase in Gross Booking Value of $10.0 billion."
   },
@@ -50,14 +65,15 @@
     "question": "By what percentage did Airbnb's net income increase in 2023 compared to the prior year?",
     "answer": "153%",
     "context": "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior year, driven by our revenue growth, increased interest income, discipline in managing our cost structure, and the release of a portion of our valuation allowance on deferred tax assets of $2.9 billion."
   }
 ]
 ```
 
+A full end-to-end code example can be found [here](https://colab.research.google.com/gist/virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb).
 ## Installation
 
 ### Using pip
 
 You can install the Financial Datasets library using pip:
 
 ```
@@ -88,21 +104,14 @@
    
 3. Install the dependencies using Poetry:
    ```
    poetry install
    ```
 
 4. You can now use the library in your Python projects.
-## Usage
-
-Here's a simple example of how to use the Financial Datasets library:
-
-```python
-# TODO - coming soon
-```
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements, 
 please open an issue or submit a pull request.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: financial-datasets Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: financial-datasets Version: 0.1.3 Summary:
 Financial datasets for LLMs License: MIT Author: Virat Singh Author-email:
 virat@virat.ai Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist:
 chromadb (>=0.4.24,<0.5.0) Requires-Dist: datasets (>=2.18.0,<3.0.0) Requires-
 Dist: instructor (>=0.6.7,<0.7.0) Requires-Dist: langchain (>=0.1.13,<0.2.0)
@@ -12,33 +12,38 @@
 Financial Datasets is an open-source Python library that allows developers to
 create synthetic financial datasets using Large Language Models (LLMs). With
 this library, you can generate realistic financial datasets based on SEC
 filings such as 10-Ks, 10-Qs, and other financial reports. [![Twitter Follow]
 (https://img.shields.io/twitter/follow/virattt?style=social)](https://
 twitter.com/virattt) ## Features - Generate synthetic financial datasets using
 LLMs - Supports various SEC filings (10-Ks, 10-Qs, etc.) - Easy integration
-with Python projects - Customizable data generation options Example dataset:
-```json [ { "question": "What was Airbnb's revenue in 2023?", "answer": "$9.9
-billion", "context": "In 2023, revenue increased by 18% to $9.9 billion
-compared to 2022, primarily due to a 14% increase in Nights and Experiences
-Booked of 54.5 million combined with higher average daily rates driving a 16%
-increase in Gross Booking Value of $10.0 billion." }, { "question": "By what
-percentage did Airbnb's net income increase in 2023 compared to the prior
-year?", "answer": "153%", "context": "Net income in 2023 increased by 153% to
-$4.8 billion, compared to the prior year, driven by our revenue growth,
-increased interest income, discipline in managing our cost structure, and the
-release of a portion of our valuation allowance on deferred tax assets of $2.9
-billion." } ] ``` ## Installation ### Using pip You can install the Financial
-Datasets library using pip: ``` pip install financial-datasets ``` ### Using
-Poetry If you prefer to use Poetry for dependency management, you can add
-Financial Datasets to your project: ``` poetry add financial-datasets ``` ###
-From the Repository If you want to install the library directly from the
-repository, follow these steps: 1. Clone the repository: ``` git clone https://
-github.com/yourusername/financial-datasets.git ``` 2. Navigate to the project
-directory: ``` cd financial-datasets ``` 3. Install the dependencies using
-Poetry: ``` poetry install ``` 4. You can now use the library in your Python
-projects. ## Usage Here's a simple example of how to use the Financial Datasets
-library: ```python # TODO - coming soon ``` ## Contributing Contributions are
-welcome! If you find any issues or have suggestions for improvements, please
-open an issue or submit a pull request. ## License This project is licensed
-under the [MIT License](link-to-license-file). ## Contributors_[_h_t_t_p_s_:_/_/
-_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_i_r_a_t_t_t_/_f_i_n_a_n_c_i_a_l_-_d_a_t_a_s_e_t_s_]
+with Python projects - Customizable data generation options ## Usage **Example
+code:** ```python import os from financial_datasets.generator import
+DatasetGenerator texts = ... # List of texts from SEC filing generator =
+DatasetGenerator( model="gpt-4-0125-preview", api_key=os.environ
+["OPENAI_API_KEY"], ) dataset = generator.generate_from_texts(texts,
+max_questions=100) ``` **Example generated dataset:** ```json [ { "question":
+"What was Airbnb's revenue in 2023?", "answer": "$9.9 billion", "context": "In
+2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due
+to a 14% increase in Nights and Experiences Booked of 54.5 million combined
+with higher average daily rates driving a 16% increase in Gross Booking Value
+of $10.0 billion." }, { "question": "By what percentage did Airbnb's net income
+increase in 2023 compared to the prior year?", "answer": "153%", "context":
+"Net income in 2023 increased by 153% to $4.8 billion, compared to the prior
+year, driven by our revenue growth, increased interest income, discipline in
+managing our cost structure, and the release of a portion of our valuation
+allowance on deferred tax assets of $2.9 billion." } ] ``` A full end-to-end
+code example can be found [here](https://colab.research.google.com/gist/
+virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb). ##
+Installation ### Using pip You can install the Financial Datasets library using
+pip: ``` pip install financial-datasets ``` ### Using Poetry If you prefer to
+use Poetry for dependency management, you can add Financial Datasets to your
+project: ``` poetry add financial-datasets ``` ### From the Repository If you
+want to install the library directly from the repository, follow these steps:
+1. Clone the repository: ``` git clone https://github.com/yourusername/
+financial-datasets.git ``` 2. Navigate to the project directory: ``` cd
+financial-datasets ``` 3. Install the dependencies using Poetry: ``` poetry
+install ``` 4. You can now use the library in your Python projects. ##
+Contributing Contributions are welcome! If you find any issues or have
+suggestions for improvements, please open an issue or submit a pull request. ##
+License This project is licensed under the [MIT License](link-to-license-file).
+## Contributors_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_i_r_a_t_t_t_/_f_i_n_a_n_c_i_a_l_-_d_a_t_a_s_e_t_s_]
```

