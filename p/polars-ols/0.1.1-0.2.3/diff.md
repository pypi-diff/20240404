# Comparing `tmp/polars_ols-0.1.1.tar.gz` & `tmp/polars_ols-0.2.3.tar.gz`

## Comparing `polars_ols-0.1.1.tar` & `polars_ols-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 polars_ols-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127      116 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.cargo/config.toml
--rw-r--r--   0     1001      127     3303 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      139 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.gitignore
--rw-r--r--   0     1001      127      912 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1067 2024-03-31 17:16:04.000000 polars_ols-0.1.1/LICENSE
--rw-r--r--   0     1001      127      671 2024-03-31 17:16:04.000000 polars_ols-0.1.1/Makefile
--rw-r--r--   0     1001      127     9347 2024-03-31 17:16:04.000000 polars_ols-0.1.1/README.md
--rw-r--r--   0     1001      127    35269 2024-03-31 17:16:04.000000 polars_ols-0.1.1/notebooks/polars_ols_demo.ipynb
--rw-r--r--   0     1001      127     3685 2024-03-31 17:16:04.000000 polars_ols-0.1.1/polars_ols/__init__.py
--rw-r--r--   0     1001      127    13458 2024-03-31 17:16:04.000000 polars_ols-0.1.1/polars_ols/least_squares.py
--rw-r--r--   0     1001      127     3464 2024-03-31 17:16:04.000000 polars_ols-0.1.1/polars_ols/utils.py
--rw-r--r--   0     1001      127       63 2024-03-31 17:16:04.000000 polars_ols-0.1.1/requirements.txt
--rw-r--r--   0     1001      127     6650 2024-03-31 17:16:04.000000 polars_ols-0.1.1/src/expressions.rs
--rw-r--r--   0     1001      127    16506 2024-03-31 17:16:04.000000 polars_ols-0.1.1/src/least_squares.rs
--rw-r--r--   0     1001      127     5290 2024-03-31 17:16:04.000000 polars_ols-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/__init__.py
--rw-r--r--   0     1001      127     6259 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/benchmark.py
--rw-r--r--   0     1001      127       87 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/requirements-test.txt
--rw-r--r--   0     1001      127    10690 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/test_ols.py
--rw-r--r--   0     1001      127    61832 2024-03-31 17:16:04.000000 polars_ols-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127     1748 2024-03-31 17:16:04.000000 polars_ols-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10014 1970-01-01 00:00:00.000000 polars_ols-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 polars_ols-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      127      116 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.cargo/config.toml
+-rw-r--r--   0     1001      127     3908 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      139 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.gitignore
+-rw-r--r--   0     1001      127      912 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1067 2024-04-04 18:39:35.000000 polars_ols-0.2.3/LICENSE
+-rw-r--r--   0     1001      127      671 2024-04-04 18:39:35.000000 polars_ols-0.2.3/Makefile
+-rw-r--r--   0     1001      127    13745 2024-04-04 18:39:35.000000 polars_ols-0.2.3/README.md
+-rw-r--r--   0     1001      127    44513 2024-04-04 18:39:35.000000 polars_ols-0.2.3/notebooks/polars_ols_demo.ipynb
+-rw-r--r--   0     1001      127     4327 2024-04-04 18:39:35.000000 polars_ols-0.2.3/polars_ols/__init__.py
+-rw-r--r--   0     1001      127    15159 2024-04-04 18:39:35.000000 polars_ols-0.2.3/polars_ols/least_squares.py
+-rw-r--r--   0     1001      127     3464 2024-04-04 18:39:35.000000 polars_ols-0.2.3/polars_ols/utils.py
+-rw-r--r--   0     1001      127       63 2024-04-04 18:39:35.000000 polars_ols-0.2.3/requirements.txt
+-rw-r--r--   0     1001      127     9320 2024-04-04 18:39:35.000000 polars_ols-0.2.3/src/expressions.rs
+-rw-r--r--   0     1001      127    16506 2024-04-04 18:39:35.000000 polars_ols-0.2.3/src/least_squares.rs
+-rw-r--r--   0     1001      127     5331 2024-04-04 18:39:35.000000 polars_ols-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/__init__.py
+-rw-r--r--   0     1001      127     6257 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/benchmark.py
+-rw-r--r--   0     1001      127       87 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/requirements-test.txt
+-rw-r--r--   0     1001      127    16848 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/test_ols.py
+-rw-r--r--   0     1001      127    61832 2024-04-04 18:39:35.000000 polars_ols-0.2.3/Cargo.lock
+-rw-r--r--   0     1001      127     1864 2024-04-04 18:39:35.000000 polars_ols-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    14452 1970-01-01 00:00:00.000000 polars_ols-0.2.3/PKG-INFO
```

### Comparing `polars_ols-0.1.1/.github/workflows/publish_to_pypi.yml` & `polars_ols-0.2.3/.github/workflows/publish_to_pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,37 @@
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
+  windows:
+    runs-on: windows-latest
+    strategy:
+      matrix:
+        target: [x64, x86]
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+          architecture: ${{ matrix.target }}
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.target }}
+          args: --release --out dist --find-interpreter
+          sccache: 'true'
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
+
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
@@ -122,15 +145,15 @@
         with:
           name: wheels
           path: dist
 
   release:
     name: Release
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, macos, sdist]
+    needs: [windows, linux, macos, sdist]
     runs-on: ubuntu-latest
     environment: pypi
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
     steps:
       - uses: actions/download-artifact@v3
         with:
```

### Comparing `polars_ols-0.1.1/.pre-commit-config.yaml` & `polars_ols-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.1/LICENSE` & `polars_ols-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.1/Makefile` & `polars_ols-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.1/README.md` & `polars_ols-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.3
+Name: polars-ols
+Version: 0.2.3
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: polars >=0.20.6
+Requires-Dist: numpy ; extra == 'dev'
+Requires-Dist: pytest >=7.4.1 ; extra == 'dev'
+Requires-Dist: pre-commit ; extra == 'dev'
+Requires-Dist: statsmodels ; extra == 'dev'
+Provides-Extra: dev
+License-File: LICENSE
+Summary: Polars Least Squares Extension
+Keywords: polars-extension,linear-regression
+Author-email: Azmy Rajab <azmy.rajab@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
 # Polars OLS
 ## Least squares extension in Polars
 
 Supports linear model estimation in [Polars](https://www.pola.rs/).
 
 This package provides efficient rust implementations of common linear
 regression variants (OLS, WLS, Ridge, Elastic Net, Non-negative least squares, Recursive least squares) and exposes
@@ -75,34 +94,80 @@
 │ 0.22  ┆ -0.07 ┆ 0.44  ┆ 1     ┆ 0.57    ┆ 0.37              ┆ 0.36            │
 └───────┴───────┴───────┴───────┴─────────┴───────────────────┴─────────────────┘
 ```
 
 The `mode` parameter is used to set the type of the output returned by all methods (`"predictions", "residuals", "coefficients"`).
 It defaults to returning predictions matching the input's length.
 
-In case `"coefficients"` is set the output's shape is the number of features specified, see below:
+In case `"coefficients"` is set the output is a [polars Struct](https://docs.pola.rs/user-guide/expressions/structs/) with coefficients as values and feature names as fields.
+It's output shape 'broadcasts' depending on context, see below:
 
 ```python
 coefficients = df.select(pl.col("y").least_squares.from_formula("x1 + x2", mode="coefficients")
-                         .alias("coefficients").round(2))
+                         .alias("coefficients"))
+
+coefficients_group = df.select("group", pl.col("y").least_squares.from_formula("x1 + x2", mode="coefficients").over("group")
+                        .alias("coefficients_group")).unique(maintain_order=True)
+
 print(coefficients)
+print(coefficients_group)
+```
+```
+shape: (1, 1)
+┌──────────────────────────────┐
+│ coefficients                 │
+│ ---                          │
+│ struct[3]                    │
+╞══════════════════════════════╡
+│ {0.977375,0.987413,0.000757} │  # <--- coef for x1, x2, and intercept added by formula API
+└──────────────────────────────┘
+shape: (2, 2)
+┌───────┬───────────────────────────────┐
+│ group ┆ coefficients_group            │
+│ ---   ┆ ---                           │
+│ i64   ┆ struct[3]                     │
+╞═══════╪═══════════════════════════════╡
+│ 1     ┆ {0.995157,0.977495,0.014344}  │
+│ 2     ┆ {0.939217,0.997441,-0.017599} │  # <--- (unique) coefficients per group
+└───────┴───────────────────────────────┘
+```
+
+For dynamic models (like `rolling_ols`) or if in a `.over`, `.group_by`, or `.with_columns` context, the
+coefficients will take the shape of the data it is applied on. For example:
+
+```python
+coefficients = df.with_columns(pl.col("y").least_squares.rls(pl.col("x1"), pl.col("x2"), mode="coefficients")
+                         .over("group").alias("coefficients"))
+
+print(coefficients.head())
 ```
 ```
-shape: (3, 1)
-┌──────────────┐
-│ coefficients │
-│ ---          │
-│ f32          │
-╞══════════════╡
-│ 0.98         │ <-- x1
-│ 0.99         │ <-- x2
-│ 0.0          │ <-- intercept added by formula api
-└──────────────┘
+shape: (5, 6)
+┌───────┬───────┬───────┬───────┬─────────┬─────────────────────┐
+│ y     ┆ x1    ┆ x2    ┆ group ┆ weights ┆ coefficients        │
+│ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---     ┆ ---                 │
+│ f64   ┆ f64   ┆ f64   ┆ i64   ┆ f64     ┆ struct[2]           │
+╞═══════╪═══════╪═══════╪═══════╪═════════╪═════════════════════╡
+│ 1.16  ┆ 0.72  ┆ 0.24  ┆ 1     ┆ 0.34    ┆ {1.235503,0.411834} │
+│ -2.16 ┆ -2.43 ┆ 0.18  ┆ 1     ┆ 0.97    ┆ {0.963515,0.760769} │
+│ -1.57 ┆ -0.63 ┆ -0.95 ┆ 1     ┆ 0.39    ┆ {0.975484,0.966029} │
+│ 0.21  ┆ 0.05  ┆ 0.23  ┆ 1     ┆ 0.8     ┆ {0.975657,0.953735} │
+│ 0.22  ┆ -0.07 ┆ 0.44  ┆ 1     ┆ 0.57    ┆ {0.97898,0.909793}  │
+└───────┴───────┴───────┴───────┴─────────┴─────────────────────┘
+```
+
+Finally, for convenience, in order to compute out-of-sample predictions you can use:
+```least_squares.{predict, predict_from_formula}```. This saves you the effort of un-nesting the coefficients and doing the dot product in
+python and instead does this in Rust, as an expression. Usage is as follows:
+
+```python
+df_test.select(pl.col("coefficients_train").least_squares.predict(pl.col("x1"), pl.col("x2")).alias("predictions_test"))
 ```
 
+
 Supported Models
 ------------
 
 Currently, this extension package supports the following variants:
 - Ordinary Least Squares: ```least_squares.ols```
 - Weighted Least Squares: ```least_squares.wls```
 - Regularized Least Squares (Lasso / Ridge / Elastic Net) ```least_squares.{lasso, ridge, elastic_net}```
@@ -145,7 +210,25 @@
 | Elastic Net             | 20.9 ms ± 0.3 ms| 134 ms ± 21 ms    | Sklearn        | 6.4x                         |
 | Recursive Least Squares | 163 ms ± 28 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 24.5x                        |
 | Rolling Least Squares   | 390 ms ± 10 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 10.2x                        |
 
 Numpy's `lstsq` is already a highly optimized call into LAPACK and so the scope for speed-up is limited.
 However, we can achieve substantial speed-ups for the more complex models by working entirely in rust
 and avoiding overhead from back and forth into python.
+
+Expect an additional relative order-of-magnitude speed up to your workflow if it involved repeated re-estimation of models in
+(python) loops.
+
+
+Credits & Related Projects
+------------
+- Rust linear algebra libraries [faer](https://faer-rs.github.io/getting-started.html) and [ndarray](https://docs.rs/ndarray/latest/ndarray/) support the implementations provided by this extension package
+- This package was templated around the very helpful: [polars-plugin-tutorial](https://marcogorelli.github.io/polars-plugins-tutorial/)
+- The python package [patsy](https://patsy.readthedocs.io/en/latest/formulas.html) is used for (optionally) building models from formulae
+- Please check out the extension package [polars-ds](https://github.com/abstractqqq/polars_ds_extension) for general data-science functionality in polars
+
+Future Work / TODOs
+------------
+- Support generic types, in rust implementations, so that both f32 and f64 types are recognized. Right now data is cast to f32 prior to estimation
+- Handle nulls more clearly
+- Add more detailed documentation on supported models, signatures, and API
+
```

