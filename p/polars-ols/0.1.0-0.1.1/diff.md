# Comparing `tmp/polars_ols-0.1.0.tar.gz` & `tmp/polars_ols-0.1.1.tar.gz`

## Comparing `polars_ols-0.1.0.tar` & `polars_ols-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 polars_ols-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127      116 2024-03-25 10:26:40.000000 polars_ols-0.1.0/.cargo/config.toml
--rw-r--r--   0     1001      127     3303 2024-03-25 10:26:40.000000 polars_ols-0.1.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      163 2024-03-25 10:26:40.000000 polars_ols-0.1.0/.gitignore
--rw-r--r--   0     1001      127      912 2024-03-25 10:26:40.000000 polars_ols-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1067 2024-03-25 10:26:40.000000 polars_ols-0.1.0/LICENSE
--rw-r--r--   0     1001      127      671 2024-03-25 10:26:40.000000 polars_ols-0.1.0/Makefile
--rw-r--r--   0     1001      127     9027 2024-03-25 10:26:40.000000 polars_ols-0.1.0/README.md
--rw-r--r--   0     1001      127     2022 2024-03-25 10:26:40.000000 polars_ols-0.1.0/polars_ols/__init__.py
--rw-r--r--   0     1001      127     8807 2024-03-25 10:26:40.000000 polars_ols-0.1.0/polars_ols/least_squares.py
--rw-r--r--   0     1001      127     3464 2024-03-25 10:26:40.000000 polars_ols-0.1.0/polars_ols/utils.py
--rw-r--r--   0     1001      127       63 2024-03-25 10:26:40.000000 polars_ols-0.1.0/requirements.txt
--rw-r--r--   0     1001      127     5366 2024-03-25 10:26:40.000000 polars_ols-0.1.0/src/expressions.rs
--rw-r--r--   0     1001      127    14577 2024-03-25 10:26:40.000000 polars_ols-0.1.0/src/least_squares.rs
--rw-r--r--   0     1001      127     4123 2024-03-25 10:26:40.000000 polars_ols-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-03-25 10:26:40.000000 polars_ols-0.1.0/tests/__init__.py
--rw-r--r--   0     1001      127     4514 2024-03-25 10:26:40.000000 polars_ols-0.1.0/tests/benchmark.py
--rw-r--r--   0     1001      127       87 2024-03-25 10:26:40.000000 polars_ols-0.1.0/tests/requirements-test.txt
--rw-r--r--   0     1001      127     9619 2024-03-25 10:26:40.000000 polars_ols-0.1.0/tests/test_ols.py
--rw-r--r--   0     1001      127    62068 2024-03-25 10:26:40.000000 polars_ols-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127     1748 2024-03-25 10:26:40.000000 polars_ols-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9694 1970-01-01 00:00:00.000000 polars_ols-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 polars_ols-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127      116 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.cargo/config.toml
+-rw-r--r--   0     1001      127     3303 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      139 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.gitignore
+-rw-r--r--   0     1001      127      912 2024-03-31 17:16:04.000000 polars_ols-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1067 2024-03-31 17:16:04.000000 polars_ols-0.1.1/LICENSE
+-rw-r--r--   0     1001      127      671 2024-03-31 17:16:04.000000 polars_ols-0.1.1/Makefile
+-rw-r--r--   0     1001      127     9347 2024-03-31 17:16:04.000000 polars_ols-0.1.1/README.md
+-rw-r--r--   0     1001      127    35269 2024-03-31 17:16:04.000000 polars_ols-0.1.1/notebooks/polars_ols_demo.ipynb
+-rw-r--r--   0     1001      127     3685 2024-03-31 17:16:04.000000 polars_ols-0.1.1/polars_ols/__init__.py
+-rw-r--r--   0     1001      127    13458 2024-03-31 17:16:04.000000 polars_ols-0.1.1/polars_ols/least_squares.py
+-rw-r--r--   0     1001      127     3464 2024-03-31 17:16:04.000000 polars_ols-0.1.1/polars_ols/utils.py
+-rw-r--r--   0     1001      127       63 2024-03-31 17:16:04.000000 polars_ols-0.1.1/requirements.txt
+-rw-r--r--   0     1001      127     6650 2024-03-31 17:16:04.000000 polars_ols-0.1.1/src/expressions.rs
+-rw-r--r--   0     1001      127    16506 2024-03-31 17:16:04.000000 polars_ols-0.1.1/src/least_squares.rs
+-rw-r--r--   0     1001      127     5290 2024-03-31 17:16:04.000000 polars_ols-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/__init__.py
+-rw-r--r--   0     1001      127     6259 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/benchmark.py
+-rw-r--r--   0     1001      127       87 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/requirements-test.txt
+-rw-r--r--   0     1001      127    10690 2024-03-31 17:16:04.000000 polars_ols-0.1.1/tests/test_ols.py
+-rw-r--r--   0     1001      127    61832 2024-03-31 17:16:04.000000 polars_ols-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127     1748 2024-03-31 17:16:04.000000 polars_ols-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10014 1970-01-01 00:00:00.000000 polars_ols-0.1.1/PKG-INFO
```

### Comparing `polars_ols-0.1.0/Cargo.toml` & `polars_ols-0.1.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_ols"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 
 [lib]
 name = "polars_ols"
 crate-type= ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ols-0.1.0/.github/workflows/publish_to_pypi.yml` & `polars_ols-0.1.1/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.0/.pre-commit-config.yaml` & `polars_ols-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.0/LICENSE` & `polars_ols-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.0/Makefile` & `polars_ols-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.0/polars_ols/least_squares.py` & `polars_ols-0.1.1/polars_ols/least_squares.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,76 @@
+from dataclasses import asdict, dataclass
+from functools import partial
 from pathlib import Path
-from typing import Literal, Optional
+from typing import Any, Dict, List, Literal, Optional
 
 import polars as pl
 from polars.plugins import register_plugin_function
 from polars.type_aliases import IntoExpr
 
 from polars_ols.utils import build_expressions_from_patsy_formula, parse_into_expr
 
-__all__ = ["least_squares", "least_squares_from_formula", "recursive_least_squares"]
+__all__ = [
+    "compute_least_squares",
+    "compute_recursive_least_squares",
+    "compute_rolling_least_squares",
+    "least_squares_from_formula",
+    "OLSKwargs",
+    "RLSKwargs",
+    "RollingKwargs",
+]
+
+
+@dataclass
+class OLSKwargs:
+    """Specifies parameters relevant for regularized linear models: LASSO / Ridge / ElasticNet.
+
+    Attributes:
+        alpha: Regularization strength. Defaults to 0.0.
+        l1_ratio: Mixing parameter for ElasticNet regularization (0 for Ridge, 1 for LASSO).
+            Defaults to None (equivalent to Ridge regression).
+        max_iter: Maximum number of iterations. Defaults to 1000 iterations.
+        tol: Tolerance for convergence criterion. Defaults to 0.0001.
+        positive: Whether to enforce non-negativity constraints on coefficients.
+            Defaults to False (no constraint on coefficients).
+    """
+
+    alpha: Optional[float] = 0.0
+    l1_ratio: Optional[float] = None
+    max_iter: Optional[int] = 1_000
+    tol: Optional[float] = 0.0001
+    positive: Optional[bool] = False  # if True, imposes non-negativity constraint on coefficients
+
+    def to_dict(self) -> Dict[str, Any]:
+        return asdict(self)
+
+
+@dataclass
+class RLSKwargs:
+    """Specifies parameters of Recursive Least Squares models."""
+
+    half_life: Optional[float] = None
+    initial_state_covariance: Optional[float] = 10.0
+    initial_state_mean: Optional[List[float] | float] = None
+
+    def to_dict(self) -> Dict[str, Any]:
+        return asdict(self)
+
+
+@dataclass
+class RollingKwargs:
+    """Specifies parameters of Rolling OLS model."""
+
+    window_size: int = 1_000_000  # defaults to expanding OLS
+    min_periods: Optional[int] = None
+    use_woodbury: Optional[bool] = None
+    alpha: Optional[float] = None  # optional ridge alpha
+
+    def to_dict(self) -> Dict[str, Any]:
+        return asdict(self)
 
 
 def _pre_process_data(
     target: pl.Expr, *features: pl.Expr, sample_weights: Optional[pl.Expr], add_intercept: bool
 ):
     """Pre-processes the input data by casting it to float32 and scaling it with sample weights if
      provided.
@@ -33,35 +92,35 @@
     if sample_weights is not None:
         sqrt_w = sample_weights.cast(pl.Float32).sqrt()
         target *= sqrt_w
         features = [expr * sqrt_w for expr in features]
     return target, features, sqrt_w
 
 
-def least_squares(
+def compute_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
     mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
-    **ols_kwargs,
+    ols_kwargs: Optional[OLSKwargs] = None,
 ) -> pl.Expr:
     """Performs least squares regression.
 
     Depending on parameters provided this method supports a combination of sample weighting (WLS),
      L1/L2 regularization,
      and/or non-negativity constraint on coefficients.
 
     Args:
         target: The target expression.
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
         mode: Mode of operation ("predictions", "residuals", "coefficients").
