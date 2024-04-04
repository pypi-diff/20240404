# Comparing `tmp/heavylight-1.0.5.tar.gz` & `tmp/heavylight-1.0.6.tar.gz`

## Comparing `heavylight-1.0.5.tar` & `heavylight-1.0.6.tar`

### file list

```diff
@@ -1,47 +1,74 @@
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 heavylight-1.0.5/mkdocs.yml
--rw-r--r--   0        0        0    81649 2020-02-02 00:00:00.000000 heavylight-1.0.5/scratch.ipynb
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 heavylight-1.0.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 heavylight-1.0.5/.github/dependabot.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 heavylight-1.0.5/.github/workflows/docs.yml
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 heavylight-1.0.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 heavylight-1.0.5/.vscode/settings.json
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 heavylight-1.0.5/developer-setup/environment-notes.md
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 heavylight-1.0.5/docs/index.md
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 heavylight-1.0.5/docs/tables.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 heavylight-1.0.5/docs/_static/custom_css.css
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 heavylight-1.0.5/docs/_static/mathjax.js
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/basic_cashflow.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/readme.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/readme_example.py
--rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/heavylight_basic.ipynb
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/heavylight_local.py
--rw-r--r--   0        0        0    72101 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/heavylight_tables.ipynb
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/sample_q_x_table.csv
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/string_lookup_investigation.ipynb
--rw-r--r--   0        0        0    70439 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/table_documentation.ipynb
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/table_maker.ipynb
--rw-r--r--   0        0        0    23075 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/vectors.ipynb
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/vectors.py
--rw-r--r--   0        0        0  1491502 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/protection_model.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/run_model.py
--rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/tables/covert_q_x_tables.ipynb
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/tables/forward_rates.csv
--rw-r--r--   0        0        0    16505 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/tables/q_x_generic.csv
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/tables/qx_generic_raw.csv
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.5/examples/std_model/tables/uk_zero_spot.csv
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 heavylight-1.0.5/src/heavylight/__init__.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 heavylight-1.0.5/src/heavylight/heavylight.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 heavylight-1.0.5/src/heavylight/heavytables.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 heavylight-1.0.5/src/heavylight/memory_optimized_cache.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 heavylight-1.0.5/src/heavylight/memory_optimized_model.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 heavylight-1.0.5/tests/test_heavylight.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 heavylight-1.0.5/tests/test_optimizations.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 heavylight-1.0.5/tests/test_optimized_cache.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 heavylight-1.0.5/tests/test_optimized_model.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 heavylight-1.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 heavylight-1.0.5/LICENSE
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 heavylight-1.0.5/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 heavylight-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 heavylight-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 heavylight-1.0.6/mkdocs.yml
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 heavylight-1.0.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 heavylight-1.0.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 heavylight-1.0.6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 heavylight-1.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 heavylight-1.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 heavylight-1.0.6/developer-setup/environment-notes.md
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/index.md
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/storage_function.md
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/tables.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/_static/custom_css.css
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/_static/mathjax.js
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/basic_cashflow.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/readme.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/readme_example.py
+-rw-r--r--   0        0        0    21406 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/memory_optimizations/example.ipynb
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/docs_check_tables_md.ipynb
+-rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/heavylight_basic.ipynb
+-rw-r--r--   0        0        0    76024 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/heavylight_tables.ipynb
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/sample_q_x_table.csv
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/string_lookup_investigation.ipynb
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/super_init_example.ipynb
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_bounds_check.ipynb
+-rw-r--r--   0        0        0    70439 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_documentation.ipynb
+-rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_documentation.md
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_maker.ipynb
+-rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/using_dataclasses.ipynb
+-rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/vectors.ipynb
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/vectors.py
+-rw-r--r--   0        0        0  1491502 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv
+-rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_documentation_files/table_documentation_32_1.png
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/protection_model.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/run_model.py
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/covert_q_x_tables.ipynb
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/qx_generic_raw.csv
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/uk_zero_spot.csv
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/protection_model.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/run_model.py
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/covert_q_x_tables.ipynb
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/qx_generic_raw.csv
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/uk_zero_spot.csv
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/__init__.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/heavylight.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/heavytables.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/make_examples.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/memory_optimized_cache.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/memory_optimized_model.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/protection_model_base.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/protection_model_np.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/readme.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/run_model_base.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/run_model_np.py
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/template/model.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_examples.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_heavylight.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_heavytables.py
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_lightmodel.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_lightmodel_df.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_memory_savings.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_optimized_cache.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 heavylight-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 heavylight-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 heavylight-1.0.6/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 heavylight-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 heavylight-1.0.6/PKG-INFO
```

### Comparing `heavylight-1.0.5/mkdocs.yml` & `heavylight-1.0.6/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -48,8 +48,9 @@
     - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
 
 extra_css:
     - _static/custom_css.css
 
 nav:
     - 'index.md'
+    - 'tables.md'
```

### Comparing `heavylight-1.0.5/.devcontainer/devcontainer.json` & `heavylight-1.0.6/.devcontainer/devcontainer.json`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 	// Or use a Dockerfile or Docker Compose file. More info: https://containers.dev/guide/dockerfile
 	"image": "mcr.microsoft.com/devcontainers/python:1-3.8-bookworm",
 	"features": {
 		"ghcr.io/devcontainers/features/docker-in-docker:2": {},
 		"ghcr.io/dhoeric/features/act:1": {},
 		"ghcr.io/hspaans/devcontainer-features/pytest:1": {},
 		"ghcr.io/meaningful-ooo/devcontainer-features/fish:1": {},
-		"ghcr.io/stuartleeks/dev-container-features/shell-history:0": {}
+		"ghcr.io/stuartleeks/dev-container-features/shell-history:0": {},
+		"ghcr.io/devcontainers/features/github-cli:1": {}
 	},
 
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
 
 	// Use 'postCreateCommand' to pip install the editable
-	// "postCreateCommand": "pip install -e .[dev]",
+	"postCreateCommand": "pip install -e .[dev]",
 	"customizations": {
 		"vscode": {
 			"extensions": [
 				"ms-python.python",
 				"github.vscode-github-actions",
 				"ms-toolsai.jupyter",
 				"ms-python.black-formatter",
```

### Comparing `heavylight-1.0.5/.github/workflows/docs.yml` & `heavylight-1.0.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/.github/workflows/python-package.yml` & `heavylight-1.0.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/developer-setup/environment-notes.md` & `heavylight-1.0.6/developer-setup/environment-notes.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,13 +12,15 @@
 The previous install should install optional dependencies `pytest` and `pytest-cov`
 
 ```sh
 # test
 pytest
 # with coverage reporting
 pytest --cov=src tests/
+# get the xml
+pytest --cov=src tests/ --cov-report xml
 ```
 
 In the devcontainer we have act installed, allowing us to verify that pytest runs in the CI/CD pipeline as well.
 ```
 act -j build -s "CODECOV_TOKEN=your-codecov-token-abc555-5555"
 ```
