# Comparing `tmp/perfassess-0.0.1.tar.gz` & `tmp/perfassess-0.0.2.tar.gz`

## Comparing `perfassess-0.0.1.tar` & `perfassess-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 perfassess-0.0.1/.gitattributes
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 perfassess-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 perfassess-0.0.1/.github/workflows/build_doc.yml
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 perfassess-0.0.1/.github/workflows/publish_package.yml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 perfassess-0.0.1/.github/workflows/python_package.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 perfassess-0.0.1/data/argument.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 perfassess-0.0.1/data/existing_file.txt
--rw-r--r--   0        0        0  3627651 2020-02-02 00:00:00.000000 perfassess-0.0.1/data/memory_evaluation.html
--rw-r--r--   0        0        0  3865508 2020-02-02 00:00:00.000000 perfassess-0.0.1/data/time_evaluation.html
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/index.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/installation.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/style.css
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/code_documentation/class_performance_assessor.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/code_documentation/main.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/code_documentation/testor.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/code_documentation/parse_argument/check_argument.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/code_documentation/parse_argument/define_argument.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/code_documentation/parse_argument/parse_argument.md
--rw-r--r--   0        0        0  3627648 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/plot/memory_evaluation.html
--rw-r--r--   0        0        0  3865497 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/plot/time_evaluation.html
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/usage/command_line.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 perfassess-0.0.1/docs/usage/module.md
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 perfassess-0.0.1/env/README.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 perfassess-0.0.1/env/perfassess.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 perfassess-0.0.1/env/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/__init__.py
--rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/class_performance_assessor.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/main.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/testor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/parse_argument/__init__.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/parse_argument/check_argument.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/parse_argument/define_argument.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 perfassess-0.0.1/src/perfassess/parse_argument/parse_argument.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 perfassess-0.0.1/tests/test_check_argument.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 perfassess-0.0.1/tests/test_main.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 perfassess-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 perfassess-0.0.1/LICENSE
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 perfassess-0.0.1/README.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 perfassess-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 perfassess-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 perfassess-0.0.2/.gitattributes
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 perfassess-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 perfassess-0.0.2/.github/workflows/build_doc.yml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 perfassess-0.0.2/.github/workflows/publish_pypi_package.yml
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 perfassess-0.0.2/.github/workflows/python_package.yml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 perfassess-0.0.2/data/argument.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 perfassess-0.0.2/data/existing_file.txt
+-rw-r--r--   0        0        0  3627651 2020-02-02 00:00:00.000000 perfassess-0.0.2/data/memory_evaluation.html
+-rw-r--r--   0        0        0  3865508 2020-02-02 00:00:00.000000 perfassess-0.0.2/data/time_evaluation.html
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/index.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/installation.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/style.css
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/code_documentation/class_performance_assessor.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/code_documentation/main.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/code_documentation/testor.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/code_documentation/parse_argument/check_argument.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/code_documentation/parse_argument/define_argument.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/code_documentation/parse_argument/parse_argument.md
+-rw-r--r--   0        0        0  3627648 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/plot/memory_evaluation.html
+-rw-r--r--   0        0        0  3865497 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/plot/time_evaluation.html
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/usage/command_line.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 perfassess-0.0.2/docs/usage/module.md
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 perfassess-0.0.2/env/README.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 perfassess-0.0.2/env/perfassess.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 perfassess-0.0.2/env/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/__init__.py
+-rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/class_performance_assessor.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/main.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/testor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/parse_argument/__init__.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/parse_argument/check_argument.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/parse_argument/define_argument.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 perfassess-0.0.2/src/perfassess/parse_argument/parse_argument.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 perfassess-0.0.2/tests/test_check_argument.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 perfassess-0.0.2/tests/test_main.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 perfassess-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 perfassess-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 perfassess-0.0.2/README.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 perfassess-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 perfassess-0.0.2/PKG-INFO
```

### Comparing `perfassess-0.0.1/mkdocs.yml` & `perfassess-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/.github/workflows/build_doc.yml` & `perfassess-0.0.2/.github/workflows/build_doc.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/.github/workflows/python_package.yml` & `perfassess-0.0.2/.github/workflows/python_package.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/data/memory_evaluation.html` & `perfassess-0.0.2/data/memory_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/data/time_evaluation.html` & `perfassess-0.0.2/data/time_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/index.md` & `perfassess-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/installation.md` & `perfassess-0.0.2/docs/installation.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # ⚙️ Installation
 
-## 👬 Cloning the repository
+## 🥹 EZ way
+
+```bash
+$ pip install perfassess
+```
+
+## 😩 From source
+### 👬 Cloning the repository
 
 You can clone the repository using `HTTPS`:
 
 ```bash
 $ git clone https://github.com/FilouPlains/perfassess.git
 ```
 
@@ -18,17 +25,16 @@
 
 ```bash
 $ cd perfassess
 ```
 
 **All next commands are assuming that you are in the `📁 perfassess/` directory. This directory will be name as `📁 ./`.**
 
