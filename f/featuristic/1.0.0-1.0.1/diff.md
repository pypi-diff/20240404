# Comparing `tmp/featuristic-1.0.0.tar.gz` & `tmp/featuristic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuristic-1.0.0.tar", last modified: Tue Apr  2 20:36:43 2024, max compression
+gzip compressed data, was "featuristic-1.0.1.tar", last modified: Thu Apr  4 19:22:44 2024, max compression
```

## Comparing `featuristic-1.0.0.tar` & `featuristic-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.928841 featuristic-1.0.0/
--rw-r--r--   0 martin     (501) staff       (20)     1054 2024-02-14 09:40:08.000000 featuristic-1.0.0/LICENSE.txt
--rw-r--r--   0 martin     (501) staff       (20)    13544 2024-04-02 20:36:43.928586 featuristic-1.0.0/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     4041 2024-04-02 20:27:28.000000 featuristic-1.0.0/pyproject.toml
--rw-r--r--   0 martin     (501) staff       (20)    10845 2024-04-02 20:33:46.000000 featuristic-1.0.0/readme.md
--rw-r--r--   0 martin     (501) staff       (20)       38 2024-04-02 20:36:43.928900 featuristic-1.0.0/setup.cfg
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.919994 featuristic-1.0.0/src/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.921321 featuristic-1.0.0/src/featuristic/
--rw-r--r--   0 martin     (501) staff       (20)      389 2024-03-29 13:31:43.000000 featuristic-1.0.0/src/featuristic/__init__.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.922458 featuristic-1.0.0/src/featuristic/datasets/
--rw-r--r--   0 martin     (501) staff       (20)       58 2024-03-29 13:31:43.000000 featuristic-1.0.0/src/featuristic/datasets/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      673 2024-03-29 13:31:43.000000 featuristic-1.0.0/src/featuristic/datasets/fetch.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.923651 featuristic-1.0.0/src/featuristic/selection/
--rw-r--r--   0 martin     (501) staff       (20)      126 2024-03-22 21:22:13.000000 featuristic-1.0.0/src/featuristic/selection/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     6889 2024-03-27 07:32:06.000000 featuristic-1.0.0/src/featuristic/selection/genetic_feature_selection.py
--rw-r--r--   0 martin     (501) staff       (20)     8978 2024-03-22 21:19:52.000000 featuristic-1.0.0/src/featuristic/selection/population.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.925779 featuristic-1.0.0/src/featuristic/synthesis/
--rw-r--r--   0 martin     (501) staff       (20)      444 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1164 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/fitness.py
--rw-r--r--   0 martin     (501) staff       (20)    13226 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/genetic_feature_synthesis.py
--rw-r--r--   0 martin     (501) staff       (20)     4294 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/mrmr.py
--rw-r--r--   0 martin     (501) staff       (20)    11903 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/population.py
--rw-r--r--   0 martin     (501) staff       (20)     1273 2024-03-22 21:20:49.000000 featuristic-1.0.0/src/featuristic/synthesis/preprocess.py
--rw-r--r--   0 martin     (501) staff       (20)     2399 2024-03-25 16:59:37.000000 featuristic-1.0.0/src/featuristic/synthesis/program.py
--rw-r--r--   0 martin     (501) staff       (20)    13678 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/symbolic_functions.py
--rw-r--r--   0 martin     (501) staff       (20)       55 2024-04-02 20:27:37.000000 featuristic-1.0.0/src/featuristic/version.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.927876 featuristic-1.0.0/src/featuristic.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)    13544 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1034 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)      227 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       12 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/top_level.txt
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.927417 featuristic-1.0.0/tests/
--rw-r--r--   0 martin     (501) staff       (20)      421 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_datasets.py
--rw-r--r--   0 martin     (501) staff       (20)      760 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_fitness.py
--rw-r--r--   0 martin     (501) staff       (20)      824 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_genetic_feature_selection.py
--rw-r--r--   0 martin     (501) staff       (20)      895 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_genetic_feature_synthesis.py
--rw-r--r--   0 martin     (501) staff       (20)      510 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_preprocess.py
--rw-r--r--   0 martin     (501) staff       (20)     1763 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_programs.py
--rw-r--r--   0 martin     (501) staff       (20)     5443 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_symbolic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.911091 featuristic-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-04 19:22:41.000000 featuristic-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-04 19:22:44.911091 featuristic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-04 19:22:41.000000 featuristic-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-04-04 19:22:41.000000 featuristic-1.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:22:44.911091 featuristic-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.903092 featuristic-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/datasets/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/selection/genetic_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/selection/population.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/genetic_feature_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/mrmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/symbolic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.911091 featuristic-1.0.1/src/featuristic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.911091 featuristic-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_genetic_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_genetic_feature_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_symbolic_functions.py
```

### Comparing `featuristic-1.0.0/LICENSE.txt` & `featuristic-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/PKG-INFO` & `featuristic-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: featuristic
-Version: 1.0.0
-Summary: An open source library using genetic algorithms for automated feature engineering and feature selection
+Version: 1.0.1
+Summary: Genetic algorithms for automated feature engineering and feature selection
 License: Copyright 2024 Martin Eastwood
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files
         (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge,
         publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished
         to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
         OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
         BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: homepage, https://www.featuristic.co.uk
+Project-URL: repository, https://github.com/martineastwood/featuristic.git
 Keywords: data,machine learning,feature engineering,feature selection,model selection,model evaluation,genetic algorithm,optimization,hyperparameter tuning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -45,15 +47,15 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata_sphinx_theme; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
 
 <p align="center">
-<img width=50% src="https://github.com/martineastwood/featuristic/blob/main/docs/_static/logo.png" alt="Featuristic" />
+<img width=50% src="https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/logo.png" alt="Featuristic" />
 </p>
 
 <p align="center">
 <i>"Because feature engineering should be a science, not an art."</i>
 </p>
 
 <div align="center">
@@ -84,19 +86,19 @@
 
 Initially, Featuristic creates a diverse population of formulas using fundamental mathematical operators such as `add`, `subtract`, `sin`, `tan`, `square`, `sqrt`, and more.
 
 For instance, a formula generated by Featuristic might look like this: `(square(feature_1) - abs(feature_2)) * feature_3`.
 
 Next, Featuristic assesses the importance of these formulas by quantifying how well they correlate with the target variable. Those formulas yielding features with the strongest correlations are then selected and recombined using a genetic algorithm to produce offspring, as illustrated below.
 
-![Symbolic Regression Example](docs/_static/symbolic_regression_example.png "Symbolic Regression Example")
+![Symbolic Regression Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/symbolic_regression_example.png "Symbolic Regression Example")
 
 These offspring may also undergo point mutations, which causes alterations to random operators within the formula. This process introduces slight variations to the formulas, enhancing the diversity of the population and potentially leading to the discovery of novel and more effective feature representations.
 
-![Mutation Example](docs/_static/mutation_example.png "Mutation Example")
+![Mutation Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/mutation_example.png "Mutation Example")
 
 This iterative process continues across multiple generations, continually refining the population of formulas with the goal of generating features that exhibit strong correlations with the target variable.
 
 ## Example
 
 Below is an example of using Featuristic's Genetic Feature Synthesis (GFS) to perform automated feature engineering. We'll start off by downloading the well known `cars` dataset from the UCI Machine Learning Repository and split it into training and testing sets. The training set will be used to train our model, while the testing set will remain unseen during the training process and will serve as an independent dataset to evaluate the model's performance.
 
@@ -118,46 +120,46 @@
 
 ```python
 synth = ft.GeneticFeatureSynthesis(
     num_features=5,
     population_size=200,
     max_generations=100,
     early_termination_iters=25,
-    parsimony_coefficient=0.05,
-    n_jobs=-1,
+    parsimony_coefficient=0.035,
+    n_jobs=1,
 )
 
 synth.fit(X_train, y_train)
 ```
 
 We can call the `transform` function to generate a dataframe containing our new features. By default, the `GeneticFeatureSynthesis` class will return both the original features and the newly synthesised features. However, we return just the new features by setting the `return_all_features` argument to `False` when we create the class. We can also combine both the `fit` and `transform` steps into one step by calling `fit_transform` instead.
 
 ```python
 generated_features = synth.transform(X_train)
 
 print(generated_features.head())
 ```
 
-|    |   displacement |   cylinders |   horsepower |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_1 |   feature_3 |   feature_2 |   feature_4 |
-|---:|---------------:|------------:|-------------:|---------:|---------------:|-------------:|---------:|------------:|------------:|------------:|------------:|------------:|
-|  0 |             89 |           4 |           62 |     2050 |           17.3 |           81 |        3 |    0.673279 | -0.00987805 |    0.566434 |   -0.917052 |    0.536626 |
-|  1 |            318 |           8 |          150 |     4077 |           14   |           72 |        1 |    0.133744 | -0.00220751 |    0.324324 |   -0.226914 |    0.318668 |
-|  2 |            383 |           8 |          170 |     3563 |           10   |           70 |        1 |    0.144654 | -0.0024558  |    0.291667 |   -0.183216 |    0.287549 |
-|  3 |            260 |           8 |          110 |     4060 |           19   |           77 |        1 |    0.153605 | -0.00237069 |    0.411765 |   -0.29502  |    0.400227 |
-|  4 |            318 |           8 |          140 |     4080 |           13.7 |           78 |        1 |    0.156848 | -0.00238971 |    0.357798 |   -0.245131 |    0.350213 |
+|    |   displacement |   cylinders |   horsepower |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_4 |   feature_11 |   feature_1 |   feature_22 |
+|---:|---------------:|------------:|-------------:|---------:|---------------:|-------------:|---------:|------------:|------------:|-------------:|------------:|-------------:|
+|  0 |             89 |           4 |           62 |     2050 |           17.3 |           81 |        3 |    -8571.63 |   -0.312535 |     -96.7449 |   -105.823  |    -0.624987 |
+|  1 |            318 |           8 |          150 |     4077 |           14   |           72 |        1 |    -2488.32 |   -0.786564 |     -75.1698 |    -34.56   |    -1.57302  |
+|  2 |            383 |           8 |          170 |     3563 |           10   |           70 |        1 |    -2017.65 |   -0.727317 |     -71.8277 |    -28.8235 |    -1.45446  |
+|  3 |            260 |           8 |          110 |     4060 |           19   |           77 |        1 |    -4150.3  |   -0.684937 |     -82.6269 |    -53.9    |    -1.36971  |
+|  4 |            318 |           8 |          140 |     4080 |           13.7 |           78 |        1 |    -3389.66 |   -0.670713 |     -81.3604 |    -43.4571 |    -1.34132  |
 
 Our newly engineered features currently have generic names. However, since Featuristic synthesizes these features by the applying mathematical expressions to the data, we can look at the underlying formulas responsible for each feature's creation.
 
 ```python
 info = synth.get_feature_info()
-print(info["formula"].iloc[1])
+print(info["formula"].iloc[0])
 ```
 
 ```
-(-(((model_year / (weight + cylinders)) + sin((weight / weight)))) + -(abs(model_year)))
+-(abs((cube(model_year) / horsepower)))
 ```
 
 Following the synthesis of our new features, we can now use another genetic algorithm for [feature selection](https://en.wikipedia.org/wiki/Feature_selection). This process sifts through all our features to identify the subset that optimally contributes to predictive performance while minimizing redundancy.
 
 To do this, we define a custom objective function that the Genetic Feature Selection algorithm will use to quantify how well each subset of features predicts the target. Please note that the function should return a value to minimize so a smaller value is better. If you want to maximize a metric, you should multiply the output of your objective_function by -1, as shown in the example below.
 
 ```python
@@ -179,27 +181,27 @@
 )
 
 selector.fit(generated_features, y_train)
 
 selected_features = selector.transform(generated_features)
 ```
 
-Let's print out the selected features to see what the Genetic Feature Selection algorithm kept. You can see below that featuristic has kept four of the original features ("displacement", "horsepower", "weight" and "origin") plus four of the features created via the Genetic Feature Synthesis.
+Let's print out the selected features to see what the Genetic Feature Selection algorithm kept. You can see below that featuristic has kept four of the original features ("weight", "acceleration", "model_year" and "origin") plus four of the features created via the Genetic Feature Synthesis.
 
 ```python
 print(selected_features.head())
 ```
 
-|    |   displacement |   horsepower |   weight |   origin |   feature_0 |   feature_1 |   feature_3 |   feature_2 |
-|---:|---------------:|-------------:|---------:|---------:|------------:|------------:|------------:|------------:|
-|  0 |             89 |           62 |     2050 |        3 |    0.673279 | -0.00987805 |    0.566434 |   -0.917052 |
-|  1 |            318 |          150 |     4077 |        1 |    0.133744 | -0.00220751 |    0.324324 |   -0.226914 |
-|  2 |            383 |          170 |     3563 |        1 |    0.144654 | -0.0024558  |    0.291667 |   -0.183216 |
-|  3 |            260 |          110 |     4060 |        1 |    0.153605 | -0.00237069 |    0.411765 |   -0.29502  |
-|  4 |            318 |          140 |     4080 |        1 |    0.156848 | -0.00238971 |    0.357798 |   -0.245131 |
+|    |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_4 |   feature_11 |   feature_1 |
+|---:|---------:|---------------:|-------------:|---------:|------------:|------------:|-------------:|------------:|
+|  0 |     2050 |           17.3 |           81 |        3 |    -8571.63 |   -0.312535 |     -96.7449 |   -105.823  |
+|  1 |     4077 |           14   |           72 |        1 |    -2488.32 |   -0.786564 |     -75.1698 |    -34.56   |
+|  2 |     3563 |           10   |           70 |        1 |    -2017.65 |   -0.727317 |     -71.8277 |    -28.8235 |
+|  3 |     4060 |           19   |           77 |        1 |    -4150.3  |   -0.684937 |     -82.6269 |    -53.9    |
+|  4 |     4080 |           13.7 |           78 |        1 |    -3389.66 |   -0.670713 |     -81.3604 |    -43.4571 |
 
 Now that we've selected our features, let's see whether they actually help our model's predictive performance on our test data set. We'll start off with the original features as a baseline.
 
 ```python
 model = LinearRegression()
 model.fit(X_train, y_train)
 preds = model.predict(X_test)
@@ -219,23 +221,23 @@
 test_features = selector.transform(synth.transform(X_test))
 preds = model.predict(test_features)
 featuristic_mae = mean_absolute_error(y_test, preds)
 print(featuristic_mae)
 ```
 
 ```
-2.1729482398016042
+1.9497667311649802
 ```
 
 ```python
 print(f"Original MAE: {original_mae}")
 print(f"Featuristic MAE: {featuristic_mae}")
 print(f"Improvement: {round((1 - (featuristic_mae / original_mae))* 100, 1)}%")
 ```
 
 ```
 Original MAE: 2.5888868138669303
-Featuristic MAE: 2.1729482398016042
-Improvement: 16.1%
+Featuristic MAE: 1.9497667311649802
+Improvement: 24.7%
 ```
 
 The new features generated / selected by the Genetic Feature Synthesis have successfully reduced our mean absolute error &#128512;
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: featuristic Version: 1.0.0 Summary: An open source
-library using genetic algorithms for automated feature engineering and feature
-selection License: Copyright 2024 Martin Eastwood Permission is hereby granted,
-free of charge, to any person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use, copy, modify,
-merge, publish, distribute, sublicense, and/or sell copies of the Software, and
-to permit persons to whom the Software is furnished to do so, subject to the
-following conditions: The above copyright notice and this permission notice
-shall be included in all copies or substantial portions of the Software. THE
-SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Keywords: data,machine learning,feature engineering,feature selection,model
-selection,model evaluation,genetic algorithm,optimization,hyperparameter tuning
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
-Language :: Python :: 3 :: Only Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE.txt Requires-Dist: matplotlib>=3.0.0
-Requires-Dist: numpy>=1.25.0 Requires-Dist: pandas>=2.0.0 Requires-Dist:
-Pyarrow>=15.0.0 Requires-Dist: scikit-learn>=1.4.0 Requires-Dist: tqdm>=4.32.0
-Requires-Dist: ucimlrepo>=0.0.5 Provides-Extra: dev Requires-Dist: black; extra
-== "dev" Requires-Dist: build; extra == "dev" Requires-Dist: coverage; extra ==
-"dev" Requires-Dist: coveralls; extra == "dev" Requires-Dist: isort; extra ==
-"dev" Requires-Dist: ipykernel; extra == "dev" Requires-Dist: nbsphinx; extra
-== "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-pydata_sphinx_theme; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pylint; extra == "dev" Requires-Dist: Sphinx; extra == "dev"
+Metadata-Version: 2.1 Name: featuristic Version: 1.0.1 Summary: Genetic
+algorithms for automated feature engineering and feature selection License:
+Copyright 2024 Martin Eastwood Permission is hereby granted, free of charge, to
+any person obtaining a copy of this software and associated documentation files
+(the "Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: homepage,
+https://www.featuristic.co.uk Project-URL: repository, https://github.com/
+martineastwood/featuristic.git Keywords: data,machine learning,feature
+engineering,feature selection,model selection,model evaluation,genetic
+algorithm,optimization,hyperparameter tuning Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE.txt Requires-Dist: matplotlib>=3.0.0 Requires-Dist: numpy>=1.25.0
+Requires-Dist: pandas>=2.0.0 Requires-Dist: Pyarrow>=15.0.0 Requires-Dist:
+scikit-learn>=1.4.0 Requires-Dist: tqdm>=4.32.0 Requires-Dist: ucimlrepo>=0.0.5
+Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: build;
+extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-Dist:
+coveralls; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
+ipykernel; extra == "dev" Requires-Dist: nbsphinx; extra == "dev" Requires-
+Dist: pre-commit; extra == "dev" Requires-Dist: pydata_sphinx_theme; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pylint; extra ==
+"dev" Requires-Dist: Sphinx; extra == "dev"
                                  [Featuristic]
         "Because feature engineering should be a science, not an art."
 [![Python Version](https://img.shields.io/pypi/pyversions/featuristic)](https:/
     /pypi.org/project/featuristic/) [![PyPI](https://img.shields.io/pypi/v/
    featuristic.svg)](https://pypi.org/project/featuristic/) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
  licenses/MIT) _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_][![Code style: black](https://img.shields.io/
@@ -55,109 +57,110 @@
 fundamental mathematical operators such as `add`, `subtract`, `sin`, `tan`,
 `square`, `sqrt`, and more. For instance, a formula generated by Featuristic
 might look like this: `(square(feature_1) - abs(feature_2)) * feature_3`. Next,
 Featuristic assesses the importance of these formulas by quantifying how well
 they correlate with the target variable. Those formulas yielding features with
 the strongest correlations are then selected and recombined using a genetic
 algorithm to produce offspring, as illustrated below. ![Symbolic Regression
-Example](docs/_static/symbolic_regression_example.png "Symbolic Regression
-Example") These offspring may also undergo point mutations, which causes
-alterations to random operators within the formula. This process introduces
-slight variations to the formulas, enhancing the diversity of the population
-and potentially leading to the discovery of novel and more effective feature
-representations. ![Mutation Example](docs/_static/mutation_example.png
-"Mutation Example") This iterative process continues across multiple
-generations, continually refining the population of formulas with the goal of
-generating features that exhibit strong correlations with the target variable.
-## Example Below is an example of using Featuristic's Genetic Feature Synthesis
-(GFS) to perform automated feature engineering. We'll start off by downloading
-the well known `cars` dataset from the UCI Machine Learning Repository and
-split it into training and testing sets. The training set will be used to train
-our model, while the testing set will remain unseen during the training process
-and will serve as an independent dataset to evaluate the model's performance.
-```python from sklearn.linear_model import LinearRegression from
-sklearn.model_selection import train_test_split, cross_val_score from
-sklearn.metrics import mean_absolute_error import featuristic as ft import
-numpy as np np.random.seed(8888) X, y = ft.fetch_cars_dataset() X_train,
-X_test, y_train, y_test = train_test_split(X, y, test_size=0.3) ``` Next, we'll
-initiate the Genetic Feature Synthesis process. We've configured the genetic
-algorithm to synthesize 5 new features for us. This entails evolving a
-population consisting of 200 individuals iteratively over 100 generations. To
-ensure optimal performance, we've set the genetic algorithm to halt early if it
-fails to improve upon the best feature identified within 25 generations.
-Additionally, for enhanced computational efficiency, we've designated n_jobs as
--1, enabling concurrent execution across all available CPUs on our computer.
-```python synth = ft.GeneticFeatureSynthesis( num_features=5,
-population_size=200, max_generations=100, early_termination_iters=25,
-parsimony_coefficient=0.05, n_jobs=-1, ) synth.fit(X_train, y_train) ``` We can
-call the `transform` function to generate a dataframe containing our new
-features. By default, the `GeneticFeatureSynthesis` class will return both the
-original features and the newly synthesised features. However, we return just
-the new features by setting the `return_all_features` argument to `False` when
-we create the class. We can also combine both the `fit` and `transform` steps
-into one step by calling `fit_transform` instead. ```python generated_features
-= synth.transform(X_train) print(generated_features.head()) ``` | |
-displacement | cylinders | horsepower | weight | acceleration | model_year |
-origin | feature_0 | feature_1 | feature_3 | feature_2 | feature_4 | |---:|----
------------:|------------:|-------------:|---------:|---------------:|---------
-----:|---------:|------------:|------------:|------------:|------------:|------
-------:| | 0 | 89 | 4 | 62 | 2050 | 17.3 | 81 | 3 | 0.673279 | -0.00987805 |
-0.566434 | -0.917052 | 0.536626 | | 1 | 318 | 8 | 150 | 4077 | 14 | 72 | 1 |
-0.133744 | -0.00220751 | 0.324324 | -0.226914 | 0.318668 | | 2 | 383 | 8 | 170
-| 3563 | 10 | 70 | 1 | 0.144654 | -0.0024558 | 0.291667 | -0.183216 | 0.287549
-| | 3 | 260 | 8 | 110 | 4060 | 19 | 77 | 1 | 0.153605 | -0.00237069 | 0.411765
-| -0.29502 | 0.400227 | | 4 | 318 | 8 | 140 | 4080 | 13.7 | 78 | 1 | 0.156848 |
--0.00238971 | 0.357798 | -0.245131 | 0.350213 | Our newly engineered features
-currently have generic names. However, since Featuristic synthesizes these
-features by the applying mathematical expressions to the data, we can look at
-the underlying formulas responsible for each feature's creation. ```python info
-= synth.get_feature_info() print(info["formula"].iloc[1]) ``` ``` (-((
-(model_year / (weight + cylinders)) + sin((weight / weight)))) + -(abs
-(model_year))) ``` Following the synthesis of our new features, we can now use
-another genetic algorithm for [feature selection](https://en.wikipedia.org/
-wiki/Feature_selection). This process sifts through all our features to
-identify the subset that optimally contributes to predictive performance while
-minimizing redundancy. To do this, we define a custom objective function that
-the Genetic Feature Selection algorithm will use to quantify how well each
-subset of features predicts the target. Please note that the function should
-return a value to minimize so a smaller value is better. If you want to
-maximize a metric, you should multiply the output of your objective_function by
--1, as shown in the example below. ```python def objective_function(X, y):
-model = LinearRegression() scores = cross_val_score(model, X, y, cv=3,
-scoring="neg_mean_absolute_error") return scores.mean() * -1 ``` Next, we set
-up the Genetic Feature Selector. We've configured the genetic algorithm to
-evolve a population consisting of 200 individuals iteratively over 100
-generations. To ensure optimal performance, we've set the genetic algorithm to
-halt early if it fails to improve upon the best feature set identified within
-25 generations. Additionally, for enhanced computational efficiency, we've set
-n_jobs as -1, enabling concurrent execution across all available CPUs on our
-computer. ```python selector = ft.GeneticFeatureSelector( objective_function,
-population_size=200, max_generations=100, early_termination_iters=25, n_jobs=-
-1, ) selector.fit(generated_features, y_train) selected_features =
-selector.transform(generated_features) ``` Let's print out the selected
-features to see what the Genetic Feature Selection algorithm kept. You can see
-below that featuristic has kept four of the original features ("displacement",
-"horsepower", "weight" and "origin") plus four of the features created via the
-Genetic Feature Synthesis. ```python print(selected_features.head()) ``` | |
-displacement | horsepower | weight | origin | feature_0 | feature_1 | feature_3
-| feature_2 | |---:|---------------:|-------------:|---------:|---------:|-----
--------:|------------:|------------:|------------:| | 0 | 89 | 62 | 2050 | 3 |
-0.673279 | -0.00987805 | 0.566434 | -0.917052 | | 1 | 318 | 150 | 4077 | 1 |
-0.133744 | -0.00220751 | 0.324324 | -0.226914 | | 2 | 383 | 170 | 3563 | 1 |
-0.144654 | -0.0024558 | 0.291667 | -0.183216 | | 3 | 260 | 110 | 4060 | 1 |
-0.153605 | -0.00237069 | 0.411765 | -0.29502 | | 4 | 318 | 140 | 4080 | 1 |
-0.156848 | -0.00238971 | 0.357798 | -0.245131 | Now that we've selected our
-features, let's see whether they actually help our model's predictive
+Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/
+_static/symbolic_regression_example.png "Symbolic Regression Example") These
+offspring may also undergo point mutations, which causes alterations to random
+operators within the formula. This process introduces slight variations to the
+formulas, enhancing the diversity of the population and potentially leading to
+the discovery of novel and more effective feature representations. ![Mutation
+Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/
+_static/mutation_example.png "Mutation Example") This iterative process
+continues across multiple generations, continually refining the population of
+formulas with the goal of generating features that exhibit strong correlations
+with the target variable. ## Example Below is an example of using Featuristic's
+Genetic Feature Synthesis (GFS) to perform automated feature engineering. We'll
+start off by downloading the well known `cars` dataset from the UCI Machine
+Learning Repository and split it into training and testing sets. The training
+set will be used to train our model, while the testing set will remain unseen
+during the training process and will serve as an independent dataset to
+evaluate the model's performance. ```python from sklearn.linear_model import
+LinearRegression from sklearn.model_selection import train_test_split,
+cross_val_score from sklearn.metrics import mean_absolute_error import
+featuristic as ft import numpy as np np.random.seed(8888) X, y =
+ft.fetch_cars_dataset() X_train, X_test, y_train, y_test = train_test_split(X,
+y, test_size=0.3) ``` Next, we'll initiate the Genetic Feature Synthesis
+process. We've configured the genetic algorithm to synthesize 5 new features
+for us. This entails evolving a population consisting of 200 individuals
+iteratively over 100 generations. To ensure optimal performance, we've set the
+genetic algorithm to halt early if it fails to improve upon the best feature
+identified within 25 generations. Additionally, for enhanced computational
+efficiency, we've designated n_jobs as -1, enabling concurrent execution across
+all available CPUs on our computer. ```python synth =
+ft.GeneticFeatureSynthesis( num_features=5, population_size=200,
+max_generations=100, early_termination_iters=25, parsimony_coefficient=0.035,
+n_jobs=1, ) synth.fit(X_train, y_train) ``` We can call the `transform`
+function to generate a dataframe containing our new features. By default, the
+`GeneticFeatureSynthesis` class will return both the original features and the
+newly synthesised features. However, we return just the new features by setting
+the `return_all_features` argument to `False` when we create the class. We can
+also combine both the `fit` and `transform` steps into one step by calling
+`fit_transform` instead. ```python generated_features = synth.transform
+(X_train) print(generated_features.head()) ``` | | displacement | cylinders |
+horsepower | weight | acceleration | model_year | origin | feature_0 |
+feature_4 | feature_11 | feature_1 | feature_22 | |---:|---------------:|------
+------:|-------------:|---------:|---------------:|-------------:|---------:|--
+----------:|------------:|-------------:|------------:|-------------:| | 0 | 89
+| 4 | 62 | 2050 | 17.3 | 81 | 3 | -8571.63 | -0.312535 | -96.7449 | -105.823 |
+-0.624987 | | 1 | 318 | 8 | 150 | 4077 | 14 | 72 | 1 | -2488.32 | -0.786564 | -
+75.1698 | -34.56 | -1.57302 | | 2 | 383 | 8 | 170 | 3563 | 10 | 70 | 1 | -
+2017.65 | -0.727317 | -71.8277 | -28.8235 | -1.45446 | | 3 | 260 | 8 | 110 |
+4060 | 19 | 77 | 1 | -4150.3 | -0.684937 | -82.6269 | -53.9 | -1.36971 | | 4 |
+318 | 8 | 140 | 4080 | 13.7 | 78 | 1 | -3389.66 | -0.670713 | -81.3604 | -
+43.4571 | -1.34132 | Our newly engineered features currently have generic
+names. However, since Featuristic synthesizes these features by the applying
+mathematical expressions to the data, we can look at the underlying formulas
+responsible for each feature's creation. ```python info =
+synth.get_feature_info() print(info["formula"].iloc[0]) ``` ``` -(abs((cube
+(model_year) / horsepower))) ``` Following the synthesis of our new features,
+we can now use another genetic algorithm for [feature selection](https://
+en.wikipedia.org/wiki/Feature_selection). This process sifts through all our
+features to identify the subset that optimally contributes to predictive
+performance while minimizing redundancy. To do this, we define a custom
+objective function that the Genetic Feature Selection algorithm will use to
+quantify how well each subset of features predicts the target. Please note that
+the function should return a value to minimize so a smaller value is better. If
+you want to maximize a metric, you should multiply the output of your
+objective_function by -1, as shown in the example below. ```python def
+objective_function(X, y): model = LinearRegression() scores = cross_val_score
+(model, X, y, cv=3, scoring="neg_mean_absolute_error") return scores.mean() * -
+1 ``` Next, we set up the Genetic Feature Selector. We've configured the
+genetic algorithm to evolve a population consisting of 200 individuals
+iteratively over 100 generations. To ensure optimal performance, we've set the
+genetic algorithm to halt early if it fails to improve upon the best feature
+set identified within 25 generations. Additionally, for enhanced computational
+efficiency, we've set n_jobs as -1, enabling concurrent execution across all
+available CPUs on our computer. ```python selector = ft.GeneticFeatureSelector
+( objective_function, population_size=200, max_generations=100,
+early_termination_iters=25, n_jobs=-1, ) selector.fit(generated_features,
+y_train) selected_features = selector.transform(generated_features) ``` Let's
+print out the selected features to see what the Genetic Feature Selection
+algorithm kept. You can see below that featuristic has kept four of the
+original features ("weight", "acceleration", "model_year" and "origin") plus
+four of the features created via the Genetic Feature Synthesis. ```python print
+(selected_features.head()) ``` | | weight | acceleration | model_year | origin
+| feature_0 | feature_4 | feature_11 | feature_1 | |---:|---------:|-----------
+----:|-------------:|---------:|------------:|------------:|-------------:|----
+--------:| | 0 | 2050 | 17.3 | 81 | 3 | -8571.63 | -0.312535 | -96.7449 | -
+105.823 | | 1 | 4077 | 14 | 72 | 1 | -2488.32 | -0.786564 | -75.1698 | -34.56 |
+| 2 | 3563 | 10 | 70 | 1 | -2017.65 | -0.727317 | -71.8277 | -28.8235 | | 3 |
+4060 | 19 | 77 | 1 | -4150.3 | -0.684937 | -82.6269 | -53.9 | | 4 | 4080 | 13.7
+| 78 | 1 | -3389.66 | -0.670713 | -81.3604 | -43.4571 | Now that we've selected
+our features, let's see whether they actually help our model's predictive
 performance on our test data set. We'll start off with the original features as
 a baseline. ```python model = LinearRegression() model.fit(X_train, y_train)
 preds = model.predict(X_test) original_mae = mean_absolute_error(y_test, preds)
 print(original_mae) ``` ``` 2.5888868138669303 ``` And now, let's see how the
 model performs with our synthesised feature set. ```python model =
 LinearRegression() model.fit(selected_features, y_train) test_features =
 selector.transform(synth.transform(X_test)) preds = model.predict
 (test_features) featuristic_mae = mean_absolute_error(y_test, preds) print
-(featuristic_mae) ``` ``` 2.1729482398016042 ``` ```python print(f"Original
+(featuristic_mae) ``` ``` 1.9497667311649802 ``` ```python print(f"Original
 MAE: {original_mae}") print(f"Featuristic MAE: {featuristic_mae}") print
 (f"Improvement: {round((1 - (featuristic_mae / original_mae))* 100, 1)}%") ```
-``` Original MAE: 2.5888868138669303 Featuristic MAE: 2.1729482398016042
-Improvement: 16.1% ``` The new features generated / selected by the Genetic
+``` Original MAE: 2.5888868138669303 Featuristic MAE: 1.9497667311649802
+Improvement: 24.7% ``` The new features generated / selected by the Genetic
 Feature Synthesis have successfully reduced our mean absolute error 
```

### Comparing `featuristic-1.0.0/pyproject.toml` & `featuristic-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "featuristic"
 
 # Versions should comply with PEP 440
-version = "1.0.0"
+version = "1.0.1"
 
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
-description = "An open source library using genetic algorithms for automated feature engineering and feature selection"
+description = "Genetic algorithms for automated feature engineering and feature selection"
 
 
 # This is an optional longer description of your project that represents
 # the body of text which users will see when they visit PyPI.
 #
 # Often, this is the same as your README, so you can just read it in from
 # that file directly (as we have already done above)
@@ -119,7 +119,17 @@
 
 
 # [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 # requires = ["setuptools>=43.0.0", "wheel"]
 # build-backend = "setuptools.build_meta"
+
+[project.urls]
+
+# Project homepage, often a link to GitHub or GitLab
+# Often specified in the [project] table
+homepage = "https://www.featuristic.co.uk"
+
+# The source code repository, don't use this if your homepage
+# is the repo
+repository = "https://github.com/martineastwood/featuristic.git"
```

### Comparing `featuristic-1.0.0/readme.md` & `featuristic-1.0.1/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-<img width=50% src="https://github.com/martineastwood/featuristic/blob/main/docs/_static/logo.png" alt="Featuristic" />
+<img width=50% src="https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/logo.png" alt="Featuristic" />
 </p>
 
 <p align="center">
 <i>"Because feature engineering should be a science, not an art."</i>
 </p>
 
 <div align="center">
@@ -34,19 +34,19 @@
 
 Initially, Featuristic creates a diverse population of formulas using fundamental mathematical operators such as `add`, `subtract`, `sin`, `tan`, `square`, `sqrt`, and more.
 
 For instance, a formula generated by Featuristic might look like this: `(square(feature_1) - abs(feature_2)) * feature_3`.
 
 Next, Featuristic assesses the importance of these formulas by quantifying how well they correlate with the target variable. Those formulas yielding features with the strongest correlations are then selected and recombined using a genetic algorithm to produce offspring, as illustrated below.
 
-![Symbolic Regression Example](docs/_static/symbolic_regression_example.png "Symbolic Regression Example")
+![Symbolic Regression Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/symbolic_regression_example.png "Symbolic Regression Example")
 
 These offspring may also undergo point mutations, which causes alterations to random operators within the formula. This process introduces slight variations to the formulas, enhancing the diversity of the population and potentially leading to the discovery of novel and more effective feature representations.
 
-![Mutation Example](docs/_static/mutation_example.png "Mutation Example")
+![Mutation Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/mutation_example.png "Mutation Example")
 
 This iterative process continues across multiple generations, continually refining the population of formulas with the goal of generating features that exhibit strong correlations with the target variable.
 
 ## Example
 
 Below is an example of using Featuristic's Genetic Feature Synthesis (GFS) to perform automated feature engineering. We'll start off by downloading the well known `cars` dataset from the UCI Machine Learning Repository and split it into training and testing sets. The training set will be used to train our model, while the testing set will remain unseen during the training process and will serve as an independent dataset to evaluate the model's performance.
 
@@ -68,46 +68,46 @@
 
 ```python
 synth = ft.GeneticFeatureSynthesis(
     num_features=5,
     population_size=200,
     max_generations=100,
     early_termination_iters=25,
-    parsimony_coefficient=0.05,
-    n_jobs=-1,
+    parsimony_coefficient=0.035,
+    n_jobs=1,
 )
 
 synth.fit(X_train, y_train)
 ```
 
 We can call the `transform` function to generate a dataframe containing our new features. By default, the `GeneticFeatureSynthesis` class will return both the original features and the newly synthesised features. However, we return just the new features by setting the `return_all_features` argument to `False` when we create the class. We can also combine both the `fit` and `transform` steps into one step by calling `fit_transform` instead.
 
 ```python
 generated_features = synth.transform(X_train)
 
 print(generated_features.head())
 ```
 
-|    |   displacement |   cylinders |   horsepower |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_1 |   feature_3 |   feature_2 |   feature_4 |
-|---:|---------------:|------------:|-------------:|---------:|---------------:|-------------:|---------:|------------:|------------:|------------:|------------:|------------:|
-|  0 |             89 |           4 |           62 |     2050 |           17.3 |           81 |        3 |    0.673279 | -0.00987805 |    0.566434 |   -0.917052 |    0.536626 |
-|  1 |            318 |           8 |          150 |     4077 |           14   |           72 |        1 |    0.133744 | -0.00220751 |    0.324324 |   -0.226914 |    0.318668 |
-|  2 |            383 |           8 |          170 |     3563 |           10   |           70 |        1 |    0.144654 | -0.0024558  |    0.291667 |   -0.183216 |    0.287549 |
-|  3 |            260 |           8 |          110 |     4060 |           19   |           77 |        1 |    0.153605 | -0.00237069 |    0.411765 |   -0.29502  |    0.400227 |
-|  4 |            318 |           8 |          140 |     4080 |           13.7 |           78 |        1 |    0.156848 | -0.00238971 |    0.357798 |   -0.245131 |    0.350213 |
+|    |   displacement |   cylinders |   horsepower |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_4 |   feature_11 |   feature_1 |   feature_22 |
+|---:|---------------:|------------:|-------------:|---------:|---------------:|-------------:|---------:|------------:|------------:|-------------:|------------:|-------------:|
+|  0 |             89 |           4 |           62 |     2050 |           17.3 |           81 |        3 |    -8571.63 |   -0.312535 |     -96.7449 |   -105.823  |    -0.624987 |
+|  1 |            318 |           8 |          150 |     4077 |           14   |           72 |        1 |    -2488.32 |   -0.786564 |     -75.1698 |    -34.56   |    -1.57302  |
+|  2 |            383 |           8 |          170 |     3563 |           10   |           70 |        1 |    -2017.65 |   -0.727317 |     -71.8277 |    -28.8235 |    -1.45446  |
+|  3 |            260 |           8 |          110 |     4060 |           19   |           77 |        1 |    -4150.3  |   -0.684937 |     -82.6269 |    -53.9    |    -1.36971  |
+|  4 |            318 |           8 |          140 |     4080 |           13.7 |           78 |        1 |    -3389.66 |   -0.670713 |     -81.3604 |    -43.4571 |    -1.34132  |
 
 Our newly engineered features currently have generic names. However, since Featuristic synthesizes these features by the applying mathematical expressions to the data, we can look at the underlying formulas responsible for each feature's creation.
 
 ```python
 info = synth.get_feature_info()
-print(info["formula"].iloc[1])
+print(info["formula"].iloc[0])
 ```
 
 ```
-(-(((model_year / (weight + cylinders)) + sin((weight / weight)))) + -(abs(model_year)))
+-(abs((cube(model_year) / horsepower)))
 ```
 
 Following the synthesis of our new features, we can now use another genetic algorithm for [feature selection](https://en.wikipedia.org/wiki/Feature_selection). This process sifts through all our features to identify the subset that optimally contributes to predictive performance while minimizing redundancy.
 
 To do this, we define a custom objective function that the Genetic Feature Selection algorithm will use to quantify how well each subset of features predicts the target. Please note that the function should return a value to minimize so a smaller value is better. If you want to maximize a metric, you should multiply the output of your objective_function by -1, as shown in the example below.
 
 ```python
@@ -129,27 +129,27 @@
 )
 
 selector.fit(generated_features, y_train)
 
 selected_features = selector.transform(generated_features)
 ```
 
-Let's print out the selected features to see what the Genetic Feature Selection algorithm kept. You can see below that featuristic has kept four of the original features ("displacement", "horsepower", "weight" and "origin") plus four of the features created via the Genetic Feature Synthesis.
+Let's print out the selected features to see what the Genetic Feature Selection algorithm kept. You can see below that featuristic has kept four of the original features ("weight", "acceleration", "model_year" and "origin") plus four of the features created via the Genetic Feature Synthesis.
 
 ```python
 print(selected_features.head())
 ```
 
-|    |   displacement |   horsepower |   weight |   origin |   feature_0 |   feature_1 |   feature_3 |   feature_2 |
-|---:|---------------:|-------------:|---------:|---------:|------------:|------------:|------------:|------------:|
-|  0 |             89 |           62 |     2050 |        3 |    0.673279 | -0.00987805 |    0.566434 |   -0.917052 |
-|  1 |            318 |          150 |     4077 |        1 |    0.133744 | -0.00220751 |    0.324324 |   -0.226914 |
-|  2 |            383 |          170 |     3563 |        1 |    0.144654 | -0.0024558  |    0.291667 |   -0.183216 |
-|  3 |            260 |          110 |     4060 |        1 |    0.153605 | -0.00237069 |    0.411765 |   -0.29502  |
-|  4 |            318 |          140 |     4080 |        1 |    0.156848 | -0.00238971 |    0.357798 |   -0.245131 |
+|    |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_4 |   feature_11 |   feature_1 |
+|---:|---------:|---------------:|-------------:|---------:|------------:|------------:|-------------:|------------:|
+|  0 |     2050 |           17.3 |           81 |        3 |    -8571.63 |   -0.312535 |     -96.7449 |   -105.823  |
+|  1 |     4077 |           14   |           72 |        1 |    -2488.32 |   -0.786564 |     -75.1698 |    -34.56   |
+|  2 |     3563 |           10   |           70 |        1 |    -2017.65 |   -0.727317 |     -71.8277 |    -28.8235 |
+|  3 |     4060 |           19   |           77 |        1 |    -4150.3  |   -0.684937 |     -82.6269 |    -53.9    |
+|  4 |     4080 |           13.7 |           78 |        1 |    -3389.66 |   -0.670713 |     -81.3604 |    -43.4571 |
 
 Now that we've selected our features, let's see whether they actually help our model's predictive performance on our test data set. We'll start off with the original features as a baseline.
 
 ```python
 model = LinearRegression()
 model.fit(X_train, y_train)
 preds = model.predict(X_test)
@@ -169,23 +169,23 @@
 test_features = selector.transform(synth.transform(X_test))
 preds = model.predict(test_features)
 featuristic_mae = mean_absolute_error(y_test, preds)
 print(featuristic_mae)
 ```
 
 ```
-2.1729482398016042
+1.9497667311649802
 ```
 
 ```python
 print(f"Original MAE: {original_mae}")
 print(f"Featuristic MAE: {featuristic_mae}")
 print(f"Improvement: {round((1 - (featuristic_mae / original_mae))* 100, 1)}%")
 ```
 
 ```
 Original MAE: 2.5888868138669303
-Featuristic MAE: 2.1729482398016042
-Improvement: 16.1%
+Featuristic MAE: 1.9497667311649802
+Improvement: 24.7%
 ```
 
 The new features generated / selected by the Genetic Feature Synthesis have successfully reduced our mean absolute error &#128512;
```

### Comparing `featuristic-1.0.0/src/featuristic/datasets/fetch.py` & `featuristic-1.0.1/src/featuristic/datasets/fetch.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic/selection/genetic_feature_selection.py` & `featuristic-1.0.1/src/featuristic/selection/genetic_feature_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     """
 
     def __init__(
         self,
         objective_function: Callable,
         population_size: int = 50,
         max_generations: int = 100,
+        tournament_size: int = 10,
         crossover_proba: float = 0.9,
         mutation_proba: float = 0.1,
         early_termination_iters: int = 15,
         n_jobs: int = -1,
         pbar: bool = True,
         verbose: bool = False,
     ) -> None:
@@ -74,14 +75,16 @@
         self.crossover_proba = crossover_proba
         self.mutation_proba = mutation_proba
         self.max_generations = max_generations
 
         self.early_termination_iters = early_termination_iters
         self.early_termination_counter = 0
 
+        self.tournament_size = tournament_size
+
         self.history = []
 
         self.best_genome = None
         self.best_cost = sys.maxsize
 
         self.is_fitted_ = False
 
@@ -153,21 +156,23 @@
         """
         self.num_genes = X.shape[1]
 
         if self.n_jobs == 1:
             self.population = SerialPopulation(
                 self.population_size,
                 self.num_genes,
+                self.tournament_size,
                 self.crossover_proba,
                 self.mutation_proba,
             )
         else:
             self.population = ParallelPopulation(
                 self.population_size,
                 self.num_genes,
+                self.tournament_size,
                 self.crossover_proba,
                 self.mutation_proba,
                 self.n_jobs,
             )
 
         if self.pbar:
             pbar = tqdm(
```

### Comparing `featuristic-1.0.0/src/featuristic/selection/population.py` & `featuristic-1.0.1/src/featuristic/selection/population.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,41 @@
     """
     A class to represent the population of programs in the genetic programming algorithm.
 
     Parameters
     ----------
     population_size : int
         The size of the population.
+
     feature_count : int
         The number of features in the dataset.
+
+    tournament_size : int, optional
+        The number of individuals to select for the tournament, by default 10.
+
     crossover_proba : float, optional
         The probability of crossover, by default 0.9.
+
     mutation_proba : float, optional
         The probability of mutation, by default 0.1.
     """
 
     def __init__(
         self,
         population_size: int,
         feature_count: int,
+        tournament_size: int = 10,
         crossover_proba: float = 0.9,
         mutation_proba: float = 0.1,
     ):
         self.population_size = population_size
         self.feature_count = feature_count
         self.crossover_proba = crossover_proba
         self.mutation_proba = mutation_proba
+        self.tournament_size = tournament_size
 
         self.population = None
         self._initialize_population()
 
     def _initialize_population(self):
         """
         Initialize the population.
@@ -200,14 +208,15 @@
     the programs are evaluated serially.
     """
 
     def __init__(
         self,
         population_size: int,
         feature_count: int,
+        tournament_size: int = 10,
         crossover_proba: float = 0.9,
         mutation_proba: float = 0.1,
     ):
         """
         Initialize the population class.
 
         Args
@@ -220,14 +229,15 @@
             The probability of crossover, by default 0.9.
         mutation_proba : float, optional
             The probability of mutation, by default 0.1.
         """
         super().__init__(
             population_size,
             feature_count,
+            tournament_size,
             crossover_proba,
             mutation_proba,
         )
 
     def evaluate(
         self, cost_func: Callable, X: pd.DataFrame, y: pd.Series
     ) -> List[float]:
@@ -257,14 +267,15 @@
     the programs are evaluated in parallel.
     """
 
     def __init__(
         self,
         population_size: int,
         feature_count: int,
+        tournament_size: int = 10,
         crossover_proba: float = 0.9,
         mutation_proba: float = 0.1,
         n_jobs: int = -1,
     ):
         """
         Initialize the population class.
 
@@ -280,14 +291,15 @@
             The probability of mutation, by default 0.1.
         n_jobs : int, optional
             The number of parallel jobs to run, by default -1 (use all available cores).
         """
         super().__init__(
             population_size,
             feature_count,
+            tournament_size,
             crossover_proba,
             mutation_proba,
         )
 
         n_jobs = cpu_count() if n_jobs == -1 else n_jobs
 
     def evaluate(
```

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/fitness.py` & `featuristic-1.0.1/src/featuristic/synthesis/fitness.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/genetic_feature_synthesis.py` & `featuristic-1.0.1/src/featuristic/synthesis/genetic_feature_synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def __init__(
         self,
         functions: Union[List[SymbolicFunction] | None] = None,
         num_features: int = 10,
         population_size: int = 100,
         max_generations: int = 25,
-        tournament_size: int = 3,
+        tournament_size: int = 10,
         crossover_proba: float = 0.85,
         parsimony_coefficient: float = 0.001,
         early_termination_iters: int = 15,
         return_all_features: bool = True,
         n_jobs: int = -1,
         pbar: bool = True,
         verbose: bool = False,
@@ -67,16 +67,16 @@
         max_generations : int
             The maximum number of generations to run. The larger the number of
             generations, the more likely it is to find a good solution, but the longer
             it will take.
 
         tournament_size : int
             The size of the tournament for selection. The larger the tournament size,
-            the more likely it is to select the best program, but the longer it will
-            take.
+            the more likely it is to select the best program, but the more computation
+            it will take.
 
         crossover_proba : float
             The probability of crossover mutation between selected parents in each
             generation.
 
         parsimony_coefficient : float
             The parsimony coefficient. Larger values penalize larger programs more and
```

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/mrmr.py` & `featuristic-1.0.1/src/featuristic/synthesis/mrmr.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/population.py` & `featuristic-1.0.1/src/featuristic/synthesis/population.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/preprocess.py` & `featuristic-1.0.1/src/featuristic/synthesis/preprocess.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/program.py` & `featuristic-1.0.1/src/featuristic/synthesis/program.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic/synthesis/symbolic_functions.py` & `featuristic-1.0.1/src/featuristic/synthesis/symbolic_functions.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/src/featuristic.egg-info/PKG-INFO` & `featuristic-1.0.1/src/featuristic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: featuristic
-Version: 1.0.0
-Summary: An open source library using genetic algorithms for automated feature engineering and feature selection
+Version: 1.0.1
+Summary: Genetic algorithms for automated feature engineering and feature selection
 License: Copyright 2024 Martin Eastwood
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files
         (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge,
         publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished
         to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
         OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
         BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: homepage, https://www.featuristic.co.uk
+Project-URL: repository, https://github.com/martineastwood/featuristic.git
 Keywords: data,machine learning,feature engineering,feature selection,model selection,model evaluation,genetic algorithm,optimization,hyperparameter tuning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -45,15 +47,15 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata_sphinx_theme; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
 
 <p align="center">
-<img width=50% src="https://github.com/martineastwood/featuristic/blob/main/docs/_static/logo.png" alt="Featuristic" />
+<img width=50% src="https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/logo.png" alt="Featuristic" />
 </p>
 
 <p align="center">
 <i>"Because feature engineering should be a science, not an art."</i>
 </p>
 
 <div align="center">
@@ -84,19 +86,19 @@
 
 Initially, Featuristic creates a diverse population of formulas using fundamental mathematical operators such as `add`, `subtract`, `sin`, `tan`, `square`, `sqrt`, and more.
 
 For instance, a formula generated by Featuristic might look like this: `(square(feature_1) - abs(feature_2)) * feature_3`.
 
 Next, Featuristic assesses the importance of these formulas by quantifying how well they correlate with the target variable. Those formulas yielding features with the strongest correlations are then selected and recombined using a genetic algorithm to produce offspring, as illustrated below.
 
-![Symbolic Regression Example](docs/_static/symbolic_regression_example.png "Symbolic Regression Example")
+![Symbolic Regression Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/symbolic_regression_example.png "Symbolic Regression Example")
 
 These offspring may also undergo point mutations, which causes alterations to random operators within the formula. This process introduces slight variations to the formulas, enhancing the diversity of the population and potentially leading to the discovery of novel and more effective feature representations.
 
-![Mutation Example](docs/_static/mutation_example.png "Mutation Example")
+![Mutation Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/_static/mutation_example.png "Mutation Example")
 
 This iterative process continues across multiple generations, continually refining the population of formulas with the goal of generating features that exhibit strong correlations with the target variable.
 
 ## Example
 
 Below is an example of using Featuristic's Genetic Feature Synthesis (GFS) to perform automated feature engineering. We'll start off by downloading the well known `cars` dataset from the UCI Machine Learning Repository and split it into training and testing sets. The training set will be used to train our model, while the testing set will remain unseen during the training process and will serve as an independent dataset to evaluate the model's performance.
 
@@ -118,46 +120,46 @@
 
 ```python
 synth = ft.GeneticFeatureSynthesis(
     num_features=5,
     population_size=200,
     max_generations=100,
     early_termination_iters=25,
-    parsimony_coefficient=0.05,
-    n_jobs=-1,
+    parsimony_coefficient=0.035,
+    n_jobs=1,
 )
 
 synth.fit(X_train, y_train)
 ```
 
 We can call the `transform` function to generate a dataframe containing our new features. By default, the `GeneticFeatureSynthesis` class will return both the original features and the newly synthesised features. However, we return just the new features by setting the `return_all_features` argument to `False` when we create the class. We can also combine both the `fit` and `transform` steps into one step by calling `fit_transform` instead.
 
 ```python
 generated_features = synth.transform(X_train)
 
 print(generated_features.head())
 ```
 
-|    |   displacement |   cylinders |   horsepower |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_1 |   feature_3 |   feature_2 |   feature_4 |
-|---:|---------------:|------------:|-------------:|---------:|---------------:|-------------:|---------:|------------:|------------:|------------:|------------:|------------:|
-|  0 |             89 |           4 |           62 |     2050 |           17.3 |           81 |        3 |    0.673279 | -0.00987805 |    0.566434 |   -0.917052 |    0.536626 |
-|  1 |            318 |           8 |          150 |     4077 |           14   |           72 |        1 |    0.133744 | -0.00220751 |    0.324324 |   -0.226914 |    0.318668 |
-|  2 |            383 |           8 |          170 |     3563 |           10   |           70 |        1 |    0.144654 | -0.0024558  |    0.291667 |   -0.183216 |    0.287549 |
-|  3 |            260 |           8 |          110 |     4060 |           19   |           77 |        1 |    0.153605 | -0.00237069 |    0.411765 |   -0.29502  |    0.400227 |
-|  4 |            318 |           8 |          140 |     4080 |           13.7 |           78 |        1 |    0.156848 | -0.00238971 |    0.357798 |   -0.245131 |    0.350213 |
+|    |   displacement |   cylinders |   horsepower |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_4 |   feature_11 |   feature_1 |   feature_22 |
+|---:|---------------:|------------:|-------------:|---------:|---------------:|-------------:|---------:|------------:|------------:|-------------:|------------:|-------------:|
+|  0 |             89 |           4 |           62 |     2050 |           17.3 |           81 |        3 |    -8571.63 |   -0.312535 |     -96.7449 |   -105.823  |    -0.624987 |
+|  1 |            318 |           8 |          150 |     4077 |           14   |           72 |        1 |    -2488.32 |   -0.786564 |     -75.1698 |    -34.56   |    -1.57302  |
+|  2 |            383 |           8 |          170 |     3563 |           10   |           70 |        1 |    -2017.65 |   -0.727317 |     -71.8277 |    -28.8235 |    -1.45446  |
+|  3 |            260 |           8 |          110 |     4060 |           19   |           77 |        1 |    -4150.3  |   -0.684937 |     -82.6269 |    -53.9    |    -1.36971  |
+|  4 |            318 |           8 |          140 |     4080 |           13.7 |           78 |        1 |    -3389.66 |   -0.670713 |     -81.3604 |    -43.4571 |    -1.34132  |
 
 Our newly engineered features currently have generic names. However, since Featuristic synthesizes these features by the applying mathematical expressions to the data, we can look at the underlying formulas responsible for each feature's creation.
 
 ```python
 info = synth.get_feature_info()
-print(info["formula"].iloc[1])
+print(info["formula"].iloc[0])
 ```
 
 ```
-(-(((model_year / (weight + cylinders)) + sin((weight / weight)))) + -(abs(model_year)))
+-(abs((cube(model_year) / horsepower)))
 ```
 
 Following the synthesis of our new features, we can now use another genetic algorithm for [feature selection](https://en.wikipedia.org/wiki/Feature_selection). This process sifts through all our features to identify the subset that optimally contributes to predictive performance while minimizing redundancy.
 
 To do this, we define a custom objective function that the Genetic Feature Selection algorithm will use to quantify how well each subset of features predicts the target. Please note that the function should return a value to minimize so a smaller value is better. If you want to maximize a metric, you should multiply the output of your objective_function by -1, as shown in the example below.
 
 ```python
@@ -179,27 +181,27 @@
 )
 
 selector.fit(generated_features, y_train)
 
 selected_features = selector.transform(generated_features)
 ```
 
-Let's print out the selected features to see what the Genetic Feature Selection algorithm kept. You can see below that featuristic has kept four of the original features ("displacement", "horsepower", "weight" and "origin") plus four of the features created via the Genetic Feature Synthesis.
+Let's print out the selected features to see what the Genetic Feature Selection algorithm kept. You can see below that featuristic has kept four of the original features ("weight", "acceleration", "model_year" and "origin") plus four of the features created via the Genetic Feature Synthesis.
 
 ```python
 print(selected_features.head())
 ```
 
-|    |   displacement |   horsepower |   weight |   origin |   feature_0 |   feature_1 |   feature_3 |   feature_2 |
-|---:|---------------:|-------------:|---------:|---------:|------------:|------------:|------------:|------------:|
-|  0 |             89 |           62 |     2050 |        3 |    0.673279 | -0.00987805 |    0.566434 |   -0.917052 |
-|  1 |            318 |          150 |     4077 |        1 |    0.133744 | -0.00220751 |    0.324324 |   -0.226914 |
-|  2 |            383 |          170 |     3563 |        1 |    0.144654 | -0.0024558  |    0.291667 |   -0.183216 |
-|  3 |            260 |          110 |     4060 |        1 |    0.153605 | -0.00237069 |    0.411765 |   -0.29502  |
-|  4 |            318 |          140 |     4080 |        1 |    0.156848 | -0.00238971 |    0.357798 |   -0.245131 |
+|    |   weight |   acceleration |   model_year |   origin |   feature_0 |   feature_4 |   feature_11 |   feature_1 |
+|---:|---------:|---------------:|-------------:|---------:|------------:|------------:|-------------:|------------:|
+|  0 |     2050 |           17.3 |           81 |        3 |    -8571.63 |   -0.312535 |     -96.7449 |   -105.823  |
+|  1 |     4077 |           14   |           72 |        1 |    -2488.32 |   -0.786564 |     -75.1698 |    -34.56   |
+|  2 |     3563 |           10   |           70 |        1 |    -2017.65 |   -0.727317 |     -71.8277 |    -28.8235 |
+|  3 |     4060 |           19   |           77 |        1 |    -4150.3  |   -0.684937 |     -82.6269 |    -53.9    |
+|  4 |     4080 |           13.7 |           78 |        1 |    -3389.66 |   -0.670713 |     -81.3604 |    -43.4571 |
 
 Now that we've selected our features, let's see whether they actually help our model's predictive performance on our test data set. We'll start off with the original features as a baseline.
 
 ```python
 model = LinearRegression()
 model.fit(X_train, y_train)
 preds = model.predict(X_test)
@@ -219,23 +221,23 @@
 test_features = selector.transform(synth.transform(X_test))
 preds = model.predict(test_features)
 featuristic_mae = mean_absolute_error(y_test, preds)
 print(featuristic_mae)
 ```
 
 ```
-2.1729482398016042
+1.9497667311649802
 ```
 
 ```python
 print(f"Original MAE: {original_mae}")
 print(f"Featuristic MAE: {featuristic_mae}")
 print(f"Improvement: {round((1 - (featuristic_mae / original_mae))* 100, 1)}%")
 ```
 
 ```
 Original MAE: 2.5888868138669303
-Featuristic MAE: 2.1729482398016042
-Improvement: 16.1%
+Featuristic MAE: 1.9497667311649802
+Improvement: 24.7%
 ```
 
 The new features generated / selected by the Genetic Feature Synthesis have successfully reduced our mean absolute error &#128512;
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: featuristic Version: 1.0.0 Summary: An open source
-library using genetic algorithms for automated feature engineering and feature
-selection License: Copyright 2024 Martin Eastwood Permission is hereby granted,
-free of charge, to any person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use, copy, modify,
-merge, publish, distribute, sublicense, and/or sell copies of the Software, and
-to permit persons to whom the Software is furnished to do so, subject to the
-following conditions: The above copyright notice and this permission notice
-shall be included in all copies or substantial portions of the Software. THE
-SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Keywords: data,machine learning,feature engineering,feature selection,model
-selection,model evaluation,genetic algorithm,optimization,hyperparameter tuning
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
-Language :: Python :: 3 :: Only Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE.txt Requires-Dist: matplotlib>=3.0.0
-Requires-Dist: numpy>=1.25.0 Requires-Dist: pandas>=2.0.0 Requires-Dist:
-Pyarrow>=15.0.0 Requires-Dist: scikit-learn>=1.4.0 Requires-Dist: tqdm>=4.32.0
-Requires-Dist: ucimlrepo>=0.0.5 Provides-Extra: dev Requires-Dist: black; extra
-== "dev" Requires-Dist: build; extra == "dev" Requires-Dist: coverage; extra ==
-"dev" Requires-Dist: coveralls; extra == "dev" Requires-Dist: isort; extra ==
-"dev" Requires-Dist: ipykernel; extra == "dev" Requires-Dist: nbsphinx; extra
-== "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-pydata_sphinx_theme; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pylint; extra == "dev" Requires-Dist: Sphinx; extra == "dev"
+Metadata-Version: 2.1 Name: featuristic Version: 1.0.1 Summary: Genetic
+algorithms for automated feature engineering and feature selection License:
+Copyright 2024 Martin Eastwood Permission is hereby granted, free of charge, to
+any person obtaining a copy of this software and associated documentation files
+(the "Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: homepage,
+https://www.featuristic.co.uk Project-URL: repository, https://github.com/
+martineastwood/featuristic.git Keywords: data,machine learning,feature
+engineering,feature selection,model selection,model evaluation,genetic
+algorithm,optimization,hyperparameter tuning Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE.txt Requires-Dist: matplotlib>=3.0.0 Requires-Dist: numpy>=1.25.0
+Requires-Dist: pandas>=2.0.0 Requires-Dist: Pyarrow>=15.0.0 Requires-Dist:
+scikit-learn>=1.4.0 Requires-Dist: tqdm>=4.32.0 Requires-Dist: ucimlrepo>=0.0.5
+Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: build;
+extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-Dist:
+coveralls; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
+ipykernel; extra == "dev" Requires-Dist: nbsphinx; extra == "dev" Requires-
+Dist: pre-commit; extra == "dev" Requires-Dist: pydata_sphinx_theme; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pylint; extra ==
+"dev" Requires-Dist: Sphinx; extra == "dev"
                                  [Featuristic]
         "Because feature engineering should be a science, not an art."
 [![Python Version](https://img.shields.io/pypi/pyversions/featuristic)](https:/
     /pypi.org/project/featuristic/) [![PyPI](https://img.shields.io/pypi/v/
    featuristic.svg)](https://pypi.org/project/featuristic/) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
  licenses/MIT) _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_][![Code style: black](https://img.shields.io/
@@ -55,109 +57,110 @@
 fundamental mathematical operators such as `add`, `subtract`, `sin`, `tan`,
 `square`, `sqrt`, and more. For instance, a formula generated by Featuristic
 might look like this: `(square(feature_1) - abs(feature_2)) * feature_3`. Next,
 Featuristic assesses the importance of these formulas by quantifying how well
 they correlate with the target variable. Those formulas yielding features with
 the strongest correlations are then selected and recombined using a genetic
 algorithm to produce offspring, as illustrated below. ![Symbolic Regression
-Example](docs/_static/symbolic_regression_example.png "Symbolic Regression
-Example") These offspring may also undergo point mutations, which causes
-alterations to random operators within the formula. This process introduces
-slight variations to the formulas, enhancing the diversity of the population
-and potentially leading to the discovery of novel and more effective feature
-representations. ![Mutation Example](docs/_static/mutation_example.png
-"Mutation Example") This iterative process continues across multiple
-generations, continually refining the population of formulas with the goal of
-generating features that exhibit strong correlations with the target variable.
-## Example Below is an example of using Featuristic's Genetic Feature Synthesis
-(GFS) to perform automated feature engineering. We'll start off by downloading
-the well known `cars` dataset from the UCI Machine Learning Repository and
-split it into training and testing sets. The training set will be used to train
-our model, while the testing set will remain unseen during the training process
-and will serve as an independent dataset to evaluate the model's performance.
-```python from sklearn.linear_model import LinearRegression from
-sklearn.model_selection import train_test_split, cross_val_score from
-sklearn.metrics import mean_absolute_error import featuristic as ft import
-numpy as np np.random.seed(8888) X, y = ft.fetch_cars_dataset() X_train,
-X_test, y_train, y_test = train_test_split(X, y, test_size=0.3) ``` Next, we'll
-initiate the Genetic Feature Synthesis process. We've configured the genetic
-algorithm to synthesize 5 new features for us. This entails evolving a
-population consisting of 200 individuals iteratively over 100 generations. To
-ensure optimal performance, we've set the genetic algorithm to halt early if it
-fails to improve upon the best feature identified within 25 generations.
-Additionally, for enhanced computational efficiency, we've designated n_jobs as
--1, enabling concurrent execution across all available CPUs on our computer.
-```python synth = ft.GeneticFeatureSynthesis( num_features=5,
-population_size=200, max_generations=100, early_termination_iters=25,
-parsimony_coefficient=0.05, n_jobs=-1, ) synth.fit(X_train, y_train) ``` We can
-call the `transform` function to generate a dataframe containing our new
-features. By default, the `GeneticFeatureSynthesis` class will return both the
-original features and the newly synthesised features. However, we return just
-the new features by setting the `return_all_features` argument to `False` when
-we create the class. We can also combine both the `fit` and `transform` steps
-into one step by calling `fit_transform` instead. ```python generated_features
-= synth.transform(X_train) print(generated_features.head()) ``` | |
-displacement | cylinders | horsepower | weight | acceleration | model_year |
-origin | feature_0 | feature_1 | feature_3 | feature_2 | feature_4 | |---:|----
------------:|------------:|-------------:|---------:|---------------:|---------
-----:|---------:|------------:|------------:|------------:|------------:|------
-------:| | 0 | 89 | 4 | 62 | 2050 | 17.3 | 81 | 3 | 0.673279 | -0.00987805 |
-0.566434 | -0.917052 | 0.536626 | | 1 | 318 | 8 | 150 | 4077 | 14 | 72 | 1 |
-0.133744 | -0.00220751 | 0.324324 | -0.226914 | 0.318668 | | 2 | 383 | 8 | 170
-| 3563 | 10 | 70 | 1 | 0.144654 | -0.0024558 | 0.291667 | -0.183216 | 0.287549
-| | 3 | 260 | 8 | 110 | 4060 | 19 | 77 | 1 | 0.153605 | -0.00237069 | 0.411765
-| -0.29502 | 0.400227 | | 4 | 318 | 8 | 140 | 4080 | 13.7 | 78 | 1 | 0.156848 |
--0.00238971 | 0.357798 | -0.245131 | 0.350213 | Our newly engineered features
-currently have generic names. However, since Featuristic synthesizes these
-features by the applying mathematical expressions to the data, we can look at
-the underlying formulas responsible for each feature's creation. ```python info
-= synth.get_feature_info() print(info["formula"].iloc[1]) ``` ``` (-((
-(model_year / (weight + cylinders)) + sin((weight / weight)))) + -(abs
-(model_year))) ``` Following the synthesis of our new features, we can now use
-another genetic algorithm for [feature selection](https://en.wikipedia.org/
-wiki/Feature_selection). This process sifts through all our features to
-identify the subset that optimally contributes to predictive performance while
-minimizing redundancy. To do this, we define a custom objective function that
-the Genetic Feature Selection algorithm will use to quantify how well each
-subset of features predicts the target. Please note that the function should
-return a value to minimize so a smaller value is better. If you want to
-maximize a metric, you should multiply the output of your objective_function by
--1, as shown in the example below. ```python def objective_function(X, y):
-model = LinearRegression() scores = cross_val_score(model, X, y, cv=3,
-scoring="neg_mean_absolute_error") return scores.mean() * -1 ``` Next, we set
-up the Genetic Feature Selector. We've configured the genetic algorithm to
-evolve a population consisting of 200 individuals iteratively over 100
-generations. To ensure optimal performance, we've set the genetic algorithm to
-halt early if it fails to improve upon the best feature set identified within
-25 generations. Additionally, for enhanced computational efficiency, we've set
-n_jobs as -1, enabling concurrent execution across all available CPUs on our
-computer. ```python selector = ft.GeneticFeatureSelector( objective_function,
-population_size=200, max_generations=100, early_termination_iters=25, n_jobs=-
-1, ) selector.fit(generated_features, y_train) selected_features =
-selector.transform(generated_features) ``` Let's print out the selected
-features to see what the Genetic Feature Selection algorithm kept. You can see
-below that featuristic has kept four of the original features ("displacement",
-"horsepower", "weight" and "origin") plus four of the features created via the
-Genetic Feature Synthesis. ```python print(selected_features.head()) ``` | |
-displacement | horsepower | weight | origin | feature_0 | feature_1 | feature_3
-| feature_2 | |---:|---------------:|-------------:|---------:|---------:|-----
--------:|------------:|------------:|------------:| | 0 | 89 | 62 | 2050 | 3 |
-0.673279 | -0.00987805 | 0.566434 | -0.917052 | | 1 | 318 | 150 | 4077 | 1 |
-0.133744 | -0.00220751 | 0.324324 | -0.226914 | | 2 | 383 | 170 | 3563 | 1 |
-0.144654 | -0.0024558 | 0.291667 | -0.183216 | | 3 | 260 | 110 | 4060 | 1 |
-0.153605 | -0.00237069 | 0.411765 | -0.29502 | | 4 | 318 | 140 | 4080 | 1 |
-0.156848 | -0.00238971 | 0.357798 | -0.245131 | Now that we've selected our
-features, let's see whether they actually help our model's predictive
+Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/
+_static/symbolic_regression_example.png "Symbolic Regression Example") These
+offspring may also undergo point mutations, which causes alterations to random
+operators within the formula. This process introduces slight variations to the
+formulas, enhancing the diversity of the population and potentially leading to
+the discovery of novel and more effective feature representations. ![Mutation
+Example](https://raw.githubusercontent.com/martineastwood/featuristic/dev/docs/
+_static/mutation_example.png "Mutation Example") This iterative process
+continues across multiple generations, continually refining the population of
+formulas with the goal of generating features that exhibit strong correlations
+with the target variable. ## Example Below is an example of using Featuristic's
+Genetic Feature Synthesis (GFS) to perform automated feature engineering. We'll
+start off by downloading the well known `cars` dataset from the UCI Machine
+Learning Repository and split it into training and testing sets. The training
+set will be used to train our model, while the testing set will remain unseen
+during the training process and will serve as an independent dataset to
+evaluate the model's performance. ```python from sklearn.linear_model import
+LinearRegression from sklearn.model_selection import train_test_split,
+cross_val_score from sklearn.metrics import mean_absolute_error import
+featuristic as ft import numpy as np np.random.seed(8888) X, y =
+ft.fetch_cars_dataset() X_train, X_test, y_train, y_test = train_test_split(X,
+y, test_size=0.3) ``` Next, we'll initiate the Genetic Feature Synthesis
+process. We've configured the genetic algorithm to synthesize 5 new features
+for us. This entails evolving a population consisting of 200 individuals
+iteratively over 100 generations. To ensure optimal performance, we've set the
+genetic algorithm to halt early if it fails to improve upon the best feature
+identified within 25 generations. Additionally, for enhanced computational
+efficiency, we've designated n_jobs as -1, enabling concurrent execution across
+all available CPUs on our computer. ```python synth =
+ft.GeneticFeatureSynthesis( num_features=5, population_size=200,
+max_generations=100, early_termination_iters=25, parsimony_coefficient=0.035,
+n_jobs=1, ) synth.fit(X_train, y_train) ``` We can call the `transform`
+function to generate a dataframe containing our new features. By default, the
+`GeneticFeatureSynthesis` class will return both the original features and the
+newly synthesised features. However, we return just the new features by setting
+the `return_all_features` argument to `False` when we create the class. We can
+also combine both the `fit` and `transform` steps into one step by calling
+`fit_transform` instead. ```python generated_features = synth.transform
+(X_train) print(generated_features.head()) ``` | | displacement | cylinders |
+horsepower | weight | acceleration | model_year | origin | feature_0 |
+feature_4 | feature_11 | feature_1 | feature_22 | |---:|---------------:|------
+------:|-------------:|---------:|---------------:|-------------:|---------:|--
+----------:|------------:|-------------:|------------:|-------------:| | 0 | 89
+| 4 | 62 | 2050 | 17.3 | 81 | 3 | -8571.63 | -0.312535 | -96.7449 | -105.823 |
+-0.624987 | | 1 | 318 | 8 | 150 | 4077 | 14 | 72 | 1 | -2488.32 | -0.786564 | -
+75.1698 | -34.56 | -1.57302 | | 2 | 383 | 8 | 170 | 3563 | 10 | 70 | 1 | -
+2017.65 | -0.727317 | -71.8277 | -28.8235 | -1.45446 | | 3 | 260 | 8 | 110 |
+4060 | 19 | 77 | 1 | -4150.3 | -0.684937 | -82.6269 | -53.9 | -1.36971 | | 4 |
+318 | 8 | 140 | 4080 | 13.7 | 78 | 1 | -3389.66 | -0.670713 | -81.3604 | -
+43.4571 | -1.34132 | Our newly engineered features currently have generic
+names. However, since Featuristic synthesizes these features by the applying
+mathematical expressions to the data, we can look at the underlying formulas
+responsible for each feature's creation. ```python info =
+synth.get_feature_info() print(info["formula"].iloc[0]) ``` ``` -(abs((cube
+(model_year) / horsepower))) ``` Following the synthesis of our new features,
+we can now use another genetic algorithm for [feature selection](https://
+en.wikipedia.org/wiki/Feature_selection). This process sifts through all our
+features to identify the subset that optimally contributes to predictive
+performance while minimizing redundancy. To do this, we define a custom
+objective function that the Genetic Feature Selection algorithm will use to
+quantify how well each subset of features predicts the target. Please note that
+the function should return a value to minimize so a smaller value is better. If
+you want to maximize a metric, you should multiply the output of your
+objective_function by -1, as shown in the example below. ```python def
+objective_function(X, y): model = LinearRegression() scores = cross_val_score
+(model, X, y, cv=3, scoring="neg_mean_absolute_error") return scores.mean() * -
+1 ``` Next, we set up the Genetic Feature Selector. We've configured the
+genetic algorithm to evolve a population consisting of 200 individuals
+iteratively over 100 generations. To ensure optimal performance, we've set the
+genetic algorithm to halt early if it fails to improve upon the best feature
+set identified within 25 generations. Additionally, for enhanced computational
+efficiency, we've set n_jobs as -1, enabling concurrent execution across all
+available CPUs on our computer. ```python selector = ft.GeneticFeatureSelector
+( objective_function, population_size=200, max_generations=100,
+early_termination_iters=25, n_jobs=-1, ) selector.fit(generated_features,
+y_train) selected_features = selector.transform(generated_features) ``` Let's
+print out the selected features to see what the Genetic Feature Selection
+algorithm kept. You can see below that featuristic has kept four of the
+original features ("weight", "acceleration", "model_year" and "origin") plus
+four of the features created via the Genetic Feature Synthesis. ```python print
+(selected_features.head()) ``` | | weight | acceleration | model_year | origin
+| feature_0 | feature_4 | feature_11 | feature_1 | |---:|---------:|-----------
+----:|-------------:|---------:|------------:|------------:|-------------:|----
+--------:| | 0 | 2050 | 17.3 | 81 | 3 | -8571.63 | -0.312535 | -96.7449 | -
+105.823 | | 1 | 4077 | 14 | 72 | 1 | -2488.32 | -0.786564 | -75.1698 | -34.56 |
+| 2 | 3563 | 10 | 70 | 1 | -2017.65 | -0.727317 | -71.8277 | -28.8235 | | 3 |
+4060 | 19 | 77 | 1 | -4150.3 | -0.684937 | -82.6269 | -53.9 | | 4 | 4080 | 13.7
+| 78 | 1 | -3389.66 | -0.670713 | -81.3604 | -43.4571 | Now that we've selected
+our features, let's see whether they actually help our model's predictive
 performance on our test data set. We'll start off with the original features as
 a baseline. ```python model = LinearRegression() model.fit(X_train, y_train)
 preds = model.predict(X_test) original_mae = mean_absolute_error(y_test, preds)
 print(original_mae) ``` ``` 2.5888868138669303 ``` And now, let's see how the
 model performs with our synthesised feature set. ```python model =
 LinearRegression() model.fit(selected_features, y_train) test_features =
 selector.transform(synth.transform(X_test)) preds = model.predict
 (test_features) featuristic_mae = mean_absolute_error(y_test, preds) print
-(featuristic_mae) ``` ``` 2.1729482398016042 ``` ```python print(f"Original
+(featuristic_mae) ``` ``` 1.9497667311649802 ``` ```python print(f"Original
 MAE: {original_mae}") print(f"Featuristic MAE: {featuristic_mae}") print
 (f"Improvement: {round((1 - (featuristic_mae / original_mae))* 100, 1)}%") ```
-``` Original MAE: 2.5888868138669303 Featuristic MAE: 2.1729482398016042
-Improvement: 16.1% ``` The new features generated / selected by the Genetic
+``` Original MAE: 2.5888868138669303 Featuristic MAE: 1.9497667311649802
+Improvement: 24.7% ``` The new features generated / selected by the Genetic
 Feature Synthesis have successfully reduced our mean absolute error 
```

### Comparing `featuristic-1.0.0/src/featuristic.egg-info/SOURCES.txt` & `featuristic-1.0.1/src/featuristic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE.txt
-README.md
 pyproject.toml
 readme.md
 src/featuristic/__init__.py
 src/featuristic/version.py
 src/featuristic.egg-info/PKG-INFO
 src/featuristic.egg-info/SOURCES.txt
 src/featuristic.egg-info/dependency_links.txt
```

### Comparing `featuristic-1.0.0/tests/test_fitness.py` & `featuristic-1.0.1/tests/test_fitness.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/tests/test_genetic_feature_selection.py` & `featuristic-1.0.1/tests/test_genetic_feature_selection.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/tests/test_genetic_feature_synthesis.py` & `featuristic-1.0.1/tests/test_genetic_feature_synthesis.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/tests/test_programs.py` & `featuristic-1.0.1/tests/test_programs.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.0/tests/test_symbolic_functions.py` & `featuristic-1.0.1/tests/test_symbolic_functions.py`

 * *Files identical despite different names*