```

### Comparing `heavylight-1.0.5/docs/index.md` & `heavylight-1.0.6/docs/storage_function.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,156 +1,137 @@
-00000000: 2320 4765 7474 696e 6720 7374 6172 7465  # Getting starte
-00000010: 640a 0a48 6561 7679 6c69 6768 7420 6973  d..Heavylight is
-00000020: 2061 206c 6967 6874 7765 6967 6874 2050   a lightweight P
-00000030: 7974 686f 6e20 6c69 6272 6172 7920 7468  ython library th
-00000040: 6174 2061 6c6c 6f77 7320 796f 7520 746f  at allows you to
-00000050: 2072 756e 2068 6561 7679 206d 6f64 656c   run heavy model
-00000060: 696e 6720 776f 726b 6c6f 6164 7320 7573  ing workloads us
-00000070: 696e 6720 6120 6661 6d69 6c69 6172 2072  ing a familiar r
-00000080: 6563 7572 7369 7665 2073 796e 7461 782e  ecursive syntax.
-00000090: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000000a0: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
-000000b0: 6e73 7461 6c6c 2068 6561 7679 6c69 6768  nstall heavyligh
-000000c0: 740a 6060 600a 0a52 6571 7569 7265 7320  t.```..Requires 
-000000d0: 5079 7468 6f6e 2033 2e38 2b0a 0a23 2320  Python 3.8+..## 
-000000e0: 5175 6963 6b20 6578 616d 706c 650a 0a4d  Quick example..M
-000000f0: 6f64 656c 7320 6172 6520 6465 6669 6e65  odels are define
-00000100: 6420 6279 2073 7562 636c 6173 7369 6e67  d by subclassing
-00000110: 2066 726f 6d20 6068 6561 7679 6c69 6768   from `heavyligh
-00000120: 742e 4d6f 6465 6c60 0a0a 6060 6070 7974  t.Model`..```pyt
-00000130: 686f 6e0a 696d 706f 7274 206e 756d 7079  hon.import numpy
-00000140: 2061 7320 6e70 0a69 6d70 6f72 7420 6865   as np.import he
-00000150: 6176 796c 6967 6874 0a0a 636c 6173 7320  avylight..class 
-00000160: 5369 6d70 6c65 4d6f 6465 6c28 6865 6176  SimpleModel(heav
-00000170: 796c 6967 6874 2e4d 6f64 656c 293a 0a0a  ylight.Model):..
-00000180: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000190: 2873 656c 662c 2069 6e69 7469 616c 5f70  (self, initial_p
-000001a0: 6f6c 735f 6966 3a20 6e70 2e6e 6461 7272  ols_if: np.ndarr
-000001b0: 6179 2c20 6d6f 7274 616c 6974 795f 7261  ay, mortality_ra
-000001c0: 7465 3a20 666c 6f61 7429 3a0a 2020 2020  te: float):.    
-000001d0: 2020 2020 2320 7374 6f72 6167 655f 6675      # storage_fu
-000001e0: 6e63 7469 6f6e 2064 6574 6572 6d69 6e65  nction determine
-000001f0: 7320 7768 6174 2067 6574 7320 7374 6f72  s what gets stor
-00000200: 6564 2069 6e20 7468 6520 7265 7375 6c74  ed in the result
-00000210: 7320 4461 7461 4672 616d 650a 2020 2020  s DataFrame.    
-00000220: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00000230: 6974 5f5f 2873 746f 7261 6765 5f66 756e  it__(storage_fun
-00000240: 6374 696f 6e3d 6c61 6d62 6461 2072 6573  ction=lambda res
-00000250: 756c 7473 3a20 6e70 2e72 6f75 6e64 286e  ults: np.round(n
-00000260: 702e 7375 6d28 7265 7375 6c74 7329 2c20  p.sum(results), 
-00000270: 3329 2920 2320 6375 7374 6f6d 697a 6520  3)) # customize 
-00000280: 686f 7720 796f 7520 6167 6772 6567 6174  how you aggregat
-00000290: 6520 7265 7375 6c74 730a 2020 2020 2020  e results.      
-000002a0: 2020 7365 6c66 2e69 6e69 7469 616c 5f70    self.initial_p
-000002b0: 6f6c 735f 6966 203d 2069 6e69 7469 616c  ols_if = initial
-000002c0: 5f70 6f6c 735f 6966 0a20 2020 2020 2020  _pols_if.       
-000002d0: 2073 656c 662e 6d6f 7274 616c 6974 795f   self.mortality_
-000002e0: 7261 7465 203d 206d 6f72 7461 6c69 7479  rate = mortality
-000002f0: 5f72 6174 650a 0a20 2020 2064 6566 2074  _rate..    def t
-00000300: 2873 656c 662c 2074 293a 0a20 2020 2020  (self, t):.     
-00000310: 2020 2072 6574 7572 6e20 740a 0a20 2020     return t..   
-00000320: 2064 6566 206e 756d 5f70 6f6c 735f 6966   def num_pols_if
-00000330: 2873 656c 662c 2074 293a 0a20 2020 2020  (self, t):.     
-00000340: 2020 2069 6620 7420 3d3d 2030 3a0a 2020     if t == 0:.  
-00000350: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000360: 2073 656c 662e 696e 6974 6961 6c5f 706f   self.initial_po
-00000370: 6c73 5f69 660a 2020 2020 2020 2020 7265  ls_if.        re
-00000380: 7475 726e 2073 656c 662e 6e75 6d5f 706f  turn self.num_po
-00000390: 6c73 5f69 6628 7420 2d20 3129 202d 2073  ls_if(t - 1) - s
-000003a0: 656c 662e 706f 6c73 5f64 6561 7468 2874  elf.pols_death(t
-000003b0: 202d 2031 2920 2320 6361 7573 6573 2065   - 1) # causes e
-000003c0: 7870 6f6e 656e 7469 616c 2074 696d 6520  xponential time 
-000003d0: 636f 6d70 6c65 7869 7479 2069 6620 756e  complexity if un
-000003e0: 6361 6368 6564 0a20 2020 2020 2020 200a  cached.        .
-000003f0: 2020 2020 6465 6620 706f 6c73 5f64 6561      def pols_dea
-00000400: 7468 2873 656c 662c 2074 293a 0a20 2020  th(self, t):.   
-00000410: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000420: 2e6e 756d 5f70 6f6c 735f 6966 2874 2920  .num_pols_if(t) 
-00000430: 2a20 7365 6c66 2e6d 6f72 7461 6c69 7479  * self.mortality
-00000440: 5f72 6174 650a 0a20 2020 2064 6566 2063  _rate..    def c
-00000450: 6173 6866 6c6f 7728 7365 6c66 2c20 7429  ashflow(self, t)
-00000460: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000470: 2073 656c 662e 6e75 6d5f 706f 6c73 5f69   self.num_pols_i
-00000480: 6628 7429 202a 2031 3030 0a20 2020 200a  f(t) * 100.    .
-00000490: 2020 2020 6465 6620 7628 7365 6c66 2c20      def v(self, 
-000004a0: 7429 3a0a 2020 2020 2020 2020 6966 2074  t):.        if t
-000004b0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-000004c0: 2020 2072 6574 7572 6e20 310a 2020 2020     return 1.    
-000004d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000004e0: 7628 7420 2d20 3129 202f 2028 3120 2b20  v(t - 1) / (1 + 
-000004f0: 7365 6c66 2e66 6f72 7761 7264 5f72 6174  self.forward_rat
-00000500: 6528 7429 290a 2020 2020 0a20 2020 2064  e(t)).    .    d
-00000510: 6566 2066 6f72 7761 7264 5f72 6174 6528  ef forward_rate(
-00000520: 7365 6c66 2c20 7429 3a0a 2020 2020 2020  self, t):.      
-00000530: 2020 7265 7475 726e 2030 2e30 340a 2020    return 0.04.  
-00000540: 2020 0a20 2020 2064 6566 2070 765f 6361    .    def pv_ca
-00000550: 7368 666c 6f77 2873 656c 662c 2074 293a  shflow(self, t):
-00000560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000570: 7365 6c66 2e63 6173 6866 6c6f 7728 7429  self.cashflow(t)
-00000580: 202a 2073 656c 662e 7628 7429 0a20 2020   * self.v(t).   
-00000590: 200a 2320 7374 6172 7420 7769 7468 2031   .# start with 1
-000005a0: 3020 706f 6c69 6369 6573 2061 6e64 2063  0 policies and c
-000005b0: 6f6e 7374 616e 7420 6d6f 7274 616c 6974  onstant mortalit
-000005c0: 7920 7261 7465 206f 6620 2e30 310a 7369  y rate of .01.si
-000005d0: 6d70 6c65 5f6d 6f64 656c 203d 2053 696d  mple_model = Sim
-000005e0: 706c 654d 6f64 656c 2869 6e69 7469 616c  pleModel(initial
-000005f0: 5f70 6f6c 735f 6966 3d6e 702e 6f6e 6573  _pols_if=np.ones
-00000600: 2828 3130 2c29 292c 206d 6f72 7461 6c69  ((10,)), mortali
-00000610: 7479 5f72 6174 653d 2e30 3129 0a23 2072  ty_rate=.01).# r
-00000620: 756e 2074 6865 206d 6f64 656c 2066 6f72  un the model for
-00000630: 2035 2074 696d 6573 7465 7073 0a73 696d   5 timesteps.sim
-00000640: 706c 655f 6d6f 6465 6c2e 5275 6e4d 6f64  ple_model.RunMod
-00000650: 656c 2870 726f 6a5f 6c65 6e3d 3529 0a23  el(proj_len=5).#
-00000660: 2063 7265 6174 6520 6120 6461 7461 6672   create a datafr
-00000670: 616d 6520 746f 2073 746f 7265 2072 6573  ame to store res
-00000680: 756c 7473 0a72 6573 756c 7473 203d 2073  ults.results = s
-00000690: 696d 706c 655f 6d6f 6465 6c2e 546f 4461  imple_model.ToDa
-000006a0: 7461 4672 616d 6528 290a 6060 600a 0a52  taFrame().```..R
-000006b0: 6573 756c 7473 2061 7265 2061 2050 616e  esults are a Pan
-000006c0: 6461 7320 6461 7461 6672 616d 653a 0a0a  das dataframe:..
-000006d0: 7c20 2020 7420 7c20 2020 6e75 6d5f 706f  |   t |   num_po
-000006e0: 6c73 5f69 6620 7c20 2020 6361 7368 666c  ls_if |   cashfl
-000006f0: 6f77 207c 2020 2066 6f72 7761 7264 5f72  ow |   forward_r
-00000700: 6174 6520 7c20 2020 706f 6c73 5f64 6561  ate |   pols_dea
-00000710: 7468 207c 2020 2020 2076 207c 2020 2070  th |     v |   p
-00000720: 765f 6361 7368 666c 6f77 207c 0a7c 2d2d  v_cashflow |.|--
-00000730: 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|------------
-00000740: 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  --:|-----------:
-00000750: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-00000760: 3a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  :|-------------:
-00000770: 7c2d 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d  |------:|-------
-00000780: 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020 3020  -------:|.|   0 
-00000790: 7c20 2020 2020 2020 2031 3020 2020 2020  |        10     
-000007a0: 7c20 2020 3130 3030 2020 2020 207c 2020  |   1000     |  
-000007b0: 2020 2020 2020 2020 2030 2e30 3420 7c20           0.04 | 
-000007c0: 2020 2020 2020 2030 2e31 2020 207c 2031         0.1   | 1
-000007d0: 2020 2020 207c 2020 2020 2020 3130 3030       |      1000
-000007e0: 2020 2020 207c 0a7c 2020 2031 207c 2020       |.|   1 |  
-000007f0: 2020 2020 2020 2039 2e39 2020 207c 2020         9.9   |  
-00000800: 2020 3939 3020 2020 2020 7c20 2020 2020    990     |     
-00000810: 2020 2020 2020 302e 3034 207c 2020 2020        0.04 |    
-00000820: 2020 2020 302e 3039 3920 7c20 302e 3936      0.099 | 0.96
-00000830: 3220 7c20 2020 2020 2020 3935 312e 3932  2 |       951.92
-00000840: 3320 7c0a 7c20 2020 3220 7c20 2020 2020  3 |.|   2 |     
-00000850: 2020 2020 392e 3830 3120 7c20 2020 2039      9.801 |    9
-00000860: 3830 2e31 2020 207c 2020 2020 2020 2020  80.1   |        
-00000870: 2020 2030 2e30 3420 7c20 2020 2020 2020     0.04 |       
-00000880: 2030 2e30 3938 207c 2030 2e39 3235 207c   0.098 | 0.925 |
-00000890: 2020 2020 2020 2039 3036 2e31 3538 207c         906.158 |
-000008a0: 0a7c 2020 2033 207c 2020 2020 2020 2020  .|   3 |        
-000008b0: 2039 2e37 3033 207c 2020 2020 3937 302e   9.703 |    970.
-000008c0: 3239 3920 7c20 2020 2020 2020 2020 2020  299 |           
-000008d0: 302e 3034 207c 2020 2020 2020 2020 302e  0.04 |        0.
-000008e0: 3039 3720 7c20 302e 3838 3920 7c20 2020  097 | 0.889 |   
-000008f0: 2020 2020 3836 322e 3539 3220 7c0a 7c20      862.592 |.| 
-00000900: 2020 3420 7c20 2020 2020 2020 2020 392e    4 |         9.
-00000910: 3630 3620 7c20 2020 2039 3630 2e35 3936  606 |    960.596
-00000920: 207c 2020 2020 2020 2020 2020 2030 2e30   |           0.0
-00000930: 3420 7c20 2020 2020 2020 2030 2e30 3936  4 |        0.096
-00000940: 207c 2030 2e38 3535 207c 2020 2020 2020   | 0.855 |      
-00000950: 2038 3231 2e31 3231 207c 0a7c 2020 2035   821.121 |.|   5
-00000960: 207c 2020 2020 2020 2020 2039 2e35 3120   |         9.51 
-00000970: 207c 2020 2020 3935 302e 3939 2020 7c20   |    950.99  | 
-00000980: 2020 2020 2020 2020 2020 302e 3034 207c            0.04 |
-00000990: 2020 2020 2020 2020 302e 3039 3520 7c20          0.095 | 
-000009a0: 302e 3832 3220 7c20 2020 2020 2020 3738  0.822 |       78
-000009b0: 312e 3634 3520 7c0a 0a                   1.645 |..
+00000000: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000010: 206e 756d 7079 2061 7320 6e70 0a69 6d70   numpy as np.imp
+00000020: 6f72 7420 6865 6176 796c 6967 6874 0a0a  ort heavylight..
+00000030: 636c 6173 7320 5369 6d70 6c65 4d6f 6465  class SimpleMode
+00000040: 6c28 6865 6176 796c 6967 6874 2e4d 6f64  l(heavylight.Mod
+00000050: 656c 293a 0a0a 2020 2020 6465 6620 5f5f  el):..    def __
+00000060: 696e 6974 5f5f 2873 656c 662c 2069 6e69  init__(self, ini
+00000070: 7469 616c 5f70 6f6c 735f 6966 3a20 6e70  tial_pols_if: np
+00000080: 2e6e 6461 7272 6179 2c20 6d6f 7274 616c  .ndarray, mortal
+00000090: 6974 795f 7261 7465 3a20 666c 6f61 7429  ity_rate: float)
+000000a0: 3a0a 2020 2020 2020 2020 2320 7374 6f72  :.        # stor
+000000b0: 6167 655f 6675 6e63 7469 6f6e 2064 6574  age_function det
+000000c0: 6572 6d69 6e65 7320 7768 6174 2067 6574  ermines what get
+000000d0: 7320 7374 6f72 6564 2069 6e20 7468 6520  s stored in the 
+000000e0: 7265 7375 6c74 7320 4461 7461 4672 616d  results DataFram
+000000f0: 650a 2020 2020 2020 2020 7375 7065 7228  e.        super(
+00000100: 292e 5f5f 696e 6974 5f5f 2873 746f 7261  ).__init__(stora
+00000110: 6765 5f66 756e 6374 696f 6e3d 6c61 6d62  ge_function=lamb
+00000120: 6461 2072 6573 756c 7473 3a20 6e70 2e72  da results: np.r
+00000130: 6f75 6e64 286e 702e 7375 6d28 7265 7375  ound(np.sum(resu
+00000140: 6c74 7329 2c20 3329 2920 2320 6375 7374  lts), 3)) # cust
+00000150: 6f6d 697a 6520 686f 7720 796f 7520 6167  omize how you ag
+00000160: 6772 6567 6174 6520 7265 7375 6c74 730a  gregate results.
+00000170: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
+00000180: 7469 616c 5f70 6f6c 735f 6966 203d 2069  tial_pols_if = i
+00000190: 6e69 7469 616c 5f70 6f6c 735f 6966 0a20  nitial_pols_if. 
+000001a0: 2020 2020 2020 2073 656c 662e 6d6f 7274         self.mort
+000001b0: 616c 6974 795f 7261 7465 203d 206d 6f72  ality_rate = mor
+000001c0: 7461 6c69 7479 5f72 6174 650a 0a20 2020  tality_rate..   
+000001d0: 2064 6566 2074 2873 656c 662c 2074 293a   def t(self, t):
+000001e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000001f0: 740a 0a20 2020 2064 6566 206e 756d 5f70  t..    def num_p
+00000200: 6f6c 735f 6966 2873 656c 662c 2074 293a  ols_if(self, t):
+00000210: 0a20 2020 2020 2020 2069 6620 7420 3d3d  .        if t ==
+00000220: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00000230: 7265 7475 726e 2073 656c 662e 696e 6974  return self.init
+00000240: 6961 6c5f 706f 6c73 5f69 660a 2020 2020  ial_pols_if.    
+00000250: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00000260: 6e75 6d5f 706f 6c73 5f69 6628 7420 2d20  num_pols_if(t - 
+00000270: 3129 202d 2073 656c 662e 706f 6c73 5f64  1) - self.pols_d
+00000280: 6561 7468 2874 202d 2031 2920 2320 6361  eath(t - 1) # ca
+00000290: 7573 6573 2065 7870 6f6e 656e 7469 616c  uses exponential
+000002a0: 2074 696d 6520 636f 6d70 6c65 7869 7479   time complexity
+000002b0: 2069 6620 756e 6361 6368 6564 0a20 2020   if uncached.   
+000002c0: 2020 2020 200a 2020 2020 6465 6620 706f       .    def po
+000002d0: 6c73 5f64 6561 7468 2873 656c 662c 2074  ls_death(self, t
+000002e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000002f0: 6e20 7365 6c66 2e6e 756d 5f70 6f6c 735f  n self.num_pols_
+00000300: 6966 2874 2920 2a20 7365 6c66 2e6d 6f72  if(t) * self.mor
+00000310: 7461 6c69 7479 5f72 6174 650a 0a20 2020  tality_rate..   
+00000320: 2064 6566 2063 6173 6866 6c6f 7728 7365   def cashflow(se
+00000330: 6c66 2c20 7429 3a0a 2020 2020 2020 2020  lf, t):.        
+00000340: 7265 7475 726e 2073 656c 662e 6e75 6d5f  return self.num_
+00000350: 706f 6c73 5f69 6628 7429 202a 2031 3030  pols_if(t) * 100
+00000360: 0a20 2020 200a 2020 2020 6465 6620 7628  .    .    def v(
+00000370: 7365 6c66 2c20 7429 3a0a 2020 2020 2020  self, t):.      
+00000380: 2020 6966 2074 203d 3d20 303a 0a20 2020    if t == 0:.   
+00000390: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000003a0: 310a 2020 2020 2020 2020 7265 7475 726e  1.        return
+000003b0: 2073 656c 662e 7628 7420 2d20 3129 202f   self.v(t - 1) /
+000003c0: 2028 3120 2b20 7365 6c66 2e66 6f72 7761   (1 + self.forwa
+000003d0: 7264 5f72 6174 6528 7429 290a 2020 2020  rd_rate(t)).    
+000003e0: 0a20 2020 2064 6566 2066 6f72 7761 7264  .    def forward
+000003f0: 5f72 6174 6528 7365 6c66 2c20 7429 3a0a  _rate(self, t):.
+00000400: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
+00000410: 2e30 340a 2020 2020 0a20 2020 2064 6566  .04.    .    def
+00000420: 2070 765f 6361 7368 666c 6f77 2873 656c   pv_cashflow(sel
+00000430: 662c 2074 293a 0a20 2020 2020 2020 2072  f, t):.        r
+00000440: 6574 7572 6e20 7365 6c66 2e63 6173 6866  eturn self.cashf
+00000450: 6c6f 7728 7429 202a 2073 656c 662e 7628  low(t) * self.v(
+00000460: 7429 0a20 2020 200a 2320 7374 6172 7420  t).    .# start 
+00000470: 7769 7468 2031 3020 706f 6c69 6369 6573  with 10 policies
+00000480: 2061 6e64 2063 6f6e 7374 616e 7420 6d6f   and constant mo
+00000490: 7274 616c 6974 7920 7261 7465 206f 6620  rtality rate of 
+000004a0: 2e30 310a 7369 6d70 6c65 5f6d 6f64 656c  .01.simple_model
+000004b0: 203d 2053 696d 706c 654d 6f64 656c 2869   = SimpleModel(i
+000004c0: 6e69 7469 616c 5f70 6f6c 735f 6966 3d6e  nitial_pols_if=n
+000004d0: 702e 6f6e 6573 2828 3130 2c29 292c 206d  p.ones((10,)), m
+000004e0: 6f72 7461 6c69 7479 5f72 6174 653d 2e30  ortality_rate=.0
+000004f0: 3129 0a23 2072 756e 2074 6865 206d 6f64  1).# run the mod
+00000500: 656c 2066 6f72 2035 2074 696d 6573 7465  el for 5 timeste
+00000510: 7073 0a73 696d 706c 655f 6d6f 6465 6c2e  ps.simple_model.
+00000520: 5275 6e4d 6f64 656c 2870 726f 6a5f 6c65  RunModel(proj_le
+00000530: 6e3d 3529 0a23 2063 7265 6174 6520 6120  n=5).# create a 
+00000540: 6461 7461 6672 616d 6520 746f 2073 746f  dataframe to sto
+00000550: 7265 2072 6573 756c 7473 0a72 6573 756c  re results.resul
+00000560: 7473 203d 2073 696d 706c 655f 6d6f 6465  ts = simple_mode
+00000570: 6c2e 546f 4461 7461 4672 616d 6528 290a  l.ToDataFrame().
+00000580: 6060 600a 0a52 6573 756c 7473 2061 7265  ```..Results are
+00000590: 2061 2050 616e 6461 7320 6461 7461 6672   a Pandas datafr
+000005a0: 616d 653a 0a0a 7c20 2020 7420 7c20 2020  ame:..|   t |   
+000005b0: 6e75 6d5f 706f 6c73 5f69 6620 7c20 2020  num_pols_if |   
+000005c0: 6361 7368 666c 6f77 207c 2020 2066 6f72  cashflow |   for
+000005d0: 7761 7264 5f72 6174 6520 7c20 2020 706f  ward_rate |   po
+000005e0: 6c73 5f64 6561 7468 207c 2020 2020 2076  ls_death |     v
+000005f0: 207c 2020 2070 765f 6361 7368 666c 6f77   |   pv_cashflow
+00000600: 207c 0a7c 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d   |.|----:|------
+00000610: 2d2d 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d  --------:|------
+00000620: 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d  -----:|---------
+00000630: 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d  ------:|--------
+00000640: 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d 2d3a 7c2d  -----:|------:|-
+00000650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -------------:|.
+00000660: 7c20 2020 3020 7c20 2020 2020 2020 2031  |   0 |        1
+00000670: 3020 2020 2020 7c20 2020 3130 3030 2020  0     |   1000  
+00000680: 2020 207c 2020 2020 2020 2020 2020 2030     |           0
+00000690: 2e30 3420 7c20 2020 2020 2020 2030 2e31  .04 |        0.1
+000006a0: 2020 207c 2031 2020 2020 207c 2020 2020     | 1     |    
+000006b0: 2020 3130 3030 2020 2020 207c 0a7c 2020    1000     |.|  
+000006c0: 2031 207c 2020 2020 2020 2020 2039 2e39   1 |         9.9
+000006d0: 2020 207c 2020 2020 3939 3020 2020 2020     |    990     
+000006e0: 7c20 2020 2020 2020 2020 2020 302e 3034  |           0.04
+000006f0: 207c 2020 2020 2020 2020 302e 3039 3920   |        0.099 
+00000700: 7c20 302e 3936 3220 7c20 2020 2020 2020  | 0.962 |       
+00000710: 3935 312e 3932 3320 7c0a 7c20 2020 3220  951.923 |.|   2 
+00000720: 7c20 2020 2020 2020 2020 392e 3830 3120  |         9.801 
+00000730: 7c20 2020 2039 3830 2e31 2020 207c 2020  |    980.1   |  
+00000740: 2020 2020 2020 2020 2030 2e30 3420 7c20           0.04 | 
+00000750: 2020 2020 2020 2030 2e30 3938 207c 2030         0.098 | 0
+00000760: 2e39 3235 207c 2020 2020 2020 2039 3036  .925 |       906
+00000770: 2e31 3538 207c 0a7c 2020 2033 207c 2020  .158 |.|   3 |  
+00000780: 2020 2020 2020 2039 2e37 3033 207c 2020         9.703 |  
+00000790: 2020 3937 302e 3239 3920 7c20 2020 2020    970.299 |     
+000007a0: 2020 2020 2020 302e 3034 207c 2020 2020        0.04 |    
+000007b0: 2020 2020 302e 3039 3720 7c20 302e 3838      0.097 | 0.88
+000007c0: 3920 7c20 2020 2020 2020 3836 322e 3539  9 |       862.59
+000007d0: 3220 7c0a 7c20 2020 3420 7c20 2020 2020  2 |.|   4 |     
+000007e0: 2020 2020 392e 3630 3620 7c20 2020 2039      9.606 |    9
+000007f0: 3630 2e35 3936 207c 2020 2020 2020 2020  60.596 |        
+00000800: 2020 2030 2e30 3420 7c20 2020 2020 2020     0.04 |       
+00000810: 2030 2e30 3936 207c 2030 2e38 3535 207c   0.096 | 0.855 |
+00000820: 2020 2020 2020 2038 3231 2e31 3231 207c         821.121 |
+00000830: 0a7c 2020 2035 207c 2020 2020 2020 2020  .|   5 |        
+00000840: 2039 2e35 3120 207c 2020 2020 3935 302e   9.51  |    950.
+00000850: 3939 2020 7c20 2020 2020 2020 2020 2020  99  |           
+00000860: 302e 3034 207c 2020 2020 2020 2020 302e  0.04 |        0.
+00000870: 3039 3520 7c20 302e 3832 3220 7c20 2020  095 | 0.822 |   
+00000880: 2020 2020 3738 312e 3634 3520 7c0a 0a        781.645 |..
```

### Comparing `heavylight-1.0.5/docs/tables.md` & `heavylight-1.0.6/docs/tables.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Tables
 
 Heavylight is design to be modular, you can pick and choose which functionality you use.
 
