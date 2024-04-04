# Comparing `tmp/polars_qt-0.1.0.tar.gz` & `tmp/polars_qt-0.1.1.tar.gz`

## Comparing `polars_qt-0.1.0.tar` & `polars_qt-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 polars_qt-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3533 2024-04-04 12:45:12.000000 polars_qt-0.1.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127       74 2024-04-04 12:45:12.000000 polars_qt-0.1.0/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-04 12:45:12.000000 polars_qt-0.1.0/.python-version
--rw-r--r--   0     1001      127      579 2024-04-04 12:45:12.000000 polars_qt-0.1.0/Makefile
--rw-r--r--   0     1001      127       70 2024-04-04 12:45:12.000000 polars_qt-0.1.0/README.md
--rw-r--r--   0     1001      127       37 2024-04-04 12:45:12.000000 polars_qt-0.1.0/polars_qt/__init__.py
--rw-r--r--   0     1001      127      574 2024-04-04 12:45:12.000000 polars_qt-0.1.0/polars_qt/funcs.py
--rw-r--r--   0     1001      127      356 2024-04-04 12:45:12.000000 polars_qt-0.1.0/polars_qt/qt.py
--rw-r--r--   0     1001      127     2597 2024-04-04 12:45:12.000000 polars_qt-0.1.0/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-04 12:45:12.000000 polars_qt-0.1.0/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-04 12:45:12.000000 polars_qt-0.1.0/rust-toolchain.toml
--rw-r--r--   0     1001      127      224 2024-04-04 12:45:12.000000 polars_qt-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-04 12:45:12.000000 polars_qt-0.1.0/src/rolling_rank.rs
--rw-r--r--   0     1001      127      587 2024-04-04 12:45:12.000000 polars_qt-0.1.0/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127    33830 2024-04-04 12:45:31.000000 polars_qt-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      550 2024-04-04 12:45:12.000000 polars_qt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_qt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 polars_qt-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     3533 2024-04-04 14:52:55.000000 polars_qt-0.1.1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127       74 2024-04-04 14:52:55.000000 polars_qt-0.1.1/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-04 14:52:55.000000 polars_qt-0.1.1/.python-version
+-rw-r--r--   0     1001      127      601 2024-04-04 14:52:55.000000 polars_qt-0.1.1/Makefile
+-rw-r--r--   0     1001      127     1448 2024-04-04 14:52:55.000000 polars_qt-0.1.1/README.md
+-rw-r--r--   0     1001      127       37 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/__init__.py
+-rw-r--r--   0     1001      127      960 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/funcs.py
+-rw-r--r--   0     1001      127      437 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/qt.py
+-rw-r--r--   0     1001      127     2597 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-04 14:52:55.000000 polars_qt-0.1.1/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-04 14:52:55.000000 polars_qt-0.1.1/rust-toolchain.toml
+-rw-r--r--   0     1001      127      473 2024-04-04 14:52:55.000000 polars_qt-0.1.1/src/if_then.rs
+-rw-r--r--   0     1001      127      237 2024-04-04 14:52:55.000000 polars_qt-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-04 14:52:55.000000 polars_qt-0.1.1/src/rolling_rank.rs
+-rw-r--r--   0     1001      127      837 2024-04-04 14:52:55.000000 polars_qt-0.1.1/tests/test_if_then.py
+-rw-r--r--   0     1001      127      587 2024-04-04 14:52:55.000000 polars_qt-0.1.1/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127    33830 2024-04-04 14:53:07.000000 polars_qt-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      550 2024-04-04 14:52:55.000000 polars_qt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 polars_qt-0.1.1/PKG-INFO
```

### Comparing `polars_qt-0.1.0/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.1/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.0/Makefile` & `polars_qt-0.1.1/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 	# .venv/bin/python -m ruff check . --fix --exit-non-zero-on-fix
 	# .venv/bin/python -m ruff format polars_qt tests
 	# .venv/bin/mypy polars_qt tests
 
 test: .venv
 	.venv/bin/python -m pytest tests
 
+dev: maturin develop
+
```

### Comparing `polars_qt-0.1.0/polars_qt/utils.py` & `polars_qt-0.1.1/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.0/src/rolling_rank.rs` & `polars_qt-0.1.1/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.0/tests/test_rolling_rank.py` & `polars_qt-0.1.1/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.0/Cargo.lock` & `polars_qt-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -631,15 +631,15 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
 ]
```

### Comparing `polars_qt-0.1.0/pyproject.toml` & `polars_qt-0.1.1/pyproject.toml`

 * *Files identical despite different names*

