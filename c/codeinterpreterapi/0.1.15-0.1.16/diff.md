# Comparing `tmp/codeinterpreterapi-0.1.15.tar.gz` & `tmp/codeinterpreterapi-0.1.16.tar.gz`

## Comparing `codeinterpreterapi-0.1.15.tar` & `codeinterpreterapi-0.1.16.tar`

### file list

```diff
@@ -1,64 +1,62 @@
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.env.example
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.pre-commit-config.yaml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.python-version
--rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/dev-setup.sh
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/mkdocs.yml
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/requirements-dev.lock
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/roadmap.todo
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.github/FUNDING.yml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.github/dependabot.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.github/workflows/ci.yml
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.github/workflows/code-check.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/bitcoin_chart.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/code_interpreter_response.md
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/code_interpreter_session.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/codebox.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/concepts_overview.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/deploy.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/file.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/index.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/installation.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/iris_dataset.md
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/settings.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/streamlit_webapp.md
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/usage.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/docs/user_request.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/analyze_dataset.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/anthropic_claude.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/chat_cli.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/chat_history_backend.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/convert_file.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/plot_sin_wave.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/show_bitcoin_chart.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/use_additional_tools.py
--rw-r--r--   0        0        0    62087 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/assets/bitcoin_chart.png
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/assets/iris.csv
--rw-r--r--   0        0        0   138297 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/assets/iris_analysis.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/frontend/__init__.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/frontend/app.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/frontend/chainlitui.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/examples/frontend/utils.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/chat_history.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/config.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/parser.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/schema.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/extract_code.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/rm_dl_link.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/modifications_check.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/remove_dl_link.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/tests/general_test.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/tests/run_examples.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/LICENSE
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/README.md
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/pyproject.toml
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.env.example
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.python-version
+-rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/dev-setup.sh
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/mkdocs.yml
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/requirements-dev.lock
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/roadmap.todo
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/FUNDING.yml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/dependabot.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/bitcoin_chart.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/code_interpreter_response.md
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/code_interpreter_session.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/codebox.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/concepts_overview.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/deploy.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/file.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/index.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/installation.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/iris_dataset.md
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/settings.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/streamlit_webapp.md
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/usage.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/user_request.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/analyze_dataset.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/anthropic_claude.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/chat_cli.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/chat_history_backend.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/convert_file.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/plot_sin_wave.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/show_bitcoin_chart.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/use_additional_tools.py
+-rw-r--r--   0        0        0    62087 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/assets/bitcoin_chart.png
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/assets/iris.csv
+-rw-r--r--   0        0        0   138297 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/assets/iris_analysis.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/app.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/chainlitui.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/_patch_parser.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chat_history.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/schema.py
+-rw-r--r--   0        0        0    20167 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/extract_code.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/rm_dl_link.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/modifications_check.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/tests/chain_test.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/tests/general_test.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/tests/run_examples.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/LICENSE
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/README.md
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/PKG-INFO
```