### Comparing `polars_ols-0.1.1/notebooks/polars_ols_demo.ipynb` & `polars_ols-0.2.3/notebooks/polars_ols_demo.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9653688602926289%*

 * *Differences: {"'cells'": "{0: {'metadata': {'execution': {'iopub.execute_input': '2024-04-04T13:54:23.334449Z', "*

 * *            "'iopub.status.busy': '2024-04-04T13:54:23.334213Z', 'iopub.status.idle': "*

 * *            "'2024-04-04T13:54:23.427330Z', 'shell.execute_reply': '2024-04-04T13:54:23.426462Z', "*

 * *            "'shell.execute_reply.started': '2024-04-04T13:54:23.334422Z'}}}, 1: "*

 * *            "{'execution_count': 2, 'metadata': {'execution': {'iopub.execute_input': "*

 * *            "'2024-04-04T13:54:23.434983Z', 'iopub.s […]*

```diff
@@ -2,39 +2,39 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "8d7bae54-e858-410c-a574-da1aa325d90a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T21:57:34.736186Z",
-                    "iopub.status.busy": "2024-03-30T21:57:34.735888Z",
-                    "iopub.status.idle": "2024-03-30T21:57:34.831262Z",
-                    "shell.execute_reply": "2024-03-30T21:57:34.830795Z",
-                    "shell.execute_reply.started": "2024-03-30T21:57:34.736162Z"
+                    "iopub.execute_input": "2024-04-04T13:54:23.334449Z",
+                    "iopub.status.busy": "2024-04-04T13:54:23.334213Z",
+                    "iopub.status.idle": "2024-04-04T13:54:23.427330Z",
+                    "shell.execute_reply": "2024-04-04T13:54:23.426462Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:23.334422Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import polars as pl\n",
                 "import polars_ols as pls\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": 2,
             "id": "a070132d-27cd-4783-9799-f3b0a9f97ba9",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:18.719338Z",
-                    "iopub.status.busy": "2024-03-30T22:35:18.718782Z",
-                    "iopub.status.idle": "2024-03-30T22:35:18.726562Z",
-                    "shell.execute_reply": "2024-03-30T22:35:18.725765Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:18.719305Z"
+                    "iopub.execute_input": "2024-04-04T13:54:23.434983Z",
+                    "iopub.status.busy": "2024-04-04T13:54:23.428344Z",
+                    "iopub.status.idle": "2024-04-04T13:54:23.449867Z",
+                    "shell.execute_reply": "2024-04-04T13:54:23.449261Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:23.434963Z"
                 }
             },
             "outputs": [],
             "source": [
                 "def _make_data(n_samples: int = 2_000, \n",
                 "               n_features: int = 5,\n",
                 "               n_groups: int = 5,\n",
@@ -47,78 +47,78 @@
                 "        group=pl.lit(np.random.randint(0, n_groups, size=n_samples)),\n",
                 "        sample_weights=pl.lit(np.random.rand(n_samples)),\n",
                 "    )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 60,
+            "execution_count": 3,
             "id": "5ad1869e-d884-48e2-8f37-f790057ada1a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:18.970433Z",
-                    "iopub.status.busy": "2024-03-30T22:35:18.969884Z",
-                    "iopub.status.idle": "2024-03-30T22:35:18.978416Z",
-                    "shell.execute_reply": "2024-03-30T22:35:18.977501Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:18.970398Z"
+                    "iopub.execute_input": "2024-04-04T13:54:23.457231Z",
+                    "iopub.status.busy": "2024-04-04T13:54:23.456764Z",
+                    "iopub.status.idle": "2024-04-04T13:54:23.472340Z",
+                    "shell.execute_reply": "2024-04-04T13:54:23.470388Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:23.457199Z"
                 }
             },
             "outputs": [],
             "source": [
                 "df = _make_data(n_samples=2_000, n_features=3, n_groups=5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 61,
+            "execution_count": 4,
             "id": "52c33d88-7625-40af-a2e3-892e02ef61a1",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:19.188898Z",
-                    "iopub.status.busy": "2024-03-30T22:35:19.188274Z",
-                    "iopub.status.idle": "2024-03-30T22:35:19.197449Z",
-                    "shell.execute_reply": "2024-03-30T22:35:19.196732Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:19.188862Z"
+                    "iopub.execute_input": "2024-04-04T13:54:23.473953Z",
+                    "iopub.status.busy": "2024-04-04T13:54:23.473734Z",
+                    "iopub.status.idle": "2024-04-04T13:54:23.484063Z",
+                    "shell.execute_reply": "2024-04-04T13:54:23.483202Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:23.473931Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>y</th><th>group</th><th>sample_weights</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>i64</td><td>f64</td></tr></thead><tbody><tr><td>0.601261</td><td>-0.052977</td><td>0.21547</td><td>-0.888736</td><td>0</td><td>0.116126</td></tr><tr><td>1.731443</td><td>0.646151</td><td>-2.423311</td><td>0.046472</td><td>3</td><td>0.323262</td></tr><tr><td>-0.708048</td><td>1.789624</td><td>-0.234373</td><td>-0.705809</td><td>1</td><td>0.757549</td></tr><tr><td>-1.017972</td><td>0.777864</td><td>0.203982</td><td>-0.168796</td><td>1</td><td>0.478503</td></tr><tr><td>1.065668</td><td>-0.483242</td><td>-0.550395</td><td>-0.171939</td><td>0</td><td>0.872105</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>-0.648736</td><td>0.021036</td><td>2.149515</td><td>-1.522977</td><td>1</td><td>0.649506</td></tr><tr><td>-0.427719</td><td>-0.216672</td><td>0.445517</td><td>0.174263</td><td>2</td><td>0.876079</td></tr><tr><td>-1.709156</td><td>-1.779753</td><td>1.061953</td><td>2.46746</td><td>1</td><td>0.118507</td></tr><tr><td>-0.255468</td><td>0.194217</td><td>1.395433</td><td>-1.367962</td><td>0</td><td>0.518952</td></tr><tr><td>1.281586</td><td>0.069997</td><td>-0.707767</td><td>-0.485081</td><td>2</td><td>0.882951</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>y</th><th>group</th><th>sample_weights</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>i64</td><td>f64</td></tr></thead><tbody><tr><td>0.688224</td><td>0.166581</td><td>-1.147806</td><td>0.299763</td><td>1</td><td>0.780783</td></tr><tr><td>-0.767423</td><td>-0.172072</td><td>0.219928</td><td>0.762563</td><td>3</td><td>0.400249</td></tr><tr><td>0.007824</td><td>0.383562</td><td>0.496249</td><td>-0.85281</td><td>4</td><td>0.06215</td></tr><tr><td>-0.117801</td><td>0.324036</td><td>-0.823265</td><td>0.560717</td><td>1</td><td>0.63399</td></tr><tr><td>-0.419271</td><td>-0.030292</td><td>0.141252</td><td>0.238569</td><td>2</td><td>0.631137</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1.143583</td><td>-1.119926</td><td>0.408306</td><td>-0.258559</td><td>1</td><td>0.042462</td></tr><tr><td>0.407077</td><td>-0.605242</td><td>-1.878244</td><td>2.090213</td><td>0</td><td>0.062762</td></tr><tr><td>1.49233</td><td>-1.087611</td><td>-0.648135</td><td>0.263403</td><td>0</td><td>0.697357</td></tr><tr><td>0.028772</td><td>-0.021442</td><td>-0.511965</td><td>0.43346</td><td>1</td><td>0.892621</td></tr><tr><td>-0.013978</td><td>0.029645</td><td>-1.051704</td><td>0.976311</td><td>2</td><td>0.111758</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 6)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 x1        \u2506 x2        \u2506 x3        \u2506 y         \u2506 group \u2506 sample_weights \u2502\n",
                             "\u2502 ---       \u2506 ---       \u2506 ---       \u2506 ---       \u2506 ---   \u2506 ---            \u2502\n",
                             "\u2502 f64       \u2506 f64       \u2506 f64       \u2506 f64       \u2506 i64   \u2506 f64            \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0.601261  \u2506 -0.052977 \u2506 0.21547   \u2506 -0.888736 \u2506 0     \u2506 0.116126       \u2502\n",
-                            "\u2502 1.731443  \u2506 0.646151  \u2506 -2.423311 \u2506 0.046472  \u2506 3     \u2506 0.323262       \u2502\n",
-                            "\u2502 -0.708048 \u2506 1.789624  \u2506 -0.234373 \u2506 -0.705809 \u2506 1     \u2506 0.757549       \u2502\n",
-                            "\u2502 -1.017972 \u2506 0.777864  \u2506 0.203982  \u2506 -0.168796 \u2506 1     \u2506 0.478503       \u2502\n",
-                            "\u2502 1.065668  \u2506 -0.483242 \u2506 -0.550395 \u2506 -0.171939 \u2506 0     \u2506 0.872105       \u2502\n",
+                            "\u2502 0.688224  \u2506 0.166581  \u2506 -1.147806 \u2506 0.299763  \u2506 1     \u2506 0.780783       \u2502\n",
+                            "\u2502 -0.767423 \u2506 -0.172072 \u2506 0.219928  \u2506 0.762563  \u2506 3     \u2506 0.400249       \u2502\n",
+                            "\u2502 0.007824  \u2506 0.383562  \u2506 0.496249  \u2506 -0.85281  \u2506 4     \u2506 0.06215        \u2502\n",
+                            "\u2502 -0.117801 \u2506 0.324036  \u2506 -0.823265 \u2506 0.560717  \u2506 1     \u2506 0.63399        \u2502\n",
+                            "\u2502 -0.419271 \u2506 -0.030292 \u2506 0.141252  \u2506 0.238569  \u2506 2     \u2506 0.631137       \u2502\n",
                             "\u2502 \u2026         \u2506 \u2026         \u2506 \u2026         \u2506 \u2026         \u2506 \u2026     \u2506 \u2026              \u2502\n",
-                            "\u2502 -0.648736 \u2506 0.021036  \u2506 2.149515  \u2506 -1.522977 \u2506 1     \u2506 0.649506       \u2502\n",
-                            "\u2502 -0.427719 \u2506 -0.216672 \u2506 0.445517  \u2506 0.174263  \u2506 2     \u2506 0.876079       \u2502\n",
-                            "\u2502 -1.709156 \u2506 -1.779753 \u2506 1.061953  \u2506 2.46746   \u2506 1     \u2506 0.118507       \u2502\n",
-                            "\u2502 -0.255468 \u2506 0.194217  \u2506 1.395433  \u2506 -1.367962 \u2506 0     \u2506 0.518952       \u2502\n",
-                            "\u2502 1.281586  \u2506 0.069997  \u2506 -0.707767 \u2506 -0.485081 \u2506 2     \u2506 0.882951       \u2502\n",
+                            "\u2502 1.143583  \u2506 -1.119926 \u2506 0.408306  \u2506 -0.258559 \u2506 1     \u2506 0.042462       \u2502\n",
+                            "\u2502 0.407077  \u2506 -0.605242 \u2506 -1.878244 \u2506 2.090213  \u2506 0     \u2506 0.062762       \u2502\n",
+                            "\u2502 1.49233   \u2506 -1.087611 \u2506 -0.648135 \u2506 0.263403  \u2506 0     \u2506 0.697357       \u2502\n",
+                            "\u2502 0.028772  \u2506 -0.021442 \u2506 -0.511965 \u2506 0.43346   \u2506 1     \u2506 0.892621       \u2502\n",
+                            "\u2502 -0.013978 \u2506 0.029645  \u2506 -1.051704 \u2506 0.976311  \u2506 2     \u2506 0.111758       \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 61,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df"
             ]
@@ -131,23 +131,23 @@
                 "### 1. Basic Usage: OLS / WLS\n",
                 "- You can use `pls.compute_least_squares` or `least_squares.ols` from the registered namespace. They are equivalent.\n",
                 "- Simply pass an expression producing strictly positive sample weights to `sample_weights` argument to perform WLS"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 62,
+            "execution_count": 5,
             "id": "c7748165-bc22-4c0d-98d0-a7813d211449",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:19.836660Z",
-                    "iopub.status.busy": "2024-03-30T22:35:19.836048Z",
-                    "iopub.status.idle": "2024-03-30T22:35:19.846571Z",
-                    "shell.execute_reply": "2024-03-30T22:35:19.845658Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:19.836622Z"
+                    "iopub.execute_input": "2024-04-04T13:54:24.124322Z",
+                    "iopub.status.busy": "2024-04-04T13:54:24.123758Z",
+                    "iopub.status.idle": "2024-04-04T13:54:24.133322Z",
+                    "shell.execute_reply": "2024-04-04T13:54:24.132460Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:24.124289Z"
                 }
             },
             "outputs": [],
             "source": [
                 "ols_expr = pls.compute_least_squares(pl.col(\"y\"),  # target\n",
                 "                          pl.col(\"x1\"), pl.col(\"x2\"), pl.col(\"x3\"),  # features\n",
                 "                          mode=\"predictions\",\n",
@@ -164,63 +164,61 @@
             "metadata": {},
             "source": [
                 "- The expressions returned are normal polars expressions. You can operate on them lazily, so for example we can compute OLS per group in parallel using `.over(...)` or multiply it by some other expression etc."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 63,
+            "execution_count": 6,
             "id": "c824074b-cecd-43ef-a8b9-bfaeb44f77ad",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:20.558068Z",
-                    "iopub.status.busy": "2024-03-30T22:35:20.557189Z",
-                    "iopub.status.idle": "2024-03-30T22:35:20.574796Z",
-                    "shell.execute_reply": "2024-03-30T22:35:20.574012Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:20.558008Z"
+                    "iopub.execute_input": "2024-04-04T13:54:24.569112Z",
+                    "iopub.status.busy": "2024-04-04T13:54:24.568388Z",
+                    "iopub.status.idle": "2024-04-04T13:54:24.591020Z",
+                    "shell.execute_reply": "2024-04-04T13:54:24.590284Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:24.569050Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (10, 9)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>y</th><th>group</th><th>sample_weights</th><th>predictions_ols_group</th><th>predictions_ols</th><th>predictions_wls_masked</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>i64</td><td>f64</td><td>f32</td><td>f32</td><td>f32</td></tr></thead><tbody><tr><td>-1.694323</td><td>1.954149</td><td>0.327192</td><td>-0.60444</td><td>1</td><td>0.117535</td><td>-0.59859</td><td>-0.589218</td><td>-0.0</td></tr><tr><td>1.773093</td><td>0.765854</td><td>-1.431583</td><td>-0.970678</td><td>4</td><td>0.839584</td><td>-1.094716</td><td>-1.103445</td><td>-0.0</td></tr><tr><td>-0.176328</td><td>0.573347</td><td>-0.614593</td><td>0.21017</td><td>4</td><td>0.705172</td><td>0.217926</td><td>0.216044</td><td>0.0</td></tr><tr><td>0.021171</td><td>0.058956</td><td>0.296067</td><td>-0.416454</td><td>2</td><td>0.753221</td><td>-0.374001</td><td>-0.375123</td><td>-0.375364</td></tr><tr><td>1.012068</td><td>-1.626015</td><td>0.2702</td><td>0.345547</td><td>1</td><td>0.973876</td><td>0.355354</td><td>0.34566</td><td>0.0</td></tr><tr><td>-0.648736</td><td>0.021036</td><td>2.149515</td><td>-1.522977</td><td>1</td><td>0.649506</td><td>-1.509339</td><td>-1.517859</td><td>-0.0</td></tr><tr><td>-0.427719</td><td>-0.216672</td><td>0.445517</td><td>0.174263</td><td>2</td><td>0.876079</td><td>0.197837</td><td>0.198173</td><td>0.198149</td></tr><tr><td>-1.709156</td><td>-1.779753</td><td>1.061953</td><td>2.46746</td><td>1</td><td>0.118507</td><td>2.431038</td><td>2.420419</td><td>0.0</td></tr><tr><td>-0.255468</td><td>0.194217</td><td>1.395433</td><td>-1.367962</td><td>0</td><td>0.518952</td><td>-1.347131</td><td>-1.330657</td><td>-0.0</td></tr><tr><td>1.281586</td><td>0.069997</td><td>-0.707767</td><td>-0.485081</td><td>2</td><td>0.882951</td><td>-0.646275</td><td>-0.640843</td><td>-0.641546</td></tr></tbody></table></div>"
+                            "<small>shape: (10, 9)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>y</th><th>group</th><th>sample_weights</th><th>predictions_ols_group</th><th>predictions_ols</th><th>predictions_wls_masked</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>i64</td><td>f64</td><td>f32</td><td>f32</td><td>f32</td></tr></thead><tbody><tr><td>-0.239948</td><td>-0.366209</td><td>-0.561918</td><td>1.118226</td><td>1</td><td>0.63232</td><td>1.167158</td><td>1.168412</td><td>0.0</td></tr><tr><td>-1.049948</td><td>-0.947574</td><td>0.942109</td><td>1.116945</td><td>0</td><td>0.750647</td><td>1.048747</td><td>1.050843</td><td>0.0</td></tr><tr><td>-0.042678</td><td>-0.969169</td><td>-0.030938</td><td>1.171227</td><td>3</td><td>0.951124</td><td>1.038779</td><td>1.040223</td><td>0.0</td></tr><tr><td>0.27957</td><td>0.731888</td><td>1.280181</td><td>-2.252596</td><td>1</td><td>0.698999</td><td>-2.290655</td><td>-2.292642</td><td>-0.0</td></tr><tr><td>0.212038</td><td>0.002932</td><td>1.518842</td><td>-1.698552</td><td>4</td><td>0.905989</td><td>-1.729258</td><td>-1.737341</td><td>-0.0</td></tr><tr><td>1.143583</td><td>-1.119926</td><td>0.408306</td><td>-0.258559</td><td>1</td><td>0.042462</td><td>-0.429676</td><td>-0.436157</td><td>-0.0</td></tr><tr><td>0.407077</td><td>-0.605242</td><td>-1.878244</td><td>2.090213</td><td>0</td><td>0.062762</td><td>2.073736</td><td>2.079016</td><td>0.0</td></tr><tr><td>1.49233</td><td>-1.087611</td><td>-0.648135</td><td>0.263403</td><td>0</td><td>0.697357</td><td>0.242394</td><td>0.241683</td><td>0.0</td></tr><tr><td>0.028772</td><td>-0.021442</td><td>-0.511965</td><td>0.43346</td><td>1</td><td>0.892621</td><td>0.505115</td><td>0.505751</td><td>0.0</td></tr><tr><td>-0.013978</td><td>0.029645</td><td>-1.051704</td><td>0.976311</td><td>2</td><td>0.111758</td><td>1.043787</td><td>1.038543</td><td>1.038414</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (10, 9)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 x1        \u2506 x2        \u2506 x3        \u2506 y         \u2506 \u2026 \u2506 sample_we \u2506 predictio \u2506 predictio \u2506 predicti \u2502\n",
                             "\u2502 ---       \u2506 ---       \u2506 ---       \u2506 ---       \u2506   \u2506 ights     \u2506 ns_ols_gr \u2506 ns_ols    \u2506 ons_wls_ \u2502\n",
                             "\u2502 f64       \u2506 f64       \u2506 f64       \u2506 f64       \u2506   \u2506 ---       \u2506 oup       \u2506 ---       \u2506 masked   \u2502\n",
                             "\u2502           \u2506           \u2506           \u2506           \u2506   \u2506 f64       \u2506 ---       \u2506 f32       \u2506 ---      \u2502\n",
                             "\u2502           \u2506           \u2506           \u2506           \u2506   \u2506           \u2506 f32       \u2506           \u2506 f32      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 -1.694323 \u2506 1.954149  \u2506 0.327192  \u2506 -0.60444  \u2506 \u2026 \u2506 0.117535  \u2506 -0.59859  \u2506 -0.589218 \u2506 -0.0     \u2502\n",
-                            "\u2502 1.773093  \u2506 0.765854  \u2506 -1.431583 \u2506 -0.970678 \u2506 \u2026 \u2506 0.839584  \u2506 -1.094716 \u2506 -1.103445 \u2506 -0.0     \u2502\n",
-                            "\u2502 -0.176328 \u2506 0.573347  \u2506 -0.614593 \u2506 0.21017   \u2506 \u2026 \u2506 0.705172  \u2506 0.217926  \u2506 0.216044  \u2506 0.0      \u2502\n",
-                            "\u2502 0.021171  \u2506 0.058956  \u2506 0.296067  \u2506 -0.416454 \u2506 \u2026 \u2506 0.753221  \u2506 -0.374001 \u2506 -0.375123 \u2506 -0.37536 \u2502\n",
-                            "\u2502           \u2506           \u2506           \u2506           \u2506   \u2506           \u2506           \u2506           \u2506 4        \u2502\n",
-                            "\u2502 1.012068  \u2506 -1.626015 \u2506 0.2702    \u2506 0.345547  \u2506 \u2026 \u2506 0.973876  \u2506 0.355354  \u2506 0.34566   \u2506 0.0      \u2502\n",
-                            "\u2502 -0.648736 \u2506 0.021036  \u2506 2.149515  \u2506 -1.522977 \u2506 \u2026 \u2506 0.649506  \u2506 -1.509339 \u2506 -1.517859 \u2506 -0.0     \u2502\n",
-                            "\u2502 -0.427719 \u2506 -0.216672 \u2506 0.445517  \u2506 0.174263  \u2506 \u2026 \u2506 0.876079  \u2506 0.197837  \u2506 0.198173  \u2506 0.198149 \u2502\n",
-                            "\u2502 -1.709156 \u2506 -1.779753 \u2506 1.061953  \u2506 2.46746   \u2506 \u2026 \u2506 0.118507  \u2506 2.431038  \u2506 2.420419  \u2506 0.0      \u2502\n",
-                            "\u2502 -0.255468 \u2506 0.194217  \u2506 1.395433  \u2506 -1.367962 \u2506 \u2026 \u2506 0.518952  \u2506 -1.347131 \u2506 -1.330657 \u2506 -0.0     \u2502\n",
-                            "\u2502 1.281586  \u2506 0.069997  \u2506 -0.707767 \u2506 -0.485081 \u2506 \u2026 \u2506 0.882951  \u2506 -0.646275 \u2506 -0.640843 \u2506 -0.64154 \u2502\n",
-                            "\u2502           \u2506           \u2506           \u2506           \u2506   \u2506           \u2506           \u2506           \u2506 6        \u2502\n",
+                            "\u2502 -0.239948 \u2506 -0.366209 \u2506 -0.561918 \u2506 1.118226  \u2506 \u2026 \u2506 0.63232   \u2506 1.167158  \u2506 1.168412  \u2506 0.0      \u2502\n",
+                            "\u2502 -1.049948 \u2506 -0.947574 \u2506 0.942109  \u2506 1.116945  \u2506 \u2026 \u2506 0.750647  \u2506 1.048747  \u2506 1.050843  \u2506 0.0      \u2502\n",
+                            "\u2502 -0.042678 \u2506 -0.969169 \u2506 -0.030938 \u2506 1.171227  \u2506 \u2026 \u2506 0.951124  \u2506 1.038779  \u2506 1.040223  \u2506 0.0      \u2502\n",
+                            "\u2502 0.27957   \u2506 0.731888  \u2506 1.280181  \u2506 -2.252596 \u2506 \u2026 \u2506 0.698999  \u2506 -2.290655 \u2506 -2.292642 \u2506 -0.0     \u2502\n",
+                            "\u2502 0.212038  \u2506 0.002932  \u2506 1.518842  \u2506 -1.698552 \u2506 \u2026 \u2506 0.905989  \u2506 -1.729258 \u2506 -1.737341 \u2506 -0.0     \u2502\n",
+                            "\u2502 1.143583  \u2506 -1.119926 \u2506 0.408306  \u2506 -0.258559 \u2506 \u2026 \u2506 0.042462  \u2506 -0.429676 \u2506 -0.436157 \u2506 -0.0     \u2502\n",
+                            "\u2502 0.407077  \u2506 -0.605242 \u2506 -1.878244 \u2506 2.090213  \u2506 \u2026 \u2506 0.062762  \u2506 2.073736  \u2506 2.079016  \u2506 0.0      \u2502\n",
+                            "\u2502 1.49233   \u2506 -1.087611 \u2506 -0.648135 \u2506 0.263403  \u2506 \u2026 \u2506 0.697357  \u2506 0.242394  \u2506 0.241683  \u2506 0.0      \u2502\n",
+                            "\u2502 0.028772  \u2506 -0.021442 \u2506 -0.511965 \u2506 0.43346   \u2506 \u2026 \u2506 0.892621  \u2506 0.505115  \u2506 0.505751  \u2506 0.0      \u2502\n",
+                            "\u2502 -0.013978 \u2506 0.029645  \u2506 -1.051704 \u2506 0.976311  \u2506 \u2026 \u2506 0.111758  \u2506 1.043787  \u2506 1.038543  \u2506 1.038414 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 63,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.lazy().with_columns(ols_expr.over(\"group\").alias(\"predictions_ols_group\"),\n",
                 "                ols_expr.alias(\"predictions_ols\"),\n",
@@ -230,68 +228,129 @@
         },
         {
             "cell_type": "markdown",
             "id": "510b4ac4-9e35-4eda-aafe-5036f38462f8",
             "metadata": {},
             "source": [
                 "- The `mode` parameter controls the type of output produced. You can choose from {`predictions`, `coefficients`, `residuals`}. It defaults to `predictions`.\n",
-                "- `coefficients` normally resizes the output to match the number of features"
+                "- `coefficients` produces a compact struct with the names of your features as fields and estimated coefficients as values"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 64,
+            "execution_count": 7,
             "id": "223fdff7-3242-4fdf-b732-570cd07a5b0a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:21.657101Z",
-                    "iopub.status.busy": "2024-03-30T22:35:21.656531Z",
-                    "iopub.status.idle": "2024-03-30T22:35:21.669548Z",
-                    "shell.execute_reply": "2024-03-30T22:35:21.668529Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:21.657067Z"
+                    "iopub.execute_input": "2024-04-04T13:54:25.174668Z",
+                    "iopub.status.busy": "2024-04-04T13:54:25.174078Z",
+                    "iopub.status.idle": "2024-04-04T13:54:25.187081Z",
+                    "shell.execute_reply": "2024-04-04T13:54:25.186095Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:25.174635Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (3, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>coefficients</th></tr><tr><td>f32</td></tr></thead><tbody><tr><td>-1.0107</td></tr><tr><td>-1.012987</td></tr><tr><td>0.002998</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>coefficients</th></tr><tr><td>struct[3]</td></tr></thead><tbody><tr><td>{-0.998207,-1.003225,-0.016527}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
-                            "shape: (3, 1)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 coefficients \u2502\n",
-                            "\u2502 ---          \u2502\n",
-                            "\u2502 f32          \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 -1.0107      \u2502\n",
-                            "\u2502 -1.012987    \u2502\n",
-                            "\u2502 0.002998     \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "shape: (1, 1)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 coefficients                    \u2502\n",
+                            "\u2502 ---                             \u2502\n",
+                            "\u2502 struct[3]                       \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 {-0.998207,-1.003225,-0.016527} \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 64,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.select(pl.col(\"y\").least_squares.ols(pl.col(\"x1\"), pl.col(\"x2\"), add_intercept=True, mode=\"coefficients\")\n",
                 "          .alias(\"coefficients\"))"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "2025d7b3-036c-45c5-a425-088ae33bef72",
+            "metadata": {},
+            "source": [
+                "- If in a `.over()`, `.group_by()`, or a `.with_columns()` context, the output of `mode=\"coefficients\"` broadcasts to the shape of your data\n",
+                "- Computing least_squares operations in `.over()` is done in parallel in rust, so it is very efficient\n",
+                "- You can use `.unnest()` to unpack the coefficients to separate numeric columns"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "4271adf2-6cb4-46ee-90c7-4e1ac1d28d93",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2024-04-04T13:54:25.778421Z",
+                    "iopub.status.busy": "2024-04-04T13:54:25.777812Z",
+                    "iopub.status.idle": "2024-04-04T13:54:25.787983Z",
+                    "shell.execute_reply": "2024-04-04T13:54:25.786979Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:25.778385Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "shape: (5, 2)\n",
+                        "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                        "\u2502 group \u2506 coefficients                    \u2502\n",
+                        "\u2502 ---   \u2506 ---                             \u2502\n",
+                        "\u2502 i64   \u2506 struct[3]                       \u2502\n",
+                        "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                        "\u2502 1     \u2506 {-1.069746,-1.00847,-0.019304}  \u2502\n",
+                        "\u2502 3     \u2506 {-0.994216,-0.956845,-0.091147} \u2502\n",
+                        "\u2502 4     \u2506 {-0.983914,-0.991226,0.05257}   \u2502\n",
+                        "\u2502 1     \u2506 {-1.069746,-1.00847,-0.019304}  \u2502\n",
+                        "\u2502 2     \u2506 {-0.955812,-1.03732,0.021365}   \u2502\n",
+                        "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n",
+                        "shape: (5, 4)\n",
+                        "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                        "\u2502 group \u2506 x1        \u2506 x2        \u2506 const     \u2502\n",
+                        "\u2502 ---   \u2506 ---       \u2506 ---       \u2506 ---       \u2502\n",
+                        "\u2502 i64   \u2506 f32       \u2506 f32       \u2506 f32       \u2502\n",
+                        "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                        "\u2502 1     \u2506 -1.069746 \u2506 -1.00847  \u2506 -0.019304 \u2502\n",
+                        "\u2502 3     \u2506 -0.994216 \u2506 -0.956845 \u2506 -0.091147 \u2502\n",
+                        "\u2502 4     \u2506 -0.983914 \u2506 -0.991226 \u2506 0.05257   \u2502\n",
+                        "\u2502 1     \u2506 -1.069746 \u2506 -1.00847  \u2506 -0.019304 \u2502\n",
+                        "\u2502 2     \u2506 -0.955812 \u2506 -1.03732  \u2506 0.021365  \u2502\n",
+                        "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n"
+                    ]
+                }
+            ],
+            "source": [
+                "df_coefficients = df.select(\"group\", pl.col(\"y\").least_squares.ols(\n",
+                "    pl.col(\"x1\"), pl.col(\"x2\"), add_intercept=True, mode=\"coefficients\").over(\"group\")\n",
+                "          .alias(\"coefficients\"))\n",
+                "print(df_coefficients.head())\n",
+                "print(df_coefficients.unnest(\"coefficients\").head())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "d2658468-466a-4d9e-916f-4b711331ec96",
             "metadata": {},
             "source": [
                 "### 2. Regularized Models\n",
                 "- Ridge `least_squares.ridge`, Lasso `least_squares.lasso`, Elastic Net `least_squares.lasso` with optional non-negative constraint are implemented\n",
                 "- Apart from ridge, which is solved in closed form, the rust implementation for regularized models is cyclic coordinate descent with a soft thresholding function that supports an arbitrary combination of L1 / L2 penalties and non-negative constraint.\n",
                 "- `sample_weights` and `mode` are general parameters applicable to all models supported by this package\n",
@@ -302,38 +361,48 @@
                 "- max_iter: maximum number of coordinate descent iterations\n",
                 "- tol: tolerance for convergence criterion\n",
                 "- positive: boolean enforcing non-negativity constraints on coefficients"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 65,
+            "execution_count": 9,
             "id": "a9ba3765-2a42-4675-bc92-2d211bdcc03b",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:35:25.872426Z",
-                    "iopub.status.busy": "2024-03-30T22:35:25.872003Z",
-                    "iopub.status.idle": "2024-03-30T22:35:25.882727Z",
-                    "shell.execute_reply": "2024-03-30T22:35:25.881421Z",
-                    "shell.execute_reply.started": "2024-03-30T22:35:25.872398Z"
+                    "iopub.execute_input": "2024-04-04T13:54:26.389189Z",
+                    "iopub.status.busy": "2024-04-04T13:54:26.388786Z",
+                    "iopub.status.idle": "2024-04-04T13:54:26.442414Z",
+                    "shell.execute_reply": "2024-04-04T13:54:26.441781Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:26.389162Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "\u001b[0;31mInit signature:\u001b[0m\n",
                             "\u001b[0mpls\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mOLSKwargs\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m\u001b[0m\n",
                             "\u001b[0;34m\u001b[0m    \u001b[0malpha\u001b[0m\u001b[0;34m:\u001b[0m \u001b[0mOptional\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mfloat\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;36m0.0\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
                             "\u001b[0;34m\u001b[0m    \u001b[0ml1_ratio\u001b[0m\u001b[0;34m:\u001b[0m \u001b[0mOptional\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mfloat\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;32mNone\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
                             "\u001b[0;34m\u001b[0m    \u001b[0mmax_iter\u001b[0m\u001b[0;34m:\u001b[0m \u001b[0mOptional\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mint\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;36m1000\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
                             "\u001b[0;34m\u001b[0m    \u001b[0mtol\u001b[0m\u001b[0;34m:\u001b[0m \u001b[0mOptional\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mfloat\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;36m0.0001\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
                             "\u001b[0;34m\u001b[0m    \u001b[0mpositive\u001b[0m\u001b[0;34m:\u001b[0m \u001b[0mOptional\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mbool\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;32mFalse\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
                             "\u001b[0;34m\u001b[0m\u001b[0;34m)\u001b[0m \u001b[0;34m->\u001b[0m \u001b[0;32mNone\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
-                            "\u001b[0;31mDocstring:\u001b[0m      Specifies parameters relevant for regularized linear models: LASSO / Ridge / ElasticNet.\n",
+                            "\u001b[0;31mDocstring:\u001b[0m     \n",
+                            "Specifies parameters relevant for regularized linear models: LASSO / Ridge / ElasticNet.\n",
+                            "\n",
+                            "Attributes:\n",
+                            "    alpha: Regularization strength. Defaults to 0.0.\n",
+                            "    l1_ratio: Mixing parameter for ElasticNet regularization (0 for Ridge, 1 for LASSO).\n",
+                            "        Defaults to None (equivalent to Ridge regression).\n",
+                            "    max_iter: Maximum number of iterations. Defaults to 1000 iterations.\n",
+                            "    tol: Tolerance for convergence criterion. Defaults to 0.0001.\n",
+                            "    positive: Whether to enforce non-negativity constraints on coefficients.\n",
+                            "        Defaults to False (no constraint on coefficients).\n",
                             "\u001b[0;31mFile:\u001b[0m           ~/projects/polars_ols/polars_ols/least_squares.py\n",
                             "\u001b[0;31mType:\u001b[0m           type\n",
                             "\u001b[0;31mSubclasses:\u001b[0m     "
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -342,52 +411,50 @@
             "source": [
                 "# inspect OLS Kwargs\n",
                 "pls.OLSKwargs?"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 75,
+            "execution_count": 10,
             "id": "e35fbf57-3edb-4450-bcf7-a6c2aeef1e6f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:41:50.013432Z",
-                    "iopub.status.busy": "2024-03-30T22:41:50.012719Z",
-                    "iopub.status.idle": "2024-03-30T22:41:50.027921Z",
-                    "shell.execute_reply": "2024-03-30T22:41:50.027343Z",
-                    "shell.execute_reply.started": "2024-03-30T22:41:50.013389Z"
+                    "iopub.execute_input": "2024-04-04T13:54:26.667506Z",
+                    "iopub.status.busy": "2024-04-04T13:54:26.666625Z",
+                    "iopub.status.idle": "2024-04-04T13:54:26.683920Z",
+                    "shell.execute_reply": "2024-04-04T13:54:26.683218Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:26.667444Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (3, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>coef_enet_non_negative</th><th>coef_ridge</th></tr><tr><td>f32</td><td>f32</td></tr></thead><tbody><tr><td>0.0</td><td>-0.908504</td></tr><tr><td>0.0</td><td>-0.907049</td></tr><tr><td>0.0</td><td>-0.914558</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>coef_enet_non_negative</th><th>coef_ridge</th></tr><tr><td>struct[3]</td><td>struct[3]</td></tr></thead><tbody><tr><td>{0.0,0.0,0.0}</td><td>{-0.904563,-0.911394,-0.913853}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
-                            "shape: (3, 2)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 coef_enet_non_negative \u2506 coef_ridge \u2502\n",
-                            "\u2502 ---                    \u2506 ---        \u2502\n",
-                            "\u2502 f32                    \u2506 f32        \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0.0                    \u2506 -0.908504  \u2502\n",
-                            "\u2502 0.0                    \u2506 -0.907049  \u2502\n",
-                            "\u2502 0.0                    \u2506 -0.914558  \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "shape: (1, 2)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 coef_enet_non_negative \u2506 coef_ridge                      \u2502\n",
+                            "\u2502 ---                    \u2506 ---                             \u2502\n",
+                            "\u2502 struct[3]              \u2506 struct[3]                       \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 {0.0,0.0,0.0}          \u2506 {-0.904563,-0.911394,-0.913853} \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 75,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "elastic_net_expr = pl.col(\"y\").least_squares.elastic_net(pl.col(\"x1\"), pl.col(\"x2\"), pl.col(\"x3\"),\n",
                 "                                                         alpha=0.0001,\n",
@@ -414,23 +481,23 @@
                 "- For those who like specifying models in patsy formula syntax, that is also supported\n",
                 "- You can either use the `least_squares_from_formula` module level public function or `least_squares.from_formula` from registed namespace\n",
                 "- It tries to be clever and maps to the correct underlying implementation based on the model specific parameters you specify"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 83,
+            "execution_count": 11,
             "id": "8965d16a-1703-4a75-9729-d8fbadb7a1c7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:47:44.970198Z",
-                    "iopub.status.busy": "2024-03-30T22:47:44.969638Z",
-                    "iopub.status.idle": "2024-03-30T22:47:44.984139Z",
-                    "shell.execute_reply": "2024-03-30T22:47:44.983511Z",
-                    "shell.execute_reply.started": "2024-03-30T22:47:44.970164Z"
+                    "iopub.execute_input": "2024-04-04T13:54:27.290216Z",
+                    "iopub.status.busy": "2024-04-04T13:54:27.289873Z",
+                    "iopub.status.idle": "2024-04-04T13:54:27.435569Z",
+                    "shell.execute_reply": "2024-04-04T13:54:27.435274Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:27.290191Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -450,15 +517,15 @@
                             "\u2502 f64         \u2506 f64         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 1.0         \u2506 1.0         \u2502\n",
                             "\u2502 1.0         \u2506 1.0         \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 83,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# compute the residuals in two equivalent ways\n",
                 "df.select(\n",
@@ -466,23 +533,23 @@
                 "    pls.least_squares_from_formula(\"y ~ x1 + x2:x3 -1\", mode=\"residuals\").alias(\"residuals_1\"), \n",
                 "    (pl.col(\"y\") - pl.col(\"y\").least_squares.from_formula(\"x1 + x2:x3 -1\", mode=\"predictions\")).alias(\"residuals_2\"),\n",
                 ").corr()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 85,
+            "execution_count": 12,
             "id": "aa610cd9-3b3f-43ce-b9cc-24a92df55307",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T22:49:58.356254Z",
-                    "iopub.status.busy": "2024-03-30T22:49:58.355351Z",
-                    "iopub.status.idle": "2024-03-30T22:49:58.365799Z",
-                    "shell.execute_reply": "2024-03-30T22:49:58.364755Z",
-                    "shell.execute_reply.started": "2024-03-30T22:49:58.356187Z"
+                    "iopub.execute_input": "2024-04-04T13:54:27.577833Z",
+                    "iopub.status.busy": "2024-04-04T13:54:27.577529Z",
+                    "iopub.status.idle": "2024-04-04T13:54:27.582123Z",
+                    "shell.execute_reply": "2024-04-04T13:54:27.581714Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:27.577813Z"
                 }
             },
             "outputs": [],
             "source": [
                 "nnls_formula_expr = pl.col(\"y\").least_squares.from_formula(\"x1 + x2 + x3\",\n",
                 "                                       alpha=0.0001,\n",
                 "                                       positive=True,\n",
@@ -502,66 +569,66 @@
             "source": [
                 "### 4. Dynamic Regression Models\n",
                 "\n",
                 "- Consider the situation where you want to compute coefficients in an expanding or rolling window manner\n",
                 "    - naively, you could manually re-compute standard OLS function over consecutive windows (e.g. `.rolling(...).agg(...)`)\n",
                 "    - ... but that would be wasteful: (X.T X) and (X.T Y) are only changing by one row (in case of expanding) or two rows (in case of rolling, an addition and a subtraction)\n",
                 "- This extension package provides rust implementations `.least_squares.{rolling_ols, expanding_ols, rls}` which efficiently update coefficients as new samples are observed\n",
-                "- See [insert URL] for details, but the key idea is to make use of Sherman-Morrison or Woodbury Identity to recursively update summary statistics or coefficient vectors\n",
+                "- The key idea is to make use of Sherman-Morrison or Woodbury Identity to recursively update summary statistics or coefficient vectors\n",
                 "- Formula API is also supported and the correct implementation is chosen based on parameters provided"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 115,
+            "execution_count": 13,
             "id": "33a8ee68-dc8b-4a2e-a590-73a4998bc33e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-03-30T23:09:02.183836Z",
-                    "iopub.status.busy": "2024-03-30T23:09:02.182878Z",
-                    "iopub.status.idle": "2024-03-30T23:09:02.208599Z",
-                    "shell.execute_reply": "2024-03-30T23:09:02.208100Z",
-                    "shell.execute_reply.started": "2024-03-30T23:09:02.183760Z"
+                    "iopub.execute_input": "2024-04-04T13:54:28.355492Z",
+                    "iopub.status.busy": "2024-04-04T13:54:28.354941Z",
+                    "iopub.status.idle": "2024-04-04T13:54:28.381642Z",
+                    "shell.execute_reply": "2024-04-04T13:54:28.381188Z",
+                    "shell.execute_reply.started": "2024-04-04T13:54:28.355460Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>rolling_ridge_coef</th><th>recursive_least_squares_coef</th><th>expanding_ols_pred</th></tr><tr><td>list[f32]</td><td>list[f32]</td><td>f32</td></tr></thead><tbody><tr><td>[0.0, 0.0, 0.0]</td><td>[-1.184433, -0.98375, -1.066094]</td><td>-0.71473</td></tr><tr><td>[0.0, 0.0, 0.0]</td><td>[-0.999859, -0.999947, -1.000197]</td><td>0.036505</td></tr><tr><td>[0.0, 0.0, 0.0]</td><td>[-1.026656, -0.932625, -1.008824]</td><td>-0.647632</td></tr><tr><td>[0.0, 0.0, 0.0]</td><td>[-0.702152, -0.826215, -1.180636]</td><td>-0.022153</td></tr><tr><td>[0.0, 0.0, 0.0]</td><td>[-1.176702, -0.996126, -1.091328]</td><td>-0.022653</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>[-0.993268, -1.003389, -0.993135]</td><td>[-0.955148, -0.971003, -0.987288]</td><td>-1.517609</td></tr><tr><td>[-0.996397, -0.98888, -0.998935]</td><td>[-0.421874, -1.801489, -0.889335]</td><td>0.198206</td></tr><tr><td>[-0.993697, -1.003618, -0.993094]</td><td>[-1.015508, -1.010919, -1.005117]</td><td>2.42057</td></tr><tr><td>[-0.994889, -1.001311, -1.006162]</td><td>[-0.782951, -1.192956, -0.957612]</td><td>-1.330491</td></tr><tr><td>[-0.995584, -0.987763, -0.999201]</td><td>[-1.075299, -1.604798, -1.420408]</td><td>-0.640809</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>rolling_ridge_coef</th><th>recursive_least_squares_coef</th><th>expanding_ols_pred</th></tr><tr><td>struct[3]</td><td>struct[3]</td><td>f32</td></tr></thead><tbody><tr><td>{0.0,0.0,0.0}</td><td>{-0.997571,-0.999412,-1.004052}</td><td>0.284141</td></tr><tr><td>{0.0,0.0,0.0}</td><td>{-1.043208,-1.009688,-0.987618}</td><td>0.553695</td></tr><tr><td>{0.0,0.0,0.0}</td><td>{-0.999444,-0.97275,-0.964744}</td><td>-0.711872</td></tr><tr><td>{0.0,0.0,0.0}</td><td>{-0.938403,-1.031698,-0.967921}</td><td>0.564383</td></tr><tr><td>{0.0,0.0,0.0}</td><td>{-0.900343,-0.9928,-1.033574}</td><td>0.263497</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>{-1.00591,-1.000234,-1.002072}</td><td>{-1.004769,-1.006106,-0.981976}</td><td>-0.436183</td></tr><tr><td>{-0.995429,-0.995031,-0.995304}</td><td>{-0.999747,-0.994992,-0.982279}</td><td>2.078985</td></tr><tr><td>{-0.995239,-0.995055,-0.995537}</td><td>{-0.997495,-0.99649,-0.982933}</td><td>0.241709</td></tr><tr><td>{-1.005733,-0.999528,-1.001679}</td><td>{-1.005132,-1.005992,-0.980991}</td><td>0.505744</td></tr><tr><td>{-1.006673,-0.995687,-1.013054}</td><td>{-1.015187,-0.9873,-1.038931}</td><td>1.038495</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 3)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 rolling_ridge_coef                \u2506 recursive_least_squares_coef      \u2506 expanding_ols_pred \u2502\n",
-                            "\u2502 ---                               \u2506 ---                               \u2506 ---                \u2502\n",
-                            "\u2502 list[f32]                         \u2506 list[f32]                         \u2506 f32                \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 [0.0, 0.0, 0.0]                   \u2506 [-1.184433, -0.98375, -1.066094]  \u2506 -0.71473           \u2502\n",
-                            "\u2502 [0.0, 0.0, 0.0]                   \u2506 [-0.999859, -0.999947, -1.000197\u2026 \u2506 0.036505           \u2502\n",
-                            "\u2502 [0.0, 0.0, 0.0]                   \u2506 [-1.026656, -0.932625, -1.008824\u2026 \u2506 -0.647632          \u2502\n",
-                            "\u2502 [0.0, 0.0, 0.0]                   \u2506 [-0.702152, -0.826215, -1.180636\u2026 \u2506 -0.022153          \u2502\n",
-                            "\u2502 [0.0, 0.0, 0.0]                   \u2506 [-1.176702, -0.996126, -1.091328\u2026 \u2506 -0.022653          \u2502\n",
-                            "\u2502 \u2026                                 \u2506 \u2026                                 \u2506 \u2026                  \u2502\n",
-                            "\u2502 [-0.993268, -1.003389, -0.993135\u2026 \u2506 [-0.955148, -0.971003, -0.987288\u2026 \u2506 -1.517609          \u2502\n",
-                            "\u2502 [-0.996397, -0.98888, -0.998935]  \u2506 [-0.421874, -1.801489, -0.889335\u2026 \u2506 0.198206           \u2502\n",
-                            "\u2502 [-0.993697, -1.003618, -0.993094\u2026 \u2506 [-1.015508, -1.010919, -1.005117\u2026 \u2506 2.42057            \u2502\n",
-                            "\u2502 [-0.994889, -1.001311, -1.006162\u2026 \u2506 [-0.782951, -1.192956, -0.957612\u2026 \u2506 -1.330491          \u2502\n",
-                            "\u2502 [-0.995584, -0.987763, -0.999201\u2026 \u2506 [-1.075299, -1.604798, -1.420408\u2026 \u2506 -0.640809          \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 rolling_ridge_coef              \u2506 recursive_least_squares_coef    \u2506 expanding_ols_pred \u2502\n",
+                            "\u2502 ---                             \u2506 ---                             \u2506 ---                \u2502\n",
+                            "\u2502 struct[3]                       \u2506 struct[3]                       \u2506 f32                \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 {0.0,0.0,0.0}                   \u2506 {-0.997571,-0.999412,-1.004052} \u2506 0.284141           \u2502\n",
+                            "\u2502 {0.0,0.0,0.0}                   \u2506 {-1.043208,-1.009688,-0.987618} \u2506 0.553695           \u2502\n",
+                            "\u2502 {0.0,0.0,0.0}                   \u2506 {-0.999444,-0.97275,-0.964744}  \u2506 -0.711872          \u2502\n",
+                            "\u2502 {0.0,0.0,0.0}                   \u2506 {-0.938403,-1.031698,-0.967921} \u2506 0.564383           \u2502\n",
+                            "\u2502 {0.0,0.0,0.0}                   \u2506 {-0.900343,-0.9928,-1.033574}   \u2506 0.263497           \u2502\n",
+                            "\u2502 \u2026                               \u2506 \u2026                               \u2506 \u2026                  \u2502\n",
+                            "\u2502 {-1.00591,-1.000234,-1.002072}  \u2506 {-1.004769,-1.006106,-0.981976} \u2506 -0.436183          \u2502\n",
+                            "\u2502 {-0.995429,-0.995031,-0.995304} \u2506 {-0.999747,-0.994992,-0.982279} \u2506 2.078985           \u2502\n",
+                            "\u2502 {-0.995239,-0.995055,-0.995537} \u2506 {-0.997495,-0.99649,-0.982933}  \u2506 0.241709           \u2502\n",
+                            "\u2502 {-1.005733,-0.999528,-1.001679} \u2506 {-1.005132,-1.005992,-0.980991} \u2506 0.505744           \u2502\n",
+                            "\u2502 {-1.006673,-0.995687,-1.013054} \u2506 {-1.015187,-0.9873,-1.038931}   \u2506 1.038495           \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 115,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.select(\n",
                 "    pl.col(\"y\").least_squares.from_formula(\"x1 + x2 + x3 -1\", \n",
@@ -574,16 +641,157 @@
                 "        half_life=21.0, # exponential memory proportional to a half-life of 21 samples\n",
                 "        initial_state_mean=[-1.0, -1.0, -1.0],  # prior mean for initial coefficients\n",
                 "        initial_state_covariance=10.0,  # inversely proportional to L2 prior towards prior mean\n",
                 "        mode=\"coefficients\",\n",
                 "    ).over(\"group\").alias(\"recursive_least_squares_coef\"),\n",
                 "    pl.col(\"y\").least_squares.expanding_ols(pl.col(\"x1\"), pl.col(\"x2\"), pl.col(\"x3\"), \n",
                 "                                           mode=\"predictions\").alias(\"expanding_ols_pred\"),\n",
-                "    \n",
-                ")\n"
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "30fe069d-8f4f-47e7-9f7b-cac7ef750823",
+            "metadata": {},
+            "source": [
+                "### 5. Out Of Sample Prediction\n",
+                "\n",
+                "- If you want to fit on some data then predict on test data, you can do so with `least_squares.predict(...)`"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 21,
+            "id": "ff412921-2c2d-46b3-baad-d54067fa3312",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2024-04-04T13:55:16.975549Z",
+                    "iopub.status.busy": "2024-04-04T13:55:16.974995Z",
+                    "iopub.status.idle": "2024-04-04T13:55:16.992064Z",
+                    "shell.execute_reply": "2024-04-04T13:55:16.990648Z",
+                    "shell.execute_reply.started": "2024-04-04T13:55:16.975516Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>group</th><th>coefficients</th></tr><tr><td>i64</td><td>struct[2]</td></tr></thead><tbody><tr><td>1</td><td>{-1.068436,-1.009836}</td></tr><tr><td>0</td><td>{-0.979399,-1.027145}</td></tr><tr><td>4</td><td>{-0.983794,-0.991228}</td></tr><tr><td>3</td><td>{-0.996063,-0.960127}</td></tr><tr><td>2</td><td>{-0.954715,-1.03776}</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (5, 2)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 group \u2506 coefficients          \u2502\n",
+                            "\u2502 ---   \u2506 ---                   \u2502\n",
+                            "\u2502 i64   \u2506 struct[2]             \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 1     \u2506 {-1.068436,-1.009836} \u2502\n",
+                            "\u2502 0     \u2506 {-0.979399,-1.027145} \u2502\n",
+                            "\u2502 4     \u2506 {-0.983794,-0.991228} \u2502\n",
+                            "\u2502 3     \u2506 {-0.996063,-0.960127} \u2502\n",
+                            "\u2502 2     \u2506 {-0.954715,-1.03776}  \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 21,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# make some random training data\n",
+                "df_train = _make_data(n_groups=1)\n",
+                "\n",
+                "# fit coefficients\n",
+                "df_coefficients = (\n",
+                "    df.lazy()\n",
+                "    .select(\n",
+                "        \"group\",\n",
+                "        pl.col(\"y\")\n",
+                "        .least_squares.ols(pl.col(\"x1\"), pl.col(\"x2\"), mode=\"coefficients\")\n",
+                "        .over(\"group\").alias(\"coefficients\"),\n",
+                "    )\n",
+                "    .unique()\n",
+                ")\n",
+                "\n",
+                "df_coefficients.collect()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 22,
+            "id": "931b667e-cf4d-4b53-be9b-85278c6fd16c",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2024-04-04T13:55:17.194466Z",
+                    "iopub.status.busy": "2024-04-04T13:55:17.193582Z",
+                    "iopub.status.idle": "2024-04-04T13:55:17.210217Z",
+                    "shell.execute_reply": "2024-04-04T13:55:17.209573Z",
+                    "shell.execute_reply.started": "2024-04-04T13:55:17.194402Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>group</th><th>predictions_test</th></tr><tr><td>i64</td><td>f32</td></tr></thead><tbody><tr><td>0</td><td>-2.424038</td></tr><tr><td>0</td><td>0.177278</td></tr><tr><td>0</td><td>-2.637851</td></tr><tr><td>0</td><td>-0.169265</td></tr><tr><td>0</td><td>0.262978</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (5, 2)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 group \u2506 predictions_test \u2502\n",
+                            "\u2502 ---   \u2506 ---              \u2502\n",
+                            "\u2502 i64   \u2506 f32              \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 0     \u2506 -2.424038        \u2502\n",
+                            "\u2502 0     \u2506 0.177278         \u2502\n",
+                            "\u2502 0     \u2506 -2.637851        \u2502\n",
+                            "\u2502 0     \u2506 -0.169265        \u2502\n",
+                            "\u2502 0     \u2506 0.262978         \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 22,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# make some test data\n",
+                "df_test = _make_data(n_groups=1)\n",
+                "\n",
+                "# 1) join on group or common index columns etc.\n",
+                "# 2) compute predictions by calling least_squares.predict(coefficient_column, *feature_columns)\n",
+                "predictions = (\n",
+                "    df_test.lazy()\n",
+                "    .join(df_coefficients, on=\"group\")\n",
+                "    .select(\n",
+                "        \"group\",\n",
+                "        pl.col(\"coefficients\").least_squares.predict(\n",
+                "            pl.col(\"x1\"), pl.col(\"x2\"), name=\"predictions_test\"\n",
+                "        )\n",
+                "    )\n",
+                "    .collect()\n",
+                ")\n",
+                "\n",
+                "predictions.head()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `polars_ols-0.1.1/polars_ols/__init__.py` & `polars_ols-0.2.3/polars_ols/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     OLSKwargs,
     RLSKwargs,
     RollingKwargs,
     compute_least_squares,
     compute_recursive_least_squares,
     compute_rolling_least_squares,
     least_squares_from_formula,
+    predict,
 )
 from polars_ols.utils import build_expressions_from_patsy_formula
 
 __all__ = [
     "compute_least_squares",
     "compute_recursive_least_squares",
     "compute_rolling_least_squares",
@@ -102,7 +103,20 @@
         )
         if kwargs.get("half_life"):
             return self.rls(*features, add_intercept=add_intercept, **kwargs)
         elif kwargs.get("window_size"):
             return self.rolling_ols(*features, add_intercept=add_intercept, **kwargs)
         else:
             return self.least_squares(*features, add_intercept=add_intercept, **kwargs)
+
+    def predict(
+        self, *features: pl.Expr, name: Optional[str] = None, add_intercept: bool = False
+    ) -> pl.Expr:
+        return predict(self._expr, *features, name=name, add_intercept=add_intercept)
+
+    def predict_from_formula(self, formula: str, name: Optional[str] = None) -> pl.Expr:
+        features, add_intercept = build_expressions_from_patsy_formula(
+            formula, include_dependent_variable=False
+        )
+        has_const = any(f.meta.output_name == "const" for f in features)
+        add_intercept &= not has_const
+        return self.predict(*features, add_intercept=add_intercept, name=name)
```

### Comparing `polars_ols-0.1.1/polars_ols/least_squares.py` & `polars_ols-0.2.3/polars_ols/least_squares.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import logging
 from dataclasses import asdict, dataclass
 from functools import partial
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional
 
 import polars as pl
 from polars.plugins import register_plugin_function
 from polars.type_aliases import IntoExpr
 
 from polars_ols.utils import build_expressions_from_patsy_formula, parse_into_expr
 
+logger = logging.getLogger(__name__)
+
 __all__ = [
     "compute_least_squares",
     "compute_recursive_least_squares",
     "compute_rolling_least_squares",
     "least_squares_from_formula",
+    "predict",
     "OLSKwargs",
     "RLSKwargs",
     "RollingKwargs",
 ]
 
 
 @dataclass
@@ -83,15 +87,18 @@
 
     Returns:
         Tuple containing the pre-processed target, features, and sample weights.
     """
     target = parse_into_expr(target).cast(pl.Float32)
     features = [f.cast(pl.Float32) for f in features]
     if add_intercept:
-        features += [target.mul(0.0).add(1.0).alias("intercept")]
+        if any(f.meta.output_name == "const" for f in features):
+            logger.info("feature named 'const' already detected, assuming it is an intercept")
+        else:
+            features += [target.mul(0.0).add(1.0).alias("const")]
     sqrt_w = 1.0
     if sample_weights is not None:
         sqrt_w = sample_weights.cast(pl.Float32).sqrt()
         target *= sqrt_w
         features = [expr * sqrt_w for expr in features]
     return target, features, sqrt_w
 
@@ -141,21 +148,26 @@
         target, *features, sample_weights=sample_weights, add_intercept=add_intercept
     )
 
     ols_kwargs: OLSKwargs = ols_kwargs or OLSKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
-        return register_plugin_function(
-            plugin_path=Path(__file__).parent,
-            function_name="least_squares_coefficients",
-            args=[target, *features],
-            kwargs=ols_kwargs.to_dict(),
-            is_elementwise=False,
-            changes_length=True,
+        return (
+            register_plugin_function(
+                plugin_path=Path(__file__).parent,
+                function_name="least_squares_coefficients",
+                args=[target, *features],
+                kwargs=ols_kwargs.to_dict(),
+                is_elementwise=False,
+                changes_length=True,
+                returns_scalar=True,
+            )
+            .alias("coefficients")
+            .struct.rename_fields([f.meta.output_name() for f in features])
         )
     else:
         predictions = (
             register_plugin_function(
                 plugin_path=Path(__file__).parent,
                 function_name="least_squares",
                 args=[target, *features],
@@ -163,57 +175,15 @@
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
-            return (target - predictions).alias("residuals")
-
-
-def least_squares_from_formula(
-    formula: str,
-    sample_weights: Optional[pl.Expr] = None,
-    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
-    **kwargs,
-) -> pl.Expr:
-    """Performs least squares regression using a formula.
-
-    Depending on choice of additional kwargs dispatches either rolling, recursive,
-    on static least squares compute functions.
-
-    Args:
-        formula: Patsy-style formula string.
-        **kwargs: Additional keyword arguments for the least squares function.
-
-    Returns:
-        Resulting expression based on the formula.
-    """
-    expressions, add_intercept = build_expressions_from_patsy_formula(
-        formula, include_dependent_variable=True
-    )
-
-    # resolve additional kwargs and relevant ols compute function
-    if kwargs.get("half_life"):
-        rls_kwargs: RLSKwargs = RLSKwargs(**kwargs)
-        func = partial(compute_recursive_least_squares, rls_kwargs=rls_kwargs)
-    elif kwargs.get("window_size"):
-        rolling_kwargs: RollingKwargs = RollingKwargs(**kwargs)
-        func = partial(compute_rolling_least_squares, rolling_kwargs=rolling_kwargs)
-    else:
-        ols_kwargs: OLSKwargs = OLSKwargs(**kwargs)
-        func = partial(compute_least_squares, ols_kwargs=ols_kwargs)
-
-    return func(
-        expressions[0],
-        *expressions[1:],
-        add_intercept=add_intercept,
-        sample_weights=sample_weights,
-        mode=mode,
-    )
+            return target - predictions
 
 
 def compute_recursive_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
@@ -256,21 +226,24 @@
     target, features, sqrt_w = _pre_process_data(
         target, *features, sample_weights=sample_weights, add_intercept=add_intercept
     )
     rls_kwargs: RLSKwargs = rls_kwargs or RLSKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
-        return register_plugin_function(
-            plugin_path=Path(__file__).parent,
-            function_name="recursive_least_squares_coefficients",
-            args=[target, *features],
-            kwargs=rls_kwargs.to_dict(),
-            is_elementwise=False,
-            changes_length=True,
+        return (
+            register_plugin_function(
+                plugin_path=Path(__file__).parent,
+                function_name="recursive_least_squares_coefficients",
+                args=[target, *features],
+                kwargs=rls_kwargs.to_dict(),
+                is_elementwise=False,
+            )
+            .alias("coefficients")
+            .struct.rename_fields([f.meta.output_name() for f in features])
         )
     else:
         predictions = (
             register_plugin_function(
                 plugin_path=Path(__file__).parent,
                 function_name="recursive_least_squares",
                 args=[target, *features],
@@ -278,15 +251,15 @@
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
-            return (target - predictions).alias("residuals")
+            return target - predictions
 
 
 def compute_rolling_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
@@ -320,21 +293,24 @@
     target, features, sqrt_w = _pre_process_data(
         target, *features, sample_weights=sample_weights, add_intercept=add_intercept
     )
     rolling_kwargs: RollingKwargs = rolling_kwargs or RollingKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
-        return register_plugin_function(
-            plugin_path=Path(__file__).parent,
-            function_name="rolling_least_squares_coefficients",
-            args=[target, *features],
-            kwargs=rolling_kwargs.to_dict(),
-            is_elementwise=False,
-            changes_length=True,
+        return (
+            register_plugin_function(
+                plugin_path=Path(__file__).parent,
+                function_name="rolling_least_squares_coefficients",
+                args=[target, *features],
+                kwargs=rolling_kwargs.to_dict(),
+                is_elementwise=False,
+            )
+            .alias("coefficients")
+            .struct.rename_fields([f.meta.output_name() for f in features])
         )
     else:
         predictions = (
             register_plugin_function(
                 plugin_path=Path(__file__).parent,
                 function_name="rolling_least_squares",
                 args=[target, *features],
@@ -342,8 +318,80 @@
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
-            return (target - predictions).alias("residuals")
+            return target - predictions
+
+
+def least_squares_from_formula(
+    formula: str,
+    sample_weights: Optional[pl.Expr] = None,
+    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+    **kwargs,
+) -> pl.Expr:
+    """Performs least squares regression using a formula.
+
+    Depending on choice of additional kwargs dispatches either rolling, recursive,
+    on static least squares compute functions.
+
+    Args:
+        formula: Patsy-style formula string.
+        **kwargs: Additional keyword arguments for the least squares function.
+
+    Returns:
+        Resulting expression based on the formula.
+    """
+    expressions, add_intercept = build_expressions_from_patsy_formula(
+        formula, include_dependent_variable=True
+    )
+
+    # resolve additional kwargs and relevant ols compute function
+    if kwargs.get("half_life"):
+        rls_kwargs: RLSKwargs = RLSKwargs(**kwargs)
+        func = partial(compute_recursive_least_squares, rls_kwargs=rls_kwargs)
+    elif kwargs.get("window_size"):
+        rolling_kwargs: RollingKwargs = RollingKwargs(**kwargs)
+        func = partial(compute_rolling_least_squares, rolling_kwargs=rolling_kwargs)
+    else:
+        ols_kwargs: OLSKwargs = OLSKwargs(**kwargs)
+        func = partial(compute_least_squares, ols_kwargs=ols_kwargs)
+
+    return func(
+        expressions[0],
+        *expressions[1:],
+        add_intercept=add_intercept,
+        sample_weights=sample_weights,
+        mode=mode,
+    )
+
+
+def predict(
+    coefficients: IntoExpr,
+    *features: pl.Expr,
+    name: Optional[str] = None,
+    add_intercept: bool = False,
+) -> pl.Expr:
+    """Helper which computes predictions as a product of (aligned) coefficients with features.
+
+    Args:
+        coefficients: Polars expression returning a coefficients struct.
+        *features: variable number of feature expressions.
+        add_intercept: boolean indicating if a constant should be added to features.
+
+    Returns:
+        polars expression denoting computed predictions.
+    """
+    if add_intercept:
+        if any(f.meta.output_name == "const" for f in features):
+            logger.warning("feature named 'const' already detected, assuming it is the intercept")
+        else:
+            features += (features[-1].mul(0.0).add(1.0).alias("const"),)
+
+    return register_plugin_function(
+        plugin_path=Path(__file__).parent,
+        function_name="predict",
+        args=[coefficients, *(f.cast(pl.Float32) for f in features)],
+        is_elementwise=False,
+    ).alias(name or "predictions")
```

### Comparing `polars_ols-0.1.1/polars_ols/utils.py` & `polars_ols-0.2.3/polars_ols/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.1/src/expressions.rs` & `polars_ols-0.2.3/src/expressions.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,144 @@
 #![allow(clippy::unit_arg, clippy::unused_unit)]
-use crate::least_squares::{
-    solve_elastic_net, solve_ols_qr, solve_recursive_least_squares, solve_ridge, solve_rolling_ols,
-};
+
 use ndarray::{Array, Array1, Array2, Axis};
 use polars::datatypes::{DataType, Field, Float32Type};
 use polars::error::{polars_err, PolarsResult};
-use polars::prelude::{
-    IntoSeries, ListBuilderTrait, ListPrimitiveChunkedBuilder, NamedFromOwned, Series,
-};
+use polars::frame::DataFrame;
+use polars::prelude::{IndexOrder, IntoSeries, NamedFromOwned, Series};
 use pyo3_polars::derive::polars_expr;
 use serde::Deserialize;
 
-/// Convert a slice of polars series into target & feature ndarray objects.
-pub fn convert_polars_to_ndarray(inputs: &[Series]) -> (Array1<f32>, Array2<f32>) {
+use crate::least_squares::{
+    solve_elastic_net, solve_ols_qr, solve_recursive_least_squares, solve_ridge, solve_rolling_ols,
+};
+
+/// convert a slice of polars series into a 2D feature array.
+fn construct_features_array(inputs: &[Series]) -> Array2<f32> {
     let m = inputs.len();
     let n = inputs[0].len();
+    // Prepare features ndarray
+    let mut x: Array<f32, _> = Array::zeros((n, m));
+    x.axis_iter_mut(Axis(1))
+        .enumerate()
+        .for_each(|(j, mut col)| {
+            // Convert Series to ndarray
+            let s = inputs[j]
+                .f32()
+                .expect("Failed to convert polars series to f32 array")
+                .to_ndarray()
+                .expect("Failed to convert f32 series to ndarray");
+            col.assign(&s);
+        });
+    x
+}
 
+/// Convert a slice of polars series into target & feature ndarray objects.
+pub fn convert_polars_to_ndarray(inputs: &[Series]) -> (Array1<f32>, Array2<f32>) {
+    let m = inputs.len();
     assert!(m > 1, "must pass at least 2 series");
 
     // prepare targets & features ndarrays. assume first series is targets and rest are features.
     let y = inputs[0]
         .f32()
         .expect("Failed to convert polars series to f32 array")
         .to_ndarray()
         .expect("Failed to convert f32 series to ndarray")
         .to_owned();
 
     // note that this was faster than converting polars series -> polars dataframe -> to_ndarray
-    let mut x: Array<f32, _> = Array::zeros((n, m - 1));
-    x.axis_iter_mut(Axis(1))
-        .enumerate()
-        .for_each(|(j, mut col)| {
-            // Convert Series to ndarray
-            let s = inputs[j + 1]
-                .f32()
-                .expect("Failed to convert polars series to f32 array")
-                .to_ndarray()
-                .expect("Failed to convert f32 series to ndarray");
-            col.assign(&s);
-        });
+    // assume first series is targets and rest are features.
+    let x = construct_features_array(&inputs[1..]);
+    assert_eq!(
+        x.len_of(Axis(0)),
+        y.len(),
+        "all input series passed must be of equal length"
+    );
+
     (y, x)
 }
 
+fn coefficients_struct_dtype(input_fields: &[Field]) -> PolarsResult<Field> {
+    // the first input field denotes the target, which we need not carry in output struct
+    Ok(Field::new(
+        "coefficients",
+        DataType::Struct(input_fields[1..].to_vec()),
+    ))
+}
+
+/// Convert the coefficients into a Polars series of struct dtype.
+fn coefficients_to_struct_series(coefficients: &Array2<f32>) -> Series {
+    // Convert 2D ndarray into DataFrame
+    let df: DataFrame = DataFrame::new(
+        coefficients
+            .axis_iter(Axis(1))
+            .enumerate()
+            .map(|(i, col)| Series::from_vec(&i.to_string(), col.to_vec()))
+            .collect::<Vec<Series>>(),
+    )
+    .unwrap();
+    // Convert DataFrame to a Series of struct dtype
+    df.into_struct("coefficients").into_series()
+}
+
+// fn list_float_dtype(input_fields: &[Field]) -> PolarsResult<Field> {
+//     let field = Field::new(
+//         input_fields[0].name(),
+//         DataType::List(Box::new(DataType::Float32)),
+//     );
+//     Ok(field.clone())
+// }
+// fn coefficients_to_series_list(coefficients: &Array2<f32>) -> Series {
+//     // convert 2d ndarray into Series of List[f32]
+//     let mut chunked_builder = ListPrimitiveChunkedBuilder::<Float32Type>::new(
+//         "",
+//         coefficients.len_of(Axis(0)),
+//         coefficients.len_of(Axis(1)),
+//         DataType::Float32,
+//     );
+//     for row in coefficients.axis_iter(Axis(0)) {
+//         match row.as_slice() {
+//             Some(row) => chunked_builder.append_slice(row),
+//             None => chunked_builder.append_slice(&row.to_vec()),
+//         }
+//     }
+//     chunked_builder.finish().into_series()
+// }
+
+/// Computes linear predictions and returns a polars series.
+fn make_predictions(features: &Array2<f32>, coefficients: Array1<f32>, name: &str) -> Series {
+    Series::from_vec(name, features.dot(&coefficients).to_vec())
+}
+
+fn convert_option_vec_to_array1(opt_vec: Option<Vec<f32>>) -> Option<Array1<f32>> {
+    opt_vec.map(Array1::from)
+}
+
 #[derive(Deserialize)]
 pub struct OLSKwargs {
     alpha: Option<f32>,
     l1_ratio: Option<f32>,
     max_iter: Option<usize>,
     tol: Option<f32>,
     positive: Option<bool>,
 }
 
-/// Computes linear predictions and returns a polars series.
-fn make_predictions(features: &Array2<f32>, coefficients: Array1<f32>, name: &str) -> Series {
-    Series::from_vec(name, features.dot(&coefficients).to_vec())
+#[derive(Deserialize)]
+pub struct RLSKwargs {
+    half_life: Option<f32>,
+    initial_state_covariance: Option<f32>,
+    initial_state_mean: Option<Vec<f32>>, // in python list[f32] | None is equivalent
+}
+
+#[derive(Deserialize)]
+pub struct RollingKwargs {
+    window_size: usize,
+    min_periods: Option<usize>,
+    use_woodbury: Option<bool>,
+    alpha: Option<f32>,
 }
 
 fn _get_least_squares_coefficients(
     targets: &Array1<f32>,
     features: &Array2<f32>,
     kwargs: OLSKwargs,
 ) -> Array1<f32> {
@@ -76,82 +157,47 @@
             kwargs.max_iter,
             kwargs.tol,
             kwargs.positive,
         )
     }
 }
 
-#[polars_expr(output_type = Float32)]
+#[polars_expr(output_type=Float32)]
 fn least_squares(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let coefficients = _get_least_squares_coefficients(&y, &x, kwargs);
     Ok(make_predictions(&x, coefficients, inputs[0].name()))
 }
 
-#[polars_expr(output_type = Float32)]
+#[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn least_squares_coefficients(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
-    Ok(Series::from_vec(
-        "coefficients",
-        _get_least_squares_coefficients(&y, &x, kwargs).to_vec(),
-    ))
-}
-
-fn list_float_dtype(input_fields: &[Field]) -> PolarsResult<Field> {
-    let field = Field::new(
-        input_fields[0].name(),
-        DataType::List(Box::new(DataType::Float32)),
-    );
-    Ok(field.clone())
-}
-
-#[derive(Deserialize)]
-pub struct RLSKwargs {
-    half_life: Option<f32>,
-    initial_state_covariance: Option<f32>,
-    initial_state_mean: Option<Vec<f32>>, // in python list[f32] | None is equivalent
-}
-
-fn convert_option_vec_to_array1(opt_vec: Option<Vec<f32>>) -> Option<Array1<f32>> {
-    opt_vec.map(Array1::from)
-}
-
-fn coefficients_to_series(coefficients: &Array2<f32>) -> Series {
-    // convert 2d ndarray into Series of List[f32]
-    let mut chunked_builder = ListPrimitiveChunkedBuilder::<Float32Type>::new(
-        "",
-        coefficients.len_of(Axis(0)),
-        coefficients.len_of(Axis(1)),
-        DataType::Float32,
-    );
-    for row in coefficients.axis_iter(Axis(0)) {
-        match row.as_slice() {
-            Some(row) => chunked_builder.append_slice(row),
-            None => chunked_builder.append_slice(&row.to_vec()),
-        }
-    }
-    chunked_builder.finish().into_series()
+    // force into 1 x K 2-d array, so that we can return a series of struct
+    let coefficients = _get_least_squares_coefficients(&y, &x, kwargs).insert_axis(Axis(0));
+    // let series = coefficients_to_series_list(&coefficients);
+    let series = coefficients_to_struct_series(&coefficients);
+    Ok(series.with_name("coefficients"))
 }
 
-#[polars_expr(output_type_func=list_float_dtype)]
+#[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn recursive_least_squares_coefficients(
     inputs: &[Series],
     kwargs: RLSKwargs,
 ) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let initial_state_mean = convert_option_vec_to_array1(kwargs.initial_state_mean);
     let coefficients = solve_recursive_least_squares(
         &y,
         &x,
         kwargs.half_life,
         kwargs.initial_state_covariance,
         initial_state_mean,
     );
-
-    let series = coefficients_to_series(&coefficients);
+    // let series = coefficients_to_series_list(&coefficients);
+    let series = coefficients_to_struct_series(&coefficients);
     Ok(series.with_name("coefficients"))
 }
 
 #[polars_expr(output_type=Float32)]
 fn recursive_least_squares(inputs: &[Series], kwargs: RLSKwargs) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let coefficients = solve_recursive_least_squares(
@@ -161,37 +207,30 @@
         kwargs.initial_state_covariance,
         None,
     );
     let predictions = (&x * &coefficients).sum_axis(Axis(1));
     Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
 }
 
-#[derive(Deserialize)]
-pub struct RollingKwargs {
-    window_size: usize,
-    min_periods: Option<usize>,
-    use_woodbury: Option<bool>,
-    alpha: Option<f32>,
-}
-
-#[polars_expr(output_type_func=list_float_dtype)]
+#[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn rolling_least_squares_coefficients(
     inputs: &[Series],
     kwargs: RollingKwargs,
 ) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let coefficients = solve_rolling_ols(
         &y,
         &x,
         kwargs.window_size,
         kwargs.min_periods,
         kwargs.use_woodbury,
         kwargs.alpha,
     );
-    let series = coefficients_to_series(&coefficients);
+    // let series = coefficients_to_series_list(&coefficients);
+    let series = coefficients_to_struct_series(&coefficients);
     Ok(series.with_name("coefficients"))
 }
 
 #[polars_expr(output_type=Float32)]
 fn rolling_least_squares(inputs: &[Series], kwargs: RollingKwargs) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let coefficients = solve_rolling_ols(
@@ -201,7 +240,27 @@
         kwargs.min_periods,
         kwargs.use_woodbury,
         kwargs.alpha,
     );
     let predictions = (&x * &coefficients).sum_axis(Axis(1));
     Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
 }
+
+/// This function provides a convenience expression to multiply fitted coefficients with features,
+/// which may be particularly useful in case predicting on test data
+/// (otherwise use direct prediction functions).
+#[polars_expr(output_type=Float32)]
+fn predict(inputs: &[Series]) -> PolarsResult<Series> {
+    // The first input is always assumed to be the coefficient struct, and the remaining
+    // input series are assumed to be an equivalent number of features.
+    let coefficients_df: DataFrame = inputs[0]
+        .struct_()
+        .expect("the first input series to predict function must be of dtype struct!")
+        .clone()
+        .unnest();
+    let features = construct_features_array(&inputs[1..]);
+    let coefficients: Array2<f32> = coefficients_df
+        .to_ndarray::<Float32Type>(IndexOrder::C)
+        .unwrap();
+    let predictions = (&features * &coefficients).sum_axis(Axis(1));
+    Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
+}
```

### Comparing `polars_ols-0.1.1/src/least_squares.rs` & `polars_ols-0.2.3/src/least_squares.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.1/src/lib.rs` & `polars_ols-0.2.3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,22 @@
         assert_close_l2!(&coefficients.slice(s![-1, ..]), &expected, 0.0001);
     }
 
     #[test]
     fn test_rolling_least_squares() {
         let (y, x1, x2) = make_data();
         let (targets, features) = convert_polars_to_ndarray(&[y.clone(), x1, x2]);
-        let coefficients =
-            solve_rolling_ols(&targets, &features, 1_000usize, Some(100usize),
-                              Some(true), None);
+        let coefficients = solve_rolling_ols(
+            &targets,
+            &features,
+            1_000usize,
+            Some(100usize),
+            Some(true),
+            None,
+        );
         let expected: Array1<f32> = array![1.0, 1.0];
         println!("{:?}", coefficients.slice(s![0, ..]));
         println!("{:?}", coefficients.slice(s![-1, ..]));
         assert_close_l2!(&coefficients.slice(s![-1, ..]), &expected, 0.0001);
     }
 
     #[test]
```

### Comparing `polars_ols-0.1.1/tests/benchmark.py` & `polars_ols-0.2.3/tests/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     ).fit(params_only=True)
     return data.lazy().with_columns(predictions=pl.lit((res.params * x).sum(1))).collect()
 
 
 if __name__ == "__main__":
     # example: python tests/benchmark.py --quiet --fast
     # we run the benchmarks in python (as opposed to rust) so that overhead of pyO3 is included
-    df = _make_data(n_features=100, n_samples=10_000)
+    df = _make_data(n_features=10, n_samples=2_000)
     runner = pyperf.Runner()
     runner.bench_func("benchmark_least_squares", benchmark_least_squares, df)
     runner.bench_func("benchmark_ridge", benchmark_ridge, df)
     runner.bench_func("benchmark_wls_from_formula", benchmark_wls_from_formula, df)
     runner.bench_func("benchmark_elastic_net", benchmark_elastic_net, df)
     runner.bench_func("benchmark_recursive_least_squares", benchmark_recursive_least_squares, df)
     runner.bench_func("benchmark_rolling_least_squares", benchmark_rolling_least_squares, df)
```

### Comparing `polars_ols-0.1.1/Cargo.lock` & `polars_ols-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1586,15 +1586,15 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ols"
-version = "0.1.1"
+version = "0.2.3"
 dependencies = [
  "approx",
  "faer",
  "faer-ext",
  "jemallocator",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `polars_ols-0.1.1/pyproject.toml` & `polars_ols-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0", "polars>=0.20.6"]
 build-backend = "maturin"
 
 [project]
 name = "polars-ols"
+description = "Polars Least Squares Extension"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
   {name = "Azmy Rajab", email = "azmy.rajab@gmail.com"}
 ]
 dependencies = [
-  "polars >= 0.19.0",
+  "polars >= 0.20.6",
 ]
 keywords = ["polars-extension", "linear-regression"]
+readme = "README.md"
+license = { file = "LICENSE" }
+
 
 [tool.maturin]
 module-name = "polars_ols._polars_ols"
 
 [project.optional-dependencies]
 dev = [
   "numpy",
@@ -75,15 +79,15 @@
   "F403",
   "F401",
   "ISC001",
 ]
 lint.pylint.max-args = 6
 
 [tool.black]
-target-version = ["py310", "py311"]
+target-version = ["py38", "py39", "py310", "py311"]
 line-length = 100
 include = '\.pyi?$' # All Python files
 exclude = '''
 (
     asv_bench/env
   | \.egg
   | \.git
```

### Comparing `polars_ols-0.1.1/PKG-INFO` & `polars_ols-0.2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.3
-Name: polars-ols
-Version: 0.1.1
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: polars >=0.19.0
-Requires-Dist: numpy ; extra == 'dev'
-Requires-Dist: pytest >=7.4.1 ; extra == 'dev'
-Requires-Dist: pre-commit ; extra == 'dev'
-Requires-Dist: statsmodels ; extra == 'dev'
-Provides-Extra: dev
-License-File: LICENSE
-Keywords: polars-extension,linear-regression
-Author-email: Azmy Rajab <azmy.rajab@gmail.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 # Polars OLS
 ## Least squares extension in Polars
 
 Supports linear model estimation in [Polars](https://www.pola.rs/).
 
 This package provides efficient rust implementations of common linear
 regression variants (OLS, WLS, Ridge, Elastic Net, Non-negative least squares, Recursive least squares) and exposes
@@ -93,34 +75,80 @@
 │ 0.22  ┆ -0.07 ┆ 0.44  ┆ 1     ┆ 0.57    ┆ 0.37              ┆ 0.36            │
 └───────┴───────┴───────┴───────┴─────────┴───────────────────┴─────────────────┘
 ```
 
 The `mode` parameter is used to set the type of the output returned by all methods (`"predictions", "residuals", "coefficients"`).
 It defaults to returning predictions matching the input's length.
 
-In case `"coefficients"` is set the output's shape is the number of features specified, see below:
+In case `"coefficients"` is set the output is a [polars Struct](https://docs.pola.rs/user-guide/expressions/structs/) with coefficients as values and feature names as fields.
+It's output shape 'broadcasts' depending on context, see below:
 
 ```python
 coefficients = df.select(pl.col("y").least_squares.from_formula("x1 + x2", mode="coefficients")
-                         .alias("coefficients").round(2))
+                         .alias("coefficients"))
+
+coefficients_group = df.select("group", pl.col("y").least_squares.from_formula("x1 + x2", mode="coefficients").over("group")
+                        .alias("coefficients_group")).unique(maintain_order=True)
+
 print(coefficients)
+print(coefficients_group)
+```
+```
+shape: (1, 1)
+┌──────────────────────────────┐
+│ coefficients                 │
+│ ---                          │
+│ struct[3]                    │
+╞══════════════════════════════╡
+│ {0.977375,0.987413,0.000757} │  # <--- coef for x1, x2, and intercept added by formula API
+└──────────────────────────────┘
+shape: (2, 2)
+┌───────┬───────────────────────────────┐
+│ group ┆ coefficients_group            │
+│ ---   ┆ ---                           │
+│ i64   ┆ struct[3]                     │
+╞═══════╪═══════════════════════════════╡
+│ 1     ┆ {0.995157,0.977495,0.014344}  │
+│ 2     ┆ {0.939217,0.997441,-0.017599} │  # <--- (unique) coefficients per group
+└───────┴───────────────────────────────┘
+```
+
+For dynamic models (like `rolling_ols`) or if in a `.over`, `.group_by`, or `.with_columns` context, the
+coefficients will take the shape of the data it is applied on. For example:
+
+```python
+coefficients = df.with_columns(pl.col("y").least_squares.rls(pl.col("x1"), pl.col("x2"), mode="coefficients")
+                         .over("group").alias("coefficients"))
+
+print(coefficients.head())
 ```
 ```
-shape: (3, 1)
-┌──────────────┐
-│ coefficients │
-│ ---          │
-│ f32          │
-╞══════════════╡
-│ 0.98         │ <-- x1
-│ 0.99         │ <-- x2
-│ 0.0          │ <-- intercept added by formula api
-└──────────────┘
+shape: (5, 6)
+┌───────┬───────┬───────┬───────┬─────────┬─────────────────────┐
+│ y     ┆ x1    ┆ x2    ┆ group ┆ weights ┆ coefficients        │
+│ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---     ┆ ---                 │
+│ f64   ┆ f64   ┆ f64   ┆ i64   ┆ f64     ┆ struct[2]           │
+╞═══════╪═══════╪═══════╪═══════╪═════════╪═════════════════════╡
+│ 1.16  ┆ 0.72  ┆ 0.24  ┆ 1     ┆ 0.34    ┆ {1.235503,0.411834} │
+│ -2.16 ┆ -2.43 ┆ 0.18  ┆ 1     ┆ 0.97    ┆ {0.963515,0.760769} │
+│ -1.57 ┆ -0.63 ┆ -0.95 ┆ 1     ┆ 0.39    ┆ {0.975484,0.966029} │
+│ 0.21  ┆ 0.05  ┆ 0.23  ┆ 1     ┆ 0.8     ┆ {0.975657,0.953735} │
+│ 0.22  ┆ -0.07 ┆ 0.44  ┆ 1     ┆ 0.57    ┆ {0.97898,0.909793}  │
+└───────┴───────┴───────┴───────┴─────────┴─────────────────────┘
+```
+
+Finally, for convenience, in order to compute out-of-sample predictions you can use:
+```least_squares.{predict, predict_from_formula}```. This saves you the effort of un-nesting the coefficients and doing the dot product in
+python and instead does this in Rust, as an expression. Usage is as follows:
+
+```python
+df_test.select(pl.col("coefficients_train").least_squares.predict(pl.col("x1"), pl.col("x2")).alias("predictions_test"))
 ```
 
+
 Supported Models
 ------------
 
 Currently, this extension package supports the following variants:
 - Ordinary Least Squares: ```least_squares.ols```
 - Weighted Least Squares: ```least_squares.wls```
 - Regularized Least Squares (Lasso / Ridge / Elastic Net) ```least_squares.{lasso, ridge, elastic_net}```
@@ -164,7 +192,23 @@
 | Recursive Least Squares | 163 ms ± 28 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 24.5x                        |
 | Rolling Least Squares   | 390 ms ± 10 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 10.2x                        |
 
 Numpy's `lstsq` is already a highly optimized call into LAPACK and so the scope for speed-up is limited.
 However, we can achieve substantial speed-ups for the more complex models by working entirely in rust
 and avoiding overhead from back and forth into python.
 
+Expect an additional relative order-of-magnitude speed up to your workflow if it involved repeated re-estimation of models in
+(python) loops.
+
+
+Credits & Related Projects
+------------
+- Rust linear algebra libraries [faer](https://faer-rs.github.io/getting-started.html) and [ndarray](https://docs.rs/ndarray/latest/ndarray/) support the implementations provided by this extension package
+- This package was templated around the very helpful: [polars-plugin-tutorial](https://marcogorelli.github.io/polars-plugins-tutorial/)
+- The python package [patsy](https://patsy.readthedocs.io/en/latest/formulas.html) is used for (optionally) building models from formulae
+- Please check out the extension package [polars-ds](https://github.com/abstractqqq/polars_ds_extension) for general data-science functionality in polars
+
+Future Work / TODOs
+------------
+- Support generic types, in rust implementations, so that both f32 and f64 types are recognized. Right now data is cast to f32 prior to estimation
+- Handle nulls more clearly
+- Add more detailed documentation on supported models, signatures, and API
```