-        **ols_kwargs: Additional keyword arguments for the OLS model. These include:
+        ols_kwargs: Additional keyword arguments specific for regularized OLS models. These include:
             - "alpha": Regularization strength. Default is 0.0.
                       Expected dtype: float.
             - "l1_ratio": Mixing parameter for ElasticNet regularization (0 for Ridge, 1 for LASSO).
                           Default is None (equivalent to Ridge regression).
                           Expected dtype: float or None.
             - "max_iter": Maximum number of iterations. Defaults to 1000 iterations.
                           Expected dtype: int or None.
@@ -77,95 +136,106 @@
         "predictions",
         "residuals",
         "coefficients",
     }, "'mode' must be one of {predictions, residuals, coefficients}"
     target, features, sqrt_w = _pre_process_data(
         target, *features, sample_weights=sample_weights, add_intercept=add_intercept
     )
-    # handle additional model specific kwargs
-    defaults = {
-        "alpha": 0.0,
-        "l1_ratio": None,
-        "max_iter": None,
-        "tol": None,
-        "positive": None,
-    }
-    supported_parameters = set(defaults)
-    assert set(ols_kwargs).issubset(supported_parameters), (
-        f"only the following parameters are supported {supported_parameters}, "
-        f"the following are not {set(ols_kwargs).difference(supported_parameters)} "
-    )
-    kwargs = {**defaults, **ols_kwargs}
+
+    ols_kwargs: OLSKwargs = ols_kwargs or OLSKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
         return register_plugin_function(
             plugin_path=Path(__file__).parent,
             function_name="least_squares_coefficients",
             args=[target, *features],
-            kwargs=kwargs,
+            kwargs=ols_kwargs.to_dict(),
             is_elementwise=False,
             changes_length=True,
         )
     else:
         predictions = (
             register_plugin_function(
                 plugin_path=Path(__file__).parent,
                 function_name="least_squares",
                 args=[target, *features],
-                kwargs=kwargs,
+                kwargs=ols_kwargs.to_dict(),
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
             return (target - predictions).alias("residuals")
 
 
-def least_squares_from_formula(formula: str, **ols_kwargs) -> pl.Expr:
-    """Performs ordinary least squares regression using a formula.
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
 
     Args:
         formula: Patsy-style formula string.
-        **ols_kwargs: Additional keyword arguments for the least squares function.
+        **kwargs: Additional keyword arguments for the least squares function.
 
     Returns:
         Resulting expression based on the formula.
     """
     expressions, add_intercept = build_expressions_from_patsy_formula(
         formula, include_dependent_variable=True
     )
-    return least_squares(
-        expressions[0], *expressions[1:], add_intercept=add_intercept, **ols_kwargs
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
     )
 
 
-def recursive_least_squares(
+def compute_recursive_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
     mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
-    **rls_kwargs,
-):
+    rls_kwargs: Optional[RLSKwargs] = None,
+) -> pl.Expr:
     """Performs an efficient recursive least squares regression (RLS).
 
     Defaults to RLS with forgetting factor of 1.0 and a high initial state variance: equivalent to
      efficient 'streaming' expanding window OLS.
 
     Args:
         target: The target expression.
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
         mode: Mode of operation ("predictions", "residuals", "coefficients").
-        **rls_kwargs: Additional keyword arguments for the recursive least squares model.
-        These include:
+        rls_kwargs: Additional keyword arguments for the recursive least squares model.
             - "half_life": Half-life parameter for exponential forgetting. Default is None
             (no forgetting).
             Expected dtype: float or None.
             - "initial_state_covariance":
             Scalar representing which behaves like an L2 regularization parameter. Larger values
              correspond to larger prior uncertainty around mean vector of state (inversely
              proportional to strength of equivalent L2 penalty).
@@ -174,53 +244,105 @@
             - "initial_state_mean": Initial mean vector of the state.
                                     Default is zero vector.
                                     Expected dtype: List[float] or None.
 
     Returns:
         Resulting expression based on the chosen mode.
     """
-
     assert mode in {
         "predictions",
         "residuals",
         "coefficients",
     }, "'mode' must be one of {predictions, residuals, coefficients}"
     target, features, sqrt_w = _pre_process_data(
         target, *features, sample_weights=sample_weights, add_intercept=add_intercept
     )
-
-    # handle additional model specific kwargs
-    defaults = {
-        "half_life": None,
-        "initial_state_covariance": None,
-        "initial_state_mean": None,
-    }
-    supported_parameters = set(defaults)
-    assert set(rls_kwargs).issubset(
-        supported_parameters
-    ), f"only the following parameters are supported {supported_parameters}"
-    kwargs = {**defaults, **rls_kwargs}
+    rls_kwargs: RLSKwargs = rls_kwargs or RLSKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
         return register_plugin_function(
             plugin_path=Path(__file__).parent,
             function_name="recursive_least_squares_coefficients",
             args=[target, *features],
-            kwargs=kwargs,
+            kwargs=rls_kwargs.to_dict(),
             is_elementwise=False,
             changes_length=True,
         )
     else:
         predictions = (
             register_plugin_function(
                 plugin_path=Path(__file__).parent,
                 function_name="recursive_least_squares",
                 args=[target, *features],
-                kwargs=kwargs,
+                kwargs=rls_kwargs.to_dict(),
+                is_elementwise=False,
+            )
+            / sqrt_w
+        )  # undo the sqrt(w) scaling implicit in predictions
+        if mode == "predictions":
+            return predictions
+        else:
+            return (target - predictions).alias("residuals")
+
+
+def compute_rolling_least_squares(
+    target: IntoExpr,
+    *features: pl.Expr,
+    sample_weights: Optional[pl.Expr] = None,
+    add_intercept: bool = False,
+    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+    rolling_kwargs: Optional[RollingKwargs] = None,
+) -> pl.Expr:
+    """Performs least squares regression in a rolling window fashion.
+
+    Args:
+        target: The target expression.
+        *features: Variable number of feature expressions.
+        sample_weights: Optional expression representing sample weights.
+        add_intercept: Whether to add an intercept column.
+        mode: Mode of operation ("predictions", "residuals", "coefficients").
+        rolling_kwargs: Additional keyword arguments for the rolling least squares model.
+            - "window_size": The size of the rolling window.
+            - "min_periods": The minimum number of observations required to produce estimates.
+            - "use_woodbury": Whether to use Woodbury matrix identity for faster computation.
+                              Defaults to True if num_features > 10.
+            - "alpha": L2 Regularization strength. Default is 0.0.
+                      Expected dtype: float.
+
+    Returns:
+        Resulting expression based on the chosen mode.
+    """
+    assert mode in {
+        "predictions",
+        "residuals",
+        "coefficients",
+    }, "'mode' must be one of {predictions, residuals, coefficients}"
+    target, features, sqrt_w = _pre_process_data(
+        target, *features, sample_weights=sample_weights, add_intercept=add_intercept
+    )
+    rolling_kwargs: RollingKwargs = rolling_kwargs or RollingKwargs()
+
+    # register either coefficient or prediction plugin functions
+    if mode == "coefficients":
+        return register_plugin_function(
+            plugin_path=Path(__file__).parent,
+            function_name="rolling_least_squares_coefficients",
+            args=[target, *features],
+            kwargs=rolling_kwargs.to_dict(),
+            is_elementwise=False,
+            changes_length=True,
+        )
+    else:
+        predictions = (
+            register_plugin_function(
+                plugin_path=Path(__file__).parent,
+                function_name="rolling_least_squares",
+                args=[target, *features],
+                kwargs=rolling_kwargs.to_dict(),
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
```

### Comparing `polars_ols-0.1.0/polars_ols/utils.py` & `polars_ols-0.1.1/polars_ols/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.0/src/expressions.rs` & `polars_ols-0.1.1/src/expressions.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #![allow(clippy::unit_arg, clippy::unused_unit)]
 use crate::least_squares::{
-    solve_elastic_net, solve_ols_qr, solve_recursive_least_squares, solve_ridge,
+    solve_elastic_net, solve_ols_qr, solve_recursive_least_squares, solve_ridge, solve_rolling_ols,
 };
 use ndarray::{Array, Array1, Array2, Axis};
 use polars::datatypes::{DataType, Field, Float32Type};
 use polars::error::{polars_err, PolarsResult};
 use polars::prelude::{
     IntoSeries, ListBuilderTrait, ListPrimitiveChunkedBuilder, NamedFromOwned, Series,
 };
@@ -111,14 +111,31 @@
     initial_state_mean: Option<Vec<f32>>, // in python list[f32] | None is equivalent
 }
 
 fn convert_option_vec_to_array1(opt_vec: Option<Vec<f32>>) -> Option<Array1<f32>> {
     opt_vec.map(Array1::from)
 }
 
+fn coefficients_to_series(coefficients: &Array2<f32>) -> Series {
+    // convert 2d ndarray into Series of List[f32]
+    let mut chunked_builder = ListPrimitiveChunkedBuilder::<Float32Type>::new(
+        "",
+        coefficients.len_of(Axis(0)),
+        coefficients.len_of(Axis(1)),
+        DataType::Float32,
+    );
+    for row in coefficients.axis_iter(Axis(0)) {
+        match row.as_slice() {
+            Some(row) => chunked_builder.append_slice(row),
+            None => chunked_builder.append_slice(&row.to_vec()),
+        }
+    }
+    chunked_builder.finish().into_series()
+}
+
 #[polars_expr(output_type_func=list_float_dtype)]
 fn recursive_least_squares_coefficients(
     inputs: &[Series],
     kwargs: RLSKwargs,
 ) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let initial_state_mean = convert_option_vec_to_array1(kwargs.initial_state_mean);
@@ -126,29 +143,15 @@
         &y,
         &x,
         kwargs.half_life,
         kwargs.initial_state_covariance,
         initial_state_mean,
     );
 
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
-    let series = chunked_builder.finish().into_series();
-
+    let series = coefficients_to_series(&coefficients);
     Ok(series.with_name("coefficients"))
 }
 
 #[polars_expr(output_type=Float32)]
 fn recursive_least_squares(inputs: &[Series], kwargs: RLSKwargs) -> PolarsResult<Series> {
     let (y, x) = convert_polars_to_ndarray(inputs);
     let coefficients = solve_recursive_least_squares(
@@ -157,7 +160,48 @@
         kwargs.half_life,
         kwargs.initial_state_covariance,
         None,
     );
     let predictions = (&x * &coefficients).sum_axis(Axis(1));
     Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
 }