-A core feature of actuarial models is the use of a variety of assumption tables, for example yield curves, mortality tables, lapse rates and expesnse tables.
+A core feature of actuarial models is the use of a variety of assumption tables, for example yield curves, mortality tables, lapse rates and expenses tables.
 
 Heavylight includes the `Table` class which provides both individual and vectorised lookups, and an opinionated format for loading tables from pandas dataframes, csv files and excel files.
 
 ```python
 from heavylight import Table
 import pandas as pd
 import numpy as np
@@ -22,11 +22,35 @@
 # we can query a single value
 print(tab[20])   # prints(0.20)
 
 # we can query multiple values at once using numpy arrays.
 rng = np.random.default_rng(seed=42)   # set up random number generator
 ages = rng.integers(low=18, high=65, size=100_000, endpoint=True)   # sample 100k ages
 vals = tab[ages]    # query the table and store values
-``` 
+```
+
+## Defining Column Types
+
+`Table` determines the type of key column based on the column name suffix, the following are supported:
+
+- `|int`: integers (...0, 1, 2, 3...), can start and end anywhere, but must be consecutive
+- `|int_bound`: as `|int` but any values are constrained to the lowest and highest values.
+- `|str`: keys are interpreted as strings, e.g. 'M' and 'F'
+- `|band`: key is numeric and treated as the upper bound on a lookup.
+
 
+## Mult-factor tables
 
+Tables aren't limited to a single key, and keys can take any of the above types.
+
+For examples, if a table `tab2` had headers `age|int` and `sex|str`, to look up the value for age `20` and sex `F`:
+
+```python
+tab2[20, 'F']
 ```
+
+This also works with by passing in numpy arrays of keys.
+```python
+ages = np.array([20, 25, 30, 22])
+sexs = np.array(['F', 'M', 'M', F])
+tab2[ages, sexs]
+```
```

### Comparing `heavylight-1.0.5/docs/_static/custom_css.css` & `heavylight-1.0.6/docs/_static/custom_css.css`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/basic_cashflow.py` & `heavylight-1.0.6/examples/basic_cashflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     def pv_cashflow(self, t):
         """present value of the cashflow occuring at time t"""
         return self.cashflow(t) * self.v(t)
     
 # %%
 
 if __name__ == "__main__":
-    model = SimpleModel(do_run = True, proj_len = 10)
+    model = SimpleModel(proj_len = 10)
     print(model.pv_cashflow.sum())
 
     print(model.v.values)
 
-    df = model.ToDataFrame()
-    print(df)
+    print(model.df)
+
+    print(model.pv_cashflow.df)
```

### Comparing `heavylight-1.0.5/examples/readme_example.py` & `heavylight-1.0.6/examples/readme_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,9 +46,9 @@
 model = Annuity(data = policy_data,
                 do_run = True,
                 proj_len = 20,
                 )
 
 print(model.pv_expected_claim.sum())
 
-model_cashflows = model.ToDataFrame()
+model_cashflows = model.df
 print(model_cashflows)
