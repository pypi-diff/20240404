# Comparing `tmp/rulexai-1.0.0.tar.gz` & `tmp/rulexai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rulexai-1.0.0.tar", last modified: Wed Apr 13 12:09:50 2022, max compression
+gzip compressed data, was "rulexai-1.1.0.tar", last modified: Thu Apr  4 10:15:40 2024, max compression
```

## Comparing `rulexai-1.0.0.tar` & `rulexai-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-04-13 12:09:50.015381 rulexai-1.0.0/
--rw-rw-rw-   0        0        0    35184 2022-04-13 08:47:13.000000 rulexai-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3399 2022-04-13 12:09:50.016381 rulexai-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2022-04-12 08:25:06.000000 rulexai-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-04-13 12:09:49.909378 rulexai-1.0.0/rulexai/
--rw-rw-rw-   0        0        0       21 2022-04-13 09:53:26.000000 rulexai-1.0.0/rulexai/__init__.py
--rw-rw-rw-   0        0        0    25154 2022-04-08 14:49:02.000000 rulexai-1.0.0/rulexai/explainer.py
--rw-rw-rw-   0        0        0    21826 2022-03-29 14:01:07.000000 rulexai-1.0.0/rulexai/importances.py
--rw-rw-rw-   0        0        0    23963 2022-04-05 11:47:32.000000 rulexai-1.0.0/rulexai/models.py
--rw-rw-rw-   0        0        0     4133 2022-03-10 09:35:36.000000 rulexai-1.0.0/rulexai/reduct.py
--rw-rw-rw-   0        0        0    17468 2022-03-29 13:24:13.000000 rulexai-1.0.0/rulexai/rule.py
-drwxrwxrwx   0        0        0        0 2022-04-13 12:09:50.012381 rulexai-1.0.0/rulexai.egg-info/
--rw-rw-rw-   0        0        0     3399 2022-04-13 12:09:49.000000 rulexai-1.0.0/rulexai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2022-04-13 12:09:49.000000 rulexai-1.0.0/rulexai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-13 12:09:49.000000 rulexai-1.0.0/rulexai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-04-13 12:09:49.000000 rulexai-1.0.0/rulexai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-04-13 12:09:49.000000 rulexai-1.0.0/rulexai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-04-13 12:09:50.025463 rulexai-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1455 2022-04-13 09:59:32.000000 rulexai-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:15:40.398352 rulexai-1.1.0/
+-rw-rw-rw-   0        0        0    35184 2024-04-04 10:04:08.000000 rulexai-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4341 2024-04-04 10:15:40.398352 rulexai-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3272 2024-04-04 10:04:08.000000 rulexai-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:15:40.381350 rulexai-1.1.0/rulexai/
+-rw-rw-rw-   0        0        0       21 2024-04-04 10:04:08.000000 rulexai-1.1.0/rulexai/__init__.py
+-rw-rw-rw-   0        0        0    25154 2024-04-04 10:04:08.000000 rulexai-1.1.0/rulexai/explainer.py
+-rw-rw-rw-   0        0        0    21826 2024-04-04 10:04:08.000000 rulexai-1.1.0/rulexai/importances.py
+-rw-rw-rw-   0        0        0    23887 2024-04-04 10:04:08.000000 rulexai-1.1.0/rulexai/models.py
+-rw-rw-rw-   0        0        0     4133 2024-04-04 10:04:08.000000 rulexai-1.1.0/rulexai/reduct.py
+-rw-rw-rw-   0        0        0    17482 2024-04-04 10:04:08.000000 rulexai-1.1.0/rulexai/rule.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:15:40.396351 rulexai-1.1.0/rulexai.egg-info/
+-rw-rw-rw-   0        0        0     4341 2024-04-04 10:15:40.000000 rulexai-1.1.0/rulexai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2024-04-04 10:15:40.000000 rulexai-1.1.0/rulexai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:15:40.000000 rulexai-1.1.0/rulexai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-04 10:15:40.000000 rulexai-1.1.0/rulexai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 10:15:40.000000 rulexai-1.1.0/rulexai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-04 10:15:40.400351 rulexai-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1495 2024-04-04 10:04:08.000000 rulexai-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:15:40.394351 rulexai-1.1.0/tests/
+-rw-rw-rw-   0        0        0     5169 2024-04-04 10:04:08.000000 rulexai-1.1.0/tests/test_conditions_importances.py
+-rw-rw-rw-   0        0        0     5310 2024-04-04 10:04:08.000000 rulexai-1.1.0/tests/test_functionalities.py
```

### Comparing `rulexai-1.0.0/LICENSE` & `rulexai-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rulexai-1.0.0/PKG-INFO` & `rulexai-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,14 @@
-Metadata-Version: 2.1
-Name: rulexai
-Version: 1.0.0
-Summary: RuleXAI is a rule-based aproach to explain the output of any machine learning model. It is suitable for classification, regression and survival tasks.
-Home-page: https://github.com/adaa-polsl/RuleXAI
-Author: Dawid Macha
-Author-email: dawid.m.macha@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RuleXAI
 
 RuleXAI is a rule-based aproach to explain the output of any machine learning model. It is suitable for classification, regression and survival tasks. 
 
 ## Instalation
 