+
+#[derive(Deserialize)]
+pub struct RollingKwargs {
+    window_size: usize,
+    min_periods: Option<usize>,
+    use_woodbury: Option<bool>,
+    alpha: Option<f32>,
+}
+
+#[polars_expr(output_type_func=list_float_dtype)]
+fn rolling_least_squares_coefficients(
+    inputs: &[Series],
+    kwargs: RollingKwargs,
+) -> PolarsResult<Series> {
+    let (y, x) = convert_polars_to_ndarray(inputs);
+    let coefficients = solve_rolling_ols(
+        &y,
+        &x,
+        kwargs.window_size,
+        kwargs.min_periods,
+        kwargs.use_woodbury,
+        kwargs.alpha,
+    );
+    let series = coefficients_to_series(&coefficients);
+    Ok(series.with_name("coefficients"))
+}
+
+#[polars_expr(output_type=Float32)]
+fn rolling_least_squares(inputs: &[Series], kwargs: RollingKwargs) -> PolarsResult<Series> {
+    let (y, x) = convert_polars_to_ndarray(inputs);
+    let coefficients = solve_rolling_ols(
+        &y,
+        &x,
+        kwargs.window_size,
+        kwargs.min_periods,
+        kwargs.use_woodbury,
+        kwargs.alpha,
+    );
+    let predictions = (&x * &coefficients).sum_axis(Axis(1));
+    Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
+}
```

### Comparing `polars_ols-0.1.0/src/least_squares.rs` & `polars_ols-0.1.1/src/least_squares.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 use faer::linalg::solvers::SolverCore;
 use faer::prelude::{SpSolver, SpSolverLstsq};
 use faer::Side;
 use faer_ext::{IntoFaer, IntoNdarray};
-use ndarray::{s, Array, Array1, Array2, ArrayView1, Axis, NewAxis};
+use ndarray::{array, s, Array, Array1, Array2, ArrayView1, Axis, NewAxis};
 // use ndarray_linalg::{Inverse, InverseC, Norm, SolveC};
 
