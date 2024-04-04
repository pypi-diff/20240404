# Comparing `tmp/sommify-0.8.1.tar.gz` & `tmp/sommify-0.8.2.tar.gz`

## Comparing `sommify-0.8.1.tar` & `sommify-0.8.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/__init__.py
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/regex.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/test.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/utils.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/countries/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/__init__.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/categories.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/constants.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/cuisine.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/embeddings.py
--rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_funnel.py
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredients.py
--rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/mean_ing_embedding_per_tag.csv
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/meat.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/modifiers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/vegetables.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/vulgar_fractions.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/cheeses.py
--rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/drinks.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/fruit.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/herbs.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/legumes.py
--rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/meats.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/nuts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/pasta.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/spices.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/data/ingredient_categories/vegetables.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/prompts/__init__.py
--rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/prompts/data/__init__.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/prompts/data/default.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/pygrape/__init__.py
--rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/pygrape/data.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/pyregion/__init__.py
--rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/pyregion/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/recipes/__init__.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/recipes/elastic.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/recipes/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/__init__.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/test_elastic.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/test_prompts.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/test_pygrape.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/test_pyregion.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/test_recipe_reader.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.1/sommify/tests/test_tag_reader.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.1/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.1/README.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sommify-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/__init__.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/regex.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/test.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/utils.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/countries/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/__init__.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/categories.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/constants.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/cuisine.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/embeddings.py
+-rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_funnel.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredients.py
+-rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/mean_ing_embedding_per_tag.csv
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/meat.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/modifiers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/vegetables.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/vulgar_fractions.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/cheeses.py
+-rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/drinks.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/fruit.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/herbs.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/legumes.py
+-rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/meats.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/nuts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/pasta.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/spices.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/data/ingredient_categories/vegetables.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/prompts/__init__.py
+-rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/prompts/data/__init__.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/prompts/data/default.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/pygrape/__init__.py
+-rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/pygrape/data.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/pyregion/__init__.py
+-rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/pyregion/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/recipes/__init__.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/recipes/elastic.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/recipes/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/__init__.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/test_elastic.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/test_prompts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/test_pygrape.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/test_pyregion.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/test_recipe_reader.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.2/sommify/tests/test_tag_reader.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.2/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.2/README.md
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sommify-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.2/PKG-INFO
```

### Comparing `sommify-0.8.1/sommify/regex.py` & `sommify-0.8.2/sommify/regex.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/test.py` & `sommify-0.8.2/sommify/test.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/utils.py` & `sommify-0.8.2/sommify/utils.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/countries/__init__.py` & `sommify-0.8.2/sommify/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/categories.py` & `sommify-0.8.2/sommify/data/categories.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/constants.py` & `sommify-0.8.2/sommify/data/constants.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/cuisine.py` & `sommify-0.8.2/sommify/data/cuisine.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/embeddings.py` & `sommify-0.8.2/sommify/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_funnel.py` & `sommify-0.8.2/sommify/data/ingredient_funnel.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredients.py` & `sommify-0.8.2/sommify/data/ingredients.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/mean_ing_embedding_per_tag.csv` & `sommify-0.8.2/sommify/data/mean_ing_embedding_per_tag.csv`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/meat.py` & `sommify-0.8.2/sommify/data/meat.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/modifiers.py` & `sommify-0.8.2/sommify/data/modifiers.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/vegetables.py` & `sommify-0.8.2/sommify/data/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/__init__.py` & `sommify-0.8.2/sommify/data/ingredient_categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/drinks.py` & `sommify-0.8.2/sommify/data/ingredient_categories/drinks.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/fruit.py` & `sommify-0.8.2/sommify/data/ingredient_categories/fruit.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/herbs.py` & `sommify-0.8.2/sommify/data/ingredient_categories/herbs.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/meats.py` & `sommify-0.8.2/sommify/data/ingredient_categories/meats.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/nuts.py` & `sommify-0.8.2/sommify/data/ingredient_categories/nuts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/spices.py` & `sommify-0.8.2/sommify/data/ingredient_categories/spices.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/data/ingredient_categories/vegetables.py` & `sommify-0.8.2/sommify/data/ingredient_categories/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/prompts/__init__.py` & `sommify-0.8.2/sommify/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/prompts/data/__init__.py` & `sommify-0.8.2/sommify/prompts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/prompts/data/default.py` & `sommify-0.8.2/sommify/prompts/data/default.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/pygrape/__init__.py` & `sommify-0.8.2/sommify/pygrape/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/pygrape/data.py` & `sommify-0.8.2/sommify/pygrape/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/pyregion/__init__.py` & `sommify-0.8.2/sommify/pyregion/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/pyregion/data.py` & `sommify-0.8.2/sommify/pyregion/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/recipes/elastic.py` & `sommify-0.8.2/sommify/recipes/elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/recipes/reader.py` & `sommify-0.8.2/sommify/recipes/reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/tests/test_elastic.py` & `sommify-0.8.2/sommify/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/tests/test_prompts.py` & `sommify-0.8.2/sommify/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/sommify/tests/test_recipe_reader.py` & `sommify-0.8.2/sommify/tests/test_recipe_reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/.gitignore` & `sommify-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/LICENSE` & `sommify-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sommify-0.8.1/pyproject.toml` & `sommify-0.8.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "sommify"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="William Brach", email="william@sommify.ai" },
   { name="Tomas Bedej", email="tomas@sommify.ai" },
 ]
 description = "A package for recipe parsing"
 dependencies = [
   "inflect==7.0.0", 
   "numpy>=1.23.2",
-  "pandas>=1.5.0",
-  "spacy>=3.0.0,<4.0.0",
-  "sentence-transformers>=2.5.1",
-  "qdrant_client>=1.8.0",
+  "pandas==1.5.0",
+  "spacy==3.0.0,<4.0.0",
+  "sentence-transformers==2.5.1",
+  "qdrant_client==1.8.0",
   "elasticsearch>=7.17.0,<8.0.0",
-  "nltk>=3.7",
-  "thefuzz>=0.19.0",
-  "unidecode>=1.3.6",
+  "nltk==3.7",
+  "thefuzz==0.19.0",
+  "unidecode==1.3.6",
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `sommify-0.8.1/PKG-INFO` & `sommify-0.8.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.3
 Name: sommify
-Version: 0.8.1
+Version: 0.8.2
 Summary: A package for recipe parsing
 Author-email: William Brach <william@sommify.ai>, Tomas Bedej <tomas@sommify.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: elasticsearch<8.0.0,>=7.17.0
 Requires-Dist: inflect==7.0.0
-Requires-Dist: nltk>=3.7
+Requires-Dist: nltk==3.7
 Requires-Dist: numpy>=1.23.2
-Requires-Dist: pandas>=1.5.0
-Requires-Dist: qdrant-client>=1.8.0
-Requires-Dist: sentence-transformers>=2.5.1
-Requires-Dist: spacy<4.0.0,>=3.0.0
-Requires-Dist: thefuzz>=0.19.0
-Requires-Dist: unidecode>=1.3.6
+Requires-Dist: pandas==1.5.0
+Requires-Dist: qdrant-client==1.8.0
+Requires-Dist: sentence-transformers==2.5.1
+Requires-Dist: spacy<4.0.0,==3.0.0
+Requires-Dist: thefuzz==0.19.0
+Requires-Dist: unidecode==1.3.6
 Description-Content-Type: text/markdown
 
 ```
 python -m build
 ```
 
 ```
```