### Comparing `codeinterpreterapi-0.1.15/mkdocs.yml` & `codeinterpreterapi-0.1.16/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/.github/FUNDING.yml` & `codeinterpreterapi-0.1.16/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/.github/workflows/ci.yml` & `codeinterpreterapi-0.1.16/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/.github/workflows/python-publish.yml` & `codeinterpreterapi-0.1.16/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/bitcoin_chart.md` & `codeinterpreterapi-0.1.16/docs/bitcoin_chart.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/code_interpreter_session.md` & `codeinterpreterapi-0.1.16/docs/code_interpreter_session.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/codebox.md` & `codeinterpreterapi-0.1.16/docs/codebox.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/deploy.md` & `codeinterpreterapi-0.1.16/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/file.md` & `codeinterpreterapi-0.1.16/docs/file.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/index.md` & `codeinterpreterapi-0.1.16/docs/index.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/installation.md` & `codeinterpreterapi-0.1.16/docs/installation.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/iris_dataset.md` & `codeinterpreterapi-0.1.16/docs/iris_dataset.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/docs/settings.md` & `codeinterpreterapi-0.1.16/docs/settings.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/examples/analyze_dataset.py` & `codeinterpreterapi-0.1.16/examples/analyze_dataset.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/examples/chat_history_backend.py` & `codeinterpreterapi-0.1.16/examples/chat_history_backend.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/examples/use_additional_tools.py` & `codeinterpreterapi-0.1.16/examples/use_additional_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 so it can download the bitcoin chart from yahoo finance
 and plot it for you
 """
 import csv
 import io
 from typing import Any
 
-from langchain.tools import BaseTool
-
 from codeinterpreterapi import CodeInterpreterSession
+from langchain_core.tools import BaseTool
 
 
 class ExampleKnowledgeBaseTool(BaseTool):
     name: str = "salary_database"
     description: str = "Use to get salary data of company employees"
 
     def _run(self, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `codeinterpreterapi-0.1.15/examples/assets/bitcoin_chart.png` & `codeinterpreterapi-0.1.16/examples/assets/bitcoin_chart.png`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/examples/assets/iris.csv` & `codeinterpreterapi-0.1.16/examples/assets/iris.csv`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/examples/assets/iris_analysis.png` & `codeinterpreterapi-0.1.16/examples/assets/iris_analysis.png`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/examples/frontend/app.py` & `codeinterpreterapi-0.1.16/examples/frontend/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import sys
 
 import streamlit as st
-from utils import get_images  # type: ignore
-
 from codeinterpreterapi import File
+from utils import get_images  # type: ignore
 
 # Page configuration
 st.set_page_config(layout="wide")
 
 st.title("Code Interpreter API 🚀")
 
 # This will create a sidebar
```

### Comparing `codeinterpreterapi-0.1.15/examples/frontend/chainlitui.py` & `codeinterpreterapi-0.1.16/examples/frontend/chainlitui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import chainlit as cl  # type: ignore
-
 from codeinterpreterapi import CodeInterpreterSession
 from codeinterpreterapi import File as CIFile
 
 UPLOADED_FILES: list[CIFile] = []
 
 
 @cl.action_callback("upload_file")
```

### Comparing `codeinterpreterapi-0.1.15/examples/frontend/utils.py` & `codeinterpreterapi-0.1.16/examples/frontend/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import shutil
 import tempfile
 from typing import Optional
 
 import streamlit as st
-
 from codeinterpreterapi import CodeInterpreterSession
 
 
 def create_temp_folder() -> str:
     """
     Creates a temp folder
     """
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/chat_history.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chat_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import asyncio
 import json
 from typing import List
 
-from codeboxapi import CodeBox  # type: ignore
-from langchain.schema import BaseChatMessageHistory
-from langchain.schema.messages import BaseMessage, messages_from_dict, messages_to_dict
+from codeboxapi import CodeBox
+from langchain_core.chat_history import BaseChatMessageHistory
+from langchain_core.messages import BaseMessage, messages_from_dict, messages_to_dict
 
 
-# TODO: This is probably not efficient, but it works for now.
 class CodeBoxChatMessageHistory(BaseChatMessageHistory):
     """
     Chat message history that stores history inside the codebox.
     """
 
     def __init__(self, codebox: CodeBox):
         self.codebox = codebox
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/config.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from typing import Optional
 
-from dotenv import load_dotenv
-from langchain.pydantic_v1 import BaseSettings, SecretStr
-from langchain.schema import SystemMessage
+from langchain_core.messages import SystemMessage
+from langchain_core.pydantic_v1 import BaseSettings, SecretStr
 
 from codeinterpreterapi.prompts import code_interpreter_system_message
 
-# .env file
-load_dotenv(dotenv_path="./.env")
-
 
 class CodeInterpreterAPISettings(BaseSettings):
     """
     CodeInterpreter API Config
     """
 
     DEBUG: bool = False
 
     # Models
-    OPENAI_API_KEY: Optional[str] = None
-    AZURE_API_KEY: Optional[str] = None
+    OPENAI_API_KEY: Optional[SecretStr] = None
+    AZURE_OPENAI_API_KEY: Optional[SecretStr] = None
     AZURE_API_BASE: Optional[str] = None
     AZURE_API_VERSION: Optional[str] = None
     AZURE_DEPLOYMENT_NAME: Optional[str] = None
     ANTHROPIC_API_KEY: Optional[SecretStr] = None
 
     # LLM Settings
     MODEL: str = "gpt-3.5-turbo"
@@ -42,9 +38,13 @@
     # CodeBox
     CODEBOX_API_KEY: Optional[str] = None
     CUSTOM_PACKAGES: list[str] = []
 
     # deprecated
     VERBOSE: bool = DEBUG
 
+    class Config:
+        env_file = "./.env"
+        extra = "ignore"
+
 
 settings = CodeInterpreterAPISettings()
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/schema.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from typing import Any
 
 from codeboxapi.schema import CodeBoxStatus
-from langchain.pydantic_v1 import BaseModel
-from langchain.schema import AIMessage, HumanMessage
+from langchain_core.messages import AIMessage, HumanMessage
+from langchain_core.pydantic_v1 import BaseModel
 
 
 class File(BaseModel):
     name: str
     content: bytes
 
     @classmethod
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/session.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,37 +11,36 @@
 from langchain.agents import (
     AgentExecutor,
     BaseSingleActionAgent,
     ConversationalAgent,
     ConversationalChatAgent,
 )
 from langchain.agents.openai_functions_agent.base import OpenAIFunctionsAgent
-from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.base import Callbacks
-from langchain.chat_models import AzureChatOpenAI, ChatAnthropic, ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
-from langchain.memory import ConversationBufferMemory
-from langchain.memory.chat_message_histories import (
-    ChatMessageHistory,
+from langchain.memory.buffer import ConversationBufferMemory
+from langchain_community.chat_message_histories.in_memory import ChatMessageHistory
+from langchain_community.chat_message_histories.postgres import (
     PostgresChatMessageHistory,
-    RedisChatMessageHistory,
 )
-from langchain.prompts.chat import MessagesPlaceholder
-from langchain.schema import BaseChatMessageHistory
-from langchain.tools import BaseTool, StructuredTool
+from langchain_community.chat_message_histories.redis import RedisChatMessageHistory
+from langchain_core.chat_history import BaseChatMessageHistory
+from langchain_core.language_models import BaseLanguageModel
+from langchain_core.prompts.chat import MessagesPlaceholder
+from langchain_core.tools import BaseTool, StructuredTool
+from langchain_openai import AzureChatOpenAI, ChatOpenAI
 
 from codeinterpreterapi.chains import (
     aget_file_modifications,
     aremove_download_link,
     get_file_modifications,
     remove_download_link,
 )
 from codeinterpreterapi.chat_history import CodeBoxChatMessageHistory
 from codeinterpreterapi.config import settings
-from codeinterpreterapi.parser import CodeAgentOutputParser, CodeChatAgentOutputParser
 from codeinterpreterapi.schema import (
     CodeInput,
     CodeInterpreterResponse,
     File,
     SessionStatus,
     UserRequest,
 )
@@ -111,52 +110,56 @@
                 "be really long, so you can use the `;` character to split lines. "
                 "Start your code on the same line as the opening quote. "
                 "Do not start your code with a line break. "
                 "For example, do 'import numpy', not '\\nimport numpy'."
                 "Variables are preserved between runs. "
                 + (
                     (
-                        f"You can use all default python packages specifically also these: {settings.CUSTOM_PACKAGES}"
+                        "You can use all default python packages "
+                        f"specifically also these: {settings.CUSTOM_PACKAGES}"
                     )
                     if settings.CUSTOM_PACKAGES
                     else ""
                 ),  # TODO: or include this in the system message
                 func=self._run_handler,
                 coroutine=self._arun_handler,
                 args_schema=CodeInput,  # type: ignore
             ),
         ]
 
     def _choose_llm(self) -> BaseChatModel:
         if (
-            settings.AZURE_API_KEY
+            settings.AZURE_OPENAI_API_KEY
             and settings.AZURE_API_BASE
             and settings.AZURE_API_VERSION
             and settings.AZURE_DEPLOYMENT_NAME
         ):
             self.log("Using Azure Chat OpenAI")
             return AzureChatOpenAI(
                 temperature=0.03,
                 base_url=settings.AZURE_API_BASE,
                 api_version=settings.AZURE_API_VERSION,
                 azure_deployment=settings.AZURE_DEPLOYMENT_NAME,
-                api_key=settings.AZURE_API_KEY,
+                api_key=settings.AZURE_OPENAI_API_KEY,
                 max_retries=settings.MAX_RETRY,
                 timeout=settings.REQUEST_TIMEOUT,
             )  # type: ignore
         if settings.OPENAI_API_KEY:
-            self.log("Using Chat OpenAI")
+            from langchain_openai import ChatOpenAI
+
             return ChatOpenAI(
                 model=settings.MODEL,
                 api_key=settings.OPENAI_API_KEY,
                 timeout=settings.REQUEST_TIMEOUT,
                 temperature=settings.TEMPERATURE,
                 max_retries=settings.MAX_RETRY,
             )  # type: ignore
         if settings.ANTHROPIC_API_KEY:
+            from langchain_anthropic import ChatAnthropic  # type: ignore
+
             if "claude" not in settings.MODEL:
                 print("Please set the claude model in the settings.")
             self.log("Using Chat Anthropic")
             return ChatAnthropic(
                 model_name=settings.MODEL,
                 temperature=settings.TEMPERATURE,
                 anthropic_api_key=settings.ANTHROPIC_API_KEY,
@@ -169,27 +172,25 @@
                 llm=self.llm,
                 tools=self.tools,
                 system_message=settings.SYSTEM_MESSAGE,
                 extra_prompt_messages=[
                     MessagesPlaceholder(variable_name="chat_history")
                 ],
             )
-            if isinstance(self.llm, ChatOpenAI)
+            if isinstance(self.llm, ChatOpenAI) or isinstance(self.llm, AzureChatOpenAI)
             else ConversationalChatAgent.from_llm_and_tools(
                 llm=self.llm,
                 tools=self.tools,
                 system_message=settings.SYSTEM_MESSAGE.content.__str__(),
-                output_parser=CodeChatAgentOutputParser(self.llm),
             )
             if isinstance(self.llm, BaseChatModel)
             else ConversationalAgent.from_llm_and_tools(
                 llm=self.llm,
                 tools=self.tools,
                 prefix=settings.SYSTEM_MESSAGE.content.__str__(),
-                output_parser=CodeAgentOutputParser(),
             )
         )
 
     def _history_backend(self) -> BaseChatMessageHistory:
         return (
             CodeBoxChatMessageHistory(codebox=self.codebox)
             if settings.HISTORY_BACKEND == "codebox"
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/extract_code.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/extract_code.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from langchain.base_language import BaseLanguageModel
-from langchain.chat_models.anthropic import ChatAnthropic
+from langchain_core.language_models import BaseLanguageModel
 
 
 def extract_python_code(
     text: str,
     llm: BaseLanguageModel,
     retry: int = 2,
 ) -> str:
@@ -15,15 +14,17 @@
     llm: BaseLanguageModel,
     retry: int = 2,
 ) -> str:
     return "TODO"
 
 
 async def test() -> None:
-    llm = ChatAnthropic(model="claude-1.3")  # type: ignore
+    from langchain_openai import ChatOpenAI
+
+    llm = ChatOpenAI()
 
     code = """
         import matplotlib.pyplot as plt
 
         x = list(range(1, 11))
         y = [29, 39, 23, 32, 4, 43, 43, 23, 43, 77]
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/modifications_check.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 import json
 from typing import List, Optional
 