-fn inv(array: &Array2<f32>, use_cholesky: bool) -> Array2<f32> {
+/// Invert square matrix input using either Cholesky or LU decomposition
+pub fn inv(array: &Array2<f32>, use_cholesky: bool) -> Array2<f32> {
     let m = array.view().into_faer();
     if use_cholesky {
-        m.cholesky(Side::Lower)
-            .expect("could not compute cholesky decomposition")
-            .inverse()
-            .as_ref()
-            .into_ndarray()
-            .to_owned()
-    } else {
-        m.partial_piv_lu()
-            .inverse()
-            .as_ref()
-            .into_ndarray()
-            .to_owned()
+        match m.cholesky(Side::Lower) {
+            Ok(cholesky) => {
+                return cholesky.inverse().as_ref().into_ndarray().to_owned();
+            }
+            Err(_) => {
+                println!("Cholesky decomposition failed, falling back to LU decomposition");
+            }
+        }
     }
+    // Fall back to LU decomposition
+    m.partial_piv_lu()
+        .inverse()
+        .as_ref()
+        .into_ndarray()
+        .to_owned()
 }
 
 /// Solves an ordinary least squares problem using QR using faer
 /// Inputs: features (2d ndarray), targets (1d ndarray)
 /// Outputs: 1-d OLS coefficients
 pub fn solve_ols_qr(y: &Array1<f32>, x: &Array2<f32>) -> Array1<f32> {
     // compute least squares solution via QR
@@ -35,20 +38,38 @@
         .as_ref()
         .into_ndarray()
         .slice(s![.., 0])
         .to_owned()
 }
 
 /// Solves the normal equations: (X^T X) coefficients = X^T Y
-fn solve_normal_equations(xtx: &Array2<f32>, xty: &Array1<f32>) -> Array1<f32> {
-    // attempt to solve via cholesky making use of X.T X being SPD
-    xtx.view()
-        .into_faer()
-        .cholesky(Side::Lower)
-        .unwrap()
+/// Attempts to solve via cholesky
+fn solve_normal_equations(xtx: &Array2<f32>, xty: &Array1<f32>, use_cholesky: bool) -> Array1<f32> {
+    // Attempt to solve via Cholesky decomposition
+    let xtx_faer = xtx.view().into_faer();
+    if use_cholesky {
+        match xtx_faer.cholesky(Side::Lower) {
+            Ok(cholesky) => {
+                // Cholesky decomposition successful
+                return cholesky
+                    .solve(&xty.slice(s![.., NewAxis]).into_faer())
+                    .as_ref()
+                    .into_ndarray()
+                    .slice(s![.., 0])
+                    .into_owned();
+            }
+            Err(_) => {
+                // Cholesky decomposition failed, fallback to LU decomposition w/ partial pivoting
+                println!("Cholesky decomposition failed, falling back to LU decomposition");
+            }
+        }
+    }
+    // Fall back to LU decomposition
+    xtx_faer
+        .partial_piv_lu()
         .solve(&xty.slice(s![.., NewAxis]).into_faer())
         .as_ref()
         .into_ndarray()
         .slice(s![.., 0])
         .into_owned()
 }
 
@@ -57,27 +78,29 @@
 pub fn solve_ridge(y: &Array1<f32>, x: &Array2<f32>, alpha: f32) -> Array1<f32> {
     assert!(alpha > 0., "alpha must be strictly positive");
     let x_t = &x.t();
     let x_t_x = x_t.dot(x);
     let x_t_y = x_t.dot(y);
     let eye = Array::eye(x_t_x.shape()[0]);
     let ridge_matrix = &x_t_x + &eye * alpha;
-    solve_normal_equations(&ridge_matrix, &x_t_y)
+    solve_normal_equations(&ridge_matrix, &x_t_y, true)
 }
 
 fn soft_threshold(x: &f32, alpha: f32, positive: bool) -> f32 {
     let mut result = x.signum() * (x.abs() - alpha).max(0.0);
     if positive {
         result = result.max(0.0);
     }
     result
 }
 
 /// Solves an elastic net regression problem of the form: 1 / (2 * n_samples) * ||y - Xw||_2
-/// + alpha * l1_ratio * ||w||_1 + 0.5 * alpha * (1 - l1_ratio) * ||w||_2
+/// + alpha * l1_ratio * ||w||_1 + 0.5 * alpha * (1 - l1_ratio) * ||w||_2.
+/// Uses cyclic coordinate descent with efficient 'naive updates' and a
+/// general soft thresholding function.
 pub fn solve_elastic_net(
     y: &Array1<f32>,
     x: &Array2<f32>,
     alpha: f32,            // strictly positive regularization parameter
     l1_ratio: Option<f32>, // scalar strictly between 0 (full ridge) and 1 (full lasso)
     max_iter: Option<usize>,
     tol: Option<f32>,       // controls convergence criteria between iterations
@@ -137,15 +160,15 @@
         lam: f32,
         half_life: Option<f32>,
         initial_state_mean: Option<Array1<f32>>,
     ) -> Self {
         // calculate forgetting_factor based on the value of half_life, default to 1.0
         // (expanding ols)
         let forgetting_factor = if let Some(half_life) = half_life {
-            0.5f32.ln() / half_life
+            (0.5f32.ln() / half_life).exp()
         } else {
             1.0
         };
 
         let coef = Array1::<f32>::zeros(num_features);
         let p = Array2::<f32>::eye(num_features) * lam;
         let k = Array1::<f32>::zeros(num_features);
@@ -160,15 +183,14 @@
 
     pub fn update(&mut self, x: &Array1<f32>, y: f32) {
         let r = 1.0 + x.t().dot(&self.p).dot(x) / self.forgetting_factor;
         self.k
             .assign(&(&self.p.dot(x) / (r * self.forgetting_factor)));
         let residuals = y - x.dot(&self.coef);
         self.coef.assign(&(&self.coef + &(&self.k * residuals)));
-        // unfortunately can't find equivalent of 'np.outer' in ndarray
         let k_ = &self.k.view().insert_axis(Axis(1)); // K x 1
         self.p
             .assign(&(&self.p / self.forgetting_factor - k_.dot(&k_.t()) * r));
     }
 
     pub fn predict(&self, x: &Array1<f32>) -> f32 {
         x.dot(&self.coef)
@@ -219,15 +241,15 @@
             .slice_mut(s![t, ..])
             .assign(&recursive_least_squares.coef.view());
         // predictions[t] = recursive_least_squares.predict(&x_t);
     }
     coefficients
 }
 
-fn outer_product(u: &ArrayView1<f32>, v: &ArrayView1<f32>) -> Array2<f32> {
+pub fn outer_product(u: &ArrayView1<f32>, v: &ArrayView1<f32>) -> Array2<f32> {
     // Reshape u and v to have a shape of (n, 1) and (1, m) respectively
     let u_reshaped = u.insert_axis(Axis(1));
     let v_reshaped = v.insert_axis(Axis(0));
 
     // Compute the outer product using broadcasting and dot product
     u_reshaped.dot(&v_reshaped)
 }
@@ -246,49 +268,55 @@
 ///
 /// The Woodbury update is a method to efficiently update the inverse of a matrix A_inv
 /// when adding or removing rows or columns from the original matrix.
 ///
 /// The Woodbury update formula is given by:
 ///
 /// ```text
-/// (A + U C V)^{-1} = A^{-1} + A^{-1} U (C^{-1} + V A^{-1} U)^{-1} V A^{-1}
+/// (A + U C V)^{-1} = A^{-1} - A^{-1} U (C^{-1} + V A^{-1} U)^{-1} V A^{-1}
 /// ```
 pub fn woodbury_update(
     a_inv: &Array2<f32>,
     u: &Array2<f32>,
     c: &Array2<f32>,
     v: &Array2<f32>,
     c_is_diag: Option<bool>,
 ) -> Array2<f32> {
     // Check if c_is_diag is Some(true)
     let inv_c = if let Some(true) = c_is_diag {
         inv_diag(c)
     } else {
         inv(c, false)
-    };
-    // compute V inv(A)
-    let v_inv_a = v.dot(a_inv);
-    let inv_a_u = a_inv.dot(u);
-    // compute term (C^{-1} + V A^{-1} U)^{-1}
-    let intermediate = inv(&(inv_c + v.dot(&inv_a_u)), false);
-    a_inv - inv_a_u.dot(&intermediate).dot(&v_inv_a)
+    }; // r x r
+       // compute V inv(A)
+    let v_inv_a = v.dot(a_inv); // r x K
+    let inv_a_u = a_inv.dot(u); // K x r
+                                // compute term (C^{-1} + V A^{-1} U)^{-1}
+    let intermediate = inv(&(inv_c + v.dot(&inv_a_u)), false); // r x r
+    a_inv - inv_a_u.dot(&intermediate).dot(&v_inv_a) // K x K
 }
 
 /// Function to update inv(X^TX) by x_update array of rank r using Woodbury Identity.
-fn update_xtx_inv(xtx_inv: &Array2<f32>, x_update: &Array2<f32>) -> Array2<f32> {
+pub fn update_xtx_inv(
+    xtx_inv: &Array2<f32>,
+    x_update: &Array2<f32>,
+    c: Option<&Array2<f32>>,
+) -> Array2<f32> {
     // Reshape x_new and x_old for Woodbury update
     let u = x_update.t().to_owned(); // K x r
     let v = u.t().to_owned(); // r x K
-    let c = Array2::eye(u.shape()[1]); // Identity matrix r x r
+
+    // let c = Array2::eye(u.shape()[1]); // Identity matrix r x r
+    let default = Array2::eye(u.shape()[1]);
+    let c = c.unwrap_or(&default);
 
     // Apply Woodbury update
-    woodbury_update(xtx_inv, &u, &c, &v, Some(true))
+    woodbury_update(xtx_inv, &u, c, &v, Some(true))
 }
 
-
 /// Solves rolling ordinary least squares (OLS) regression.
 ///
 /// This function calculates the coefficients of the linear regression model
 /// using rolling windows. It takes a dependent variable `y`, an independent variable matrix `x`,
 /// the size of the rolling window, the minimum number of periods required to calculate
 /// coefficients, and an optional flag to specify whether to use Woodbury matrix identity
 /// for additional efficiency in case of large number of features.
@@ -305,74 +333,92 @@
 ///
 pub fn solve_rolling_ols(
     y: &Array1<f32>,
     x: &Array2<f32>,
     window_size: usize,
     min_periods: Option<usize>,
     use_woodbury: Option<bool>,
+    alpha: Option<f32>,
 ) -> Array2<f32> {
     let n = x.shape()[0];
     let k = x.shape()[1]; // Number of independent variables
-    let min_periods = min_periods.unwrap_or(1);
-    let use_woodbury = use_woodbury.unwrap_or(false);
+    let min_periods = min_periods.unwrap_or(std::cmp::min(k, window_size));
+    // default to using woodbury if number of features is relatively large.
+    let use_woodbury = use_woodbury.unwrap_or(k > 60);
     let mut coefficients = Array2::zeros((n, k));
+    let alpha = alpha.unwrap_or(0.0);
+
+    // we allow the user to pass a min_periods < k, but this may result in
+    // unstable warm-up coefficients. TODO: It might make sense to log a warning
+    debug_assert!(
+        min_periods >= k && min_periods < window_size,
+        "min_periods must be greater or equal to the number of regressors \
+             in the model and less than the window size"
+    );
 
     // Initialize X^T X, inv(X.T X), and X^T Y
-    let x_window = x.slice(s![..window_size, ..]);
-    let y_window = y.slice(s![..window_size]);
-    let mut xty = x_window.t().dot(&y_window);
-    let mut xtx = x_window.t().dot(&x_window);
+    let x_warmup = x.slice(s![..min_periods, ..]);
+    let y_warmup = y.slice(s![..min_periods]);
+    let mut xty = x_warmup.t().dot(&y_warmup);
+    let mut xtx = x_warmup.t().dot(&x_warmup);
+
+    // add ridge penalty
+    if alpha > 0. {
+        xtx = xtx + Array2::<f32>::eye(k) * alpha
+    }
 
     // Use woodbury to propagate inv(X.T X) & (X.T Y)
     if use_woodbury {
         // assign warm-up coefficients
-        let mut xtx_inv = inv(&xtx, true);
+        let mut xtx_inv = inv(&xtx, false);
         let coef_warmup = xtx_inv.t().dot(&xty);
         coefficients
-            .slice_mut(s![min_periods, ..])
+            .slice_mut(s![min_periods - 1, ..])
             .assign(&coef_warmup);
 
+        // make c [[-1, 0], [0, 1]]; which drops old and adds new
+        let c: Array2<f32> = array![[-1., 0.], [0., 1.]];
+
         // Slide the window and update coefficients
-        for i in min_periods + 1..n {
+        for i in min_periods..n {
             let i_start = i.saturating_sub(window_size);
 
             let x_new = x.row(i);
 
             if i > window_size {
                 let x_prev = x.row(i_start);
 
                 // create rank 2 update array
                 let mut x_update = ndarray::stack(Axis(0), &[x_prev, x_new]).unwrap(); // 2 x K
 
                 // multiply x_old row by -1.0 (subtract the previous contribution)
                 x_update.row_mut(0).mapv_inplace(|elem| -elem);
 
                 // update inv(XTX) and XTY
-                xtx_inv = update_xtx_inv(&xtx_inv, &x_update);
+                xtx_inv = update_xtx_inv(&xtx_inv, &x_update, Some(&c));
                 xty = xty + &x_new * y[i]  // add new contribution
                     - &x_prev * y[i_start] // subtract old contribution
                 ;
             } else {
                 let x_update = x_new.insert_axis(Axis(0)).into_owned(); // 1 x K
-                xtx_inv = update_xtx_inv(&xtx_inv, &x_update);
+                xtx_inv = update_xtx_inv(&xtx_inv, &x_update, None);
                 xty = xty + &x_new * y[i];
             }
-            let coefficients_i = xtx_inv.dot(&xty);
-            coefficients.slice_mut(s![i, ..]).assign(&coefficients_i);
+            coefficients.slice_mut(s![i, ..]).assign(&xtx_inv.dot(&xty));
         }
     } else {
         // update X.T X & X.T Y and solve normal equations at every time step
         // assign warm-up coefficients
-        let coef_warmup = solve_normal_equations(&xtx, &xty);
+        let coef_warmup = solve_normal_equations(&xtx, &xty, false);
         coefficients
-            .slice_mut(s![min_periods, ..])
+            .slice_mut(s![min_periods - 1, ..])
             .assign(&coef_warmup);
 
         // Slide the window and update coefficients
-        for i in min_periods + 1..n {
+        for i in min_periods..n {
             let i_start = i.saturating_sub(window_size);
 
             // update XTX w/ latest data point
             let x_new = x.row(i);
 
             // Add new contributions
             xtx += &outer_product(&x_new, &x_new);
@@ -382,13 +428,13 @@
             if i > window_size {
                 let x_prev = x.row(i_start);
                 xtx -= &outer_product(&x_prev, &x_prev);
                 xty = xty - &x_prev * y[i_start];
             }
 
             // update coefficients
-            let coefficients_i = solve_normal_equations(&xtx, &xty);
+            let coefficients_i = solve_normal_equations(&xtx, &xty, true);
             coefficients.slice_mut(s![i, ..]).assign(&coefficients_i);
         }
     }
     coefficients
 }
```

### Comparing `polars_ols-0.1.0/src/lib.rs` & `polars_ols-0.1.1/src/lib.rs`

 * *Files 23% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 use pyo3::types::PyModule;
 use pyo3::{pymodule, PyResult, Python};
 
 #[cfg(test)]
 mod tests {
     use crate::expressions::convert_polars_to_ndarray;
     use crate::least_squares::{
-        solve_elastic_net, solve_ols_qr, solve_recursive_least_squares, solve_ridge,
-        solve_rolling_ols, woodbury_update,
+        inv, outer_product, solve_elastic_net, solve_ols_qr, solve_recursive_least_squares,
+        solve_ridge, solve_rolling_ols, update_xtx_inv, woodbury_update,
     };
     use ndarray::prelude::*;
     use ndarray_linalg::assert_close_l2;
     use ndarray_rand::rand_distr::Normal;
     use ndarray_rand::RandomExt;
     use polars::datatypes::DataType::Float32;
     use polars::prelude::*;
@@ -76,38 +76,70 @@
     }
 
     #[test]
     fn test_rolling_least_squares() {
         let (y, x1, x2) = make_data();
         let (targets, features) = convert_polars_to_ndarray(&[y.clone(), x1, x2]);
         let coefficients =
-            solve_rolling_ols(&targets, &features, 1_000usize, Some(100usize), Some(false));
+            solve_rolling_ols(&targets, &features, 1_000usize, Some(100usize),
+                              Some(true), None);
         let expected: Array1<f32> = array![1.0, 1.0];
         println!("{:?}", coefficients.slice(s![0, ..]));
         println!("{:?}", coefficients.slice(s![-1, ..]));
         assert_close_l2!(&coefficients.slice(s![-1, ..]), &expected, 0.0001);
     }
 
     #[test]
     fn test_woodbury_update() {
         // Test matrices
-        let a_inv = array![[0.5, 0.0], [0.0, 0.5]]; // A^{-1}
+        let a = array![[0.5, 0.2], [0.0, 0.5]]; // A^{-1}
+        let a_inv = inv(&a, false);
         let u = array![[1.0, 2.0], [3.0, 4.0]]; // U
-        let c = array![[2.0, 0.0], [0.0, 2.0]]; // C
+        let c = array![[1.0, 0.0], [0.0, 1.0]]; // C
         let v = array![[1.0, 0.0], [0.0, 1.0]]; // V
 
         // Expected result
-        let expected_result = array![[0.625, -0.25], [-0.375, 0.25]]; // Expected result
+        let expected_result = inv(&(&a + &u.dot(&c).dot(&v)), false);
 
         // Compute the Woodbury update
         let result = woodbury_update(&a_inv, &u, &c, &v, Some(true));
 
+        // test confirms: inv(A + UCV) == A{-1} - A^{-1} U (C^{-1} + V A^{-1} U)^{-1} V A^{-1}
+
         // Compare with expected result
         assert_close_l2!(&result, &expected_result, 0.00001);
     }
+
+    #[test]
+    fn test_update_xtx_inv() {
+        // Test matrices
+        let x = Array2::<f32>::random((252, 5), Normal::new(0., 1.).unwrap());
+
+        let xtx = x.t().dot(&x);
+        let mut xtx_inv = inv(&xtx, true);
+
+        let x_new = array![0.5, 2., -0.3, 0.1, 0.2];
+        let x_new = x_new.view(); // new data point
+        let x_old = x.slice(s![0, ..]); // old data point
+
+        // create rank 2 update array
+        let x_update = ndarray::stack(Axis(0), &[x_old, x_new]).unwrap().clone(); // 2 x K
+
+        let c: Array2<f32> = array![[-1., 0.], [0., 1.]]; // subtract x_old, add x_new
+
+        // update xtx inv with [x_old, x_new] using woodbury
+        xtx_inv = update_xtx_inv(&xtx_inv, &x_update, Some(&c));
+
+        // test non fancy xtx update + invert
+        let expected = inv(
+            &(&xtx - &outer_product(&x_old, &x_old) + &outer_product(&x_new, &x_new)),
+            true,
+        );
+        assert_close_l2!(&xtx_inv, &expected, 0.00001);
+    }
 }
 
 #[cfg(target_os = "linux")]
 use jemallocator::Jemalloc;
 
 #[global_allocator]
 #[cfg(target_os = "linux")]
```

### Comparing `polars_ols-0.1.0/tests/test_ols.py` & `polars_ols-0.1.1/tests/test_ols.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import time
 from contextlib import contextmanager
 
 import numpy as np
 import polars as pl
 import statsmodels.formula.api as smf
 from sklearn.linear_model import ElasticNet
+from statsmodels.regression.rolling import RollingOLS
 
-from polars_ols import least_squares, least_squares_from_formula
+from polars_ols import OLSKwargs, compute_least_squares, least_squares_from_formula
 
 
 @contextmanager
 def timer(msg: str | None = None, precision: int = 3) -> float:
     start = time.perf_counter()
     end = start
     yield lambda: end - start
@@ -31,15 +32,17 @@
 
 
 def test_ols():
     df = _make_data()
     # compute OLS solution w/ polars (via QR in rust) [2.331s]
     with timer("OLS rust"):
         for _ in range(1_000):
-            expr = least_squares(pl.col("y"), pl.col("x1"), pl.col("x2")).alias("predictions")
+            expr = compute_least_squares(pl.col("y"), pl.col("x1"), pl.col("x2")).alias(
+                "predictions"
+            )
             df = df.lazy().with_columns(expr).collect()
 
     # compute OLS w/ lstsq numpy [4.583s]
     with timer("OLS numpy"):
         for _ in range(1_000):
             x, y = df.select("x1", "x2").to_numpy(), df.select("y").to_numpy().flatten()
             coef = np.linalg.lstsq(x, y, rcond=None)[0]
@@ -64,15 +67,15 @@
     x, y = df.select("x1", "x2").to_numpy(), df["y"].to_numpy()
     coef = np.linalg.lstsq(x, y, rcond=None)[0]
     assert np.allclose(residuals.flatten(), y - x @ coef, rtol=1.0e-4, atol=1.0e-4)
 
 
 def test_ols_intercept():
     df = _make_data()
-    expr = least_squares(pl.col("y"), pl.col("x1"), pl.col("x2"), add_intercept=True).alias(
+    expr = compute_least_squares(pl.col("y"), pl.col("x1"), pl.col("x2"), add_intercept=True).alias(
         "predictions"
     )
     y_hat = df.select(expr).to_numpy().flatten()
     expected = smf.ols(formula="y ~ x1 + x2", data=df).fit().predict(df).to_numpy()
     assert np.allclose(y_hat, expected, atol=1.0e-4, rtol=1.0e-4)
 
 
@@ -104,19 +107,19 @@
             x = df.select("x1", "x2").to_numpy()
             y = df.select("y").to_numpy().flatten()
             coef_expected = np.linalg.solve((x.T @ x) + np.eye(x.shape[1]) * alpha, x.T @ y)
             expected = x @ coef_expected
 
     with timer("ridge rust"):
         for _ in range(1_000):
-            expr = least_squares(
+            expr = compute_least_squares(
                 pl.col("y"),
                 pl.col("x1"),
                 pl.col("x2"),
-                alpha=alpha,
+                ols_kwargs=OLSKwargs(alpha=alpha),
             ).alias("predictions")
             df = df.lazy().with_columns(expr).collect()
     assert np.allclose(df["predictions"].to_numpy(), expected, rtol=1.0e-4, atol=1.0e-4)
 
 
 def test_wls():
     array = np.random.normal(size=(10_000, 2))
@@ -132,21 +135,21 @@
     ).cast(pl.Float32)
 
     weights = np.hstack([np.ones(8_000) * 1.0 / 10**2, np.ones(2_000) * 1.0 / 0.1**2])
     weights /= weights.mean()
 
     df = df.with_columns(sample_weight=weights).cast(pl.Float32)
 
-    expr_wls = least_squares(
+    expr_wls = compute_least_squares(
         pl.col("y"),
         pl.col("x1"),
         pl.col("x2"),
         sample_weights=pl.col("sample_weight"),
     ).alias("predictions_wls")
-    expr_ols = least_squares(
+    expr_ols = compute_least_squares(
         pl.col("y"),
         pl.col("x1"),
         pl.col("x2"),
     ).alias("predictions_ols")
     df = df.lazy().with_columns(expr_wls, expr_ols).collect()
 
     y_hat_wls = smf.wls(data=df, formula="y ~ x1 + x2 -1", weights=weights).fit().predict()
@@ -186,15 +189,15 @@
                 "x1 + x2 -1",
                 mode="coefficients",
                 l1_ratio=0.5,
                 alpha=0.1,
                 max_iter=1_000,
                 tol=0.0001,
             )
-            .alias("predictions")
+            .alias("coefficients")
         )
         .collect()
         .to_numpy()
         .flatten()
     )
     assert np.allclose(mdl.coef_, coef, rtol=1.0e-4, atol=1.0e-4)
 
@@ -216,15 +219,15 @@
                 mode="coefficients",
                 l1_ratio=0.5,
                 alpha=0.1,
                 max_iter=1_000,
                 tol=0.0001,
                 positive=True,
             )
-            .alias("predictions")
+            .alias("coefficients")
         )
         .collect()
         .to_numpy()
         .flatten()
     )
     assert np.allclose(mdl.coef_, coef, rtol=1.0e-4, atol=1.0e-4)
 
@@ -242,17 +245,17 @@
                 pl.col("x2"),
                 mode="coefficients",
                 # equivalent to expanding window (no forgetting)
                 half_life=None,
                 # arbitrarily weak L2 (diffuse) prior
                 initial_state_covariance=1_000_000.0,
             )
-            .alias("predictions")
+            .alias("coefficients")
         )
