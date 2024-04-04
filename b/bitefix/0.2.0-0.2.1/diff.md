# Comparing `tmp/bitefix-0.2.0.tar.gz` & `tmp/bitefix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitefix-0.2.0.tar", last modified: Sat Mar 23 06:51:05 2024, max compression
+gzip compressed data, was "bitefix-0.2.1.tar", last modified: Thu Apr  4 05:47:35 2024, max compression
```

## Comparing `bitefix-0.2.0.tar` & `bitefix-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:51:05.808290 bitefix-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-23 06:49:59.000000 bitefix-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-03-23 06:51:05.808290 bitefix-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-03-23 06:49:59.000000 bitefix-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:51:05.808290 bitefix-0.2.0/bitefix/
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-03-23 06:51:02.000000 bitefix-0.2.0/bitefix/BiteFixAIAgents.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-23 06:51:02.000000 bitefix-0.2.0/bitefix/BiteFixAICrew.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-23 06:51:02.000000 bitefix-0.2.0/bitefix/BiteFixAIRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-23 06:51:02.000000 bitefix-0.2.0/bitefix/BiteFixAITasks.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-23 06:49:59.000000 bitefix-0.2.0/bitefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-03-23 06:49:59.000000 bitefix-0.2.0/bitefix/bitefix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:51:05.808290 bitefix-0.2.0/bitefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-03-23 06:51:05.000000 bitefix-0.2.0/bitefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-23 06:51:05.000000 bitefix-0.2.0/bitefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 06:51:05.000000 bitefix-0.2.0/bitefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-23 06:51:05.000000 bitefix-0.2.0/bitefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-23 06:51:05.000000 bitefix-0.2.0/bitefix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-23 06:51:05.808290 bitefix-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-23 06:49:59.000000 bitefix-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:34.996323 bitefix-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 05:46:36.000000 bitefix-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-04 05:47:34.996323 bitefix-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-04 05:46:36.000000 bitefix-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:34.996323 bitefix-0.2.1/bitefix/
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAIAgents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAICrew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAIRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAITasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 05:46:36.000000 bitefix-0.2.1/bitefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-04 05:46:36.000000 bitefix-0.2.1/bitefix/bitefix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:34.996323 bitefix-0.2.1/bitefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 05:47:34.996323 bitefix-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-04 05:46:36.000000 bitefix-0.2.1/setup.py
```

### Comparing `bitefix-0.2.0/LICENSE` & `bitefix-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.0/PKG-INFO` & `bitefix-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,26 @@
-Metadata-Version: 2.1
-Name: bitefix
-Version: 0.2.0
-Summary: Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
-Home-page: https://github.com/Pallavi-Sinha-12/bitefix
-Author: Pallavi Sinha
-Author-email: dataaienthusiast128@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: crewai==0.14.4
-Requires-Dist: langchain==0.1.9
-Requires-Dist: crewai-tools==0.0.12
-
 # BiteFix 🛠️
 
 ![Last commit](https://img.shields.io/github/last-commit/Pallavi-Sinha-12/bitefix?color=green&label=Last%20commit)
 ![Repo size](https://img.shields.io/github/repo-size/Pallavi-Sinha-12/bitefix?color=orange&label=Repo%20size)
 [![Stars](https://img.shields.io/github/stars/Pallavi-Sinha-12/bitefix?color=yellow&label=Stars)](https://github.com/Pallavi-Sinha-12/Expense-Tracker-Chatbot/stargazers)
 [![Forks](https://img.shields.io/github/forks/Pallavi-Sinha-12/bitefix?color=orange&label=Forks)](https://github.com/Pallavi-Sinha-12/bitefix/forks)
 
 
-BiteFix is an advanced and efficient tool designed to revolutionize the error-fixing process using the capabilities of Large Language Models (LLM). It is a Python library that offers a range of decorators to help you debug your code and fix errors in a matter of seconds.
+BiteFix is an advanced and efficient Python library designed to revolutionize the error-fixing process which leverages multi agents framework concept to provide a seamless debugging experience. It offers decorators to help you debug your code when the function throws runtime errors.
 
 ## Table of Contents 📋
 
 - [Introduction](#Introduction)
 - [Technologies Used](#Technologies-Used)
 - [Getting Started](#Getting-Started)
 - [Examples](#Examples)
 - [Contributing](#Contributing)
 - [Feedback](#Feedback)
+- [Conclusion](#Conclusion)
 - [Contact](#Contact)
 - [License](#License)
 - [References](#References)
 
 ## Introduction
 
 By offering decorators, BiteFix empowers you to enhance the error-handling experience in your functions. When a decorated function encounters an error, the decorator orchestrates a team of AI Agents, each specializing in a unique aspect of error resolution. Here's a brief overview of the AI Agents:
@@ -69,53 +53,61 @@
 
 ## Examples
 
 Let's take a look at some examples to understand how BiteFix works. Bitefix offers two decorators: `@resolve` and `@resolve_with_openai`.
 
 ### Example 1 : Using Open AI Models
 
-Let's say you have a function that is supposed to return longest length of subsequence in a given list. We can use `@resolve_with_openai` decorator with our function to help us resolve the error if the function fails while execution.
+Let's say you have a function that calculates the maximum profit that can be obtained from a given array of stock prices.
+We will use `@resolve_with_openai` decorator with our function to help us resolve the error if some runtime error occurs while executing the function.
 
 ```python
 
 from bitefix import resolve_with_openai
 
-@resolve_with_openai(openai_api_key="YOUR_OPENAI_KEY", model_name="gpt-4", temperature=0.7, export_dir = "export", verbose=True)
-def length_of_lis(nums):
-    if not nums:
-        return 0
-
-    dp = [1] * len(nums)
-
-    for i in range(1, len(nums)):
-        for j in range(i):
-            if nums[i] > nums[j]:
-                dp[i] = dp[i + 1]
+function_description = """
+This function calculates the maximum profit that can be obtained from a given array of stock prices, aiding in financial analysis.
+Stock prices represent daily closing prices of a stock over time, obtained from financial data sources.
+"""
+
+@resolve_with_openai(openai_api_key="YOUR_OPENAI_KEY", model_name="gpt-4", function_description= function_description, export_dir="logs", verbose=True)
+def max_profit(stock_prices):
+
+    min_price = stock_prices[0]
+    max_profit = 0 
+
+    for price in stock_prices[1:]:
+        min_price = min(min_price, price)
+        max_profit = max(max_profit, price - min_price)
 
-    return max(dp)
+    return max_profit
 
 ```
 
 `openai_api_key` : The OpenAI API key to use the OpenAI's model. You can get the API key from [here](https://beta.openai.com/account/api-keys).
-`model_name` : The name of the model to be used. By default, it uses OpenAI's gpt-4 model.
-`temperature` : The temperature parameter for the model. By default, it is set to 0.7.
-`export_dir` : The directory path to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. It will export the report if a directory is provided. By default, it is set to None.
-`verbose` : If set to True, it will print the debugging steps. By default, it is set to True.
+`model_name` (optional) : The name of the model to be used. By default, it uses OpenAI's gpt-4 model.
+`function_description` (optional) : The description of the function to be used to understand the context of the function. By default, it is set to None.
+`temperature` (optional) : The temperature parameter for the model. By default, it is set to 0.7.
+`export_dir` (optional) : The directory path to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. It will export the report if a directory is provided. By default, it is set to None.
+`verbose` (optional) : If set to True, it will print the debugging steps. By default, it is set to True.
 
 Now, let's call the function and see how it works.
 
 ```python
 
-input_list = [10, 9, 2, 5, 3, 7, 101, 18]
-result = length_of_lis(input_list)
-print(result)
+stock_prices = [7, 1, 5, 3, 6, 4, None]
+max_profit = max_profit(stock_prices)
+print("Maximum profit from stock market analysis:", max_profit)
 
 ```
 
-Here is the recorded output of the function execution - [bitefix_decorator_example](https://drive.google.com/file/d/1JKeKCbhwSRkx4MfrVtz1oAtW_n4Up1rN/view?usp=sharing)
+Below is the Error Resolution Report generated by the decorator.
+![Error Resolution Report](assets/max_profit_bitefix_demo.png)
+
+Here is the full demo for the above example - [bitefix_decorator_example](https://drive.google.com/file/d/1_5lOo9HZIhYyenV-Y0WG_TuCVIgTg9hT/view?usp=sharing)
 
 
 We can see how this decorator provided us step by step debugging of the function in case of failure by using crew of Python AI coders. It also provided us with the solution to the error.
 
 ### Example 2 : Using Open Source Models
 
 If we want to use some other Large Language Model instead of OpenAI, we can use `@resolve` decorator with our function to help us resolve the error if the function fails while execution. This helps us to use any custom trained model as well for error resolution.
@@ -133,31 +125,34 @@
 ```python
 
 from bitefix import resolve
 from langchain_community.llms import Ollama
 
 llm = Ollama("openhermes")
 
-@resolve(llm = llm, export_dir = None, verbose=True)
-def length_of_lis(nums):
-    if not nums:
-        return 0
-
-    dp = [1] * len(nums)
-
-    for i in range(1, len(nums)):
-        for j in range(i):
-            if nums[i] > nums[j]:
-                dp[i] = dp[i + 1]
+@resolve_with_openai(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
+def max_profit(stock_prices):
+
+    min_price = stock_prices[0]
+    max_profit = 0 
+
+    for price in stock_prices[1:]:
+        min_price = min(min_price, price)
+        max_profit = max(max_profit, price - min_price)
+
+    return max_profit
+
+stock_prices = [7, 1, 5, 3, 6, 4, None]
+max_profit = max_profit(stock_prices)
+print("Maximum profit from stock market analysis:", max_profit)
 
-    return max(dp)
 
 ```
 
-Note : Here `export_dir` and `verbose` are optional parameters.
+Note : Here `function_description`, `export_dir` and `verbose` are optional parameters.
 
 Similarly, we can use any other Large Language Model with the decorator.
 
 ## Contributing
 
 Contributions are always welcome!
 
@@ -178,14 +173,19 @@
 ## Feedback
 
 'bitefix' library is just a small step towards making the error-fixing process more efficient using the capabilities of Large Language Models. We have to go a long way to make this better.
 Feel free to send me feedback at dataaienthusiast128@gmail.com. Let me know if you have any suggestions on how to make this project better.
 
 If you liked the project support it by giving a star :star: to this repo.
 
+## Conclusion
+
+- BiteFix is a powerful Python library that leverages the capabilities of Large Language Models to streamline the error-fixing process in Python. By offering decorators that orchestrate a team of AI Agents, BiteFix helps you resolve the runtime errors in your code efficiently. 
+- ONE IMPORTANT OBSERVATION IS THAT CURRENTLY BITEFIX SHOWS GOOD RESULTS WITH INDEPENDENT FUNCTIONS. FOR FUNCTIONS WHICH CAN HAVE NESTED FUNCTIONS OR CLASSES, THE RESULTS MAY VARY. IN THOSE CASES, WE CAN CHOOSE TO GIVE THE FUNCTION DESCRIPTION TO THE DECORATOR TO GET BETTER RESULTS.
+
 ## Contact
 [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pallavi-sinha-09540917b/)[![GitHub](https://img.shields.io/badge/GitHub-555555?style=for-the-badge&logo=github&logoColor=white&)](https://github.com/Pallavi-Sinha-12)
 
 ## License
 
 This project is licensed under the terms of the [MIT license](https://choosealicense.com/licenses/mit/)
 
@@ -193,8 +193,8 @@
 
 - crewAI: Cutting-edge framework for orchestrating role-playing, autonomous AI agents. https://github.com/joaomdmoura/crewAI
 
 - langchain: Python library for interacting with the Langchain API. https://api.python.langchain.com/en/latest/langchain_api_reference.html#
 
 - OpenAI: OpenAI is an artificial intelligence research laboratory consisting of the for-profit corporation OpenAI LP and its parent company, the non-profit OpenAI Inc. https://openai.com/
 
-- Ollama: Ollama allows you to run open-source large language models, such as Openhermes, Llama 2, locally. https://ollama.ai/
+- Ollama: Ollama allows you to run open-source large language models, such as Openhermes, Llama 2, locally. https://ollama.ai/
```

### Comparing `bitefix-0.2.0/README.md` & `bitefix-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,44 @@
+Metadata-Version: 2.1
+Name: bitefix
+Version: 0.2.1
+Summary: Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
+Home-page: https://github.com/Pallavi-Sinha-12/bitefix
+Author: Pallavi Sinha
+Author-email: dataaienthusiast128@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: crewai==0.14.4
+Requires-Dist: langchain==0.1.9
+Requires-Dist: crewai-tools==0.0.12
+
 # BiteFix 🛠️
 
 ![Last commit](https://img.shields.io/github/last-commit/Pallavi-Sinha-12/bitefix?color=green&label=Last%20commit)
 ![Repo size](https://img.shields.io/github/repo-size/Pallavi-Sinha-12/bitefix?color=orange&label=Repo%20size)
 [![Stars](https://img.shields.io/github/stars/Pallavi-Sinha-12/bitefix?color=yellow&label=Stars)](https://github.com/Pallavi-Sinha-12/Expense-Tracker-Chatbot/stargazers)
 [![Forks](https://img.shields.io/github/forks/Pallavi-Sinha-12/bitefix?color=orange&label=Forks)](https://github.com/Pallavi-Sinha-12/bitefix/forks)
 
 
-BiteFix is an advanced and efficient tool designed to revolutionize the error-fixing process using the capabilities of Large Language Models (LLM). It is a Python library that offers a range of decorators to help you debug your code and fix errors in a matter of seconds.
+BiteFix is an advanced and efficient Python library designed to revolutionize the error-fixing process which leverages multi agents framework concept to provide a seamless debugging experience. It offers decorators to help you debug your code when the function throws runtime errors.
 
 ## Table of Contents 📋
 
 - [Introduction](#Introduction)
 - [Technologies Used](#Technologies-Used)
 - [Getting Started](#Getting-Started)
 - [Examples](#Examples)
 - [Contributing](#Contributing)
 - [Feedback](#Feedback)
+- [Conclusion](#Conclusion)
 - [Contact](#Contact)
 - [License](#License)
 - [References](#References)
 
 ## Introduction
 
 By offering decorators, BiteFix empowers you to enhance the error-handling experience in your functions. When a decorated function encounters an error, the decorator orchestrates a team of AI Agents, each specializing in a unique aspect of error resolution. Here's a brief overview of the AI Agents:
@@ -52,53 +71,61 @@
 
 ## Examples
 
 Let's take a look at some examples to understand how BiteFix works. Bitefix offers two decorators: `@resolve` and `@resolve_with_openai`.
 
 ### Example 1 : Using Open AI Models
 
-Let's say you have a function that is supposed to return longest length of subsequence in a given list. We can use `@resolve_with_openai` decorator with our function to help us resolve the error if the function fails while execution.
+Let's say you have a function that calculates the maximum profit that can be obtained from a given array of stock prices.
+We will use `@resolve_with_openai` decorator with our function to help us resolve the error if some runtime error occurs while executing the function.
 
 ```python
 
 from bitefix import resolve_with_openai
 
-@resolve_with_openai(openai_api_key="YOUR_OPENAI_KEY", model_name="gpt-4", temperature=0.7, export_dir = "export", verbose=True)
-def length_of_lis(nums):
-    if not nums:
-        return 0
-
-    dp = [1] * len(nums)
-
-    for i in range(1, len(nums)):
-        for j in range(i):
-            if nums[i] > nums[j]:
-                dp[i] = dp[i + 1]
+function_description = """
+This function calculates the maximum profit that can be obtained from a given array of stock prices, aiding in financial analysis.
+Stock prices represent daily closing prices of a stock over time, obtained from financial data sources.
+"""
+
+@resolve_with_openai(openai_api_key="YOUR_OPENAI_KEY", model_name="gpt-4", function_description= function_description, export_dir="logs", verbose=True)
+def max_profit(stock_prices):
+
+    min_price = stock_prices[0]
+    max_profit = 0 
+
+    for price in stock_prices[1:]:
+        min_price = min(min_price, price)
+        max_profit = max(max_profit, price - min_price)
 
-    return max(dp)
+    return max_profit
 
 ```
 
 `openai_api_key` : The OpenAI API key to use the OpenAI's model. You can get the API key from [here](https://beta.openai.com/account/api-keys).
-`model_name` : The name of the model to be used. By default, it uses OpenAI's gpt-4 model.
-`temperature` : The temperature parameter for the model. By default, it is set to 0.7.
-`export_dir` : The directory path to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. It will export the report if a directory is provided. By default, it is set to None.
-`verbose` : If set to True, it will print the debugging steps. By default, it is set to True.
+`model_name` (optional) : The name of the model to be used. By default, it uses OpenAI's gpt-4 model.
+`function_description` (optional) : The description of the function to be used to understand the context of the function. By default, it is set to None.
+`temperature` (optional) : The temperature parameter for the model. By default, it is set to 0.7.
+`export_dir` (optional) : The directory path to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. It will export the report if a directory is provided. By default, it is set to None.
+`verbose` (optional) : If set to True, it will print the debugging steps. By default, it is set to True.
 
 Now, let's call the function and see how it works.
 
 ```python
 
-input_list = [10, 9, 2, 5, 3, 7, 101, 18]
-result = length_of_lis(input_list)
-print(result)
+stock_prices = [7, 1, 5, 3, 6, 4, None]
+max_profit = max_profit(stock_prices)
+print("Maximum profit from stock market analysis:", max_profit)
 
 ```
 
-Here is the recorded output of the function execution - [bitefix_decorator_example](https://drive.google.com/file/d/1JKeKCbhwSRkx4MfrVtz1oAtW_n4Up1rN/view?usp=sharing)
+Below is the Error Resolution Report generated by the decorator.
+![Error Resolution Report](assets/max_profit_bitefix_demo.png)
+
+Here is the full demo for the above example - [bitefix_decorator_example](https://drive.google.com/file/d/1_5lOo9HZIhYyenV-Y0WG_TuCVIgTg9hT/view?usp=sharing)
 
 
 We can see how this decorator provided us step by step debugging of the function in case of failure by using crew of Python AI coders. It also provided us with the solution to the error.
 
 ### Example 2 : Using Open Source Models
 
 If we want to use some other Large Language Model instead of OpenAI, we can use `@resolve` decorator with our function to help us resolve the error if the function fails while execution. This helps us to use any custom trained model as well for error resolution.
@@ -116,31 +143,34 @@
 ```python
 
 from bitefix import resolve
 from langchain_community.llms import Ollama
 
 llm = Ollama("openhermes")
 
-@resolve(llm = llm, export_dir = None, verbose=True)
-def length_of_lis(nums):
-    if not nums:
-        return 0
-
-    dp = [1] * len(nums)
-
-    for i in range(1, len(nums)):
-        for j in range(i):
-            if nums[i] > nums[j]:
-                dp[i] = dp[i + 1]
+@resolve_with_openai(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
+def max_profit(stock_prices):
+
+    min_price = stock_prices[0]
+    max_profit = 0 
+
+    for price in stock_prices[1:]:
+        min_price = min(min_price, price)
+        max_profit = max(max_profit, price - min_price)
+
+    return max_profit
+
+stock_prices = [7, 1, 5, 3, 6, 4, None]
+max_profit = max_profit(stock_prices)
+print("Maximum profit from stock market analysis:", max_profit)
 
-    return max(dp)
 
 ```
 
-Note : Here `export_dir` and `verbose` are optional parameters.
+Note : Here `function_description`, `export_dir` and `verbose` are optional parameters.
 
 Similarly, we can use any other Large Language Model with the decorator.
 
 ## Contributing
 
 Contributions are always welcome!
 
@@ -161,14 +191,19 @@
 ## Feedback
 
 'bitefix' library is just a small step towards making the error-fixing process more efficient using the capabilities of Large Language Models. We have to go a long way to make this better.
 Feel free to send me feedback at dataaienthusiast128@gmail.com. Let me know if you have any suggestions on how to make this project better.
 
 If you liked the project support it by giving a star :star: to this repo.
 
+## Conclusion
+
+- BiteFix is a powerful Python library that leverages the capabilities of Large Language Models to streamline the error-fixing process in Python. By offering decorators that orchestrate a team of AI Agents, BiteFix helps you resolve the runtime errors in your code efficiently. 
+- ONE IMPORTANT OBSERVATION IS THAT CURRENTLY BITEFIX SHOWS GOOD RESULTS WITH INDEPENDENT FUNCTIONS. FOR FUNCTIONS WHICH CAN HAVE NESTED FUNCTIONS OR CLASSES, THE RESULTS MAY VARY. IN THOSE CASES, WE CAN CHOOSE TO GIVE THE FUNCTION DESCRIPTION TO THE DECORATOR TO GET BETTER RESULTS.
+
 ## Contact
 [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pallavi-sinha-09540917b/)[![GitHub](https://img.shields.io/badge/GitHub-555555?style=for-the-badge&logo=github&logoColor=white&)](https://github.com/Pallavi-Sinha-12)
 
 ## License
 
 This project is licensed under the terms of the [MIT license](https://choosealicense.com/licenses/mit/)
 
@@ -176,8 +211,8 @@
 
 - crewAI: Cutting-edge framework for orchestrating role-playing, autonomous AI agents. https://github.com/joaomdmoura/crewAI
 
 - langchain: Python library for interacting with the Langchain API. https://api.python.langchain.com/en/latest/langchain_api_reference.html#
 
 - OpenAI: OpenAI is an artificial intelligence research laboratory consisting of the for-profit corporation OpenAI LP and its parent company, the non-profit OpenAI Inc. https://openai.com/
 
-- Ollama: Ollama allows you to run open-source large language models, such as Openhermes, Llama 2, locally. https://ollama.ai/
+- Ollama: Ollama allows you to run open-source large language models, such as Openhermes, Llama 2, locally. https://ollama.ai/
```

### Comparing `bitefix-0.2.0/bitefix/BiteFixAIAgents.py` & `bitefix-0.2.1/bitefix/BiteFixAIAgents.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.0/bitefix/BiteFixAICrew.py` & `bitefix-0.2.1/bitefix/BiteFixAICrew.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.0/bitefix/BiteFixAIRunner.py` & `bitefix-0.2.1/bitefix/BiteFixAIRunner.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.0/bitefix/BiteFixAITasks.py` & `bitefix-0.2.1/bitefix/BiteFixAITasks.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.0/bitefix/bitefix_utils.py` & `bitefix-0.2.1/bitefix/bitefix_utils.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.0/bitefix.egg-info/PKG-INFO` & `bitefix-0.2.1/bitefix.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: bitefix
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
 Home-page: https://github.com/Pallavi-Sinha-12/bitefix
 Author: Pallavi Sinha
 Author-email: dataaienthusiast128@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crewai==0.14.4
 Requires-Dist: langchain==0.1.9
 Requires-Dist: crewai-tools==0.0.12
 
 # BiteFix 🛠️
 
 ![Last commit](https://img.shields.io/github/last-commit/Pallavi-Sinha-12/bitefix?color=green&label=Last%20commit)
 ![Repo size](https://img.shields.io/github/repo-size/Pallavi-Sinha-12/bitefix?color=orange&label=Repo%20size)
 [![Stars](https://img.shields.io/github/stars/Pallavi-Sinha-12/bitefix?color=yellow&label=Stars)](https://github.com/Pallavi-Sinha-12/Expense-Tracker-Chatbot/stargazers)
 [![Forks](https://img.shields.io/github/forks/Pallavi-Sinha-12/bitefix?color=orange&label=Forks)](https://github.com/Pallavi-Sinha-12/bitefix/forks)
 
 
-BiteFix is an advanced and efficient tool designed to revolutionize the error-fixing process using the capabilities of Large Language Models (LLM). It is a Python library that offers a range of decorators to help you debug your code and fix errors in a matter of seconds.
+BiteFix is an advanced and efficient Python library designed to revolutionize the error-fixing process which leverages multi agents framework concept to provide a seamless debugging experience. It offers decorators to help you debug your code when the function throws runtime errors.
 
 ## Table of Contents 📋
 
 - [Introduction](#Introduction)
 - [Technologies Used](#Technologies-Used)
 - [Getting Started](#Getting-Started)
 - [Examples](#Examples)
 - [Contributing](#Contributing)
 - [Feedback](#Feedback)
+- [Conclusion](#Conclusion)
 - [Contact](#Contact)
 - [License](#License)
 - [References](#References)
 
 ## Introduction
 
 By offering decorators, BiteFix empowers you to enhance the error-handling experience in your functions. When a decorated function encounters an error, the decorator orchestrates a team of AI Agents, each specializing in a unique aspect of error resolution. Here's a brief overview of the AI Agents:
@@ -69,53 +71,61 @@
 
 ## Examples
 
 Let's take a look at some examples to understand how BiteFix works. Bitefix offers two decorators: `@resolve` and `@resolve_with_openai`.
 
 ### Example 1 : Using Open AI Models
 
-Let's say you have a function that is supposed to return longest length of subsequence in a given list. We can use `@resolve_with_openai` decorator with our function to help us resolve the error if the function fails while execution.
+Let's say you have a function that calculates the maximum profit that can be obtained from a given array of stock prices.
+We will use `@resolve_with_openai` decorator with our function to help us resolve the error if some runtime error occurs while executing the function.
 
 ```python
 
 from bitefix import resolve_with_openai
 
-@resolve_with_openai(openai_api_key="YOUR_OPENAI_KEY", model_name="gpt-4", temperature=0.7, export_dir = "export", verbose=True)
-def length_of_lis(nums):
-    if not nums:
-        return 0
-
-    dp = [1] * len(nums)
-
-    for i in range(1, len(nums)):
-        for j in range(i):
-            if nums[i] > nums[j]:
-                dp[i] = dp[i + 1]
+function_description = """
+This function calculates the maximum profit that can be obtained from a given array of stock prices, aiding in financial analysis.
+Stock prices represent daily closing prices of a stock over time, obtained from financial data sources.
+"""
+
+@resolve_with_openai(openai_api_key="YOUR_OPENAI_KEY", model_name="gpt-4", function_description= function_description, export_dir="logs", verbose=True)
+def max_profit(stock_prices):
+
+    min_price = stock_prices[0]
+    max_profit = 0 
+
+    for price in stock_prices[1:]:
+        min_price = min(min_price, price)
+        max_profit = max(max_profit, price - min_price)
 
-    return max(dp)
+    return max_profit
 
 ```
 
 `openai_api_key` : The OpenAI API key to use the OpenAI's model. You can get the API key from [here](https://beta.openai.com/account/api-keys).
-`model_name` : The name of the model to be used. By default, it uses OpenAI's gpt-4 model.
-`temperature` : The temperature parameter for the model. By default, it is set to 0.7.
-`export_dir` : The directory path to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. It will export the report if a directory is provided. By default, it is set to None.
-`verbose` : If set to True, it will print the debugging steps. By default, it is set to True.
+`model_name` (optional) : The name of the model to be used. By default, it uses OpenAI's gpt-4 model.
+`function_description` (optional) : The description of the function to be used to understand the context of the function. By default, it is set to None.
+`temperature` (optional) : The temperature parameter for the model. By default, it is set to 0.7.
+`export_dir` (optional) : The directory path to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. It will export the report if a directory is provided. By default, it is set to None.
+`verbose` (optional) : If set to True, it will print the debugging steps. By default, it is set to True.
 
 Now, let's call the function and see how it works.
 
 ```python
 
-input_list = [10, 9, 2, 5, 3, 7, 101, 18]
-result = length_of_lis(input_list)
-print(result)
+stock_prices = [7, 1, 5, 3, 6, 4, None]
+max_profit = max_profit(stock_prices)
+print("Maximum profit from stock market analysis:", max_profit)
 
 ```
 
-Here is the recorded output of the function execution - [bitefix_decorator_example](https://drive.google.com/file/d/1JKeKCbhwSRkx4MfrVtz1oAtW_n4Up1rN/view?usp=sharing)
+Below is the Error Resolution Report generated by the decorator.
+![Error Resolution Report](assets/max_profit_bitefix_demo.png)
+
+Here is the full demo for the above example - [bitefix_decorator_example](https://drive.google.com/file/d/1_5lOo9HZIhYyenV-Y0WG_TuCVIgTg9hT/view?usp=sharing)
 
 
 We can see how this decorator provided us step by step debugging of the function in case of failure by using crew of Python AI coders. It also provided us with the solution to the error.
 
 ### Example 2 : Using Open Source Models
 
 If we want to use some other Large Language Model instead of OpenAI, we can use `@resolve` decorator with our function to help us resolve the error if the function fails while execution. This helps us to use any custom trained model as well for error resolution.
@@ -133,31 +143,34 @@
 ```python
 
 from bitefix import resolve
 from langchain_community.llms import Ollama
 
 llm = Ollama("openhermes")
 
-@resolve(llm = llm, export_dir = None, verbose=True)
-def length_of_lis(nums):
-    if not nums:
-        return 0
-
-    dp = [1] * len(nums)
-
-    for i in range(1, len(nums)):
-        for j in range(i):
-            if nums[i] > nums[j]:
-                dp[i] = dp[i + 1]
+@resolve_with_openai(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
+def max_profit(stock_prices):
+
+    min_price = stock_prices[0]
+    max_profit = 0 
+
+    for price in stock_prices[1:]:
+        min_price = min(min_price, price)
+        max_profit = max(max_profit, price - min_price)
+
+    return max_profit
+
+stock_prices = [7, 1, 5, 3, 6, 4, None]
+max_profit = max_profit(stock_prices)
+print("Maximum profit from stock market analysis:", max_profit)
 
-    return max(dp)
 
 ```
 
-Note : Here `export_dir` and `verbose` are optional parameters.
+Note : Here `function_description`, `export_dir` and `verbose` are optional parameters.
 
 Similarly, we can use any other Large Language Model with the decorator.
 
 ## Contributing
 
 Contributions are always welcome!
 
@@ -178,14 +191,19 @@
 ## Feedback
 
 'bitefix' library is just a small step towards making the error-fixing process more efficient using the capabilities of Large Language Models. We have to go a long way to make this better.
 Feel free to send me feedback at dataaienthusiast128@gmail.com. Let me know if you have any suggestions on how to make this project better.
 
 If you liked the project support it by giving a star :star: to this repo.
 
+## Conclusion
+
+- BiteFix is a powerful Python library that leverages the capabilities of Large Language Models to streamline the error-fixing process in Python. By offering decorators that orchestrate a team of AI Agents, BiteFix helps you resolve the runtime errors in your code efficiently. 
+- ONE IMPORTANT OBSERVATION IS THAT CURRENTLY BITEFIX SHOWS GOOD RESULTS WITH INDEPENDENT FUNCTIONS. FOR FUNCTIONS WHICH CAN HAVE NESTED FUNCTIONS OR CLASSES, THE RESULTS MAY VARY. IN THOSE CASES, WE CAN CHOOSE TO GIVE THE FUNCTION DESCRIPTION TO THE DECORATOR TO GET BETTER RESULTS.
+
 ## Contact
 [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pallavi-sinha-09540917b/)[![GitHub](https://img.shields.io/badge/GitHub-555555?style=for-the-badge&logo=github&logoColor=white&)](https://github.com/Pallavi-Sinha-12)
 
 ## License
 
 This project is licensed under the terms of the [MIT license](https://choosealicense.com/licenses/mit/)
```

### Comparing `bitefix-0.2.0/setup.py` & `bitefix-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="bitefix",
-    version="0.2.0",
+    version="0.2.1",
     description="""Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
     It initializes a crew of AI agents which work together to diagnose the error, generate ideas to fix the error, 
     evaluate the ideas to choose the best and develop the code to fix the error.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pallavi Sinha",
     packages=find_packages(include=["bitefix"]),
@@ -20,8 +20,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=required,
     license="MIT",
     url="https://github.com/Pallavi-Sinha-12/bitefix",
+    python_requires=">=3.11",
 )
```