-from langchain.base_language import BaseLanguageModel
-from langchain.chat_models.anthropic import ChatAnthropic
+from langchain_core.language_models import BaseLanguageModel
 
 from codeinterpreterapi.prompts import determine_modifications_prompt
 
 
 def get_file_modifications(
     code: str,
     llm: BaseLanguageModel,
-    retry: int = 2,
+    retry: int = 4,
 ) -> Optional[List[str]]:
     if retry < 1:
         return None
 
     prompt = determine_modifications_prompt.format(code=code)
 
-    result = llm.predict(prompt, stop="```")
+    result = llm.invoke(prompt)
 
     try:
-        result = json.loads(result)
+        result = json.loads(result.content)
     except json.JSONDecodeError:
         result = ""
     if not result or not isinstance(result, dict) or "modifications" not in result:
         return get_file_modifications(code, llm, retry=retry - 1)
     return result["modifications"]
 
 
 async def aget_file_modifications(
     code: str,
     llm: BaseLanguageModel,
-    retry: int = 2,
+    retry: int = 4,
 ) -> Optional[List[str]]:
     if retry < 1:
         return None
 
     prompt = determine_modifications_prompt.format(code=code)
 
-    result = await llm.apredict(prompt, stop="```")
+    result = await llm.ainvoke(prompt)
 
     try:
