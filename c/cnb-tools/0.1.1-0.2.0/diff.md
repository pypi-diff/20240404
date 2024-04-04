# Comparing `tmp/cnb_tools-0.1.1.tar.gz` & `tmp/cnb_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnb_tools-0.1.1.tar", max compression
+gzip compressed data, was "cnb_tools-0.2.0.tar", max compression
```

## Comparing `cnb_tools-0.1.1.tar` & `cnb_tools-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-12-01 08:54:37.092267 cnb_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0     2839 2023-12-04 19:41:28.900524 cnb_tools-0.1.1/README.md
--rw-r--r--   0        0        0       81 2023-12-01 08:54:37.093356 cnb_tools-0.1.1/cnb_tools/__init__.py
--rw-r--r--   0        0        0       54 2023-12-01 08:54:37.094051 cnb_tools-0.1.1/cnb_tools/__main__.py
--rw-r--r--   0        0        0      825 2023-12-04 04:25:58.248817 cnb_tools-0.1.1/cnb_tools/main_cli.py
--rw-r--r--   0        0        0     1670 2023-12-05 00:49:13.225652 cnb_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 cnb_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 21:14:14.440131 cnb_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3419 2024-03-22 21:14:14.440280 cnb_tools-0.2.0/README.md
+-rw-r--r--   0        0        0       81 2024-03-22 21:14:14.440477 cnb_tools-0.2.0/cnb_tools/__init__.py
+-rw-r--r--   0        0        0       54 2024-03-22 21:14:14.440603 cnb_tools-0.2.0/cnb_tools/__main__.py
+-rw-r--r--   0        0        0     2359 2024-04-01 19:58:34.033172 cnb_tools-0.2.0/cnb_tools/classes/annotation.py
+-rw-r--r--   0        0        0     1350 2024-04-01 19:58:34.033515 cnb_tools-0.2.0/cnb_tools/classes/base.py
+-rw-r--r--   0        0        0     1003 2024-04-01 19:58:34.033747 cnb_tools-0.2.0/cnb_tools/classes/participant.py
+-rw-r--r--   0        0        0      988 2024-04-01 19:58:34.034075 cnb_tools-0.2.0/cnb_tools/classes/queue.py
+-rw-r--r--   0        0        0     2123 2024-04-01 22:53:45.728542 cnb_tools-0.2.0/cnb_tools/classes/submission.py
+-rw-r--r--   0        0        0     3535 2024-04-04 16:24:02.597596 cnb_tools-0.2.0/cnb_tools/commands/submission_cli.py
+-rw-r--r--   0        0        0     1183 2024-04-04 16:17:12.393627 cnb_tools-0.2.0/cnb_tools/main_cli.py
+-rw-r--r--   0        0        0     1688 2024-04-04 19:43:53.397715 cnb_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 cnb_tools-0.2.0/PKG-INFO
```

### Comparing `cnb_tools-0.1.1/LICENSE` & `cnb_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.1.1/README.md` & `cnb_tools-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -47,40 +47,55 @@
 
 Generate a new Synapse [Personal Access Token (PAT)] with all token
 permissions enabled, then copy-paste it into `authtoken`. Save the file.
 
 For security, we recommend updating its permissions so that other
 users on your machine do not have read access to your credentials, e.g.
 
-```sh
+```console
 chmod 600 ~/.synapseConfig
 ```
 
 ## Installation
 
-```sh
+For best practice, use a Python environment to install **cnb-tools**
+rather than directly into your base env.  In our docs, we will be
+using [miniconda], but you can use [miniforge], [venv], [pyenv], etc.
+
+<!-- termynal -->
+```console
+# Create a new env and activate it
+conda create -n cnb-tools python=3.12 -y
+conda activate cnb-tools
+
+# Install cnb-tools using pip
 pip install cnb-tools
 ```
 
-> [!NOTE]
+> ⓘ **NOTE**
+>
 > **cnb-tools** builds off of the Synapse Python Client — by
 > installing **cnb-tools**, you will also be installing **synapseclient**.
 >  
 > → [Read its docs.]
 
 Verify the installation with:
 