-        .select(pl.col("predictions").list.to_array(2))
+        .select(pl.col("coefficients").list.to_array(2))
         .collect()
         .to_numpy()
         .T
     )
 
     # full sample OLS
     coef_ols = (
@@ -280,23 +283,51 @@
                 pl.col("x2"),
                 mode="coefficients",
                 # equivalent to expanding window (no forgetting)
                 half_life=None,
                 initial_state_covariance=1.0e-6,  # arbitrarily strong L2 prior
                 initial_state_mean=[0.25, 0.25],  # custom prior
             )
-            .alias("predictions")
+            .alias("coefficients")
         )
-        .select(pl.col("predictions").list.to_array(2))
+        .select(pl.col("coefficients").list.to_array(2))
         .collect()
         .to_numpy()
         .T
     )
 
     # given few samples and strong prior strength, the coefficients are nearly
     # identical to the prior
     assert np.allclose(coef_rls_prior[0], [0.25, 0.25], rtol=1.0e-3, atol=1.0e-3)
     assert np.allclose(coef_rls_prior[10], [0.25, 0.25], rtol=1.0e-3, atol=1.0e-3)
 
     # as number of samples seen grows, the coefficients start to diverge from prior
     # & eventually converge to ground truth.
     assert not np.allclose(coef_rls_prior[-1], [0.5, 0.5], rtol=1.0e-4, atol=1.0e-4)