-        result = json.loads(result)
+        result = json.loads(result.content)
     except json.JSONDecodeError:
         result = ""
     if not result or not isinstance(result, dict) or "modifications" not in result:
         return await aget_file_modifications(code, llm, retry=retry - 1)
     return result["modifications"]
 
 
 async def test() -> None:
-    llm = ChatAnthropic(model="claude-2")  # type: ignore
+    from langchain_openai import ChatOpenAI
+
+    llm = ChatOpenAI()
 
     code = """
         import matplotlib.pyplot as plt
 
         x = list(range(1, 11))
         y = [29, 39, 23, 32, 4, 43, 43, 23, 43, 77]
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/chains/rm_dl_link.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/rm_dl_link.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from langchain.base_language import BaseLanguageModel
-from langchain.chat_models.openai import ChatOpenAI
-from langchain.schema import AIMessage, OutputParserException
+from langchain_core.exceptions import OutputParserException
+from langchain_core.language_models import BaseLanguageModel
+from langchain_core.messages import AIMessage
+from langchain_openai import ChatOpenAI
 
 from codeinterpreterapi.prompts import remove_dl_link_prompt
 
 
 def remove_download_link(
     input_response: str,
     llm: BaseLanguageModel,
 ) -> str:
     messages = remove_dl_link_prompt.format_prompt(
         input_response=input_response
     ).to_messages()
-    message = llm.predict_messages(messages)
+    message = llm.invoke(messages)
 
     if not isinstance(message, AIMessage):
         raise OutputParserException("Expected an AIMessage")
 
     assert isinstance(message.content, str), "TODO: add image support"
     return message.content
 
@@ -24,15 +25,15 @@
 async def aremove_download_link(
     input_response: str,
     llm: BaseLanguageModel,
 ) -> str:
     messages = remove_dl_link_prompt.format_prompt(
         input_response=input_response
     ).to_messages()
-    message = await llm.apredict_messages(messages)
+    message = await llm.ainvoke(messages)
 
     if not isinstance(message, AIMessage):
         raise OutputParserException("Expected an AIMessage")
 
     assert isinstance(message.content, str), "TODO: add image support"
     return message.content
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/modifications_check.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/modifications_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langchain.prompts import PromptTemplate
+from langchain_core.prompts import PromptTemplate
 
 determine_modifications_prompt = PromptTemplate(
     input_variables=["code"],
     template="The user will input some code and you need to determine "
     "if the code makes any changes to the file system. \n"
     "With changes it means creating new files or modifying existing ones.\n"
     "Format your answer as JSON inside a codeblock with a "
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/remove_dl_link.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/remove_dl_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
-from langchain.schema import AIMessage, HumanMessage, SystemMessage
+from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
+from langchain_core.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
 
 remove_dl_link_prompt = ChatPromptTemplate(
     input_variables=["input_response"],
     messages=[
         SystemMessage(
             content="The user will send you a response and you need "
             "to remove the download link from it.\n"
```

### Comparing `codeinterpreterapi-0.1.15/src/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/system_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langchain.schema import SystemMessage
+from langchain_core.messages import SystemMessage
 
 system_message = SystemMessage(
     content="""
 You are using an AI Assistant capable of tasks related to data science, data analysis, data visualization, and file manipulation. Capabilities include:
 
 - Image Manipulation: Zoom, crop, color grade, enhance resolution, format conversion.
 - QR Code Generation: Create QR codes.