-```sh
-cnb-tools --version
+```console
+cnb-tools
 ```
 
 ## License
 
 **cnb-tools** is released under the Apache 2.0 license.
 
 [https://sage-bionetworks-challenges.github.io/cnb-tools]: https://sage-bionetworks-challenges.github.io/cnb-tools
 [https://github.com/Sage-Bionetworks-Challenges/cnb-tools]: https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 [DREAM Challenges]: https://dreamchallenges.org/
 [Python 3.9+]: https://www.python.org/downloads/
 [Synapse account]: https://www.synapse.org/#!LoginPlace:0
 [Personal Access Token (PAT)]: https://www.synapse.org/#!PersonalAccessTokens:
-[Read its docs.]: https://python-docs.synapse.org/build/html/index.html
+[miniconda]: https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html
+[miniforge]: https://github.com/conda-forge/miniforge
+[venv]: https://docs.python.org/3/library/venv.html
+[pyenv]: https://github.com/pyenv/pyenv
+[Read its docs.]: https://python-docs.synapse.org/
```

#### html2text {}

```diff
@@ -12,20 +12,27 @@
 3.9+] - [Synapse account] To fully utilize **cnb-tools**, you must have a
 Synapse account and provide your credentials to the tool. To do so, create a
 `.synapseConfig` file in your home directory, and enter the following: ```yaml
 [authentication] authtoken = "YOUR PAT" ``` Generate a new Synapse [Personal
 Access Token (PAT)] with all token permissions enabled, then copy-paste it into
 `authtoken`. Save the file. For security, we recommend updating its permissions
 so that other users on your machine do not have read access to your
-credentials, e.g. ```sh chmod 600 ~/.synapseConfig ``` ## Installation ```sh
-pip install cnb-tools ``` > [!NOTE] > **cnb-tools** builds off of the Synapse
-Python Client â by > installing **cnb-tools**, you will also be installing
-**synapseclient**. > > â [Read its docs.] Verify the installation with: ```sh
-cnb-tools --version ``` ## License **cnb-tools** is released under the Apache
-2.0 license. [https://sage-bionetworks-challenges.github.io/cnb-tools]: https:/
-/sage-bionetworks-challenges.github.io/cnb-tools [https://github.com/Sage-
-Bionetworks-Challenges/cnb-tools]: https://github.com/Sage-Bionetworks-
-Challenges/cnb-tools [DREAM Challenges]: https://dreamchallenges.org/ [Python
-3.9+]: https://www.python.org/downloads/ [Synapse account]: https://
-www.synapse.org/#!LoginPlace:0 [Personal Access Token (PAT)]: https://
-www.synapse.org/#!PersonalAccessTokens: [Read its docs.]: https://python-
-docs.synapse.org/build/html/index.html
+credentials, e.g. ```console chmod 600 ~/.synapseConfig ``` ## Installation For
+best practice, use a Python environment to install **cnb-tools** rather than
+directly into your base env. In our docs, we will be using [miniconda], but you
+can use [miniforge], [venv], [pyenv], etc. ```console # Create a new env and
+activate it conda create -n cnb-tools python=3.12 -y conda activate cnb-tools #
+Install cnb-tools using pip pip install cnb-tools ``` > â **NOTE** > > **cnb-
+tools** builds off of the Synapse Python Client â by > installing **cnb-
+tools**, you will also be installing **synapseclient**. > > â [Read its
+docs.] Verify the installation with: ```console cnb-tools ``` ## License **cnb-
+tools** is released under the Apache 2.0 license. [https://sage-bionetworks-
+challenges.github.io/cnb-tools]: https://sage-bionetworks-challenges.github.io/
+cnb-tools [https://github.com/Sage-Bionetworks-Challenges/cnb-tools]: https://
+github.com/Sage-Bionetworks-Challenges/cnb-tools [DREAM Challenges]: https://
+dreamchallenges.org/ [Python 3.9+]: https://www.python.org/downloads/ [Synapse
+account]: https://www.synapse.org/#!LoginPlace:0 [Personal Access Token (PAT)]:
+https://www.synapse.org/#!PersonalAccessTokens: [miniconda]: https://
+docs.conda.io/projects/miniconda/en/latest/miniconda-install.html [miniforge]:
+https://github.com/conda-forge/miniforge [venv]: https://docs.python.org/3/
+library/venv.html [pyenv]: https://github.com/pyenv/pyenv [Read its docs.]:
+https://python-docs.synapse.org/
```