-RuleXAI can be installed from PyPI
+RuleXAI can be installed from [PyPI](https://pypi.org/project/rulexai/)
 
 ```bash
 pip install rulexai
 ```
 
 Or you can clone the repository and run:
 ```bash
@@ -48,37 +26,38 @@
 
 
 # load iris dataset
 data = load_iris()
 df = pd.DataFrame(data['data'], columns=data['feature_names'])
 df['class'] = data['target']
 
-
 # train a SVM classifier
 X_train,X_test,y_train,y_test = train_test_split(df.drop(columns=["class"]), df["class"], test_size=0.2, random_state=0)
 svm = SVC(kernel='rbf', probability=True)
 svm.fit(X_train, y_train)
-
+predictions = svm.predict(X_train)
+# prepare model predictions to be fed to RuleXAI, remember to change numerical predictions to labels (in this example it is simply converting predictions to a string)
+model_predictions = pd.DataFrame(predictions.astype(str), columns=[y_train.name], index = y_train.index)
 
 # use Explainer to explain model output
-explainer =  Explainer(X = X_train,model_predictions = y_train.astype(str), type = "classification")
+explainer =  Explainer(X = X_train,model_predictions = model_predictions, type = "classification")
 explainer.explain()
+
+print(explainer.condition_importances_)
 ```
 
 ## Sample notebooks
 
-* **[Classification]()**  - in this notebook, the data from https://www.kaggle.com/c/titanic is analysed to show the advantages and possibilities of using the RuleXAI library for in-depth analysis of the dataset for classification task. The use of RuleXAI to explain rule-based and tree-based models was also compared. 
+* **[Classification](https://rulexai.readthedocs.io/en/latest/rst/tutorials/classification.html)**  - in this notebook, the data from https://www.kaggle.com/c/titanic is analysed to show the advantages and possibilities of using the RuleXAI library for in-depth analysis of the dataset for classification task. The use of RuleXAI to explain rule-based and tree-based models was also compared. 
    
-* **[Regression]()** - notebook showing the use of RuleXAI to explain rule-based regression model
+* **[Regression](https://rulexai.readthedocs.io/en/latest/rst/tutorials/regression.html)** - notebook showing the use of RuleXAI to explain rule-based regression model
    
-* **[Survival]()** - notebook showing the use of RuleXAI to explain rule-based survival model
+* **[Survival](https://rulexai.readthedocs.io/en/latest/rst/tutorials/survival.html)** - notebook showing the use of RuleXAI to explain rule-based survival model
     
-* **[Black-box model]()** explainability - the purpose of this notebook is to demonstrate the possibility of using RuleXAI to explain any black box models.
+* **[Black-box model](https://rulexai.readthedocs.io/en/latest/rst/tutorials/black-box_model_aproximation.html)** explainability - the purpose of this notebook is to demonstrate the possibility of using RuleXAI to explain any black box models.
      
-* **[Transformation]()** - notebook showing the use of RuleXAI to transform a dataset. Often datasets contain missing values and nominal values. Most available algorithms do not support either missing values or nominal values. Many algorithms require the data to be rescaled beforehand. The RuleXAI library is able to convert a dataset with nominal and missing values into a binary dataset containing as attributes the conditions describing the dataset and as values “1” when the condition is satisfied for the example and “0” when the condition is not satisfied.
+* **[Transformation](https://rulexai.readthedocs.io/en/latest/rst/tutorials/dataset_transformation.html)** - notebook showing the use of RuleXAI to transform a dataset. Often datasets contain missing values and nominal values. Most available algorithms do not support either missing values or nominal values. Many algorithms require the data to be rescaled beforehand. The RuleXAI library is able to convert a dataset with nominal and missing values into a binary dataset containing as attributes the conditions describing the dataset and as values “1” when the condition is satisfied for the example and “0” when the condition is not satisfied.
    
 
 ## Documentation
-Full documentation is available [here]()
-
-
+Full documentation is available [here](https://rulexai.readthedocs.io/en/latest/index.html)
```

### Comparing `rulexai-1.0.0/rulexai/explainer.py` & `rulexai-1.1.0/rulexai/explainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,15 @@
             label_name = y.columns[0]
         else:
             label_name = y.name
 
         if type == "regression":
             model = RegressionModel(model = model, feature_names= X.columns, label_name=label_name)
         elif type == "survival":
-            model = SurvivalModel(model=model, fetures_names = X.columns, survival_status_name=label_name)
+            model = SurvivalModel(model=model, feature_names = X.columns, survival_status_name=label_name)
         else:
                                         
             model = ClassificationModel(model = model, feature_names = X.columns, class_names = np.unique(y), label_name = label_name)
 
         super().__init__(model, X, y, type)
 
 class Explainer(BaseExplainer):
```

### Comparing `rulexai-1.0.0/rulexai/importances.py` & `rulexai-1.1.0/rulexai/importances.py`

 * *Files identical despite different names*

### Comparing `rulexai-1.0.0/rulexai/models.py` & `rulexai-1.1.0/rulexai/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from rulekit.operator import BaseOperator
+from rulekit._operator import BaseOperator
 import numpy as np
 from .rule import Rule, CompoundCondition, ElementaryCondition
 from rulekit import RuleKit
 from rulekit.classification import RuleClassifier
 from rulekit.regression import RuleRegressor
 from rulekit.params import Measures
 import pandas as pd
@@ -480,17 +480,17 @@
             else:
                 value = valueset[1:-1]
                 elementaryCondition = ElementaryCondition(attribute, str(value), column_index=self.column_indexes[attribute])
                                           
 
             compoundCondition.add_subcondition(elementaryCondition)
 
-        consequence_att, consequence_value = consequence.split(" = ")
-        consequence_val = consequence_value[1:-1]
-        consequence = ElementaryCondition(consequence_att, consequence_val, column_index=self.column_indexes[attribute])
+        consequence_att = "survival_curve"
+        consequence_val = ""
+        consequence = ElementaryCondition(consequence_att, consequence_val, column_index=0)
 
         return Rule(compoundCondition, consequence)
 
 
 class BlackBoxModel:
     def __init__(self, X_model, model_predictions, type) -> None:
         RuleKit.init()
```

### Comparing `rulexai-1.0.0/rulexai/reduct.py` & `rulexai-1.1.0/rulexai/reduct.py`

 * *Files identical despite different names*

### Comparing `rulexai-1.0.0/rulexai/rule.py` & `rulexai-1.1.0/rulexai/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import enum
 import numpy as np
 from typing import List
-np.warnings.filterwarnings('ignore')
+import warnings
+warnings.filterwarnings('ignore')
 
 # creating enumerations using class
 class LogicalOperator(enum.Enum):
     conjuction = 1
     alternative = 2
```

### Comparing `rulexai-1.0.0/setup.py` & `rulexai-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with io.open(f"{current_path}/README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="rulexai",
-    version="1.0.0",
+    version="1.1.0",
     author="Dawid Macha",
     author_email="dawid.m.macha@gmail.com",
     description="RuleXAI is a rule-based aproach to explain the output of any machine learning model. It is suitable for classification, regression and survival tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adaa-polsl/RuleXAI",
     packages=setuptools.find_packages(),
@@ -26,16 +26,17 @@
         "Operating System :: Unix",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     install_requires=[
-        "pandas ~= 1.2.1",
-        "numpy ~= 1.20.3",
-        "matplotlib ~= 3.4.2",
-        "rulekit ~= 1.6.0",
+        "pandas >= 1.5.0, < 2.3.0",
+        "numpy ~= 1.26.4",
+        "matplotlib ~= 3.8.3",
+        "rulekit ~= 1.7.6",
+        "lifelines ~= 0.28.0"
     ],
     test_suite="tests",
 )
```