```

### Comparing `codeinterpreterapi-0.1.15/tests/general_test.py` & `codeinterpreterapi-0.1.16/tests/general_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,43 +22,54 @@
 def run_sync(session: CodeInterpreterSession) -> bool:
     try:
         assert session.start() == "started"
 
         assert (
             "3.1"
             in session.generate_response(
-                "Compute pi using Monte Carlo simulation in Python and show me the result."
+                "Compute pi using Monte Carlo simulation in "
+                "Python and show me the result."
             ).content
         )
 
         assert (
             ".xlsx"
             in session.generate_response(
                 "Convert this csv file to excel.",
                 files=[File.from_path("examples/assets/iris.csv")],
             )
             .files[0]
             .name
         )
 
+        assert (
+            ".png"
+            in session.generate_response(
+                "Plot the current stock price of Tesla.",
+            )
+            .files[0]
+            .name
+        )
+
     finally:
         assert session.stop() == "stopped"
 
     return True
 
 
 async def run_async(session: CodeInterpreterSession) -> bool:
     try:
         assert (await session.astart()) == "started"
 
         assert (
             "3.1"
             in (
                 await session.agenerate_response(
-                    "Compute pi using Monte Carlo simulation in Python and show me the result."
+                    "Compute pi using Monte Carlo simulation in "
+                    "Python and show me the result."
                 )
             ).content
         )
 
         assert (
             ".xlsx"
             in (
@@ -67,14 +78,25 @@
                     files=[File.from_path("examples/assets/iris.csv")],
                 )
             )
             .files[0]
             .name
         )
 