```

### Comparing `heavylight-1.0.5/examples/notebook/heavylight_basic.ipynb` & `heavylight-1.0.6/examples/notebook/heavylight_basic.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896037946428571%*

 * *Differences: {"'cells'": "{7: {'execution_count': 4}, 11: {'outputs': [OrderedDict([('name', 'stderr'), "*

 * *            "('output_type', 'stream'), ('text', "*

 * *            "['/Users/lewisfogden/Dev/heavylight/src/heavylight/heavylight.py:78: UserWarning: "*

 * *            'Warning: `do_run` will be removed in a future version, use `proj_len` to control '*

 * *            'projection\\n\', \'  warnings.warn("Warning: `do_run` will be removed in a future '*

 * *            'version, use `proj_len` to control projection")\\n\'])])]}, 15: { […]*

```diff
@@ -86,15 +86,15 @@
             "metadata": {},
             "source": [
                 "Rather than using a table of mortality rates, we could define a function"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 4,
             "id": "46737aba-0264-4795-8edb-1ba95ff25598",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "def q_x(t):\n",
@@ -134,15 +134,24 @@
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "6684b54a-fafd-4c28-bae2-6c9196d24064",
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/Users/lewisfogden/Dev/heavylight/src/heavylight/heavylight.py:78: UserWarning: Warning: `do_run` will be removed in a future version, use `proj_len` to control projection\n",
+                        "  warnings.warn(\"Warning: `do_run` will be removed in a future version, use `proj_len` to control projection\")\n"
+                    ]
+                }
+            ],
             "source": [
                 "model = Annuity(data = policy_data,\n",
                 "                basis = basis,\n",
                 "                do_run = True,\n",
                 "                proj_len = 40,\n",
                 "                )"
             ]
@@ -211,127 +220,151 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
+                            "      <th>t</th>\n",
                             "      <th>deaths</th>\n",
                             "      <th>expected_claim</th>\n",
                             "      <th>mortality_rate</th>\n",
                             "      <th>number_alive</th>\n",
-                            "      <th>t</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
+                            "      <td>0</td>\n",
                             "      <td>0.661143</td>\n",
                             "      <td>550.000000</td>\n",
                             "      <td>0.066114</td>\n",
                             "      <td>10.000000</td>\n",
-                            "      <td>0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
+                            "      <td>1</td>\n",
                             "      <td>0.641139</td>\n",
                             "      <td>513.637151</td>\n",
                             "      <td>0.068653</td>\n",
                             "      <td>9.338857</td>\n",
-                            "      <td>1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
+                            "      <td>2</td>\n",
                             "      <td>0.620078</td>\n",
                             "      <td>478.374486</td>\n",
                             "      <td>0.071292</td>\n",
                             "      <td>8.697718</td>\n",
-                            "      <td>2</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
+                            "      <td>3</td>\n",
                             "      <td>0.598033</td>\n",
                             "      <td>444.270217</td>\n",
                             "      <td>0.074036</td>\n",
                             "      <td>8.077640</td>\n",
-                            "      <td>3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
+                            "      <td>4</td>\n",
                             "      <td>0.575091</td>\n",
                             "      <td>411.378405</td>\n",
                             "      <td>0.076888</td>\n",
                             "      <td>7.479607</td>\n",
-                            "      <td>4</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     deaths  expected_claim  mortality_rate  number_alive  t\n",
-                            "0  0.661143      550.000000        0.066114     10.000000  0\n",
-                            "1  0.641139      513.637151        0.068653      9.338857  1\n",
-                            "2  0.620078      478.374486        0.071292      8.697718  2\n",
-                            "3  0.598033      444.270217        0.074036      8.077640  3\n",
-                            "4  0.575091      411.378405        0.076888      7.479607  4"
+                            "   t    deaths  expected_claim  mortality_rate  number_alive\n",
+                            "0  0  0.661143      550.000000        0.066114     10.000000\n",
+                            "1  1  0.641139      513.637151        0.068653      9.338857\n",
+                            "2  2  0.620078      478.374486        0.071292      8.697718\n",
+                            "3  3  0.598033      444.270217        0.074036      8.077640\n",
+                            "4  4  0.575091      411.378405        0.076888      7.479607"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "model_cashflows = model.ToDataFrame()\n",
+                "model_cashflows = model.df\n",
                 "model_cashflows.head()"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "5c5e9e0b",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "|    |   t |   deaths |   expected_claim |   mortality_rate |   number_alive |\n",
+                        "|---:|----:|---------:|-----------------:|-----------------:|---------------:|\n",
+                        "|  0 |   0 | 0.661143 |          550     |        0.0661143 |       10       |\n",
+                        "|  1 |   1 | 0.641139 |          513.637 |        0.0686529 |        9.33886 |\n",
+                        "|  2 |   2 | 0.620078 |          478.374 |        0.071292  |        8.69772 |\n",
+                        "|  3 |   3 | 0.598033 |          444.27  |        0.0740356 |        8.07764 |\n",
+                        "|  4 |   4 | 0.575091 |          411.378 |        0.0768878 |        7.47961 |\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(model_cashflows.head(5).to_markdown())"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "38da052e-6a1f-4075-9621-da401e9561ac",
             "metadata": {},
             "source": [
                 "Plot the key output"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "ee35f832-25c3-4d16-abed-23704666ae45",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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n0mJz80bb7xBz549XRN4JSYmsnTpUtf2pnAu4dePsymcy5+bNWsWFouFSZMmudbV9/lUQfnRP//5T6ZMmcJTTz3F999/T69evUhKSiI3N9fsaPWqW7duHD582LV8++23Zkc6b8XFxfTq1Ys5c+acdvsLL7zA7NmzmTt3LmvXrsXf35+kpCTKysoaOen5+bXjBBgxYkSt8/vhhx82YsLzl5yczIQJE1izZg3Lli2jsrKSK664guLiYtc+kydPZtGiRXz88cckJyeTlZXF6NGjTUxdd2dznAD33HNPrfP5wgsvmJT43MTExDBr1ixSU1PZsGEDl112GVdffTXbtm0Dmsa5hF8/TvD8c/lT69ev580336Rnz5611tf7+TTEMAzDGDBggDFhwgTXz9XV1UZ0dLQxc+ZME1PVr6eeesro1auX2TEaFGAsXLjQ9bPT6TSioqKMF1980bUuLy/PcDgcxocffmhCwvrx8+M0DMMYP368cfXVV5uSp6Hk5uYagJGcnGwYRs258/b2Nj7++GPXPjt27DAAIyUlxayY5+3nx2kYhjF06FDj4YcfNi9UA2nRooXx1ltvNdlzedLJ4zSMpnUuCwsLjU6dOhnLli2rdVwNcT71DgpQUVFBamoqw4cPd62zWq0MHz6clJQUE5PVv927dxMdHU379u0ZO3YsmZmZZkdqUBkZGWRnZ9c6t8HBwQwcOLDJnVuAVatWERERQXx8PPfffz/Hjh0zO9J5yc/PByA0NBSA1NRUKisra53PLl26EBcX59Hn8+fHedIHH3xAWFgY3bt3Z9q0aZSUlJgRr15UV1ezYMECiouLSUxMbLLn8ufHeVJTOZcTJkxg1KhRtc4bNMx/mx55s8D6dvToUaqrq4mMjKy1PjIykp07d5qUqv4NHDiQefPmER8fz+HDh3nmmWcYPHgwW7duJTAw0Ox4DSI7OxvgtOf25LamYsSIEYwePZp27dqxd+9ennjiCUaOHElKSgo2m83seHXmdDqZNGkSF110Ed27dwdqzqfdbickJKTWvp58Pk93nAC33HILbdq0ITo6mi1btvDYY4+Rnp7OJ598YmLauktLSyMxMZGysjICAgJYuHAhCQkJbNq0qUmdyzMdJzSdc7lgwQK+//571q9ff8q2hvhvUwWlGRk5cqTr+549ezJw4EDatGnDRx99xF133WViMqkPN910k+v7Hj160LNnTzp06MCqVasYNmyYicnOzYQJE9i6dWuTGCf1S850nPfee6/r+x49etCqVSuGDRvG3r176dChQ2PHPGfx8fFs2rSJ/Px8/vWvfzF+/HiSk5PNjlXvznScCQkJTeJcHjhwgIcffphly5bh4+PTKM+pj3iAsLAwbDbbKaONc3JyiIqKMilVwwsJCaFz587s2bPH7CgN5uT5a27nFqB9+/aEhYV55PmdOHEiixcvZuXKlcTExLjWR0VFUVFRQV5eXq39PfV8nuk4T2fgwIEAHnc+7XY7HTt2pG/fvsycOZNevXrx6quvNrlzeabjPB1PPJepqank5ubSp08fvLy88PLyIjk5mdmzZ+Pl5UVkZGS9n08VFGr+sPr27cvy5ctd65xOJ8uXL6/1GWJTU1RUxN69e2nVqpXZURpMu3btiIqKqnVuCwoKWLt2bZM+twAHDx7k2LFjHnV+DcNg4sSJLFy4kBUrVtCuXbta2/v27Yu3t3et85menk5mZqZHnc9fO87T2bRpE4BHnc/TcTqdlJeXN5lzeSYnj/N0PPFcDhs2jLS0NDZt2uRa+vXrx9ixY13f1/v5PP8xvU3DggULDIfDYcybN8/Yvn27ce+99xohISFGdna22dHqzSOPPGKsWrXKyMjIML777jtj+PDhRlhYmJGbm2t2tPNSWFhobNy40di4caMBGC+99JKxceNGY//+/YZhGMasWbOMkJAQ49NPPzW2bNliXH311Ua7du2M0tJSk5PXzS8dZ2FhofHoo48aKSkpRkZGhvH1118bffr0MTp16mSUlZWZHf2s3X///UZwcLCxatUq4/Dhw66lpKTEtc99991nxMXFGStWrDA2bNhgJCYmGomJiSamrrtfO849e/YYM2bMMDZs2GBkZGQYn376qdG+fXtjyJAhJievm8cff9xITk42MjIyjC1bthiPP/64YbFYjK+++sowjKZxLg3jl4+zqZzL0/n51Un1fT5VUH7ir3/9qxEXF2fY7XZjwIABxpo1a8yOVK9uvPFGo1WrVobdbjdat25t3HjjjcaePXvMjnXeVq5caQCnLOPHjzcMo+ZS4z/84Q9GZGSk4XA4jGHDhhnp6enmhj4Hv3ScJSUlxhVXXGGEh4cb3t7eRps2bYx77rnH4wr26Y4PMN59913XPqWlpcYDDzxgtGjRwvDz8zOuvfZa4/Dhw+aFPge/dpyZmZnGkCFDjNDQUMPhcBgdO3Y0pk6dauTn55sbvI7uvPNOo02bNobdbjfCw8ONYcOGucqJYTSNc2kYv3ycTeVcns7PC0p9n0+LYRjGub33IiIiItIwNAZFRERE3I4KioiIiLgdFRQRERFxOyooIiIi4nZUUERERMTtqKCIiIiI21FBEREREbejgiIiIiJuRwVFRERE3I4Kioi4lUsuuYRJkyaZHUNETKaCIiIiIm5H9+IREbdx++23895779Val5GRQdu2bc0JJCKmUUEREbeRn5/PyJEj6d69OzNmzAAgPDwcm81mcjIRaWxeZgcQETkpODgYu92On58fUVFRZscRERNpDIqIiIi4HRUUERERcTsqKCLiVux2O9XV1WbHEBGTqaCIiFtp27Yta9euZd++fRw9ehSn02l2JBExgQqKiLiVRx99FJvNRkJCAuHh4WRmZpodSURMoMuMRURExO3oHRQRERFxOyooIiIi4nZUUERERMTtqKCIiIiI21FBEREREbejgiIiIiJuRwVFRERE3I4KioiIiLgdFRQRERFxOyooIiIi4nZUUERERMTt/H+ULMP6uQRgbAAAAABJRU5ErkJggg==\n",
+                        "image/png": "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n0mJz80bb7xBz549XRN4JSYmsnTpUtf2pnAu4dePsymcy5+bNWsWFouFSZMmudbV9/lUQfnRP//5T6ZMmcJTTz3F999/T69evUhKSiI3N9fsaPWqW7duHD582LV8++23Zkc6b8XFxfTq1Ys5c+acdvsLL7zA7NmzmTt3LmvXrsXf35+kpCTKysoaOen5+bXjBBgxYkSt8/vhhx82YsLzl5yczIQJE1izZg3Lli2jsrKSK664guLiYtc+kydPZtGiRXz88cckJyeTlZXF6NGjTUxdd2dznAD33HNPrfP5wgsvmJT43MTExDBr1ixSU1PZsGEDl112GVdffTXbtm0Dmsa5hF8/TvD8c/lT69ev580336Rnz5611tf7+TTEMAzDGDBggDFhwgTXz9XV1UZ0dLQxc+ZME1PVr6eeesro1auX2TEaFGAsXLjQ9bPT6TSioqKMF1980bUuLy/PcDgcxocffmhCwvrx8+M0DMMYP368cfXVV5uSp6Hk5uYagJGcnGwYRs258/b2Nj7++GPXPjt27DAAIyUlxayY5+3nx2kYhjF06FDj4YcfNi9UA2nRooXx1ltvNdlzedLJ4zSMpnUuCwsLjU6dOhnLli2rdVwNcT71DgpQUVFBamoqw4cPd62zWq0MHz6clJQUE5PVv927dxMdHU379u0ZO3YsmZmZZkdqUBkZGWRnZ9c6t8HBwQwcOLDJnVuAVatWERERQXx8PPfffz/Hjh0zO9J5yc/PByA0NBSA1NRUKisra53PLl26EBcX59Hn8+fHedIHH3xAWFgY3bt3Z9q0aZSUlJgRr15UV1ezYMECiouLSUxMbLLn8ufHeVJTOZcTJkxg1KhRtc4bNMx/mx55s8D6dvToUaqrq4mMjKy1PjIykp07d5qUqv4NHDiQefPmER8fz+HDh3nmmWcYPHgwW7duJTAw0Ox4DSI7OxvgtOf25LamYsSIEYwePZp27dqxd+9ennjiCUaOHElKSgo2m83seHXmdDqZNGkSF110Ed27dwdqzqfdbickJKTWvp58Pk93nAC33HILbdq0ITo6mi1btvDYY4+Rnp7OJ598YmLauktLSyMxMZGysjICAgJYuHAhCQkJbNq0qUmdyzMdJzSdc7lgwQK+//571q9ff8q2hvhvUwWlGRk5cqTr+549ezJw4EDatGnDRx99xF133WViMqkPN910k+v7Hj160LNnTzp06MCqVasYNmyYicnOzYQJE9i6dWuTGCf1S850nPfee6/r+x49etCqVSuGDRvG3r176dChQ2PHPGfx8fFs2rSJ/Px8/vWvfzF+/HiSk5PNjlXvznScCQkJTeJcHjhwgIcffphly5bh4+PTKM+pj3iAsLAwbDbbKaONc3JyiIqKMilVwwsJCaFz587s2bPH7CgN5uT5a27nFqB9+/aEhYV55PmdOHEiixcvZuXKlcTExLjWR0VFUVFRQV5eXq39PfV8nuk4T2fgwIEAHnc+7XY7HTt2pG/fvsycOZNevXrx6quvNrlzeabjPB1PPJepqank5ubSp08fvLy88PLyIjk5mdmzZ+Pl5UVkZGS9n08VFGr+sPr27cvy5ctd65xOJ8uXL6/1GWJTU1RUxN69e2nVqpXZURpMu3btiIqKqnVuCwoKWLt2bZM+twAHDx7k2LFjHnV+DcNg4sSJLFy4kBUrVtCuXbta2/v27Yu3t3et85menk5mZqZHnc9fO87T2bRpE4BHnc/TcTqdlJeXN5lzeSYnj/N0PPFcDhs2jLS0NDZt2uRa+vXrx9ixY13f1/v5PP8xvU3DggULDIfDYcybN8/Yvn27ce+99xohISFGdna22dHqzSOPPGKsWrXKyMjIML777jtj+PDhRlhYmJGbm2t2tPNSWFhobNy40di4caMBGC+99JKxceNGY//+/YZhGMasWbOMkJAQ49NPPzW2bNliXH311Ua7du2M0tJSk5PXzS8dZ2FhofHoo48aKSkpRkZGhvH1118bffr0MTp16mSUlZWZHf2s3X///UZwcLCxatUq4/Dhw66lpKTEtc99991nxMXFGStWrDA2bNhgJCYmGomJiSamrrtfO849e/YYM2bMMDZs2GBkZGQYn376qdG+fXtjyJAhJievm8cff9xITk42MjIyjC1bthiPP/64YbFYjK+++sowjKZxLg3jl4+zqZzL0/n51Un1fT5VUH7ir3/9qxEXF2fY7XZjwIABxpo1a8yOVK9uvPFGo1WrVobdbjdat25t3HjjjcaePXvMjnXeVq5caQCnLOPHjzcMo+ZS4z/84Q9GZGSk4XA4jGHDhhnp6enmhj4Hv3ScJSUlxhVXXGGEh4cb3t7eRps2bYx77rnH4wr26Y4PMN59913XPqWlpcYDDzxgtGjRwvDz8zOuvfZa4/Dhw+aFPge/dpyZmZnGkCFDjNDQUMPhcBgdO3Y0pk6dauTn55sbvI7uvPNOo02bNobdbjfCw8ONYcOGucqJYTSNc2kYv3ycTeVcns7PC0p9n0+LYRjGub33IiIiItIwNAZFRERE3I4KioiIiLgdFRQRERFxOyooIiIi4nZUUERERMTtqKCIiIiI21FBEREREbejgiIiIiJuRwVFRERE3I4Kioi4lUsuuYRJkyaZHUNETKaCIiIiIm5H9+IREbdx++23895779Val5GRQdu2bc0JJCKmUUEREbeRn5/PyJEj6d69OzNmzAAgPDwcm81mcjIRaWxeZgcQETkpODgYu92On58fUVFRZscRERNpDIqIiIi4HRUUERERcTsqKCLiVux2O9XV1WbHEBGTqaCIiFtp27Yta9euZd++fRw9ehSn02l2JBExgQqKiLiVRx99FJvNRkJCAuHh4WRmZpodSURMoMuMRURExO3oHRQRERFxOyooIiIi4nZUUERERMTtqKCIiIiI21FBEREREbejgiIiIiJuRwVFRERE3I4KioiIiLgdFRQRERFxOyooIiIi4nZUUERERMTt/H+ULMP6uQRgbAAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "model_cashflows.plot(x=\"t\", y=\"expected_claim\");"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "60355de2-d475-40d7-9cef-119abbd6507a",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAiwAAAGwCAYAAACKOz5MAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy88F64QAAAACXBIWXMAAA9hAAAPYQGoP6dpAABI70lEQVR4nO3dd3gUdeLH8fdmk02BJARCGgSSUKUFCBBRUX4SCaiIHbFQjsOznlxscCcglgM99BRR7KJYQE8RKxYUFKVD6CAlECCNUFJJ253fH5HVKG1DktlsPq/n2edJZmcnny8Tsx9nZ75jMQzDQERERMSNeZkdQEREROR0VFhERETE7amwiIiIiNtTYRERERG3p8IiIiIibk+FRURERNyeCouIiIi4PW+zA9QEh8NBRkYGgYGBWCwWs+OIiIjIGTAMg4KCAqKiovDyOvUxFI8oLBkZGURHR5sdQ0RERKph3759tGzZ8pTreERhCQwMBCoHHBQUZHIaERERORP5+flER0c738dPxSMKy/GPgYKCglRYRERE6pkzOZ1DJ92KiIiI26tWYXn++eeJiYnBz8+PxMREVq5cedJ1P/roI3r16kWTJk1o1KgR3bt3Z86cOVXWMQyDSZMmERkZib+/P0lJSezYsaM60URERMQDuVxY5s2bR0pKCpMnT2bt2rXEx8eTnJxMTk7OCddv2rQp//rXv1i2bBkbNmxg9OjRjB49mq+++sq5zpNPPsmMGTN48cUXWbFiBY0aNSI5OZmSkpLqj0xEREQ8hsUwDMOVFyQmJtK7d29mzpwJVF5SHB0dzd1338348ePPaBs9e/bksssu49FHH8UwDKKiorj33nu57777AMjLyyM8PJzZs2dzww03/On1paWllJaWOr8/ftJOXl7eKc9hsdvtlJeXuzJckSp8fHywWq1mxxAR8Qj5+fkEBwef9v0bXDzptqysjDVr1jBhwgTnMi8vL5KSkli2bNlpX28YBt999x3bt2/niSeeACAtLY2srCySkpKc6wUHB5OYmMiyZctOWFimTp3KlClTzji3YRhkZWVx9OjRM36NyMk0adKEiIgIzfkjIlKHXCosubm52O12wsPDqywPDw9n27ZtJ31dXl4eLVq0oLS0FKvVygsvvMAll1wCQFZWlnMbf9zm8ef+aMKECaSkpDi/P36E5WSOl5WwsDACAgL0RiPV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e5LamR3pjOmYtoiISAPxzLe/sDb9KIF+3sy4oQc+1vpTA+pPUhEREam2n3bm8sLiXQBMu7ob0U0DTE7kGhUWERERD5dbWMq4eakYBgzv04rLukWaHcllKiwiIiIezOEwuPf99RwsqLwL86TLO5kdqVpUWERERDzYq0t3s+SXg/h6ezHzxp7426xmR6oWFRYREREPtX7fUZ5cuB2AyUM60z480ORE1afCIiIi4oEKSsq5+711VDgMLusayfA+0WZHOisqLCIiIh7GMAz+OX8T6YeLadHEn39f3bXeT3ipwiIiIuJhPli9n0/XZ2D1svDcjT0I9q//k6aqsIiIiHiQnTkFTP5kMwD3DmxPz1YhJieqGSosIiIiHqKk3M5d767jWLmdC9qGctuFbcyOVGNUWERERDzE459vZVtWAaGNbTw9LB4vr/p93srvqbCIiIh4gIWbspizfC8AT13fnbBAP5MT1SwVFhERkXpu/5FiHvjfegD+dmEcF7VvbnKimqfCIiIiUo+VVTi489115JdUEB/dhHsHdjA7Uq1QYREREanH/v3FVtbvO0qwvw/P39gDm7dnvrV75qhEREQagM83ZDL75z0A/HdYPC1DAswNVItUWEREROqh3QcLefDDDQDc3r8NF3cMNzlR7VJhERERqWeOldm54521FJZWkBjblHsvaW92pFqnwiIiIlLPTFqw6df5Vnx5bngPvK2e/3bu+SMUERHxIO+v3scHa/bjZYEZw7sTFuRZ862cjAqLiIhIPbE1M5+JH28CIOWS9pzXJtTkRHVHhUVERKQeKCgp54531lJa4aB/h+bc0b+t2ZHqlAqLiIiImzMMg/EfbiQtt4ioYD/+e313j7pP0JlQYREREXFzb/68h883ZuJjtTDzpp6ENLKZHanOqbCIiIi4sXXpR3j8i60ATBh8Dj1bhZicyBwqLCIiIm7qSFEZd727jnK7weAuEYw+P8bsSKZRYREREXFDDodByvupHDh6jJhmATxxbTcsloZ13srvqbCIiIi4oVlLdvH99oP4envxwk0JBPn5mB3JVCosIiIibuaHXw7y1NfbAXhkaGc6RQWZnMh8KiwiIiJuZN/hYv4+dx0OA27oHc2w3q3MjuQWVFhERETcxLEyO3+bs4ajxeXEtwzm4Ss6mx3JbaiwiIiIuAHDMPjX/I1sycynWSMbs25OwM/H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\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAiwAAAGwCAYAAACKOz5MAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/H5lhTAAAACXBIWXMAAA9hAAAPYQGoP6dpAABI70lEQVR4nO3dd3gUdeLH8fdmk02BJARCGgSSUKUFCBBRUX4SCaiIHbFQjsOznlxscCcglgM99BRR7KJYQE8RKxYUFKVD6CAlECCNUFJJ253fH5HVKG1DktlsPq/n2edJZmcnny8Tsx9nZ75jMQzDQERERMSNeZkdQEREROR0VFhERETE7amwiIiIiNtTYRERERG3p8IiIiIibk+FRURERNyeCouIiIi4PW+zA9QEh8NBRkYGgYGBWCwWs+OIiIjIGTAMg4KCAqKiovDyOvUxFI8oLBkZGURHR5sdQ0RERKph3759tGzZ8pTreERhCQwMBCoHHBQUZHIaERERORP5+flER0c738dPxSMKy/GPgYKCglRYRERE6pkzOZ1DJ92KiIiI26tWYXn++eeJiYnBz8+PxMREVq5cedJ1P/roI3r16kWTJk1o1KgR3bt3Z86cOVXWMQyDSZMmERkZib+/P0lJSezYsaM60URERMQDuVxY5s2bR0pKCpMnT2bt2rXEx8eTnJxMTk7OCddv2rQp//rXv1i2bBkbNmxg9OjRjB49mq+++sq5zpNPPsmMGTN48cUXWbFiBY0aNSI5OZmSkpLqj0xEREQ8hsUwDMOVFyQmJtK7d29mzpwJVF5SHB0dzd1338348ePPaBs9e/bksssu49FHH8UwDKKiorj33nu57777AMjLyyM8PJzZs2dzww03/On1paWllJaWOr8/ftJOXl7eKc9hsdvtlJeXuzJckSp8fHywWq1mxxAR8Qj5+fkEBwef9v0bXDzptqysjDVr1jBhwgTnMi8vL5KSkli2bNlpX28YBt999x3bt2/niSeeACAtLY2srCySkpKc6wUHB5OYmMiyZctOWFimTp3KlClTzji3YRhkZWVx9OjRM36NyMk0adKEiIgIzfkjIlKHXCosubm52O12wsPDqywPDw9n27ZtJ31dXl4eLVq0oLS0FKvVygsvvMAll1wCQFZWlnMbf9zm8ef+aMKECaSkpDi/P36E5WSOl5WwsDACAgL0RiPV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e5LamR3pjOmYtoiISAPxzLe/sDb9KIF+3sy4oQc+1vpTA+pPUhEREam2n3bm8sLiXQBMu7ob0U0DTE7kGhUWERERD5dbWMq4eakYBgzv04rLukWaHcllKiwiIiIezOEwuPf99RwsqLwL86TLO5kdqVpUWERERDzYq0t3s+SXg/h6ezHzxp7426xmR6oWFRYREREPtX7fUZ5cuB2AyUM60z480ORE1afCIiIi4oEKSsq5+711VDgMLusayfA+0WZHOisqLCIiIh7GMAz+OX8T6YeLadHEn39f3bXeT3ipwiIiIuJhPli9n0/XZ2D1svDcjT0I9q//k6aqsIiIiHiQnTkFTP5kMwD3DmxPz1YhJieqGSosIiIiHqKk3M5d767jWLmdC9qGctuFbcyOVGNUWERERDzE459vZVtWAaGNbTw9LB4vr/p93srvqbCIiIh4gIWbspizfC8AT13fnbBAP5MT1SwVFhERkXpu/5FiHvjfegD+dmEcF7VvbnKimqfCIiIiUo+VVTi489115JdUEB/dhHsHdjA7Uq1QYREREanH/v3FVtbvO0qwvw/P39gDm7dnvrV75qhEREQagM83ZDL75z0A/HdYPC1DAswNVItUWEREROqh3QcLefDDDQDc3r8NF3cMNzlR7VJhERERqWeOldm54521FJZWkBjblHsvaW92pFqnwiIiIlLPTFqw6df5Vnx5bngPvK2e/3bu+SMUERHxIO+v3scHa/bjZYEZw7sTFuRZ862cjAqLiIhIPbE1M5+JH28CIOWS9pzXJtTkRHVHhUVERKQeKCgp54531lJa4aB/h+bc0b+t2ZHqlAqLiIiImzMMg/EfbiQtt4ioYD/+e313j7pP0JlQYREREXFzb/68h883ZuJjtTDzpp6ENLKZHanOqbCIiIi4sXXpR3j8i60ATBh8Dj1bhZicyBwqLCIiIm7qSFEZd727jnK7weAuEYw+P8bsSKZRYREREXFDDodByvupHDh6jJhmATxxbTcsloZ13srvqbCIiIi4oVlLdvH99oP4envxwk0JBPn5mB3JVCosIiIibuaHXw7y1NfbAXhkaGc6RQWZnMh8KiwiIiJuZN/hYv4+dx0OA27oHc2w3q3MjuQWVFhERETcxLEyO3+bs4ajxeXEtwzm4Ss6mx3JbaiwiIiIuAHDMPjX/I1sycynWSMbs25OwM/H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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -350,40 +383,40 @@
             "outputs": [],
             "source": [
                 "## Calculate the present value"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 13,
             "id": "eefd51a4-9050-4e45-a1e8-77206cafe9d0",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "def npv(cashflows, rate):\n",
                 "    return sum(cashflow / ((1 + rate) ** t) for t, cashflow in enumerate(cashflows, 1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 14,
             "id": "cd8ff8bb-1674-4f8c-809a-540456c571e6",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "4364.808437169173"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "npv(model_cashflows[\"expected_claim\"], 0.04)"
             ]
@@ -394,50 +427,50 @@
             "metadata": {},
             "source": [
                 "Quick check that the NPV formula is sensible"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 15,
             "id": "537d294e-184c-414c-b927-84d53eb3ec92",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "5963.772020370224"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "npv(model_cashflows[\"expected_claim\"], 0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 16,
             "id": "aabb14a3-77c9-41e6-a302-6e9955ccbd2c",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "5963.772020370224"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_cashflows.expected_claim.sum()"
             ]
@@ -463,13 +496,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.0"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `heavylight-1.0.5/examples/notebook/heavylight_local.py` & `heavylight-1.0.6/src/heavylight/heavylight.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,160 @@
-import types
-from typing import List
 import warnings
-from inspect import signature
+import types
+from inspect import signature, getmembers
 import pandas as pd
 
-class Table:
-    """A Table has one or more keys, and a single column of values"""
-
-    def __init__(self, series):
-        """Initialise a table with a series - for multiple keys use a multikey index"""
-        self.series = series
-
-    def __getitem__(self, key):
-        return self.series.at[key]
-    
-    def __call__(self, key):
-        return self.series.at[key]
-    
-    def values(self, key):
-        return self.series.loc[key].values
-
-    @staticmethod
-    def from_csv(filename, sep=",", type_identifier = "|"):
-        """Read in a table from a csv file, type encoding is via the header:
-        
-        <keyname1>|<type1>,<keyname2>|<type2>....<value>|<typeN>
-        where type is one of "str", "int", "float"
-        """
-        column_types = {"str":str, "int": int, "float": float}
-        with open(filename, "r") as csv_file:
-            header = next(csv_file).strip("\n").split(sep)
-        tid = type_identifier
-        header_mapper_str = {item:item.split(tid)[1] for item in header}
-        header_mapper_types = {col:column_types[val] for col, val in header_mapper_str.items()}
-        df = pd.read_csv(filename, sep=sep, dtype=header_mapper_types)
-        # strip `tid` from column names
-        df.columns = [col.split("|")[0] for col in df.columns]
-        df.set_index(list(df.columns[:-1]), inplace=True)
-        series = df[df.columns[0]]
-        return Table(series=series)
-
-
 class _Cache:
     """Cache provides controllable memoization for model methods"""
 
-    def __init__(self, func: types.MethodType, param_len: int):
+    def __init__(self, func, param_len, param_names):
         self.func = func
         self.param_len = param_len
+        self.param_names = param_names
         self.has_one_param = self.param_len == 1
-        self.values = dict()
-        self.__name__ = "Cache: " + func.__name__
+        self._store = dict()
+        self.__name__ = func.__name__
 
-    def __call__(self, *arg:list):
-        if arg in self.values:
-            return self.values[arg]
+    def __call__(self, *arg):
+        if arg in self._store:
+            return self._store[arg]
         else:
             result = self.func(*arg)
-            self.values[arg] = result
+            self._store[arg] = result
             return result
 
-    def __repr__(self) -> str:
-        return f"<Cache Function: {self.func.__name__} Size: {len(self.values)}>"
+    def __repr__(self):
+        return f"<Cache Function: {self.func.__name__} Params: {self.param_names} Size: {len(self._store)}>"
+    
+    def sum(self):
+        """return the sum of all values in the Cache Function"""
+        return sum(self._store.values())
+    
+    @property
+    def keys(self):
+        return list(self._store.keys())
+
+    @property
+    def values(self):
+        return list(self._store.values())
+    
+    @property
+    def df(self):
+        """return the cache as a pandas dataframe"""
+        df = pd.DataFrame(data=self.keys, columns=self.param_names)
+        df[self.__name__] = self.values
+        # df = df.set_index(list(self.param_names))  # TODO: decide if keys should be indexes or not.
+        return df
 
 class Model:
-    def __init__(self, *, do_run: bool = False, verbose=False, proj_len: int|types.NoneType = None, **kwargs,):
+    def __init__(self, *, do_run = None, proj_len:int = 0, **kwargs,):
         """Base Class to subclass for user models.
 
+        When the model is instanced it is run to proj_len, if non-zero.
+
+        Parameters
+        ----------
+        - proj_len: length of projection to run
+        
+
         All variables/methods in user models should be lower case, using underscore as spaces.
 
         Class level methods:
           RunModel(proj_len):
-            if the model has not been auto-run at initialisation, run it for projection length.
+            Run the model to proj_len.
 
         Special user methods:
           BeforeRun(self):
             If this is specified in the user model it called before the projection starts, e.g. to set up some specific variables
 
           AfterRun(self):
             user method, called after Run is completed, e.g. can use to calculate NPVs of variables
 
         methods/variables to avoid:
         methods/variables starting with an underscore `_` are treated as internal.  You may break functionality if you create your own.
 
         """
 
+        if do_run is not None:
+            warnings.warn("Warning: `do_run` will be removed in a future version, use `proj_len` to control projection")
+        else:
+            do_run = proj_len > 0
+
         self._cached = False
         self._is_run = False
-        if verbose:
-            print("== Run Parameters ==")
-            print("    do_run:", do_run)
-            print("    proj_len:", proj_len)
-            print()
         
         if do_run:
+            # TODO: this can be cleaned up once do_run is removed
             if not isinstance(proj_len, int):
                 raise ValueError("proj_len must be an integer")
-            elif proj_len <= 0:
-                raise ValueError("proj_len must have value greater than 0")
+            elif proj_len < 0:
+                raise ValueError("proj_len must be non-negative")
             self.proj_len = proj_len
-        else:
-            if verbose: print("== Not Running - call Run() manually ==")
-       
-        if verbose: print("== Storing Arguments ==")
+
+        # store all keyword arguments as attributes
         for k, v in kwargs.items():
             if k in dir(self):
+                # TODO: include a strict mode that raises on duplicates?
                 warnings.warn("Warning: Duplicate Item: "+str(k))
             setattr(self, k, v)
-            if verbose:
-                print("    Updated: ", k, " : ", v)
 
         # cacheify
-        if verbose: print("== Caching Functions ==")
-        self._cache_funcs(verbose)
+        self._cache_funcs()
 
         if do_run and proj_len > 0:
-            self.RunModel(proj_len, verbose)
-        if verbose: print("== Run complete == ")
+            self.RunModel(proj_len)
 
-
-    def RunModel(self, proj_len, verbose=False):
+    def RunModel(self, proj_len: int):
         if self._is_run:
+            # TODO: replace this with ability to run further, but warn that earlier values not recalculated?
             raise ValueError("Run has already been completed.")
-
-        if verbose: print(f"== Running Projection | length: {proj_len} ==")
         
         if hasattr(self, "BeforeRun"):
-            if verbose: print("    Calling BeforeRun")
             self.BeforeRun()
 
         if not self._cached:
             raise ValueError("Functions have not been cached")  # NB: this shouldn't occur as now caching in instance
         for t in range(proj_len):
-            for var in self._funcs.keys():
-                func = getattr(self, var)
-                if func.has_one_param:   # skip functions with more than one parameter
+            for name, func in self._funcs.items():
+                if func.has_one_param and func.param_names[0] == 't':   # skip functions with more than one parameter
                     func(t)   #call each function in turn, starting from t==0
         self._is_run = True
+
         if hasattr(self, "AfterRun"):
-            if verbose: print("    Calling AfterRun")
             return self.AfterRun()
     
-    def _cache_funcs(self, verbose : bool=False):
+    def _cache_funcs(self):
         if self._cached:
             raise ValueError("Cache has already been set-up, please create a new instance")
 
         self._funcs = {}
 
-        for method_name in dir(self):
-            method = getattr(self, method_name)
-
+        for method_name, method in getmembers(self):
             if method_name[0] != "_" and method_name[0].islower() and isinstance(method, types.MethodType):
                 param_count = len(signature(method).parameters) # count the parameters in the function.
-                cached_method = _Cache(method, param_count)
+                param_names = tuple(signature(method).parameters)
+                cached_method = _Cache(method, param_count, param_names)
                 setattr(self, method_name, cached_method)
                 self._funcs[method_name] = cached_method
-                if verbose: print(f"    Cached: {method_name}")
-
-        
+       
         self._cached = True
+    
+    def _info(self):
+        """Print info about the model"""
+        for name, func in self._funcs.items():
+            print(f"{name}: {func}")
         
-    def ToDataFrame(self):
+    def ToDataFrame(self, param = 't'):
         """return a pandas dataframe of all single parameter columns"""
         df = pd.DataFrame()
         for func in self._funcs:
-            if self._funcs[func].has_one_param:
+            if self._funcs[func].has_one_param and self._funcs[func].param_names[0] == param:
                 df[func] = pd.Series(self._funcs[func].values)
-        return df
+
+        # if t is in the dataframe, move it to first position
+        if "t" in df.columns:
+            df.insert(0, "t", df.pop("t"))
+        return df
+    
+    @property
+    def df(self):
+        return self.ToDataFrame()
```

### Comparing `heavylight-1.0.5/examples/notebook/heavylight_tables.ipynb` & `heavylight-1.0.6/examples/notebook/heavylight_tables.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9859403935185185%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1}, 3: {'execution_count': 2}, 5: {'execution_count': 3}, 7: "*

 * *            "{'execution_count': 4}, 9: {'execution_count': 5, 'outputs': {0: {'execution_count': "*

 * *            "5}}}, 10: {'execution_count': 6, 'outputs': {0: {'execution_count': 6}}}, 12: "*

 * *            "{'execution_count': 8, 'source': {delete: [2]}}, 14: {'execution_count': 9, "*

 * *            "'outputs': {0: {'execution_count': 9}}}, 16: {'execution_count': 10, 'outputs': {0: "*

 * *            "{'execution_coun […]*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "source": [
                 "# Heavylight example notebook"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "2c0620e8-f047-4c82-b924-a8a88f6efef7",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from heavylight import Model, Table\n",