+
+
+def test_rolling_least_squares():
+    df = _make_data()
+    with timer("rolling ols"):
+        coef_rolling = (
+            df.lazy()
+            .select(
+                pl.col("y")
+                .least_squares.rolling_ols(
+                    pl.col("x1"),
+                    pl.col("x2"),
+                    mode="coefficients",
+                    window_size=252,
+                    min_periods=2,
+                )
+                .alias("coefficients")
+            )
+            .select(pl.col("coefficients").list.to_array(2))
+            .collect()
+            .to_numpy()
+            .T
+        )
+    with timer("rolling ols statsmodels"):
+        mdl = RollingOLS(
+            df["y"].to_numpy(), df[["x1", "x2"]].to_numpy(), window=252, min_nobs=2, expanding=True
+        ).fit()
+    assert np.allclose(coef_rolling[1:], mdl.params[1:].astype("float32"), rtol=1.0e-3, atol=1.0e-3)
```

### Comparing `polars_ols-0.1.0/Cargo.lock` & `polars_ols-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -51,23 +51,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f2a05fd1bd10b2527e20a2cd32d8873d115b8b39fe219ee25f42a8aca6ba278"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "approx"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
 name = "argminmax"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
  "num-traits",
 ]
@@ -964,15 +955,15 @@
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
- "approx 0.4.0",
+ "approx",
  "cblas-sys",
  "libc",
  "matrixmultiply",
  "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