-## 🐍📦 Installing with pip
+### 🐍📦 Installing with pip
 
 Simply launch this command in the `📁 ./` directory:
 
 ```bash
 $ python3 -m pip install .
 ```
 
 **You are now able to launch the program!**
-
```

### Comparing `perfassess-0.0.1/docs/style.css` & `perfassess-0.0.2/docs/style.css`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/code_documentation/class_performance_assessor.md` & `perfassess-0.0.2/docs/code_documentation/class_performance_assessor.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/plot/memory_evaluation.html` & `perfassess-0.0.2/docs/plot/memory_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/plot/time_evaluation.html` & `perfassess-0.0.2/docs/plot/time_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/usage/command_line.md` & `perfassess-0.0.2/docs/usage/command_line.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/docs/usage/module.md` & `perfassess-0.0.2/docs/usage/module.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/env/README.md` & `perfassess-0.0.2/env/README.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/env/perfassess.yml` & `perfassess-0.0.2/env/perfassess.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/src/perfassess/class_performance_assessor.py` & `perfassess-0.0.2/src/perfassess/class_performance_assessor.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/src/perfassess/main.py` & `perfassess-0.0.2/src/perfassess/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 
 With "output_directory/" being the output directory of your choice
 """
 
 __authors__ = ["Lucas ROUAUD"]
 __contact__ = ["lucas.rouaud@gmail.com"]
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __date__ = "22/03/2024"
 __copyright__ = "MIT License"
 
 
 # [C]
 from .class_performance_assessor import PerformanceAssessor
 # [P]
```

### Comparing `perfassess-0.0.1/src/perfassess/parse_argument/check_argument.py` & `perfassess-0.0.2/src/perfassess/parse_argument/check_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/src/perfassess/parse_argument/define_argument.py` & `perfassess-0.0.2/src/perfassess/parse_argument/define_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/src/perfassess/parse_argument/parse_argument.py` & `perfassess-0.0.2/src/perfassess/parse_argument/parse_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/tests/test_check_argument.py` & `perfassess-0.0.2/tests/test_check_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/tests/test_main.py` & `perfassess-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/.gitignore` & `perfassess-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/LICENSE` & `perfassess-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.1/README.md` & `perfassess-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,22 @@
 
 - `numpy ≥ 1.26.0`
 - `plotly ≥ 5.19.0`
 - `pyyaml ≥ 6.0.1`
 
 ## ⚙️ Installation
 
-### 👬 Cloning the repository
+### 🥹 EZ way
+
+```bash
+$ pip install perfassess
+```
+
+### 😩 From source
+#### 👬 Cloning the repository
 
 You can clone the repository using `HTTPS`:
 
 ```bash
 $ git clone https://github.com/FilouPlains/perfassess.git
 ```
 
@@ -43,15 +50,15 @@
 
 ```bash
 $ cd perfassess
 ```
 
 **All next commands are assuming that you are in the `📁 perfassess/` directory. This directory will be name as `📁 ./`.**
 
-### 🐍📦 Installing with pip
+#### 🐍📦 Installing with pip
 
 Simply launch this command in the `📁 ./` directory:
 
 ```bash
 $ python3 -m pip install .
 ```
 
@@ -152,23 +159,23 @@
 > 
 > Packages are identify with `__init__.py` files and allow relatives import.
 
 ### 🔍 Describing possible parameters
 
 | **Argument**             | **Mandatory?** | **Type and usage**                  | **Description**                                    |
 | :----------------------- | :------------: | :---------------------------------- | :------------------------------------------------- |
-| **`-s` or `--script`**   |      Yes       | `-s script.py`                      | The script that contain the function to test.      |
-| **`-o` or `--output`**   |      Yes       | `-o output_directory/`              | The directory where the plot have to be produced.  |
-| **`-f` or `--function`** |       No       | `-f main`                           | The function to test.                              |
-| **`-a` or `--argument`** |       No       | `-a argument.yml`                   | The argument to passe to the function to test*.    |
+| **`-s`<br>`--script`**   |      Yes       | `-s script.py`                      | The script that contain the function to test.      |
+| **`-o`<br>`--output`**   |      Yes       | `-o output_directory/`              | The directory where the plot have to be produced.  |
+| **`-f`<br>`--function`** |       No       | `-f main`                           | The function to test.                              |
+| **`-a`<br>`--argument`** |       No       | `-a argument.yml`                   | The argument to passe to the function to test*.    |
 | **`--n_field`**          |       No       | `-n_field 2`                        | The number of field to keep**.                     |
 | **`--package`**          |       No       | `--package package/__init__.py`     | The `__init__.py` file of the top package to test. |
 | **`--subpackage`**       |       No       | `-o package/subpackage/__init__.py` | The `__init__.py` file of the subpackage to test.  |
