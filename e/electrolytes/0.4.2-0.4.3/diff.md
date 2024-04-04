# Comparing `tmp/electrolytes-0.4.2.tar.gz` & `tmp/electrolytes-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.4.2.tar", last modified: Thu Feb 29 14:13:04 2024, max compression
+gzip compressed data, was "electrolytes-0.4.3.tar", last modified: Thu Apr  4 20:21:51 2024, max compression
```

## Comparing `electrolytes-0.4.2.tar` & `electrolytes-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:13:04.127753 electrolytes-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35130 2024-02-29 14:12:55.000000 electrolytes-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-02-29 14:13:04.127753 electrolytes-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-02-29 14:12:55.000000 electrolytes-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:13:04.123753 electrolytes-0.4.2/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-02-29 14:12:55.000000 electrolytes-0.4.2/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-02-29 14:12:55.000000 electrolytes-0.4.2/electrolytes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   174238 2024-02-29 14:12:55.000000 electrolytes-0.4.2/electrolytes/db1.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:12:55.000000 electrolytes-0.4.2/electrolytes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:13:04.127753 electrolytes-0.4.2/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-02-29 14:13:04.000000 electrolytes-0.4.2/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-29 14:13:04.000000 electrolytes-0.4.2/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 14:13:04.000000 electrolytes-0.4.2/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-29 14:13:04.000000 electrolytes-0.4.2/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-29 14:13:04.000000 electrolytes-0.4.2/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-29 14:13:04.000000 electrolytes-0.4.2/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-29 14:12:55.000000 electrolytes-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 14:13:04.127753 electrolytes-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:13:04.127753 electrolytes-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-29 14:12:55.000000 electrolytes-0.4.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-29 14:12:55.000000 electrolytes-0.4.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-29 14:12:55.000000 electrolytes-0.4.2/tests/test_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:21:51.088262 electrolytes-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35130 2024-04-04 20:21:46.000000 electrolytes-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-04 20:21:51.088262 electrolytes-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-04 20:21:46.000000 electrolytes-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:21:51.084262 electrolytes-0.4.3/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-04 20:21:46.000000 electrolytes-0.4.3/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-04 20:21:46.000000 electrolytes-0.4.3/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174238 2024-04-04 20:21:46.000000 electrolytes-0.4.3/electrolytes/db1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:21:46.000000 electrolytes-0.4.3/electrolytes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:21:51.088262 electrolytes-0.4.3/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-04 20:21:51.000000 electrolytes-0.4.3/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-04 20:21:51.000000 electrolytes-0.4.3/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:21:51.000000 electrolytes-0.4.3/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 20:21:51.000000 electrolytes-0.4.3/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-04 20:21:51.000000 electrolytes-0.4.3/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 20:21:51.000000 electrolytes-0.4.3/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-04 20:21:46.000000 electrolytes-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:21:51.088262 electrolytes-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:21:51.088262 electrolytes-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-04 20:21:46.000000 electrolytes-0.4.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-04 20:21:46.000000 electrolytes-0.4.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 20:21:46.000000 electrolytes-0.4.3/tests/test_lock.py
```

### Comparing `electrolytes-0.4.2/LICENSE.txt` & `electrolytes-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.4.2/PKG-INFO` & `electrolytes-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.4.2
+Version: 0.4.3
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -21,33 +21,33 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: typer<0.10,>=0.9.0
+Requires-Dist: typer-slim<0.13,>=0.12.0
 Requires-Dist: pydantic<3,>=2.0.3
 Requires-Dist: filelock<4,>=3.12.3
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Provides-Extra: type
-Requires-Dist: mypy==1.*; extra == "type"
-Requires-Dist: pytest<9,>=7; extra == "type"
+Requires-Dist: ruff; extra == "lint"
+Provides-Extra: typing
+Requires-Dist: mypy==1.*; extra == "typing"
+Requires-Dist: pytest<9,>=7; extra == "typing"
 Provides-Extra: test
 Requires-Dist: pytest<9,>=7; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # electrolytes
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 [![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
 **electrolytes** provides command-line and programmatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
```

### Comparing `electrolytes-0.4.2/README.md` & `electrolytes-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # electrolytes
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 [![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
 **electrolytes** provides command-line and programmatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
```

### Comparing `electrolytes-0.4.2/electrolytes/__init__.py` & `electrolytes-0.4.3/electrolytes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,32 @@
     ValidationInfo,
     model_validator,
     TypeAdapter,
 )
 from filelock import FileLock
 from typer import get_app_dir
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 
 class Constituent(BaseModel, populate_by_name=True, frozen=True):
     id: Optional[int] = None
     name: str
-    u_neg: Annotated[list[float], Field(alias="uNeg")] = (
-        []
-    )  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-    u_pos: Annotated[list[float], Field(alias="uPos")] = (
-        []
-    )  # [+1, +2, +3, ..., +pos_count]
-    pkas_neg: Annotated[list[float], Field(alias="pKaNeg")] = (
-        []
-    )  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-    pkas_pos: Annotated[list[float], Field(alias="pKaPos")] = (
-        []
-    )  # [+1, +2, +3, ..., +pos_count]
+    u_neg: Annotated[
+        list[float], Field(alias="uNeg")
+    ] = []  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+    u_pos: Annotated[
+        list[float], Field(alias="uPos")
+    ] = []  # [+1, +2, +3, ..., +pos_count]
+    pkas_neg: Annotated[
+        list[float], Field(alias="pKaNeg")
+    ] = []  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+    pkas_pos: Annotated[
+        list[float], Field(alias="pKaPos")
+    ] = []  # [+1, +2, +3, ..., +pos_count]
     neg_count: Annotated[int, Field(alias="negCount", validate_default=True)] = None  # type: ignore
     pos_count: Annotated[int, Field(alias="posCount", validate_default=True)] = None  # type: ignore
 
     def mobilities(self) -> Sequence[float]:
         n = max(self.neg_count, self.pos_count, 3)
         ret = (
             [0.0] * (n - self.pos_count)
@@ -184,19 +184,21 @@
     def _save_user_constituents(self) -> None:
         data = _dump_constituents(list(self._user_constituents.values()))
         self._user_constituents_file.parent.mkdir(parents=True, exist_ok=True)
         with self:
             self._user_constituents_file.write_bytes(data)
         self._user_constituents_dirty = False
 
-    def __enter__(self) -> None:
+    def __enter__(self) -> "_Database":
         if not self._user_constituents_lock.is_locked:
             self._invalidate_user_constituents()
         self._user_constituents_lock.acquire()
 
+        return self
+
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         try:
             if (
                 self._user_constituents_lock.lock_counter == 1
                 and self._user_constituents_dirty
             ):
                 self._save_user_constituents()
```

### Comparing `electrolytes-0.4.2/electrolytes/__main__.py` & `electrolytes-0.4.3/electrolytes/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,62 @@
         name for name in database.user_defined() if name.startswith(incomplete.upper())
     ]
 
 
 @app.command()
 def add(
     name: Annotated[str, typer.Argument(autocompletion=complete_name_user_defined)],
-    p1: Annotated[tuple[float, float], typer.Option("+1", help="Mobility (*1e-9) and pKa for +1", show_default=False)] = (None, None),  # type: ignore
-    p2: Annotated[tuple[float, float], typer.Option("+2", help="Mobility (*1e-9) and pKa for +2", show_default=False)] = (None, None),  # type: ignore
-    p3: Annotated[tuple[float, float], typer.Option("+3", help="Mobility (*1e-9) and pKa for +3", show_default=False)] = (None, None),  # type: ignore
-    p4: Annotated[tuple[float, float], typer.Option("+4", help="Mobility (*1e-9) and pKa for +4", show_default=False)] = (None, None),  # type: ignore
-    p5: Annotated[tuple[float, float], typer.Option("+5", help="Mobility (*1e-9) and pKa for +5", show_default=False)] = (None, None),  # type: ignore
-    p6: Annotated[tuple[float, float], typer.Option("+6", help="Mobility (*1e-9) and pKa for +6", show_default=False)] = (None, None),  # type: ignore
-    m1: Annotated[tuple[float, float], typer.Option("-1", help="Mobility (*1e-9) and pKa for -1", show_default=False)] = (None, None),  # type: ignore
-    m2: Annotated[tuple[float, float], typer.Option("-2", help="Mobility (*1e-9) and pKa for -2", show_default=False)] = (None, None),  # type: ignore
-    m3: Annotated[tuple[float, float], typer.Option("-3", help="Mobility (*1e-9) and pKa for -3", show_default=False)] = (None, None),  # type: ignore
-    m4: Annotated[tuple[float, float], typer.Option("-4", help="Mobility (*1e-9) and pKa for -4", show_default=False)] = (None, None),  # type: ignore
-    m5: Annotated[tuple[float, float], typer.Option("-5", help="Mobility (*1e-9) and pKa for -5", show_default=False)] = (None, None),  # type: ignore
-    m6: Annotated[tuple[float, float], typer.Option("-6", help="Mobility (*1e-9) and pKa for -6", show_default=False)] = (None, None),  # type: ignore
+    p1: Annotated[
+        tuple[float, float],
+        typer.Option("+1", help="Mobility (*1e-9) and pKa for +1", show_default=False),
+    ] = (None, None),  # type: ignore
+    p2: Annotated[
+        tuple[float, float],
+        typer.Option("+2", help="Mobility (*1e-9) and pKa for +2", show_default=False),
+    ] = (None, None),  # type: ignore
+    p3: Annotated[
+        tuple[float, float],
+        typer.Option("+3", help="Mobility (*1e-9) and pKa for +3", show_default=False),
+    ] = (None, None),  # type: ignore
+    p4: Annotated[
+        tuple[float, float],
+        typer.Option("+4", help="Mobility (*1e-9) and pKa for +4", show_default=False),
+    ] = (None, None),  # type: ignore
+    p5: Annotated[
+        tuple[float, float],
+        typer.Option("+5", help="Mobility (*1e-9) and pKa for +5", show_default=False),
+    ] = (None, None),  # type: ignore
+    p6: Annotated[
+        tuple[float, float],
+        typer.Option("+6", help="Mobility (*1e-9) and pKa for +6", show_default=False),
+    ] = (None, None),  # type: ignore
+    m1: Annotated[
+        tuple[float, float],
+        typer.Option("-1", help="Mobility (*1e-9) and pKa for -1", show_default=False),
+    ] = (None, None),  # type: ignore
+    m2: Annotated[
+        tuple[float, float],
+        typer.Option("-2", help="Mobility (*1e-9) and pKa for -2", show_default=False),
+    ] = (None, None),  # type: ignore
+    m3: Annotated[
+        tuple[float, float],
+        typer.Option("-3", help="Mobility (*1e-9) and pKa for -3", show_default=False),
+    ] = (None, None),  # type: ignore
+    m4: Annotated[
+        tuple[float, float],
+        typer.Option("-4", help="Mobility (*1e-9) and pKa for -4", show_default=False),
+    ] = (None, None),  # type: ignore
+    m5: Annotated[
+        tuple[float, float],
+        typer.Option("-5", help="Mobility (*1e-9) and pKa for -5", show_default=False),
+    ] = (None, None),  # type: ignore
+    m6: Annotated[
+        tuple[float, float],
+        typer.Option("-6", help="Mobility (*1e-9) and pKa for -6", show_default=False),
+    ] = (None, None),  # type: ignore
     force: Annotated[
         bool,
         typer.Option(
             "-f",
             help="Do not prompt before replacing a user-defined component with the same name",
         ),
     ] = False,
@@ -96,15 +132,15 @@
 
 
 @app.command()
 def info(
     names: Annotated[
         Optional[list[str]],
         typer.Argument(help="Component names", autocompletion=complete_name),
-    ] = None
+    ] = None,
 ) -> None:
     """
     Show the properties of components.
 
     If no names are given, print the number of components in the database.
     """
     if names:
@@ -154,15 +190,15 @@
 @app.command()
 def ls(
     user: Annotated[
         Optional[bool],
         typer.Option(
             "--user/--default", help="List only user-defined/default components"
         ),
-    ] = None
+    ] = None,
 ) -> None:
     """List components in the database."""
 
     if user:
         names = database.user_defined()
     elif user is not None:
         names = [name for name in database if not database.is_user_defined(name)]
@@ -240,15 +276,15 @@
 @app.callback()
 def common(
     version: Annotated[
         bool,
         typer.Option(
             "--version", help="Show version and exit.", callback=version_callback
         ),
-    ] = False
+    ] = False,
 ) -> None:
     """Database of electrolytes and their properties."""
     pass
 
 
 if __name__ == "__main__":
     app(prog_name=__package__)
```

### Comparing `electrolytes-0.4.2/electrolytes/db1.json` & `electrolytes-0.4.3/electrolytes/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.4.2/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.4.3/electrolytes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.4.2
+Version: 0.4.3
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -21,33 +21,33 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: typer<0.10,>=0.9.0
+Requires-Dist: typer-slim<0.13,>=0.12.0
 Requires-Dist: pydantic<3,>=2.0.3
 Requires-Dist: filelock<4,>=3.12.3
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Provides-Extra: type
-Requires-Dist: mypy==1.*; extra == "type"
-Requires-Dist: pytest<9,>=7; extra == "type"
+Requires-Dist: ruff; extra == "lint"
+Provides-Extra: typing
+Requires-Dist: mypy==1.*; extra == "typing"
+Requires-Dist: pytest<9,>=7; extra == "typing"
 Provides-Extra: test
 Requires-Dist: pytest<9,>=7; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # electrolytes
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 [![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
 **electrolytes** provides command-line and programmatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
```

### Comparing `electrolytes-0.4.2/pyproject.toml` & `electrolytes-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,24 +25,24 @@
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "typer>=0.9.0,<0.10",
+    "typer-slim>=0.12.0,<0.13",
     "pydantic>=2.0.3,<3",
     "filelock>=3.12.3,<4",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
-lint = ["black"]
-type = [
+lint = ["ruff"]
+typing = [
     "mypy==1.*",
     "pytest>=7,<9",
 ]
 test = [
     "pytest>=7,<9",
     "pytest-cov",
 ]
```

### Comparing `electrolytes-0.4.2/tests/test_api.py` & `electrolytes-0.4.3/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
 
 import electrolytes
-from electrolytes import *
+from electrolytes import Constituent, database
 
 
 def test_version() -> None:
     assert isinstance(electrolytes.__version__, str)
 
 
 def test_list_components() -> None:
     assert database
-    l = list(database)
-    assert len(l) == len(database)
-    assert isinstance(l[0], str)
-    assert l == sorted(l)
-    assert "LYSINE" in l
-    assert "CYSTINE" in l
-    assert "SILVER" in l
+    lst = list(database)
+    assert len(lst) == len(database)
+    assert isinstance(lst[0], str)
+    assert lst == sorted(lst)
+    assert "LYSINE" in lst
+    assert "CYSTINE" in lst
+    assert "SILVER" in lst
 
 
 def test_get_component() -> None:
     c = database["LYSINE"]
     assert isinstance(c, Constituent)
     assert c.name == "LYSINE"
     assert c.name in database
```

### Comparing `electrolytes-0.4.2/tests/test_cli.py` & `electrolytes-0.4.3/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from typer.testing import CliRunner
 
 import electrolytes
-from electrolytes import *
+from electrolytes import Constituent, database
 from electrolytes.__main__ import app
 
 
 runner = CliRunner()
 
 
 def test_version() -> None:
```

### Comparing `electrolytes-0.4.2/tests/test_lock.py` & `electrolytes-0.4.3/tests/test_lock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import pytest
-
 import subprocess
 from time import sleep
 
-from electrolytes import *
+from electrolytes import Constituent, database
 
 
 def test_lock_api_cli() -> None:
     name = "TES7342982891"
     try:
         del database[name]
     except KeyError:
```