+        assert (
+            ".png"
+            in (
+                await session.agenerate_response(
+                    "Plot the current stock price of Tesla.",
+                )
+            )
+            .files[0]
+            .name
+        )
+
     finally:
         assert await session.astop() == "stopped"
 
     return True
 
 
 if __name__ == "__main__":
```

### Comparing `codeinterpreterapi-0.1.15/LICENSE` & `codeinterpreterapi-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.15/README.md` & `codeinterpreterapi-0.1.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -111,31 +111,14 @@
 So, if you want to contribute, feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
 Just open an issue or pull request and I will review it.
 
 Please also submit any bugs you find as an issue with a minimal code example or screenshot.
 This helps me a lot in improving the code.
 
-Before submitting a pull request, please run the pre-commit hooks to ensure that the code is formatted correctly.
-
-```bash
-pre-commit install
-pre-commit run --all-files
-```
-
-Thanks!
-
-## Streamlit WebApp
-
-To start the web application created with streamlit:
-
-```bash
-streamlit run frontend/app.py --browser.gatherUsageStats=False
-```
-
 ## Contact
 
 You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
 But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://discord.gg/Vaq25XJvvW) DMs.
 
 ## Support this project
```

### Comparing `codeinterpreterapi-0.1.15/pyproject.toml` & `codeinterpreterapi-0.1.16/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [project]
 name = "codeinterpreterapi"
-version = "0.1.15"
+version = "0.1.16"
 description = "CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter."
-authors = [
-    { name = "Shroominic", email = "contact@shroominic.com" }
-]
+authors = [{ name = "Shroominic", email = "contact@shroominic.com" }]
 dependencies = [
-    "openai",
-    "langchain",
-    "codeboxapi>=0.0.19",
-    "python-dotenv",
-    "pydantic>=2",
-    "pydantic-settings>=2",
+    "langchain-openai>=0.1.1",
+    "codeboxapi>=0.1.19",
+    "langchain>=0.1.14",
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">= 3.9.7, <3.12"
-keywords = ["codeinterpreter", "chatgpt", "codeinterpreterapi", "api", "langchain", "codeboxapi"]
+keywords = [
+    "codeinterpreter",
+    "chatgpt",
+    "codeinterpreterapi",
+    "api",
+    "langchain",
+    "codeboxapi",
+]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 [project.urls]
 Code = "https://github.com/shroominic/codeinterpreter-api"
 Docs = "https://shroominic.github.io/codeinterpreter-api"
 
@@ -43,28 +46,18 @@
     "ipython",
     "pre-commit",
     "codeinterpreterapi[all]",
     "mkdocs-material>=9.4",
 ]
 
 [project.optional-dependencies]