@@ -27,15 +27,15 @@
             "metadata": {},
             "source": [
                 "Define the model as a class - note that it doesn't need to be defined in terms of `t` for time, but this is fairly standard"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "2fa05b8f-c670-43c8-8a2a-dbe050661c64",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "class Annuity(Model):\n",
@@ -64,15 +64,15 @@
             "metadata": {},
             "source": [
                 "Define the data for the model, as a python dictionary (can use any storage object)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "a5497421-ce9d-44b7-991f-df61dc3a2db3",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "policy_data = {\n",
@@ -87,15 +87,15 @@
             "metadata": {},
             "source": [
                 "Creating a basis, pulling q_x from a csv file (made by `table_maker.ipynb`)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "id": "f6f4aa4a-6d10-467e-a715-a0cdbf84a7b9",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "basis = {\n",
@@ -111,15 +111,15 @@
             },
             "source": [
                 "check that the table is working"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "id": "31ea4f90",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -455,38 +455,38 @@
                             "46     46     0.384566\n",
                             "47     47     0.399713\n",
                             "48     48     0.415461\n",
                             "49     49     0.431832\n",
                             "50     50     0.448851"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "basis[\"q_x\"].df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "id": "fcde100b-0dfc-4efc-aae9-b9ea08bdada0",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.141392"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "basis[\"q_x\"][20]"
             ]
@@ -497,51 +497,50 @@
             "metadata": {},
             "source": [
                 "Create an instance of the model, passing in the data and basis."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "id": "6684b54a-fafd-4c28-bae2-6c9196d24064",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "model = Annuity(data = policy_data,\n",
                 "                basis = basis,\n",
-                "                do_run = True,\n",
                 "                proj_len = 40,\n",
                 "                )"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fe23fa8c-c58b-4991-b4d9-2af0eb2b15ca",
             "metadata": {},
             "source": [
                 "We can look-up individual results of the model directly"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "id": "2460b718-9c85-4cae-8779-b42d6031726e",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "379.74840601212895"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model.expected_claim(5)"
             ]
@@ -552,15 +551,15 @@
             "metadata": {},
             "source": [
                 "Pull all single parameter functions into a dataframe"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "77c5845a-a119-4476-aa47-f0403c1450c8",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
@@ -640,35 +639,35 @@
                             "0  0  0.661143      550.000000        0.066114     10.000000\n",
                             "1  1  0.641139      513.637151        0.068653      9.338857\n",
                             "2  2  0.620078      478.374486        0.071292      8.697718\n",
                             "3  3  0.598033      444.270217        0.074036      8.077640\n",
                             "4  4  0.575091      411.378405        0.076888      7.479607"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "model_cashflows = model.ToDataFrame()\n",
+                "model_cashflows = model.df\n",
                 "model_cashflows.head()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "38da052e-6a1f-4075-9621-da401e9561ac",
             "metadata": {},
             "source": [
                 "Plot the key output"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "ee35f832-25c3-4d16-abed-23704666ae45",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
@@ -683,15 +682,15 @@
             ],
             "source": [
                 "model_cashflows.plot(x=\"t\", y=\"expected_claim\");"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "id": "60355de2-d475-40d7-9cef-119abbd6507a",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
@@ -741,15 +740,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "4364.808437169173"
+                            "4364.808437169175"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -772,15 +771,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "5963.772020370226"
+                            "5963.772020370224"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -808,25 +807,183 @@
                 }
             ],
             "source": [
                 "model_cashflows.expected_claim.sum()"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "340610e3",
+            "metadata": {},
+            "source": [
+                "We can also view the dataframe for an individual model variable"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 18,
+            "id": "df3ef70c",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>t</th>\n",
+                            "      <th>deaths</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>0</td>\n",
+                            "      <td>0.661143</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>1</td>\n",
+                            "      <td>0.641139</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>2</td>\n",
+                            "      <td>0.620078</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>3</td>\n",
+                            "      <td>0.598033</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>4</td>\n",
+                            "      <td>0.575091</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   t    deaths\n",
+                            "0  0  0.661143\n",
+                            "1  1  0.641139\n",
+                            "2  2  0.620078\n",
+                            "3  3  0.598033\n",
+                            "4  4  0.575091"
+                        ]
+                    },
+                    "execution_count": 18,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "model.deaths.df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
             "id": "b6805aec-90ff-49fa-b8a7-bd1dcc737edd",
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>t</th>\n",
+                            "      <th>number_alive</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>35</th>\n",
+                            "      <td>35</td>\n",
+                            "      <td>0.056652</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>36</th>\n",
+                            "      <td>36</td>\n",
+                            "      <td>0.042400</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>37</th>\n",
+                            "      <td>37</td>\n",
+                            "      <td>0.031314</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>38</th>\n",
+                            "      <td>38</td>\n",
+                            "      <td>0.022805</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>39</th>\n",
+                            "      <td>39</td>\n",
+                            "      <td>0.016365</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "     t  number_alive\n",
+                            "35  35      0.056652\n",
+                            "36  36      0.042400\n",
+                            "37  37      0.031314\n",
+                            "38  38      0.022805\n",
+                            "39  39      0.016365"
+                        ]
+                    },
+                    "execution_count": 19,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "model.number_alive.df.tail()"
+            ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "258f4f5a",
+            "id": "87576628",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `heavylight-1.0.5/examples/notebook/sample_q_x_table.csv` & `heavylight-1.0.6/examples/notebook/sample_q_x_table.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/notebook/string_lookup_investigation.ipynb` & `heavylight-1.0.6/examples/notebook/string_lookup_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/notebook/table_documentation.ipynb` & `heavylight-1.0.6/examples/notebook/table_documentation.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/notebook/table_maker.ipynb` & `heavylight-1.0.6/examples/notebook/table_maker.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/notebook/vectors.ipynb` & `heavylight-1.0.6/examples/notebook/vectors.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9859489468864469%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1}, 2: {'execution_count': 2}, 3: {'execution_count': 3, "*

 * *            "'outputs': {0: {'execution_count': 3}}}, 4: {'execution_count': 4, 'outputs': {0: "*

 * *            "{'execution_count': 4}}}, 5: {'execution_count': 5}, 6: {'execution_count': 6, "*

 * *            "'outputs': {0: {'execution_count': 6}}}, 7: {'execution_count': 7}, 8: "*

 * *            "{'execution_count': 8}, 9: {'execution_count': 9}, 10: {'execution_count': 10, "*

 * *            "'outputs': {0: {'execution_count […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import heavylight\n",
                 "import pandas as pd\n",
                 "import numpy as np"
             ]
@@ -16,15 +16,15 @@
             "metadata": {},
             "source": [
                 "# A Vectorised Actuarial Contingency Model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class Life(heavylight.Model):\n",
                 "    time_step = 1/12\n",
                 "    def num_pols_if(self, t):\n",
                 "        if t == 0:\n",
@@ -52,136 +52,136 @@
                 "    def q_x(self, t):\n",
                 "        \"\"\"annual mortality rate\"\"\"\n",
                 "        return self.basis[\"mortality\"][self.age_rounded(t)]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([32.08333333, 42.        , 25.58333333])"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ages = np.array([32+1/12, 42, 25+7/12])\n",
                 "ages"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([2.67361111, 3.5       , 2.13194444])"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ages ** 1/12"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mortality = heavylight.Table.read_csv(\"sample_q_x_table.csv\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.141392  , 0.14691122])"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "mortality[np.array([20, 21])]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "basis = {\"mortality\": mortality}"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "num_model_points = 3\n",
                 "data = {\n",
                 "    \"initial_policies\": np.ones(num_model_points),\n",
                 "    \"initial_age\" : np.array([32+1/12, 42, 25+7/12]),\n",
                 "    }"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "model = Life(data=data, basis=basis)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.01372978, 0.0078071 , 0.01795082])"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model.num_pols_if(2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -502,22 +502,22 @@
                             "15  [0.8856621527884767, 0.9145793933046585, 0.868...  \n",
                             "16  [0.8856621527884767, 0.9145793933046585, 0.868...  \n",
                             "17  [0.8885085168518441, 0.9145793933046585, 0.868...  \n",
                             "18  [0.8885085168518441, 0.9175266940906103, 0.868...  \n",
                             "19  [0.8885085168518441, 0.9175266940906103, 0.868...  "
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model.num_pols_if(20)\n",
-                "model.ToDataFrame()"
+                "model.df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -536,13 +536,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.12.2"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `heavylight-1.0.5/examples/notebook/vectors.py` & `heavylight-1.0.6/examples/notebook/vectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # %%
 import heavylight
 import pandas as pd
 import numpy as np
 
 # A Vectorised Actuarial Contingency Model
 
+# This code is out of date/unmaintained but includes some examples of usage.
+
 # %%
 class Life(heavylight.Model):
     time_step = 1/12
 
     def t(self, t):
         return np.ones(self.data["data_count"]) * t
     
@@ -25,26 +27,26 @@
             return self.num_pols_if(t) * self.q_x_m(t)
     
     def age(self, t):
         """age at time t"""
         if t == 0:
             return self.data["initial_age"] # floating point
         else:
-            return self.age(t-1) + Life.time_step
+            return self.age(t - 1) + Life.time_step
     
     def age_rounded(self, t):
-        return np.round(self.age(t))
+        return np.round(self.age(t)).astype(int)
     
     def q_x_m(self, t):
         """monthly mortality rate"""
         return self.q_x(t) ** (Life.time_step)
     
     def q_x(self, t):
         """annual mortality rate"""
-        return self.basis["mortality"].values(self.age_rounded(t))
+        return self.basis["mortality"][self.age_rounded(t)]
     
     def premium(self, t):
         #print(self.data["premium"])
         #print(self.num_pols_if(t))
         return self.data["premium"] * self.num_pols_if(t)
     
     def claim(self, t):
@@ -56,32 +58,29 @@
         return self.premium(t) - self.claim(t)
     
     def mpnum(self, t):
         return self.data["mp_num"]
 
 
 # %%
-mortality = heavylight.Table.from_csv("sample_q_x_table.csv")
-
-# %%
-mortality.series.loc[np.array([20, 21])]
+mortality = heavylight.Table.read_csv("sample_q_x_table.csv")
 
 # %%
 basis = {"mortality": mortality}
 
 # %%
 
 
 def make_random_data(num_pols):
     rng = np.random.default_rng(seed=42)
     return_data = {}
     return_data["data_count"] = num_pols
     return_data["initial_policies"] = np.ones(num_pols)
     return_data["mp_num"] = np.arange(num_pols)
-    return_data["initial_age"] = rng.uniform(low=20.0, high=21.0, size=num_pols)
+    return_data["initial_age"] = rng.uniform(low=20.0, high=25.0, size=num_pols)
     return_data["premium"] = rng.beta(a=2, b=5, size=num_pols) * 100 + 50
     return_data["sum_assured"] = return_data["premium"] * 100 # rng.uniform(low=10.0, high=20, size=num_pols)
     return return_data
 
 """
 data = {
     "initial_policies": np.ones(num_model_points),
@@ -92,24 +91,17 @@
 """
 
 # num_model_points = 3
 
 
 # %%
 data = make_random_data(1000)
-model = Life(data=data, basis=basis) #, do_run=True, proj_len = 5)
-
-# %%
-model.RunModel(proj_len=120, verbose=True)
-#df = model.ToDataFrame()
-
+model = Life(data=data, basis=basis, proj_len=10) #, do_run=True, proj_len = 5)
 
 
-#for t in range(10):
-#    print(t, model.net_cashflow(t))
 
 # %%
 def expand(model, variable):
     """return a variable from the model as a dataframe
     rows = time
     columns = variables
     """
@@ -129,15 +121,15 @@
 
 # %%
 
 def dfize(model):
     columns = {}
     for func in model._funcs:
         func_values = getattr(model,func).values
-        if isinstance(list(func_values.values())[0], np.ndarray):
+        if isinstance(func_values.values[0], np.ndarray):
             # multi-index
             temp_df = pd.DataFrame(func_values).T.stack()
             columns[func] = temp_df
         else:
             print(f"Still to deal with {func}")
     return pd.concat(columns, axis=1)
```

### Comparing `heavylight-1.0.5/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv` & `heavylight-1.0.6/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/std_model/protection_model.py` & `heavylight-1.0.6/examples/std_model/protection_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             return self.num_pols_if(t) * self.basis["expense_pp"]/12 * self.inflation_factor(t)
       
     def pv_expenses(self, t):
         return self.v(t) * self.expenses(t)
 
     def num_pols_if(self, t):
         """number of policies in force"""
-        if t==0:
+        if t == 0:
             return self.data["init_pols_if"]
         elif t > self.data["term_y"] * 12:
             return 0
         else:
             return self.num_pols_if(t-1) - self.num_exits(t-1) - self.num_deaths(t-1)
     
     def num_exits(self, t):
@@ -84,15 +84,14 @@
         return self.data["age_at_entry"] + t//12
     
     
     def q_x_12(self, t):
         return 1-(1- self.q_x_rated(t))**(1/12)
     
     def q_x(self, t):
-        capped_duration = min(self.duration(t), 5)   # mortality table has a maximum duration of 5
-        return self.basis["mort_table"][self.age(t), capped_duration, self.data["smoker_status"]]
+        return self.basis["mort_table"][self.age(t), self.duration(t), self.data["smoker_status"]]
             
     def q_x_rated(self, t):
         return max(0, min(1 , self.q_x(t) * (1 + self.data["extra_mortality"]) ) )
         
     def commission(self, t):
         return 0
```

### Comparing `heavylight-1.0.5/examples/std_model/protection_risk_model_generic.xlsx` & `heavylight-1.0.6/examples/std_model/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/std_model/run_model.py` & `heavylight-1.0.6/src/heavylight/examples/protection/run_model_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# -*- coding: utf-8 -*-
-# required libraries:
-# heavylight
-# pip install heavylight
+# Example Protection Model
+#
+#
 
 # %%
 import heavylight
 from heavylight import Table
-from protection_model import TermAssurance
+from protection_model_base import TermAssurance
 
 def solve_prot_premium(model: heavylight.Model, data: dict, basis: dict):
     
     data = data.copy()
 
     pricing_entries = {
             "annual_premium":1,
             "init_pols_if":1,
             }
     
     data.update(pricing_entries)
 
     proj_len = data["term_y"] * 12 + 1
 
-    model_inst = model(data=data, basis=basis, proj_len=proj_len, do_run=True)
+    model_inst = model(data=data, basis=basis, proj_len=proj_len)
             
     # extract npvs
     npv_claims = model_inst.pv_claims.sum()
     npv_expenses = model_inst.pv_expenses.sum()
     npv_premiums = model_inst.pv_premiums.sum()
             
     # calculate premium
@@ -46,23 +45,22 @@
         "forward_rates": Table.read_csv(r"tables/forward_rates.csv"),
     }
 
     data = {
         "sum_assured": 100_000,
         "age_at_entry": 49,
         "term_y": 35,
-        "smoker_status": "S",
+        "smoker_status": "N",
         "shape": "level",
         "annual_premium": 1,
         "init_pols_if": 1,
         "extra_mortality": 0,
         "sex": "F"
     }
 
-    model = TermAssurance(basis=basis, data=data, proj_len=data["term_y"]*12 + 12, do_run=True)
-    print(model.ToDataFrame())
+    model = TermAssurance(basis=basis, data=data, proj_len=data["term_y"] * 12 + 12)
   
     monthly_premium = solve_prot_premium(TermAssurance, data, basis)
     print("Premium: ", monthly_premium)
```

### Comparing `heavylight-1.0.5/examples/std_model/tables/covert_q_x_tables.ipynb` & `heavylight-1.0.6/examples/std_model/tables/covert_q_x_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/std_model/tables/forward_rates.csv` & `heavylight-1.0.6/examples/std_model/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/std_model/tables/q_x_generic.csv` & `heavylight-1.0.6/examples/std_model/tables/q_x_generic.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-age|int,duration|int,smoker_status|str,q_x|float
+age|int_bound,duration|int_bound,smoker_status|str,q_x|float
 18,0,N,0.000231067
 19,0,N,0.00023532
 20,0,N,0.000239936
 21,0,N,0.000244937
 22,0,N,0.000250346
 23,0,N,0.000256188
 24,0,N,0.00026249
```

### Comparing `heavylight-1.0.5/examples/std_model/tables/qx_generic_raw.csv` & `heavylight-1.0.6/examples/std_model/tables/qx_generic_raw.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/examples/std_model/tables/uk_zero_spot.csv` & `heavylight-1.0.6/examples/std_model/tables/uk_zero_spot.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/src/heavylight/heavylight.py` & `heavylight-1.0.6/src/heavylight/memory_optimized_cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,161 @@
-import warnings
-import types
-from inspect import signature, getmembers
+from typing import Callable
+from collections import defaultdict
+from dataclasses import dataclass
+from functools import wraps
+from typing import Any, Callable, Tuple, Union, FrozenSet
 import pandas as pd
 
-class Table:
-    """A Table has one or more keys, and a single column of values"""
+@dataclass(frozen=True)
+class FunctionCall:
+    func_name: str
+    args: tuple
+    kwargs: FrozenSet[Tuple[str, Any]]
 
-    def __init__(self, series):
-        """Initialise a table with a series - for multiple keys use a multikey index"""
-        self.series = series
-
-    def __getitem__(self, key):
-        return self.series.at[key]
-    
-    def __call__(self, key):
-        return self.series.at[key]
-    
-    def values(self, key):
-        return self.series.loc[key].values
-
-    @staticmethod
-    def read_csv(filename, sep=",", type_identifier = "|"):
-        """Read in a table from a csv file, type encoding is via the header:
-        
-        <keyname1>|<type1>,<keyname2>|<type2>....<value>|<typeN>
-        where type is one of "str", "int", "float"
-        """
-        column_types = {"str": str, "int": int, "float": float}
-        with open(filename, "r") as csv_file:
-            header = next(csv_file).strip("\n").split(sep)
-        tid = type_identifier
-        header_mapper_str = {item:item.split(tid)[1] for item in header}
-        header_mapper_types = {col:column_types[val] for col, val in header_mapper_str.items()}
-        df = pd.read_csv(filename, sep=sep, dtype=header_mapper_types)
-        # strip `tid` from column names
-        df.columns = [col.split("|")[0] for col in df.columns]
-        df.set_index(list(df.columns[:-1]), inplace=True)
-        series = df[df.columns[0]]
-        return Table(series=series)
-
-
-class _Cache:
-    """Cache provides controllable memoization for model methods"""
+    def __repr__(self):
+        if len(self.kwargs) == 0:
+            if len(self.args) == 1:
+                return f"{self.func_name}({self.args[0]})"
+            return f"{self.func_name}{self.args}"
+        return f"{self.func_name}({', '.join(map(str, self.args))}, {', '.join(f'{k}={v}' for k, v in self.kwargs)})"
+
+ArgsHash = Tuple[Tuple, frozenset]
+
+class CacheGraph:
+    """
+    The cache graph maintains data structures necessary for caching and memory-optimizing collections of recursive functions.
+    It is applied to functions as a decorator
+    """
+    def __init__(self):
+        self.reset()
 
-    def __init__(self, func, param_len):
-        self.func = func
-        self.param_len = param_len
-        self.has_one_param = self.param_len == 1
-        self._store = dict()
-        self.__name__ = "Cache: " + func.__name__
-
-    def __call__(self, *arg):
-        if arg in self._store:
-            return self._store[arg]
-        else:
-            result = self.func(*arg)
-            self._store[arg] = result
-            return result
+    def reset(self):
+        """
+        Clear all internal state of the cache graph.
+        """
+        self.stack: list[FunctionCall] = [] # what function is currently being called
+        self._caches: defaultdict[str, dict[ArgsHash, Any]] = defaultdict(dict) # Results of function calls, ugly keys like ((1, 2), frozenset([('a', 1)]))
+        self._caches_agg: defaultdict[str, dict[ArgsHash, Any]] = defaultdict(dict)
+        self.graph: defaultdict[FunctionCall, set[FunctionCall]] = defaultdict(set) # Call graph, graph[caller] = [callee1, callee2, ...]
+        # Typically aggregated results for a function at a timestep.
+        # What is the last function that needs the result of a function? Used to help in clearing the cache
+        self.last_needed_by: dict[FunctionCall, FunctionCall] = {}
+        # can_clear[caller] = [callee1, callee2, ...] means that caller can clear the cache of callee1 and callee2
+        self.can_clear: dict[FunctionCall, list[FunctionCall]] = defaultdict(list)
+        self.all_calls: set[FunctionCall] = set()
+        self.cache_misses: defaultdict[FunctionCall, int] = defaultdict(int)
+
+    def check_if_cached(self, function_call: FunctionCall):
+        name_in_cache = function_call.func_name in self._caches
+        return name_in_cache and (function_call.args, function_call.kwargs) in self._caches[function_call.func_name]
+    
+    def optimize(self):
+        self.can_clear = defaultdict(list)
+        for callee, caller in self.last_needed_by.items():
+            self.can_clear[caller].append(callee)
+        uncleared_calls = self.all_calls - set(self.last_needed_by.keys())
+        for call in uncleared_calls:
+            self.can_clear[call].append(call)
+
+    def optimize_and_reset(self):
+        self.optimize()
+        can_clear = self.can_clear
+        self.reset()
+        self.can_clear = can_clear
+
+    def __call__(self, storage_func: Union[Callable[[int], Any], None] = None):
+        def custom_cache_decorator(func):
+            @wraps(func)
+            def wrapper(*args, **kwargs):
+                frozen_kwargs = frozenset(kwargs.items())
+                function_call = FunctionCall(func.__name__, args, frozen_kwargs)
+                if self.stack:
+                    self.graph[self.stack[-1]].add(function_call)
+                    self.last_needed_by[function_call] = self.stack[-1]
+                if not self.check_if_cached(function_call):
+                    self.all_calls.add(function_call)
+                    self.cache_misses[function_call] += 1
+                    self.stack.append(function_call)
+                    result = func(*args, **kwargs)
+                    self._caches[func.__name__][(args, frozen_kwargs)] = result
+                    for clearable_call in self.can_clear[function_call]:
+                        del self._caches[clearable_call.func_name][(clearable_call.args, clearable_call.kwargs)]
+                    self.stack.pop()
+                    self._store_result(storage_func, func, (args, frozen_kwargs), result)
+                    return result
+                return self._caches[func.__name__][(args, frozen_kwargs)]
+            decorator = CacheMethod(self, wrapper, storage_func)
+            return decorator
+        return custom_cache_decorator
+    
+    def _store_result(self, storage_func: Union[Callable, None], func: Callable, args_hash: ArgsHash, raw_result: Any):
+        """We might want to store an intermediate result"""
+        if storage_func is None:
+            return
+        stored_result = storage_func(raw_result)
+        self._caches_agg[func.__name__][args_hash] = stored_result
 
-    def __repr__(self):
-        return f"<Cache Function: {self.func.__name__} Size: {len(self._store)}>"
+    def size(self):
+        return sum(len(cache) for cache in self._caches.values())
     
-    def sum(self):
-        """return the sum of all values in the Cache Function"""
-        return sum(self._store.values())
+    @property
+    def cache(self):
+        caches = defaultdict(dict, {func_name: {get_pretty_key(k): v for k, v in cache.items()} for func_name, cache in self._caches.items()})
+        return caches
     
     @property
-    def values(self):
-        return list(self._store.values())
-
-
-class Model:
-    def __init__(self, *, do_run = False, verbose = False, proj_len = None, **kwargs,):
-        """Base Class to subclass for user models.
-
-        All variables/methods in user models should be lower case, using underscore as spaces.
+    def cache_agg(self):
+        caches = defaultdict(dict, {func_name: {get_pretty_key(k): v for k, v in cache.items()} for func_name, cache in self._caches_agg.items()})
+        return caches
+
+class CacheMethod:
+    def __init__(self, cache_graph: CacheGraph, func: Callable, agg_func: Union[Callable, None] = None):
+        self.cache_graph = cache_graph
+        self.func = func
+        self.agg_func = agg_func
 
-        Class level methods:
-          RunModel(proj_len):
-            if the model has not been auto-run at initialisation, run it for projection length.
+    @property
+    def df(self):
+        return pd.DataFrame({self.func.__name__: self.cache})
 
-        Special user methods:
-          BeforeRun(self):
-            If this is specified in the user model it called before the projection starts, e.g. to set up some specific variables
+    @property
+    def df_agg(self):
+        return pd.DataFrame({self.func.__name__: self.cache_agg})
 
-          AfterRun(self):
-            user method, called after Run is completed, e.g. can use to calculate NPVs of variables
+    # only run the dictionary comprehension for the particular method we want to access
+    # simply returning self.cache_graph.caches[self.func.__name__] would run the dictionary comprehension for all methods
+    @property
+    def cache(self):
+        return {get_pretty_key(k): v for k, v in self._cache.items()}
+    
+    @property
+    def cache_agg(self):
+        return {get_pretty_key(k): v for k, v in self._cache_agg.items()}
 
-        methods/variables to avoid:
-        methods/variables starting with an underscore `_` are treated as internal.  You may break functionality if you create your own.
+    @property
+    def _cache(self):
+        return self.cache_graph._caches[self.func.__name__]
 
-        """
+    @property
+    def _cache_agg(self):
+        return self.cache_graph._caches_agg[self.func.__name__]
 
-        self._cached = False
-        self._is_run = False
-        if verbose:
-            print("== Run Parameters ==")
-            print("    do_run:", do_run)
-            print("    proj_len:", proj_len)
-            print()
-        
-        if do_run:
-            if not isinstance(proj_len, int):
-                raise ValueError("proj_len must be an integer")
-            elif proj_len <= 0:
-                raise ValueError("proj_len must have value greater than 0")
-            self.proj_len = proj_len
+    def __setitem__(self, key, value):
+        if isinstance(key, int):
+            self._cache[((key,), frozenset())] = value
         else:
-            if verbose: print("== Not Running - call Run() manually ==")
-       
-        if verbose: print("== Storing Arguments ==")
-        for k, v in kwargs.items():
-            if k in dir(self):
-                warnings.warn("Warning: Duplicate Item: "+str(k))
-            setattr(self, k, v)
-            if verbose:
-                print("    Updated: ", k, " : ", v)
-
-        # cacheify
-        if verbose: print("== Caching Functions ==")
-        self._cache_funcs(verbose)
-
-        if do_run and proj_len > 0:
-            self.RunModel(proj_len, verbose)
-        if verbose: print("== Run complete == ")
-
-
-    def RunModel(self, proj_len, verbose = False):
-        if self._is_run:
-            raise ValueError("Run has already been completed.")
-
-        if verbose: print(f"== Running Projection | length: {proj_len} ==")
-        
-        if hasattr(self, "BeforeRun"):
-            if verbose: print("    Calling BeforeRun")
-            self.BeforeRun()
-
-        if not self._cached:
-            raise ValueError("Functions have not been cached")  # NB: this shouldn't occur as now caching in instance
-        for t in range(proj_len):
-            for name, func in self._funcs.items():
-                #func = getattr(self, var)
-                if func.has_one_param:   # skip functions with more than one parameter
-                    func(t)   #call each function in turn, starting from t==0
-        self._is_run = True
-        if hasattr(self, "AfterRun"):
-            if verbose: print("    Calling AfterRun")
-            return self.AfterRun()
-    
-    def _cache_funcs(self, verbose: bool = False):
-        if self._cached:
-            raise ValueError("Cache has already been set-up, please create a new instance")
-
-        self._funcs = {}
-
-        for method_name, method in getmembers(self):
-            #method = getattr(self, method_name)
-
-            if method_name[0] != "_" and method_name[0].islower() and isinstance(method, types.MethodType):
-                param_count = len(signature(method).parameters) # count the parameters in the function.
-                cached_method = _Cache(method, param_count)
-                setattr(self, method_name, cached_method)
-                self._funcs[method_name] = cached_method
-                if verbose: print(f"    Cached: {method_name}")
-
-        
-        self._cached = True
-        
-    def ToDataFrame(self):
-        """return a pandas dataframe of all single parameter columns"""
-        df = pd.DataFrame()
-        for func in self._funcs:
-            if self._funcs[func].has_one_param:
-                df[func] = pd.Series(self._funcs[func].values)
-
-        # if t is in the dataframe, move it to first position
-        if "t" in df.columns:
-            df.insert(0, "t", df.pop("t"))
-        return df
+            self._cache[(key, frozenset())] = value
+
+    def __repr__(self):
+        return f"<Cache Function: {self.func.__name__}, Size: {len(self._cache)}>"
+    
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.func(*args, **kwds)
+    
+def get_pretty_key(key: ArgsHash):
+    if len(key[0]) == 1 and len(key[1]) == 0:
+        return key[0][0]
+    elif len(key[1]) == 0:
+        return key[0]
+    else:
+        return key
+
```

### Comparing `heavylight-1.0.5/src/heavylight/heavytables.py` & `heavylight-1.0.6/src/heavylight/heavytables.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,26 @@
 # Lookup classes
 # Each key column requires an input class which maps from the source datatype to an integer
 
 class IntegerLookup:
     def get(self, values):
         return values
 
+class IntegerLookupSafe:
+    """An integer lookup that checks bounds"""
+    def __init__(self, lower, upper):
+        self.lower = lower
+        self.upper = upper
+    
+    def get(self, values):
+        # TODO: replace np.all with np.any for faster failing (probably doesn't improve performance)
+        if not np.all((self.lower <= values) & (values <= self.upper)):
+            raise KeyError(f'values are not between table minimum ({self.lower}) and maximum ({self.upper})')
+        return values
+
 class BoundIntLookup:
     def __init__(self, lower, upper):
         self.lower = int(lower)
         self.upper = int(upper)
     
     def get(self, numpy_array):
         return np.clip(numpy_array, self.lower, self.upper)
@@ -92,41 +104,53 @@
         return self.get_value(*keys)
     
 class Table:
     """Table provides multi-key compatible high performance table lookup.
     """
     col_types = "int", "int_bound", "str", "band", "float"
 
-    def __init__(self, df:pd.DataFrame):
+    def __init__(self, df:pd.DataFrame, rectify=False, safe=True):
         """Initialise a table from a dataframe.
         
+        parameters:
+         - `rectify`: force table to be rectangular (default False)
+         - `safe`: validates that integers are between bounds (default True)
+
         Tables should be in long format:
          - the final column containing the values to look up
          - all other columns contain keys to lookup
          - tables should be contingous, i.e. no gaps in integer keys.
          - tables should be complete if viewed as square matrixes (i.e. all combinations of keys are input).  If not, you should fill any gaps with np.nan or a suitable value.
 
         The type of key is determined by the suffix on the column name:
         `|int`: integers (...0, 1, 2, 3...), can start and end anywhere, but must be consecutive
         `|int_bound`: as `|int` but any values are constrained to the lowest and highest values.
         `|str': keys are interpreted as strings, e.g. 'M' and 'F'
         `|band`: key is numeric and treated as the upper bound on a lookup.
         `|float`: not currently available due to floating point equality, use int or band depending on use case.
         """
+        if rectify:
+            df = Table.rectify(df)
+
         key_cols = list(df.columns[:-1])
         df = df.sort_values(key_cols[::-1]) # sort by reverse order
 
         df_int_keys = df.copy() # this will have keys overridden as we work through mappers
 
         # prepare the mappers
         self.mappers = []
         for col in key_cols:
             col_type = col.split("|")[1] # "int", "str" etc
             if col_type == "int":
-                self.mappers.append(IntegerLookup()) # just so we have .get (a bit inefficient?)
+                if safe:
+                    lower = df[col].min()
+                    upper = df[col].max()                    
+                    self.mappers.append(IntegerLookupSafe(lower=lower, upper=upper))
+                else:
+                    self.mappers.append(IntegerLookup())
             elif col_type == "int_bound":
                 # bound integer forces values to be between the lowest and highest value in the table, for example maximum durations in mortality tables.
                 lower = df[col].min()
                 upper = df[col].max()
                 self.mappers.append(BoundIntLookup(lower=lower, upper=upper))
             elif col_type in ["str", "band"]:
                 df_col = pd.DataFrame(df[col].unique(), columns=["band_name"]).reset_index().sort_values("band_name")
@@ -156,15 +180,15 @@
         # print(keys, type(keys))
         if not isinstance(keys, tuple):
             keys = keys, #force to be a tuple
         return self.get(*keys)
 
     def __repr__(self):
         # TODO: return a nice representation of the table, e.g. head/keys etc.
-        return repr(self.df)
+        return self.df.__repr__()
     
     @staticmethod
     def rectify(df: pd.DataFrame, fill=np.nan) -> pd.DataFrame:
         """Convert a triangular (incomplete) dataframe into a valid rectangular dataframe
         
         any missing points will be filled with `fill`, default: np.nan
         """
```

### Comparing `heavylight-1.0.5/src/heavylight/memory_optimized_model.py` & `heavylight-1.0.6/src/heavylight/memory_optimized_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,146 @@
 from inspect import getmembers, signature
-from typing import Callable, List, Union
+from typing import Callable, Dict, List, Union, Any
 from types import MethodType
-from heavylight.memory_optimized_cache import CacheGraph, _Cache
+from heavylight.memory_optimized_cache import CacheGraph, CacheMethod, FunctionCall
 import pandas as pd
+import numpy as np
+
+
+def default_agg_function(x: Any):
+    """Default aggregation function for storing results."""
+    if isinstance(x, np.ndarray) and issubclass(x.dtype.type, np.number):
+        return np.sum(x)
+    return x
 
 
 class LightModel:
     """Base class to subclass from for recursive actuarial models.
 
     Inheriting from this class causes functions starting with a lowercase letter to be cached.
     A cached function will only be called once for each unique set of arguments.
     Caching is necessary for recursive actuarial calculations to be efficient.
 
     This means that the function will only be called once for each unique set of arguments, important for recursive actuarial models.
 
     Parameters
     ----------
-    storage_function: Callable[[int], Any], optional
-        This function is applied to the results of cached methods that have a single parameter `t`.
-        (e.g. `def pols_if(self, t):`).  The default is None, no values will be stored.
-        `storage_function=np.sum` will cause the sum of the results to be stored.
-        `storage_function=lambda x: x[0] if isinstance(x, np.ndarray) else x` will store the first element.
-        `storage_function=lambda x: x` will store the raw results.
+    agg_function: Callable[[int], Any], optional
+        This function is applied to the results of methods starting with a lowercase letter.
 
     Class level methods:
         RunModel(proj_len):
         if the model has not been auto-run at initialisation, run it for projection length.
 
     methods/variables to avoid:
     methods/variables starting with an underscore `_` are treated as internal.  You may break functionality if you create your own.
     """
-    
-    def __init__(self, storage_function: Union[Callable, None] = None):
+
+    def __init__(self, agg_function: Union[Callable, None] = default_agg_function):
         self.cache_graph = CacheGraph()
-        self._single_param_timestep_funcs: List[_Cache]  = []
-        self._storage_function = storage_function
+        self._single_param_timestep_funcs: List[CacheMethod] = []
+        self._funcs: Dict[MethodType, CacheMethod] = {}
         # happens after setting up attributes
         for method_name, method in getmembers(self):
-            if not method_name[0].islower() or method_name.startswith("_") or not isinstance(method, MethodType):
+            if (
+                not method_name[0].islower()
+                or method_name.startswith("_")
+                or not isinstance(method, MethodType)
+            ):
                 continue
-            is_single_param_t = check_if_single_parameter_t(method)
+            method_agg_function = getattr(method, "agg_function", None)
+            if not hasattr(method, "agg_function"): # only provide class-level agg_function if method-level is not provided
+                method_agg_function = agg_function
+            cached_method = self.cache_graph(method_agg_function)(method)
+            self._funcs[method] = cached_method
+            is_single_param_t = check_single_parameter_name(method, "t")
             if is_single_param_t:
-                cached_method = self.cache_graph(self._storage_function)(method)
                 self._single_param_timestep_funcs.append(cached_method)
-            else:
-                cached_method = self.cache_graph()(method)
             setattr(self, method_name, cached_method)
 
     def RunModel(self, proj_len: int):
         """
         Run the model for a projection length.
         All single parameter timestep functions will be run for each timestep.
         """
-        for t in range(proj_len+1):
+        for t in range(proj_len + 1):
             for func in self._single_param_timestep_funcs:
-                func(t)
+                # We avoid recalling any functions that have already been cached, resolves issue #15 lewisfogden/heavylight
+                if (
+                    not FunctionCall(func.func.__name__, (t,), frozenset())
+                    in self.cache_graph.all_calls
+                ):
+                    func(t)
 
     def ResetCache(self):
         """Reset the cache, useful if you want to run the model again with different parameters."""
         self.cache_graph.reset()
 
     def OptimizeMemoryAndReset(self):
         """
         Calling this clears the cache, and causes the cache to be optimized.
         Optimizing the cache means that only needed results are stored, and intermediate results are cleared.
         """
         self.cache_graph.optimize_and_reset()
 
-    def TimestepFunctions(self):
+    @property
+    def timestep_functions(self):
         """List the cached functions that have a single parameter `t`."""
-        return [cache._func.__name__ for cache in self._single_param_timestep_funcs]
-    
-    def StoredResults(self):
-        """
-        Return a dictionary of all stored results. 
-        The dictionary is of the form:
-        {function_name: {timestep: stored_result}}
-        """
-        return self.cache_graph.stored_results
-    
-    def ToDataFrame(self):
+        return [cache.func.__name__ for cache in self._single_param_timestep_funcs]
+
+    @property
+    def cache(self):
+        return self.cache_graph.cache
+
+    @property
+    def cache_agg(self):
+        return self.cache_graph.cache_agg
+
+    @property
+    def df(self):
+        return self.ToDataFrame(is_agg=False)
+
+    @property
+    def df_agg(self):
+        return self.ToDataFrame(is_agg=True)
+
+    def ToDataFrame(self, param_name="t", is_agg=False):
         """Return a pandas dataframe of all single parameter timestep results."""
-        df = pd.DataFrame(self.StoredResults())
+        get_method_cache = _get_method_cache_factory(is_agg)
+        filtered_cache = {}
+        for method, cache_method in self._funcs.items():
+            if not check_single_parameter_name(method, param_name):
+                continue
+            if is_agg and cache_method.agg_func is None:
+                continue
+            filtered_cache[method.__name__] = get_method_cache(cache_method)
+        df = pd.DataFrame(filtered_cache)
         # if t is in the dataframe, move it to first position
         if "t" in df.columns:
             df.insert(0, "t", df.pop("t"))
         return df
 
 
-def check_if_single_parameter_t(func: Callable):
+def check_single_parameter_name(func: Callable, name: str):
     sig = signature(func)
-    return 't' in sig.parameters and len(sig.parameters) == 1
+    return len(sig.parameters) == 1 and name in sig.parameters
+
+
+def agg(agg_function: Union[Callable, None]):
+    """
+    Register the storage function on a function.
+    Used for storing aggregated results before cache eviction to reduce memory consumption.
+    """
+
+    def decorator(func: Callable):
+        func.agg_function = agg_function # type: ignore
+        return func
+
+    return decorator
+
+
+def _get_method_cache_factory(is_agg: bool):
+    if is_agg:
+        accessor: Callable[[CacheMethod], Dict] = lambda method: method.cache_agg
+    else:
+        accessor: Callable[[CacheMethod], Dict] = lambda method: method.cache
+    return accessor
```

### Comparing `heavylight-1.0.5/tests/test_optimizations.py` & `heavylight-1.0.6/tests/test_memory_savings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import numpy as np
 from heavylight import LightModel
-from typing import Union, Callable
 import numpy as np
 import pytest
 
 class SimpleModel(LightModel):
-    """This class has some hard coded"""
 
-    def __init__(self, initial_pols_if: np.ndarray, storage_function: Union[Callable, None] = None, mortality_rate = .01):
-        super().__init__(storage_function=storage_function)
+    def __init__(self, initial_pols_if: np.ndarray, mortality_rate = .01):
+        super().__init__()
         self.initial_pols_if = initial_pols_if
         self.mortality_rate = mortality_rate
 
     def t(self, t):
         return np.int64(t) # to calculate nbytes for memory consumption
 
     def num_pols_if(self, t):
@@ -37,15 +35,15 @@
         return np.float64(0.04)
     
     def pv_cashflow(self, t):
         return self.cashflow(t) * self.v(t)
 
 def calculate_cache_graph_size(model: LightModel):
     cg = model.cache_graph
-    return sum(val.nbytes for cache in cg.caches.values() for val in cache.values())
+    return sum(val.nbytes for cache in cg._caches.values() for val in cache.values())
 
 def run_model_calculate_max_cache(model: SimpleModel, max_time: int):
     max_cache_size = 0
     for t in range(max_time+1):
         model.pv_cashflow(t)
         cache_size = calculate_cache_graph_size(model)
         max_cache_size = max(max_cache_size, cache_size)
@@ -60,7 +58,18 @@
 
 @pytest.mark.timeout(4)
 def test_memory_savings():
     model = SimpleModel(np.ones((1000,)))
     assert get_memory_savings_ratio(model, 100) < .01
     assert sum(model.cache_graph.cache_misses.values()) > 0 # verify that misses are being tracked
     assert all(misses == 1 for misses in model.cache_graph.cache_misses.values())
+
+def test_cache_misses():
+    sm = SimpleModel(np.linspace(.1, 1, 10))
+    sm.RunModel(5)
+    assert len(sm.cache_graph.cache_misses.values()) > 0
+    assert all(x == 1 for x in sm.cache_graph.cache_misses.values())
+    sm.OptimizeMemoryAndReset()
+    assert len(sm.cache_graph.cache_misses.values()) == 0
+    sm.RunModel(5)
+    assert len(sm.cache_graph.cache_misses.values()) > 0
+    assert all(x == 1 for x in sm.cache_graph.cache_misses.values())
```

### Comparing `heavylight-1.0.5/tests/test_optimized_cache.py` & `heavylight-1.0.6/tests/test_optimized_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,34 +16,36 @@
     cg = CacheGraph()
     @cg(lambda x: x**2)
     def fib(n):
         if n < 2:
             return n
         return fib(n - 1) + fib(n - 2)
     fib(5)
-    assert len(cg.stored_results["fib"]) == 6
-    for k, v in cg.stored_results["fib"].items():
+    assert len(cg.cache_agg["fib"]) == 6
+    for k, v in cg.cache_agg["fib"].items():
         assert v == fib(k)**2
 
 def test_cache_dunders():
     cg = CacheGraph()
     @cg()
     def fib(n):
         if n < 2:
             return n
         return fib(n - 1) + fib(n - 2)
     fib(5)
     assert repr(fib) == "<Cache Function: fib, Size: 6>"
     assert len(fib.cache) == 6
-    test_key = ((5,), frozenset())
-    assert fib.cache[test_key] == cg.caches['fib'][test_key] == 5
+    test_key = 5
+    assert fib.cache[test_key] == cg.cache['fib'][test_key] == 5
+    assert fib.cache[5] == 5 # prettified keys
     fib[5] = 10
-    assert fib.cache[test_key] == cg.caches['fib'][test_key] == 10
+    assert fib.cache[test_key] == cg.cache['fib'][test_key] == 10
+    assert fib.cache[5] == 10
     fib[(5,)] = 100
-    assert fib.cache[test_key] == cg.caches['fib'][test_key] == 100
+    assert fib.cache[test_key] == cg.cache['fib'][test_key] == 100
 
 @pytest.mark.timeout(4)
 def test_cache_graph_memory_optimization():
     cg = CacheGraph()
 
     @cg()
     def fib(n: int):
```

### Comparing `heavylight-1.0.5/tests/test_optimized_model.py` & `heavylight-1.0.6/tests/test_lightmodel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,112 @@
 import numpy as np
 from heavylight import LightModel
+from heavylight.memory_optimized_model import agg
 from typing import Union, Callable
 import pytest
 
 class SimpleModel(LightModel):
 
-    def __init__(self, initial_pols_if: np.ndarray, storage_function: Union[Callable, None] = None, mortality_rate = .01):
-        super().__init__(storage_function=storage_function)
+    def __init__(self, initial_pols_if: np.ndarray, mortality_rate = .01):
+        super().__init__()
         self.initial_pols_if = initial_pols_if
         self.mortality_rate = mortality_rate
 
     def t(self, t):
         return t
-
+    
     def num_pols_if(self, t):
         if t == 0:
             return self.initial_pols_if
         else:
             return self.num_pols_if(t - 1) - self.pols_death(t - 1) # causes exponential time complexity if uncached
-        
+    
     def pols_death(self, t):
         return self.num_pols_if(t) * self.mortality_rate
 
     def cashflow(self, t):
         return self.num_pols_if(t) * 100
     
     def v(self, t):
         """discount factor for time t --> time 0"""
         if t == 0:
             return 1
         else:
             return self.v(t - 1) / (1 + self.forward_rate(t))
     
+    @agg(lambda x: x * 2)
     def forward_rate(self, t):
         return 0.04
     
     def pv_cashflow(self, t):
         """present value of the cashflow occuring at time t"""
         return self.cashflow(t) * self.v(t)
     
     def fib(self, t, mult_factor):
         if t <= 1:
             return t
         return mult_factor * self.fib(t - 1, mult_factor) + self.fib(t - 2, mult_factor)
 
-def test_forward_rate():
-    sm = SimpleModel(np.linspace(.1, 1, 10), np.sum)
+def test_method_call_and_cache_retrievals():
+    sm = SimpleModel(np.linspace(.1, 1, 10))
     sm.forward_rate(0)
-    assert sm.forward_rate.cache[((0,), frozenset())] == .04
-    assert len(sm.StoredResults()) == 1
-    assert len(sm.StoredResults()['forward_rate']) == 1
-    assert sm.StoredResults()['forward_rate'][0] == .04
-
+    assert sm.forward_rate.cache[0] == .04
+    assert sm.cache_graph._caches['forward_rate'][((0,), frozenset())] == .04
+    assert sm.cache_graph.cache['forward_rate'][0] == .04
+    assert len(sm.cache_graph.cache) == 1
+    assert len(sm.forward_rate.cache) == 1
     sm.forward_rate(5)
     assert len(sm.forward_rate.cache) == 2
-
+    assert len(sm.cache_graph.cache) == 1
 
 def test_timestep_functions():
-    sm = SimpleModel(np.linspace(.1, 1, 10), np.sum)
-    timestep_functions = sm.TimestepFunctions()
+    sm = SimpleModel(np.linspace(.1, 1, 10))
+    timestep_functions = sm.timestep_functions
     expected_functions = ['t', 'num_pols_if', 'pols_death', 'cashflow', 'v', 'pv_cashflow', 'forward_rate']
     assert set(timestep_functions) == set(expected_functions) # no duplicates
-    sm.RunModel(5)
-    # The timestep functions are the ones displayed in StoredResults()
-    assert set(sm.StoredResults().keys()) == set(expected_functions)
 
 @pytest.mark.timeout(4)
-def test_caching():
-    sm = SimpleModel(np.linspace(.1, 1, 10), np.sum)
+def test_caching_speedups():
+    sm = SimpleModel(np.linspace(.1, 1, 10))
     assert len(sm.num_pols_if.cache) == 0
     sm.RunModel(200)
     assert len(sm.num_pols_if.cache) == 201
-    assert type(sm.StoredResults()['num_pols_if'][200]) == np.float64
     # fib did not get called because it is not single parameter time function
     assert len(sm.fib.cache) == 0
     sm.fib(200, 1.1)
     # but it is still cached
     assert len(sm.fib.cache) == 201
 
-def test_dataframe():
-    sm = SimpleModel(np.linspace(.1, 1, 10), np.sum)
-    sm.RunModel(5)
-    df = sm.ToDataFrame()
-    assert df.shape == (6, 7)
-    assert df['t'].tolist() == [0, 1, 2, 3, 4, 5]
-
 def test_reset_cache():
-    sm = SimpleModel(np.linspace(.1, 1, 10), storage_function=np.sum, mortality_rate=.01)
+    sm = SimpleModel(np.linspace(.1, 1, 10))
     sm.RunModel(5)
-    assert round(sm.StoredResults()['pols_death'][0], 10) == .055
+    assert round(np.sum(sm.pols_death.cache[0]), 10) == .055
     sm.mortality_rate = .02
     sm.RunModel(5)
-    assert round(sm.StoredResults()['pols_death'][0], 10) == .055
+    assert round(np.sum(sm.pols_death.cache[0]), 10) == .055
     sm.ResetCache()
     sm.RunModel(5)
-    assert round(sm.StoredResults()['pols_death'][0], 10) == .11
-    
+    assert round(np.sum(sm.pols_death.cache[0]), 10) == .11
 
+class TestPrettyCacheModel(LightModel):
+    def __init__(self):
+        super().__init__()
+    def t(self, t):
+        return self.wowee(t, 1) + self.zowee(t, x=1)
+    def wowee(self, t, x):
+        return 1
+    def zowee(self, t, x):
+        return 2
+    
+def test_pretty_cache():
+    pretty_model = TestPrettyCacheModel()
+    pretty_model.ResetCache()
+    pretty_model.RunModel(0)
+    assert pretty_model.cache_graph.cache['wowee'][(0,1)] == 1
+    assert pretty_model.wowee.cache[(0,1)] == 1
+    assert pretty_model.cache_graph.cache['zowee'][((0,),frozenset({'x': 1}.items()))] == 2
+    assert pretty_model.zowee.cache[((0,),frozenset({'x': 1}.items()))] == 2
+    assert pretty_model.cache_graph.cache['t'][0] == 3
+    assert pretty_model.t.cache[0] == 3
+    # can inject into the cache
+    pretty_model.zowee[1] = 'hello cache'
+    assert pretty_model.zowee.cache[1] == 'hello cache'
```

### Comparing `heavylight-1.0.5/.gitignore` & `heavylight-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/LICENSE` & `heavylight-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.5/README.md` & `heavylight-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![codecov](https://codecov.io/gh/actuarialopensource/heavylight/graph/badge.svg?token=40623XGSZS)](https://codecov.io/gh/actuarialopensource/heavylight)
+[![codecov](https://codecov.io/gh/lewisfogden/heavylight/graph/badge.svg?token=P81UIDV4FZ)](https://codecov.io/gh/lewisfogden/heavylight)
 
 # heavylight
 
 A lightweight actuarial modelling framework for Python
 
 - single script
 - installation optional: package with your models.
```

### Comparing `heavylight-1.0.5/pyproject.toml` & `heavylight-1.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 src-dir = "src"
 
 [project]
 name = "heavylight"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Lewis Fogden", email="lewisfogden@gmail.com" },
+  { name="Matthew Caseres", email="matthewcaseres@outlook.com"}
 ]
 description = "Heavylight Actuarial Modelling Framework"
 readme = "README.md"
 requires-python = ">=3.8"
 
 dependencies = [
     "pandas>=1.2",
@@ -44,8 +45,9 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lewisfogden/heavylight/"
-"Bug Tracker" = "https://github.com/lewisfogden/heavylight/issues"
+"Bug Tracker" = "https://github.com/lewisfogden/heavylight/issues"
+"Documentation" = "https://lewisfogden.github.io/heavylight/"
```

### Comparing `heavylight-1.0.5/PKG-INFO` & `heavylight-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.3
 Name: heavylight
-Version: 1.0.5
+Version: 1.0.6
 Summary: Heavylight Actuarial Modelling Framework
 Project-URL: Homepage, https://github.com/lewisfogden/heavylight/
 Project-URL: Bug Tracker, https://github.com/lewisfogden/heavylight/issues
-Author-email: Lewis Fogden <lewisfogden@gmail.com>
+Project-URL: Documentation, https://lewisfogden.github.io/heavylight/
+Author-email: Lewis Fogden <lewisfogden@gmail.com>, Matthew Caseres <matthewcaseres@outlook.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: pandas>=1.2
 Provides-Extra: dev
 Requires-Dist: numpy; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
 Requires-Dist: pytest==7.4.3; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Description-Content-Type: text/markdown
 
-[![codecov](https://codecov.io/gh/actuarialopensource/heavylight/graph/badge.svg?token=40623XGSZS)](https://codecov.io/gh/actuarialopensource/heavylight)
+[![codecov](https://codecov.io/gh/lewisfogden/heavylight/graph/badge.svg?token=P81UIDV4FZ)](https://codecov.io/gh/lewisfogden/heavylight)
 
 # heavylight
 
 A lightweight actuarial modelling framework for Python
 
 - single script
 - installation optional: package with your models.
```