### Comparing `cnb_tools-0.1.1/pyproject.toml` & `cnb_tools-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "cnb-tools"
-version = "0.1.1"
+version = "0.2.0"
 description = "Convenience tools/functions for challenges and benchmarking on Synapse.org"
 license = "Apache-2.0"
 authors = ["Sage CNB Team <cnb@sagebase.org>"]
 maintainers = [
     "Verena Chung <verena.chung@sagebase.org>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sage-Bionetworks-Challenges/cnb-tools"
 documentation = "https://sage-bionetworks-challenges.github.io/cnb-tools"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
@@ -26,15 +26,15 @@
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9.0"}
-synapseclient = "3.2.0"
+synapseclient = "4.1.1"
 
 [tool.poetry.scripts]
 cnb-tools = "cnb_tools.main_cli:app"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Sage-Bionetworks-Challenges/cnb-tools/issues"
 
@@ -42,11 +42,12 @@
 pytest = "^7.4.3"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.4.14"
 mkdocstrings = "^0.24.0"
 mkdocstrings-python = "^1.7.5"
+termynal = "^0.11.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cnb_tools-0.1.1/PKG-INFO` & `cnb_tools-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cnb-tools
-Version: 0.1.1
+Version: 0.2.0
 Summary: Convenience tools/functions for challenges and benchmarking on Synapse.org
 Home-page: https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 License: Apache-2.0
 Author: Sage CNB Team
 Author-email: cnb@sagebase.org
 Maintainer: Verena Chung
 Maintainer-email: verena.chung@sagebase.org
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: synapseclient (==3.2.0)
+Requires-Dist: synapseclient (==4.1.1)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/Sage-Bionetworks-Challenges/cnb-tools/issues
 Project-URL: Documentation, https://sage-bionetworks-challenges.github.io/cnb-tools
 Project-URL: Repository, https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -79,41 +79,56 @@
 
 Generate a new Synapse [Personal Access Token (PAT)] with all token
 permissions enabled, then copy-paste it into `authtoken`. Save the file.
 
 For security, we recommend updating its permissions so that other
 users on your machine do not have read access to your credentials, e.g.
 
-```sh
+```console
 chmod 600 ~/.synapseConfig
 ```
 
 ## Installation
 
-```sh
+For best practice, use a Python environment to install **cnb-tools**
+rather than directly into your base env.  In our docs, we will be
+using [miniconda], but you can use [miniforge], [venv], [pyenv], etc.
+
+<!-- termynal -->
+```console
+# Create a new env and activate it
+conda create -n cnb-tools python=3.12 -y
+conda activate cnb-tools
+
+# Install cnb-tools using pip
 pip install cnb-tools
 ```
 
-> [!NOTE]
+> ⓘ **NOTE**
+>
 > **cnb-tools** builds off of the Synapse Python Client — by
 > installing **cnb-tools**, you will also be installing **synapseclient**.
 >  
 > → [Read its docs.]
 
 Verify the installation with:
 
-```sh
-cnb-tools --version
+```console
+cnb-tools
 ```
 
 ## License
 
 **cnb-tools** is released under the Apache 2.0 license.
 
 [https://sage-bionetworks-challenges.github.io/cnb-tools]: https://sage-bionetworks-challenges.github.io/cnb-tools
 [https://github.com/Sage-Bionetworks-Challenges/cnb-tools]: https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 [DREAM Challenges]: https://dreamchallenges.org/
 [Python 3.9+]: https://www.python.org/downloads/
 [Synapse account]: https://www.synapse.org/#!LoginPlace:0
 [Personal Access Token (PAT)]: https://www.synapse.org/#!PersonalAccessTokens:
-[Read its docs.]: https://python-docs.synapse.org/build/html/index.html
+[miniconda]: https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html
+[miniforge]: https://github.com/conda-forge/miniforge
+[venv]: https://docs.python.org/3/library/venv.html
+[pyenv]: https://github.com/pyenv/pyenv
+[Read its docs.]: https://python-docs.synapse.org/
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: cnb-tools Version: 0.1.1 Summary: Convenience
+Metadata-Version: 2.1 Name: cnb-tools Version: 0.2.0 Summary: Convenience
 tools/functions for challenges and benchmarking on Synapse.org Home-page:
 https://github.com/Sage-Bionetworks-Challenges/cnb-tools License: Apache-2.0
 Author: Sage CNB Team Author-email: cnb@sagebase.org Maintainer: Verena Chung
 Maintainer-email: verena.chung@sagebase.org Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 1 - Planning Classifier: Intended Audience ::
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Dist: synapseclient (==3.2.0) Requires-
+Libraries :: Python Modules Requires-Dist: synapseclient (==4.1.1) Requires-
 Dist: typer[all] (>=0.9.0,<0.10.0) Project-URL: Bug Tracker, https://
 github.com/Sage-Bionetworks-Challenges/cnb-tools/issues Project-URL:
 Documentation, https://sage-bionetworks-challenges.github.io/cnb-tools Project-
 URL: Repository, https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 Description-Content-Type: text/markdown
 ![cnb-tools](https://raw.githubusercontent.com/Sage-Bionetworks-Challenges/cnb-
                      tools/main/docs/assets/cnb-tools.png)
@@ -32,20 +32,27 @@
 3.9+] - [Synapse account] To fully utilize **cnb-tools**, you must have a
 Synapse account and provide your credentials to the tool. To do so, create a
 `.synapseConfig` file in your home directory, and enter the following: ```yaml
 [authentication] authtoken = "YOUR PAT" ``` Generate a new Synapse [Personal
 Access Token (PAT)] with all token permissions enabled, then copy-paste it into
 `authtoken`. Save the file. For security, we recommend updating its permissions
 so that other users on your machine do not have read access to your
-credentials, e.g. ```sh chmod 600 ~/.synapseConfig ``` ## Installation ```sh
-pip install cnb-tools ``` > [!NOTE] > **cnb-tools** builds off of the Synapse
-Python Client â by > installing **cnb-tools**, you will also be installing
-**synapseclient**. > > â [Read its docs.] Verify the installation with: ```sh
-cnb-tools --version ``` ## License **cnb-tools** is released under the Apache
-2.0 license. [https://sage-bionetworks-challenges.github.io/cnb-tools]: https:/
-/sage-bionetworks-challenges.github.io/cnb-tools [https://github.com/Sage-
-Bionetworks-Challenges/cnb-tools]: https://github.com/Sage-Bionetworks-
-Challenges/cnb-tools [DREAM Challenges]: https://dreamchallenges.org/ [Python
-3.9+]: https://www.python.org/downloads/ [Synapse account]: https://
-www.synapse.org/#!LoginPlace:0 [Personal Access Token (PAT)]: https://
-www.synapse.org/#!PersonalAccessTokens: [Read its docs.]: https://python-
-docs.synapse.org/build/html/index.html
+credentials, e.g. ```console chmod 600 ~/.synapseConfig ``` ## Installation For
+best practice, use a Python environment to install **cnb-tools** rather than
+directly into your base env. In our docs, we will be using [miniconda], but you
+can use [miniforge], [venv], [pyenv], etc. ```console # Create a new env and
+activate it conda create -n cnb-tools python=3.12 -y conda activate cnb-tools #
+Install cnb-tools using pip pip install cnb-tools ``` > â **NOTE** > > **cnb-
+tools** builds off of the Synapse Python Client â by > installing **cnb-
+tools**, you will also be installing **synapseclient**. > > â [Read its
+docs.] Verify the installation with: ```console cnb-tools ``` ## License **cnb-
+tools** is released under the Apache 2.0 license. [https://sage-bionetworks-
+challenges.github.io/cnb-tools]: https://sage-bionetworks-challenges.github.io/
+cnb-tools [https://github.com/Sage-Bionetworks-Challenges/cnb-tools]: https://
+github.com/Sage-Bionetworks-Challenges/cnb-tools [DREAM Challenges]: https://
+dreamchallenges.org/ [Python 3.9+]: https://www.python.org/downloads/ [Synapse
+account]: https://www.synapse.org/#!LoginPlace:0 [Personal Access Token (PAT)]:
+https://www.synapse.org/#!PersonalAccessTokens: [miniconda]: https://
+docs.conda.io/projects/miniconda/en/latest/miniconda-install.html [miniforge]:
+https://github.com/conda-forge/miniforge [venv]: https://docs.python.org/3/
+library/venv.html [pyenv]: https://github.com/pyenv/pyenv [Read its docs.]:
+https://python-docs.synapse.org/
```