-localbox = [
-    "jupyter-kernel-gateway",
-]
-frontend = [
-    "streamlit",
-]
-image_support = [
-    "Pillow",
-]
-all = [
-    "jupyter-kernel-gateway",
-    "streamlit",
-    "Pillow",
-]
+localbox = ["codeboxapi[local_support]"]
+frontend = ["streamlit"]
+image_support = ["codeboxapi[image_support]"]
+all = ["codeboxapi[all]", "codeinterpreterapi[frontend]"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.pytest.ini_options]
 addopts = "-p no:warnings"
 
@@ -78,7 +71,10 @@
 max-line-length = 120
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 disallow_untyped_calls = true
 disallow_incomplete_defs = true
+
+[tool.ruff.lint]
+select = ["E", "F", "I"]
```

### Comparing `codeinterpreterapi-0.1.15/PKG-INFO` & `codeinterpreterapi-0.1.16/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: codeinterpreterapi
-Version: 0.1.15
+Version: 0.1.16
 Summary: CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter.
 Project-URL: Code, https://github.com/shroominic/codeinterpreter-api
 Project-URL: Docs, https://shroominic.github.io/codeinterpreter-api
 Author-email: Shroominic <contact@shroominic.com>
 License: # MIT License
         
         Copyright (c) 2023 Dominic Bäumer
@@ -28,32 +28,29 @@
         SOFTWARE.
 License-File: LICENSE
 Keywords: api,chatgpt,codeboxapi,codeinterpreter,codeinterpreterapi,langchain
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <3.12,>=3.9.7
-Requires-Dist: codeboxapi>=0.0.19
-Requires-Dist: langchain
-Requires-Dist: openai
-Requires-Dist: pydantic-settings>=2
-Requires-Dist: pydantic>=2
-Requires-Dist: python-dotenv
+Requires-Dist: codeboxapi>=0.1.19
+Requires-Dist: langchain-openai>=0.1.1
+Requires-Dist: langchain>=0.1.14
 Provides-Extra: all
-Requires-Dist: jupyter-kernel-gateway; extra == 'all'
-Requires-Dist: pillow; extra == 'all'
-Requires-Dist: streamlit; extra == 'all'
+Requires-Dist: codeboxapi[all]; extra == 'all'
+Requires-Dist: codeinterpreterapi[frontend]; extra == 'all'
 Provides-Extra: frontend
 Requires-Dist: streamlit; extra == 'frontend'
 Provides-Extra: image-support
-Requires-Dist: pillow; extra == 'image-support'
+Requires-Dist: codeboxapi[image-support]; extra == 'image-support'
 Provides-Extra: localbox
-Requires-Dist: jupyter-kernel-gateway; extra == 'localbox'
+Requires-Dist: codeboxapi[local-support]; extra == 'localbox'
 Description-Content-Type: text/markdown
 
 # 👾 Code Interpreter API
 
 [![Version](https://badge.fury.io/py/codeinterpreterapi.svg)](https://badge.fury.io/py/codeinterpreterapi)
 [![code-check](https://github.com/shroominic/codeinterpreter-api/actions/workflows/code-check.yml/badge.svg)](https://github.com/shroominic/codeinterpreter-api/actions/workflows/code-check.yml)
 ![Downloads](https://img.shields.io/pypi/dm/codeinterpreterapi)
@@ -165,31 +162,14 @@
 So, if you want to contribute, feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
 Just open an issue or pull request and I will review it.
 
 Please also submit any bugs you find as an issue with a minimal code example or screenshot.
 This helps me a lot in improving the code.
 
-Before submitting a pull request, please run the pre-commit hooks to ensure that the code is formatted correctly.
-
-```bash
-pre-commit install
-pre-commit run --all-files
-```
-
-Thanks!
-
-## Streamlit WebApp
-
-To start the web application created with streamlit:
-
-```bash
-streamlit run frontend/app.py --browser.gatherUsageStats=False
-```
-
 ## Contact
 
 You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
 But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://discord.gg/Vaq25XJvvW) DMs.
 
 ## Support this project
```