-| **`-h` or `--help`**     |       No       | Flag                                | Display the help and exit the program.             |
-| **`-v` or `--version`**  |       No       | Flag                                | Display the version and exit the program.          |
+| **`-h`<br>`--help`**     |       No       | Flag                                | Display the help and exit the program.             |
+| **`-v`<br>`--version`**  |       No       | Flag                                | Display the version and exit the program.          |
 
 - **\* =** If you want to test a function that requires arguments, you can give to the command line interface a `argument.yml` file that contains all required arguments. If the tested function requires an argument like `toto`, you can put in the YAML file:
 
 ```yml
 toto: 10
 ```
```

### Comparing `perfassess-0.0.1/pyproject.toml` & `perfassess-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "perfassess"
-version = "0.0.1"
+version = "0.0.2"
 description = "Access the performance of a given function and create plot."
 authors = [{ name = "Lucas ROUAUD", email = "lucas.rouaud@gmail.com" }]
 maintainers = [{ name = "Lucas ROUAUD", email = "lucas.rouaud@gmail.com" }]
 license = { text = "MIT License" }
 readme = "README.md"
 keywords = ["python", "performance", "assessor", "time", "memory", "plot"]
 classifiers = [
```

### Comparing `perfassess-0.0.1/PKG-INFO` & `perfassess-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: perfassess
-Version: 0.0.1
+Version: 0.0.2
 Summary: Access the performance of a given function and create plot.
 Project-URL: Homepage, https://github.com/FilouPlains/perfassess
 Project-URL: Documentation, https://filouplains.github.io/performance_assessor/
 Project-URL: Repository, https://github.com/FilouPlains/perfassess
 Author-email: Lucas ROUAUD <lucas.rouaud@gmail.com>
 Maintainer-email: Lucas ROUAUD <lucas.rouaud@gmail.com>
 License: MIT License
@@ -40,15 +40,22 @@
 
 - `numpy ≥ 1.26.0`
 - `plotly ≥ 5.19.0`
 - `pyyaml ≥ 6.0.1`
 
 ## ⚙️ Installation
 
-### 👬 Cloning the repository
+### 🥹 EZ way
+
+```bash
+$ pip install perfassess
+```
+
+### 😩 From source
+#### 👬 Cloning the repository
 
 You can clone the repository using `HTTPS`:
 
 ```bash
 $ git clone https://github.com/FilouPlains/perfassess.git
 ```
 
@@ -62,15 +69,15 @@
 
 ```bash
 $ cd perfassess
 ```
 
 **All next commands are assuming that you are in the `📁 perfassess/` directory. This directory will be name as `📁 ./`.**
 
-### 🐍📦 Installing with pip
+#### 🐍📦 Installing with pip
 
 Simply launch this command in the `📁 ./` directory:
 
 ```bash
 $ python3 -m pip install .
 ```
 
@@ -171,23 +178,23 @@
 > 
 > Packages are identify with `__init__.py` files and allow relatives import.
 
 ### 🔍 Describing possible parameters
 
 | **Argument**             | **Mandatory?** | **Type and usage**                  | **Description**                                    |
 | :----------------------- | :------------: | :---------------------------------- | :------------------------------------------------- |
-| **`-s` or `--script`**   |      Yes       | `-s script.py`                      | The script that contain the function to test.      |
-| **`-o` or `--output`**   |      Yes       | `-o output_directory/`              | The directory where the plot have to be produced.  |
-| **`-f` or `--function`** |       No       | `-f main`                           | The function to test.                              |
-| **`-a` or `--argument`** |       No       | `-a argument.yml`                   | The argument to passe to the function to test*.    |
+| **`-s`<br>`--script`**   |      Yes       | `-s script.py`                      | The script that contain the function to test.      |
+| **`-o`<br>`--output`**   |      Yes       | `-o output_directory/`              | The directory where the plot have to be produced.  |
+| **`-f`<br>`--function`** |       No       | `-f main`                           | The function to test.                              |
+| **`-a`<br>`--argument`** |       No       | `-a argument.yml`                   | The argument to passe to the function to test*.    |
 | **`--n_field`**          |       No       | `-n_field 2`                        | The number of field to keep**.                     |
 | **`--package`**          |       No       | `--package package/__init__.py`     | The `__init__.py` file of the top package to test. |
 | **`--subpackage`**       |       No       | `-o package/subpackage/__init__.py` | The `__init__.py` file of the subpackage to test.  |
-| **`-h` or `--help`**     |       No       | Flag                                | Display the help and exit the program.             |
-| **`-v` or `--version`**  |       No       | Flag                                | Display the version and exit the program.          |
+| **`-h`<br>`--help`**     |       No       | Flag                                | Display the help and exit the program.             |
+| **`-v`<br>`--version`**  |       No       | Flag                                | Display the version and exit the program.          |
 
 - **\* =** If you want to test a function that requires arguments, you can give to the command line interface a `argument.yml` file that contains all required arguments. If the tested function requires an argument like `toto`, you can put in the YAML file:
 
 ```yml
 toto: 10
 ```
```