@@ -1595,17 +1586,17 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ols"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
- "approx 0.5.1",
+ "approx",
  "faer",
  "faer-ext",
  "jemallocator",
  "ndarray",
  "ndarray-linalg",
  "ndarray-rand",
  "num-traits",
```

### Comparing `polars_ols-0.1.0/pyproject.toml` & `polars_ols-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.1.0/PKG-INFO` & `polars_ols-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,93 @@
-Metadata-Version: 2.3
-Name: polars-ols
-Version: 0.1.0
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
-regression variants (OLS, WLS, Ridge, Elastic Net, Recursive least squares, Non-negative least squares) and exposes
+regression variants (OLS, WLS, Ridge, Elastic Net, Non-negative least squares, Recursive least squares) and exposes
 them as simple polars expressions which can easily be integrated into your workflow.
 
 ### Why?
 
-1. **High Performance**: implementations are written in rust and make use of optimized rust linear-algebra crates & LAPACK routines. See benchmark section.
-2. **Polars Integration**: avoids unnecessary conversions from lazy to eager mode and to other formats or multiple libraries (e.g. numpy, sklearn) to do simple linear regressions.
+1. **High Performance**: implementations are written in rust and make use of optimized rust linear-algebra crates & LAPACK routines. See [benchmark](#benchmark) section.
+2. **Polars Integration**: avoids unnecessary conversions from lazy to eager mode and to external libraries (e.g. numpy, sklearn) to do simple linear regressions.
 Chain least squares formulae like any other expression in polars.
-3. **Efficient Implementation**:
-   - Numerically stable algorithms are chosen where possible (e.g. QR, Cholesky).
+3. **Efficient Implementations**:
+   - Numerically stable algorithms are chosen where appropriate (e.g. QR, Cholesky).
    - Flexible model specification allows arbitrary combination of sample weighting, L1/L2 regularization, & non-negativity constraints on parameters.
    - Efficient rank-1 update algorithms used for moving window regressions.
 4. **Easy Parallelism**: Computing OLS predictions, in parallel, across groups can not be easier: call `.over()` or `group_by` just like any other polars' expression and benefit from full Rust parallelism.
 5. **Formula API**: supports building models via patsy syntax: `y ~ x1 + x2 + x3:x4 -1` (like statsmodels) which automatically converts to equivalent polars expressions.
 
 Installation
 ------------
 
-First, you need to [install Polars](https://pola-rs.github.io/polars/user-guide/installation/). Then simply run the below to install the `polars-ols` extension:
+First, you need to [install Polars](https://pola-rs.github.io/polars/user-guide/installation/). Then run the below to install the `polars-ols` extension:
 ```console
 pip install polars-ols
 ```
 
 API & Examples
 ------------
 
 Importing `polars_ols` will register the namespace `least_squares` provided by this package.
-You can build models either by either specifying columns (`pl.col(...)`) for your targets and features or using
-the formula api (patsy syntax). See below for examples.
-```python
-import polars as pl
-import polars_ols as pls
+You can build models either by either specifying polars expressions (e.g. `pl.col(...)`) for your targets and features or using
+the formula api (patsy syntax). All models support the following general (optional) arguments:
+- `mode` - a literal which determines the type of output produced by the model
+- `add_intercept` - a boolean specifying if an intercept feature should be added to the features
+- `sample_weights` - a column or expression providing non-negative weights applied to the samples
 
-ols_expr = pl.col("y").least_squares.from_formula("x1 + x2").over("group").alias("predictions_ols")
-lasso_expr = pl.col("y").least_squares.lasso(pl.col("x1"), pl.col("x2"), alpha=0.01).alias("predictions_lasso")
-```
+Remaining parameters are model specific, for example `alpha` penalty parameter used by regularized least squares models.
 
-Alternatively, you also access public methods provided by the package as well:
+See below for basic usage examples.
+Please refer to the [tests](./tests/test_ols.py) or [demo notebook](./notebooks/polars_ols_demo.ipynb) for detailed examples.
 
 ```python
 import polars as pl
-import polars_ols as pls
-
-enet_expr = pls.least_squares_from_formula("y ~ x1 + x2",
-                                          sample_weights=pl.col("weights"),  # specify column with sample weights (WLS)
-                                          alpha=0.0001,   # specify regularization parameter
-                                          l1_ratio=0.5,  # set 50% L1 penalty & 50% L2 penalty
-                                          positive=True,  # enforce non-negativity on coefficients
-                                          ).over("group").alias("predictions_enet")
-```
-
-The methods provided by the `least_squares` namespace return polars expressions which your polars dataframe
-can access normally:
+import polars_ols as pls  # registers 'least_squares' namespace
 
-```python
 df = pl.DataFrame({"y": [1.16, -2.16, -1.57, 0.21, 0.22, 1.6, -2.11, -2.92, -0.86, 0.47],
                    "x1": [0.72, -2.43, -0.63, 0.05, -0.07, 0.65, -0.02, -1.64, -0.92, -0.27],
                    "x2": [0.24, 0.18, -0.95, 0.23, 0.44, 1.01, -2.08, -1.36, 0.01, 0.75],
                    "group": [1, 1, 1, 1, 1, 2, 2, 2, 2, 2],
                    "weights": [0.34, 0.97, 0.39, 0.8, 0.57, 0.41, 0.19, 0.87, 0.06, 0.34],
                    })
-predictions = df.with_columns(ols_expr.round(2), enet_expr.round(2), lasso_expr.round(2))
 
-print(predictions)
+lasso_expr = pl.col("y").least_squares.lasso(pl.col("x1"), pl.col("x2"), alpha=0.0001, add_intercept=True).over("group")
+wls_expr = pls.least_squares_from_formula("y ~ x1 + x2 -1", sample_weights=pl.col("weights"))
+
+predictions = df.with_columns(lasso_expr.round(2).alias("predictions_lasso"),
+                              wls_expr.round(2).alias("predictions_wls"))
+
+print(predictions.head(5))
 ```
 ```
-shape: (10, 8)
-┌───────┬───────┬───────┬───────┬─────────┬─────────────────┬──────────────────┬───────────────────┐
-│ y     ┆ x1    ┆ x2    ┆ group ┆ weights ┆ predictions_ols ┆ predictions_enet ┆ predictions_lasso │
-│ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---     ┆ ---             ┆ ---              ┆ ---               │
-│ f64   ┆ f64   ┆ f64   ┆ i64   ┆ f64     ┆ f32             ┆ f32              ┆ f32               │
-╞═══════╪═══════╪═══════╪═══════╪═════════╪═════════════════╪══════════════════╪═══════════════════╡
-│ 1.16  ┆ 0.72  ┆ 0.24  ┆ 1     ┆ 0.34    ┆ 0.97            ┆ 0.93             ┆ 0.93              │
-│ -2.16 ┆ -2.43 ┆ 0.18  ┆ 1     ┆ 0.97    ┆ -2.23           ┆ -2.19            ┆ -2.18             │
-│ -1.57 ┆ -0.63 ┆ -0.95 ┆ 1     ┆ 0.39    ┆ -1.54           ┆ -1.52            ┆ -1.54             │
-│ 0.21  ┆ 0.05  ┆ 0.23  ┆ 1     ┆ 0.8     ┆ 0.29            ┆ 0.27             ┆ 0.27              │
-│ 0.22  ┆ -0.07 ┆ 0.44  ┆ 1     ┆ 0.57    ┆ 0.37            ┆ 0.35             ┆ 0.36              │
-│ 1.6   ┆ 0.65  ┆ 1.01  ┆ 2     ┆ 0.41    ┆ 1.6             ┆ 1.62             ┆ 1.62              │
-│ -2.11 ┆ -0.02 ┆ -2.08 ┆ 2     ┆ 0.19    ┆ -2.11           ┆ -2.08            ┆ -2.05             │
-│ -2.92 ┆ -1.64 ┆ -1.36 ┆ 2     ┆ 0.87    ┆ -2.91           ┆ -2.92            ┆ -2.92             │
-│ -0.86 ┆ -0.92 ┆ 0.01  ┆ 2     ┆ 0.06    ┆ -0.87           ┆ -0.87            ┆ -0.88             │
-│ 0.47  ┆ -0.27 ┆ 0.75  ┆ 2     ┆ 0.34    ┆ 0.48            ┆ 0.49             ┆ 0.47              │
-└───────┴───────┴───────┴───────┴─────────┴─────────────────┴──────────────────┴───────────────────┘
+shape: (5, 7)
+┌───────┬───────┬───────┬───────┬─────────┬───────────────────┬─────────────────┐
+│ y     ┆ x1    ┆ x2    ┆ group ┆ weights ┆ predictions_lasso ┆ predictions_wls │
+│ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---     ┆ ---               ┆ ---             │
+│ f64   ┆ f64   ┆ f64   ┆ i64   ┆ f64     ┆ f32               ┆ f32             │
+╞═══════╪═══════╪═══════╪═══════╪═════════╪═══════════════════╪═════════════════╡
+│ 1.16  ┆ 0.72  ┆ 0.24  ┆ 1     ┆ 0.34    ┆ 0.97              ┆ 0.93            │
+│ -2.16 ┆ -2.43 ┆ 0.18  ┆ 1     ┆ 0.97    ┆ -2.23             ┆ -2.18           │
+│ -1.57 ┆ -0.63 ┆ -0.95 ┆ 1     ┆ 0.39    ┆ -1.54             ┆ -1.54           │
+│ 0.21  ┆ 0.05  ┆ 0.23  ┆ 1     ┆ 0.8     ┆ 0.29              ┆ 0.27            │
+│ 0.22  ┆ -0.07 ┆ 0.44  ┆ 1     ┆ 0.57    ┆ 0.37              ┆ 0.36            │
+└───────┴───────┴───────┴───────┴─────────┴───────────────────┴─────────────────┘
 ```
 
-A `mode` parameter is used to set the type of the output returned by all methods (`"predictions", "residuals", "coefficients"`).
-Defaults to returning predictions.
+The `mode` parameter is used to set the type of the output returned by all methods (`"predictions", "residuals", "coefficients"`).
+It defaults to returning predictions matching the input's length.
 
-In case `"coefficients"` is passed the output's shape is the number of features specified, and otherwise
-the output will match the input's length. See below:
+In case `"coefficients"` is set the output's shape is the number of features specified, see below:
 
 ```python
 coefficients = df.select(pl.col("y").least_squares.from_formula("x1 + x2", mode="coefficients")
                          .alias("coefficients").round(2))
-
 print(coefficients)
 ```
 ```
 shape: (3, 1)
 ┌──────────────┐
 │ coefficients │
 │ ---          │
@@ -128,56 +95,57 @@
 ╞══════════════╡
 │ 0.98         │ <-- x1
 │ 0.99         │ <-- x2
 │ 0.0          │ <-- intercept added by formula api
 └──────────────┘
 ```
 
-The only exception is dynamic models (e.g. recursive or rolling window least squares) where the coefficients as of each
-sample are recorded in a `list[f32]` dtype (the length of each list is number of features).
-
-```python
-coefficients_rls = df.select(pl.col("y").least_squares.rls(
-                pl.col("x1"),
-                pl.col("x2"),
-                mode="coefficients",
-                half_life=None, # equivalent to expanding window (no forgetting)
-                initial_state_covariance=0.25,  # inversely proportional to L2 prior
-                initial_state_mean=[0.0, 0.0],  # custom prior
-            ).alias("coefficients_rls"))
-
-print(coefficients_rls)
-```
-```
-shape: (10, 1)
-┌──────────────────────┐
-│ coefficients_rls     │
-│ ---                  │
-│ list[f32]            │
-╞══════════════════════╡
-│ [0.182517, 0.060839] │
-│ [0.583966, 0.010787] │
-│ [0.646492, 0.233397] │
-│ [0.646885, 0.239023] │
-│ [0.645457, 0.252556] │
-│ [0.686584, 0.395498] │
-│ [0.666145, 0.647716] │
-│ [0.759064, 0.727013] │
-│ [0.77024, 0.723971]  │
-│ [0.765996, 0.73275]  │
-└──────────────────────┘
-```
-
 Supported Models
 ------------
 
 Currently, this extension package supports the following variants:
 - Ordinary Least Squares: ```least_squares.ols```
 - Weighted Least Squares: ```least_squares.wls```
 - Regularized Least Squares (Lasso / Ridge / Elastic Net) ```least_squares.{lasso, ridge, elastic_net}```
 - Non-negative Least Squares: ```least_squares.nnls```
-- Formula API: ```least_squares.from_formula```
+
+As well as efficient implementations of moving window models:
 - Recursive Least Squares: ```least_squares.rls```
+- Rolling / Expanding Window OLS: ```least_squares.{rolling_ols, expanding_ols}```
+
+An arbitrary combination of sample_weights, L1/L2 penalties, and non-negativity constraints can be specified with
+the ```least_squares.from_formula``` and ```least_squares.least_squares``` entry-points.
+
+Benchmark
+------------
+The usual caveats of benchmarks apply here, but the below should still be indicative of the
+type of performance improvements to expect when using this package.
+
+This benchmark was run on randomly generated data with [pyperf](https://github.com/psf/pyperf) on my Apple M2 Max macbook
+(32GB RAM, MacOS Sonoma 14.2.1). See [benchmark.py](./tests/benchmark.py) for implementation.
 
-Notice that an arbitrary combination of sample_weights, L1/L2 penalties, and non-negativity constraint can be used with
-both the ```least_squares.from_formula``` and ```least_squares.least_squares``` (except for `least_squares.rls`).
+<a id="bennchmark"></a>
 
+### n_samples=2_000, n_features=5
+
+| Model                   | polars_ols       | Python Benchmark  | Benchmark Type | Speed-up vs Python Benchmark |
+|-------------------------|------------------|-------------------|----------------|------------------------------|
+| Least Squares           | 283 ± 4 us       | 509 ± 313 us      | Numpy          | 1.8x                         |
+| Ridge                   | 262 ± 3 us       | 369 ± 231 us      | Numpy          | 1.4x                         |
+| Weighted Least Squares  | 493 ± 7 us       | 2.13 ms ± 0.22 ms | Statsmodels    | 4.3x                         |
+| Elastic Net             | 326 ± 3 us       | 87.3 ms ± 9.0 ms  | Sklearn        | 268.2x                       |
+| Recursive Least Squares | 1.39 ms ± 0.01 ms| 22.3 ms ± 0.2 ms  | Statsmodels    | 16.0x                        |
+| Rolling Least Squares   | 2.72 ms ± 0.03 ms| 22.3 ms ± 0.2 ms  | Statsmodels    | 8.2x                         |
+
+### n_samples=10_000, n_features=100
+| Model                   | polars_ols       | Python Benchmark  | Benchmark Type | Speed-up vs Python Benchmark |
+|-------------------------|------------------|-------------------|----------------|------------------------------|
+| Least Squares           | 15.6 ms ± 0.2 ms| 29.9 ms ± 8.6 ms  | Numpy          | 1.9x                         |
+| Ridge                   | 5.81 ms ± 0.05 ms| 5.21 ms ± 0.94 ms | Numpy          | 0.9x                         |
+| Weighted Least Squares  | 16.8 ms ± 0.2 ms| 82.4 ms ± 9.1 ms  | Statsmodels    | 4.9x                         |
+| Elastic Net             | 20.9 ms ± 0.3 ms| 134 ms ± 21 ms    | Sklearn        | 6.4x                         |
+| Recursive Least Squares | 163 ms ± 28 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 24.5x                        |
+| Rolling Least Squares   | 390 ms ± 10 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 10.2x                        |
+
+Numpy's `lstsq` is already a highly optimized call into LAPACK and so the scope for speed-up is limited.
+However, we can achieve substantial speed-ups for the more complex models by working entirely in rust
+and avoiding overhead from back and forth into python.
```

