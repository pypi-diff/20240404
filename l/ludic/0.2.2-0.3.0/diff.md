# Comparing `tmp/ludic-0.2.2.tar.gz` & `tmp/ludic-0.3.0.tar.gz`

## Comparing `ludic-0.2.2.tar` & `ludic-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,74 @@
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.2.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.2.2/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.2.2/mkdocs.yaml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.2.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 ludic-0.2.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/catalog.md
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/getting-started.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/htmx.md
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/requirements.txt
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.2.2/docs/web-framework.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/README.md
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/bulk_update.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/click_to_edit.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/click_to_load.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/delete_row.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/edit_row.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 ludic-0.2.2/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/__init__.py
--rw-r--r--   0        0        0    15439 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/attrs.py
--rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/base.py
--rw-r--r--   0        0        0    19060 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/css.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/format.py
--rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/py.typed
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/styles.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/types.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/utils.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/forms.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/lists.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/loaders.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/tables.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/typography.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/catalog/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/__init__.py
--rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/app.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/parsers.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/requests.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/responses.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 ludic-0.2.2/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_components.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_elements.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_exceptions.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_formatting.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_styles.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.2.2/tests/test_types.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.2.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.2.2/LICENCE
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 ludic-0.2.2/README.md
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ludic-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 ludic-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.3.0/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.3.0/mkdocs.yaml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.3.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/catalog.md
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/getting-started.md
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/htmx.md
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/web-framework.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/README.md
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/bulk_update.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/click_to_load.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/delete_row.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/edit_row.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/infinite_scroll.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/__init__.py
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/attrs.py
+-rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/components.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/format.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/utils.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/items.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/collect.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/themes.py
+-rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/types.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/app.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/parsers.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/requests.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/responses.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_components.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_elements.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_formatting.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_styles.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_themes.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/web/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.3.0/LICENCE
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 ludic-0.3.0/README.md
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ludic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 ludic-0.3.0/PKG-INFO
```

### Comparing `ludic-0.2.2/.pre-commit-config.yaml` & `ludic-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/CONTRIBUTING.md` & `ludic-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/mkdocs.yaml` & `ludic-0.3.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/.github/workflows/publish.yaml` & `ludic-0.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/.github/workflows/test.yaml` & `ludic-0.3.0/.github/workflows/test.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -49,13 +49,13 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools setuptools_scm
         python -m pip install .[full,test]
 
     - name: Test with pytest
       run: |
-        pytest --cov=. --cov-report xml:coverage.xml
+        pytest --cov --cov-report xml:coverage.xml
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v4.1.0
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `ludic-0.2.2/docs/catalog.md` & `ludic-0.3.0/docs/catalog.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,26 +106,26 @@
     </li>
     <li id="about">
         <a href="/about">About</a>
     </li>
 </ul>
 ```
 
-## Lists
+## Items
 
-The module `ludic.catalog.lists` contains the following components:
+The module `ludic.catalog.items` contains the following components:
 
 * `Pairs`
 * `Key`
 * `Value`
 
 Here is the definition:
 
 ```python
-# ludic/catalog/lists.py
+# ludic/catalog/items.py
 
 class Key(Component[PrimitiveChildren, GlobalAttrs]):
     def render(self) -> dt: ...
 
 class Value(Component[PrimitiveChildren, GlobalAttrs]):
     def render(self) -> dd: ...
 
@@ -135,15 +135,15 @@
 class Pairs(Component[Key | Value, PairsAttrs]):
     def render(self) -> dl: ...
 ```
 
 There are two possible ways to instantiate these components:
 
 ```python
-from ludic.catalog.lists import Pairs, Key, Value
+from ludic.catalog.items import Pairs, Key, Value
 
 Pairs(
     Key("Name"),
     Value("John"),
     Key("Age"),
     Value(42),
 )
@@ -279,38 +279,42 @@
 
 class TableHead(Component[AnyChildren, GlobalAttrs]):
     def render(self) -> tr: ...
 
 THead = TypeVar("THead", bound=BaseElement, default=TableHead)
 TRow = TypeVar("TRow", bound=BaseElement, default=TableRow)
 
-class TableType(ComponentStrict[THead, *tuple[TRow, ...], GlobalAttrs]): ...
+class Table(ComponentStrict[THead, *tuple[TRow, ...], GlobalAttrs]): ...
     def render(self) -> table: ...
-
-class Table(TableType[TableHead, TableRow]): ...
 ```
 
 This allows the following instantiations:
 
 ```python
-from ludic.catalog.tables import Table, TableHead, TableRow, TableType
+from ludic.catalog.tables import Table, TableHead, TableRow
+
+Table(
+    TableHead("Name", "Age"),
+    TableRow("John", 42),
+    TableRow("Jane", 23),
+)
+```
+
+You can also specify different types of header and body:
+
+```python
+from ludic.catalog.tables import Table
 
 from your_app.components import PersonHead, PersonRow
 
-TableType[PersonHead, PersonRow](
+Table[PersonHead, PersonRow](
     PersonHead("Name", "Age"),
     PersonRow("John", 42),
     PersonRow("Jane", 23),
 )
-
-Table(
-    TableHead("Name", "Age"),
-    TableRow("John", 42),
-    TableRow("Jane", 23),
-)
 ```
 
 ### Generating Table Rows
 
 !!! warning "Experimental"
 
     This module is in an experimental state. It is not clear yet how to make the generation of tables from annotations and combine them with forms, button actions, and so on. The idea is to make it flexible and extensible.
```

### Comparing `ludic-0.2.2/docs/components.md` & `ludic-0.3.0/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/docs/getting-started.md` & `ludic-0.3.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/docs/htmx.md` & `ludic-0.3.0/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/docs/index.md` & `ludic-0.3.0/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 ## Features
 
 - Seamless **&lt;/&gt; htmx** integration for rapid web development in **pure Python**
 - **Type-Guided components** utilizing Python's typing system
 - Uses the power of **Starlette** and **Async** for high-performance web development
 - Build HTML with the ease and power of Python **f-strings**
+- Add CSS styling to your components with **themes**
 
 ## Ideals
 
 This framework allows HTML generation in Python while utilizing Python's typing system. Our goal is to enable the creation of dynamic web applications with reusable components, all while offering a greater level of type safety than raw HTML.
 
 **Key Ideas:**
 
@@ -48,15 +49,15 @@
     TableHead("Id", "Name"),
     TableRow("1", "John"),
     TableRow("2", "Jane"),
     TableRow("3", "Bob"),
 )
 ```
 
-This structure can be type-checked thanks to Python's rich type system. Additionally, this `Table` component could have **dynamic properties** like sorting or even modification of data on the server.
+This structure can be type-checked thanks to Python's rich type system. Additionally, this `Table` component could have **dynamic properties** like sorting or filtering.
 
 ## Quick Example
 
 ```python
 from ludic.html import b, span
 from ludic.web import LudicApp
```

### Comparing `ludic-0.2.2/docs/web-framework.md` & `ludic-0.3.0/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/examples/README.md` & `ludic-0.3.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/examples/bulk_update.py` & `ludic-0.3.0/examples/bulk_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Annotated, Self, override
 
 from examples import Body, Header, Page, app, init_db
 from ludic.catalog.buttons import ButtonPrimary
 from ludic.catalog.forms import FieldMeta, Form
+from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import ColumnMeta, Table, create_rows
-from ludic.html import span
+from ludic.html import span, style
 from ludic.types import Attrs
 from ludic.web.endpoints import Endpoint
 from ludic.web.parsers import ListParser
 
 db = init_db()
 
 
@@ -25,36 +26,45 @@
 class PeopleAttrs(Attrs):
     people: list[PersonAttrs]
 
 
 class Toast(span):
     id: str = "toast"
     target: str = f"#{id}"
-    styles = {
-        target: {
-            "background": "#E1F0DA",
-            "margin": "10px 20px",
-            "opacity": "0",
-            "transition": "opacity 3s ease-out",
-        },
-        f"{target}.htmx-settling": {
-            "opacity": "100",
-        },
-    }
+    styles = style.use(
+        lambda theme: {
+            Toast.target: {
+                "background": theme.colors.success,
+                "margin": "10px 20px",
+                "opacity": "0",
+                "transition": "opacity 3s ease-out",
+            },
+            f"{Toast.target}.htmx-settling": {
+                "opacity": "100",
+            },
+        }
+    )
 
     @override
     def render(self) -> span:
         return span(*self.children, id=self.id)
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
         Header("Bulk Update"),
-        Body(await PeopleTable.get()),
+        Body(
+            Quote(
+                "This demo shows how to implement a common pattern where rows are "
+                "selected and then bulk updated.",
+                source_url="https://htmx.org/examples/bulk-update/",
+            ),
+            await PeopleTable.get(),
+        ),
     )
 
 
 @app.endpoint("/people/")
 class PeopleTable(Endpoint[PeopleAttrs]):
     @classmethod
     async def post(cls, data: ListParser[PersonAttrs]) -> Toast:
```

### Comparing `ludic-0.2.2/examples/click_to_edit.py` & `ludic-0.3.0/examples/click_to_edit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Annotated, NotRequired, Self, override
 
 from examples import Body, Header, Page, app, init_db
 from ludic.catalog.buttons import ButtonDanger, ButtonPrimary
 from ludic.catalog.forms import FieldMeta, Form, create_fields
-from ludic.catalog.lists import Pairs
+from ludic.catalog.items import Pairs
+from ludic.catalog.quotes import Quote
 from ludic.html import div
 from ludic.types import Attrs
 from ludic.web.endpoints import Endpoint
 from ludic.web.exceptions import NotFoundError
 from ludic.web.parsers import Parser, ValidationError
 
 db = init_db()
@@ -28,15 +29,22 @@
     ]
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
         Header("Click To Edit"),
-        Body(*[Contact(**contact.dict()) for contact in db.contacts.values()]),
+        Body(
+            Quote(
+                "The click to edit pattern provides a way to offer inline editing "
+                "of all or part of a record without a page refresh.",
+                source_url="https://htmx.org/examples/click-to-edit/",
+            ),
+            *[Contact(**contact.dict()) for contact in db.contacts.values()],
+        ),
     )
 
 
 @app.endpoint("/contacts/{id}")
 class Contact(Endpoint[ContactAttrs]):
     @classmethod
     async def get(cls, id: str) -> Self:
```

### Comparing `ludic-0.2.2/examples/click_to_load.py` & `ludic-0.3.0/examples/click_to_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Self, override
 
 from examples import Body, Header, Page, app
 from ludic.attrs import ButtonAttrs
 from ludic.catalog.buttons import ButtonPrimary
+from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.html import td
 from ludic.types import Attrs, Blank, Component, ComponentStrict
 from ludic.web import Endpoint
 from ludic.web.datastructures import QueryParams
 
 
@@ -60,15 +61,22 @@
 
 
 @app.get("/")
 async def index() -> Page:
     slice = await ContactsSlice.get(QueryParams(page=1))
     return Page(
         Header("Click To Edit"),
-        Body(ContactsTable(*slice.render().children)),
+        Body(
+            Quote(
+                "This example shows how to implement click-to-load the next page in "
+                "a table of data.",
+                source_url="https://htmx.org/examples/click-to-load/",
+            ),
+            ContactsTable(*slice.render().children),
+        ),
     )
 
 
 @app.endpoint("/contacts/")
 class ContactsSlice(Endpoint[ContactsSliceAttrs]):
     @classmethod
     async def get(cls, params: QueryParams) -> Self:
```

### Comparing `ludic-0.2.2/examples/delete_row.py` & `ludic-0.3.0/examples/delete_row.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Self, override
 
 from examples import Body, Header, Page, app, init_db
+from ludic.attrs import Attrs, HtmxAttrs
 from ludic.catalog.buttons import ButtonDanger
-from ludic.catalog.tables import TableHead, TableRow
-from ludic.html import table, tbody, thead
-from ludic.types import Attrs
+from ludic.catalog.quotes import Quote
+from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.web.endpoints import Endpoint
 from ludic.web.exceptions import NotFoundError
 
 db = init_db()
 
 
 class PersonAttrs(Attrs):
@@ -22,15 +22,22 @@
     people: list[PersonAttrs]
 
 
 @app.get("/")
 def index() -> Page:
     return Page(
         Header("Delete Row"),
-        Body(PeopleTable.get()),
+        Body(
+            Quote(
+                "This example shows how to implement a delete button that removes "
+                "a table row upon completion.",
+                source_url="https://htmx.org/examples/delete-row/",
+            ),
+            PeopleTable.get(),
+        ),
     )
 
 
 @app.endpoint("/people/{id}")
 class PersonRow(Endpoint[PersonAttrs]):
     @classmethod
     def delete(cls, id: str) -> None:
@@ -51,26 +58,26 @@
 
 @app.endpoint("/people/")
 class PeopleTable(Endpoint[PeopleAttrs]):
     styles = {
         "tr.htmx-swapping td": {
             "opacity": "0",
             "transition": "opacity 1s ease-out",
-        },
+        }
     }
 
     @classmethod
     def get(cls) -> Self:
         return cls(people=[person.dict() for person in db.people.values()])
 
     @override
-    def render(self) -> table:
-        return table(
-            thead(TableHead("Name", "Email", "Active", "")),
-            tbody(
-                *(PersonRow(**person) for person in self.attrs["people"]),
+    def render(self) -> Table[TableHead, PersonRow]:
+        return Table[TableHead, PersonRow](
+            TableHead("Name", "Email", "Active", ""),
+            *(PersonRow(**person) for person in self.attrs["people"]),
+            body_attrs=HtmxAttrs(
                 hx_confirm="Are you sure?",
                 hx_target="closest tr",
                 hx_swap="outerHTML swap:1s",
             ),
             style={"text-align": "center"},
         )
```

### Comparing `ludic-0.2.2/examples/edit_row.py` & `ludic-0.3.0/examples/edit_row.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Annotated, NotRequired, Self, override
 
 from examples import Body, Header, Page, app, init_db
+from ludic.attrs import Attrs, HtmxAttrs
 from ludic.catalog.buttons import ButtonPrimary, ButtonSecondary
-from ludic.catalog.tables import ColumnMeta, TableHead, TableRow
-from ludic.html import div, input, table, tbody, thead
-from ludic.types import Attrs, JavaScript
+from ludic.catalog.forms import InputField
+from ludic.catalog.quotes import Quote
+from ludic.catalog.tables import ColumnMeta, Table, TableHead, TableRow
+from ludic.html import div
+from ludic.types import JavaScript
 from ludic.web.endpoints import Endpoint
 from ludic.web.exceptions import NotFoundError
 from ludic.web.parsers import Parser
 
 db = init_db()
 
 
@@ -22,15 +25,21 @@
     people: list[PersonAttrs]
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
         Header("Edit Row"),
-        Body(await PeopleTable.get()),
+        Body(
+            Quote(
+                "This example shows how to implement editable rows.",
+                source_url="https://htmx.org/examples/edit-row/",
+            ),
+            await PeopleTable.get(),
+        ),
     )
 
 
 @app.endpoint("/people/{id}")
 class PersonRow(Endpoint[PersonAttrs]):
     on_click_script: JavaScript = JavaScript(
         """
@@ -89,16 +98,16 @@
             raise NotFoundError("Person not found")
 
         return cls(**person.dict())
 
     @override
     def render(self) -> TableRow:
         return TableRow(
-            input(name="name", value=self.attrs["name"]),
-            input(name="email", value=self.attrs["email"]),
+            InputField(name="name", value=self.attrs["name"]),
+            InputField(name="email", value=self.attrs["email"]),
             div(
                 ButtonSecondary("Cancel", hx_get=self.url_for(PersonRow)),
                 ButtonPrimary(
                     "Save",
                     hx_put=self.url_for(PersonRow),
                     hx_include="closest tr",
                 ),
@@ -110,17 +119,14 @@
 @app.endpoint("/people/")
 class PeopleTable(Endpoint[PeopleAttrs]):
     @classmethod
     async def get(cls) -> Self:
         return cls(people=[person.dict() for person in db.people.values()])
 
     @override
-    def render(self) -> table:
-        return table(
-            thead(TableHead("Name", "Email", "Action")),
-            tbody(
-                *(PersonRow(**person) for person in self.attrs["people"]),
-                hx_target="closest tr",
-                hx_swap="outerHTML",
-            ),
+    def render(self) -> Table[TableHead, PersonRow]:
+        return Table[TableHead, PersonRow](
+            TableHead("Name", "Email", "Action"),
+            *(PersonRow(**person) for person in self.attrs["people"]),
+            body_attrs=HtmxAttrs(hx_target="closest tr", hx_swap="outerHTML"),
             style={"text-align": "center"},
         )
```

### Comparing `ludic-0.2.2/examples/lazy_loading.py` & `ludic-0.3.0/examples/lazy_loading.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import asyncio
 
-from examples import Body, Header, Loading, Page, app
+from examples import Body, Header, Page, app
 from ludic.catalog.loaders import LazyLoader
+from ludic.catalog.quotes import Quote
 from ludic.html import div, svg
 from ludic.types import Safe
 from ludic.web import Request
 
 
 @app.get("/")
 async def homepage(request: Request) -> Page:
     return Page(
         Header("Lazy Loading"),
         Body(
+            Quote(
+                "This example shows how to lazily load an element on a page.",
+                source_url="https://htmx.org/examples/lazy-load/",
+            ),
             div(
-                LazyLoader(
-                    load_url=request.url_for(load_svg, seconds=3), placeholder=Loading()
-                ),
+                LazyLoader(load_url=request.url_for(load_svg, seconds=3)),
                 style={"text-align": "center"},
-            )
+            ),
         ),
     )
 
 
 @app.get("/load/{seconds:int}")
 async def load_svg(seconds: int) -> svg:
     await asyncio.sleep(seconds)
```

### Comparing `ludic-0.2.2/ludic/attrs.py` & `ludic-0.3.0/ludic/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Annotated, Literal
 
 from .base import Attrs as Attrs
 from .base import NoAttrs as NoAttrs
-from .css import CSSProperties
+from .styles import CSSProperties
 
 
 class Alias(str):
     """Alias type for attributes."""
 
 
 class HtmlAttrs(Attrs, total=False):
```

### Comparing `ludic-0.2.2/ludic/base.py` & `ludic-0.3.0/ludic/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,28 @@
-from abc import ABCMeta, abstractmethod
+from abc import ABCMeta
 from collections.abc import Callable, Iterator, Mapping, MutableMapping, Sequence
 from typing import (
     Any,
     ClassVar,
     Generic,
     Never,
     TypeAlias,
     TypedDict,
     Unpack,
     cast,
 )
 
 from typing_extensions import TypeVar, TypeVarTuple
 
-from .css import CSSProperties
 from .format import FormatContext, format_attrs, format_element
+from .styles import GlobalStyles, Theme, get_default_theme
 from .utils import get_element_attrs_annotations
 
 ELEMENT_REGISTRY: MutableMapping[str, list[type["BaseElement"]]] = {}
 
-# FIXME: Currently, it is impossible to properly type nested CSS properties
-# defined similar as in SCSS, it will be possible when the following PEP is
-# implemented and supported by type checkers: https://peps.python.org/pep-0728/
-GlobalStyles = Mapping[str, "CSSProperties | GlobalStyles"]
-"""CSS styles for elements or components which are defined by setting the ``styles``
-class property.
-
-Example usage:
-
-    class Page(Component[AnyChildren, NoAttrs]):
-        styles = {
-            "body": {
-                "background-color": "red",
-            },
-        }
-"""
-
 
 class Safe(str):
     """Marker for a string that is safe to use as is without HTML escaping.
 
     That means the content of the string is not escaped when rendered.
 
     Usage:
@@ -88,21 +71,24 @@
 
 
 class BaseElement(metaclass=ABCMeta):
     html_header: ClassVar[str | None] = None
     html_name: ClassVar[str | None] = None
 
     always_pair: ClassVar[bool] = False
-    styles: ClassVar[GlobalStyles] = {}
-
     formatter: ClassVar[FormatContext] = FormatContext("element_formatter")
 
+    classes: ClassVar[Sequence[str]] = []
+    styles: ClassVar["GlobalStyles"] = {}
+
     children: Sequence[Any]
     attrs: Mapping[str, Any]
 
+    _theme: Theme | None = None
+
     def __init_subclass__(cls) -> None:
         ELEMENT_REGISTRY.setdefault(cls.__name__, [])
         ELEMENT_REGISTRY[cls.__name__].append(cls)
 
     def __str__(self) -> str:
         return self.to_string()
 
@@ -121,40 +107,69 @@
     def __eq__(self, other: Any) -> bool:
         return (
             type(self) is type(other)
             and self.children == other.children
             and self.attrs == other.attrs
         )
 
-    def _format_attributes(self, is_html: bool = False) -> str:
+    def _format_attributes(
+        self, classes: list[str] | None = None, is_html: bool = False
+    ) -> str:
         attrs: dict[str, Any]
         if is_html:
-            attrs = format_attrs(type(self), dict(self.attrs), True)
+            attrs = format_attrs(type(self), dict(self.attrs), is_html=True)
         else:
             attrs = self.aliased_attrs
+
+        if classes:
+            if "class" in attrs:
+                attrs["class"] += " " + " ".join(classes)
+            else:
+                attrs["class"] = " ".join(classes)
+
         return " ".join(f'{key}="{value}"' for key, value in attrs.items())
 
     def _format_children(
         self,
         format_fun: Callable[[Any], str] = format_element,
     ) -> str:
-        return "".join(format_fun(child) for child in self.children)
+        formatted = []
+        for child in self.children:
+            if (
+                isinstance(child, BaseElement)
+                and child._theme is None
+                and self._theme is not None
+            ):
+                child.theme = self.theme
+            formatted.append(format_fun(child))
+        return "".join(formatted)
 
     @property
     def aliased_attrs(self) -> dict[str, Any]:
         """Attributes as a dict with keys renamed to their aliases."""
         return format_attrs(type(self), dict(self.attrs))
 
     @property
     def text(self) -> str:
+        """Get the text content of the element."""
         return "".join(
             child.text if isinstance(child, BaseElement) else str(child)
             for child in self.children
         )
 
+    @property
+    def theme(self) -> Theme:
+        """Get the theme of the element."""
+        return self._theme or get_default_theme()
+
+    @theme.setter
+    def theme(self, value: Theme) -> None:
+        """Set the theme of the element."""
+        self._theme = value
+
     def is_simple(self) -> bool:
         """Check if the element is simple (i.e. contains only one primitive type)."""
         return len(self) == 1 and isinstance(self.children[0], str | int | float | bool)
 
     def has_attributes(self) -> bool:
         """Check if the element has any attributes."""
         return bool(self.attrs)
@@ -192,24 +207,28 @@
             element += " />"
 
         return element
 
     def to_html(self) -> str:
         """Convert an element tree to an HTML string."""
         dom = self
+        classes = list(dom.classes)
+
         while dom != (rendered_dom := dom.render()):
+            rendered_dom._theme = dom._theme
             dom = rendered_dom
+            classes += dom.classes
 
         element_tag = f"{dom.html_header}\n" if dom.html_header else ""
 
         hidden = dom.html_name == "__hidden__"
         element_tag = "" if hidden else f"<{dom.html_name}"
 
-        if dom.has_attributes():
-            attributes_str = dom._format_attributes(is_html=True)
+        if not hidden and (dom.has_attributes() or classes):
+            attributes_str = dom._format_attributes(classes, is_html=True)
             element_tag += f" {attributes_str}"
 
         if dom.children or dom.always_pair:
             children_str = dom._format_children()
             element_tag += (
                 children_str if hidden else f">{children_str}</{dom.html_name}>"
             )
@@ -222,14 +241,15 @@
         """Get the attributes of this component that are defined in the given element.
 
         This is useful so that you can pass common attributes to an element
         without having to pass them from a parent one by one.
 
         Args:
             cls (type[BaseElement]): The element to get the attributes of.
+
         """
         return {
             key: value
             for key, value in self.attrs.items()
             if key in get_element_attrs_annotations(cls)
         }
 
@@ -304,90 +324,7 @@
         self,
         *children: *TChildrenArgs,
         # FIXME: https://github.com/python/typing/issues/1399
         **attrs: Unpack[TAttrs],  # type: ignore
     ) -> None:
         self.attrs = cast(TAttrs, attrs)
         self.children = tuple(self.formatter.extract(*children))
-
-
-class Blank(Element[TChildren, NoAttrs]):
-    """Element representing no element at all, just children.
-
-    The purpose of this element is to be able to return only children
-    when rendering a component.
-    """
-
-    html_name = "__hidden__"
-
-    def __init__(self, *children: TChildren) -> None:
-        super().__init__(*self.formatter.extract(*children))
-
-
-class Component(Element[TChildren, TAttrs], metaclass=ABCMeta):
-    """Base class for components.
-
-    A component subclasses an :class:`Element` and represents any element
-    that can be rendered in Ludic.
-
-    Example usage:
-
-        class PersonAttrs(Attributes):
-            age: NotRequired[int]
-
-        class Person(Component[PersonAttrs]):
-            @override
-            def render(self) -> dl:
-                return dl(
-                    dt("Name"),
-                    dd(self.attrs["name"]),
-                    dt("Age"),
-                    dd(self.attrs.get("age", "N/A")),
-                )
-
-    Now the component can be used in any other component or element:
-
-        >>> div(Person(name="John Doe", age=30), id="person-detail")
-
-    """
-
-    @abstractmethod
-    def render(self) -> BaseElement:
-        """Render the component as an instance of :class:`BaseElement`."""
-
-
-class ComponentStrict(ElementStrict[*TChildrenArgs, TAttrs], metaclass=ABCMeta):
-    """Base class for strict components.
-
-    A component subclasses an :class:`ElementStrict` and represents any
-    element that can be rendered in Ludic. The difference between
-    :class:`Component` and :class:`ComponentStrict` is that the latter
-    expects concrete types of children. It allows specification
-    of each child's type.
-
-    Example usage:
-
-        class PersonAttrs(Attributes):
-            age: NotRequired[int]
-
-        class Person(ComponentStrict[str, str, PersonAttrs]):
-            @override
-            def render(self) -> dl:
-                return dl(
-                    dt("Name"),
-                    dd(" ".join(self.children),
-                    dt("Age"),
-                    dd(self.attrs.get("age", "N/A")),
-                )
-
-    Valid usage would look like this:
-
-        >>> div(Person("John", "Doe", age=30), id="person-detail")
-
-    In this case, we specified that Person expects two string children.
-    First child is the first name, and the second is the second name.
-    We also specify age as an optional key-word argument.
-    """
-
-    @abstractmethod
-    def render(self) -> BaseElement:
-        """Render the component as an instance of :class:`BaseElement`."""
```

### Comparing `ludic-0.2.2/ludic/css.py` & `ludic-0.3.0/ludic/styles/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections.abc import Mapping
 from typing import Literal, TypedDict
 
 CSSProperties = TypedDict(
     "CSSProperties",
     {
         # A
         "align-content": Literal[
@@ -602,7 +603,24 @@
         "word-wrap": Literal["normal", "break-word"],
         "writing-mode": Literal["horizontal-tb", "vertical-rl", "vertical-lr"],
         # Z
         "z-index": str,
     },
     total=False,
 )
+
+# FIXME: Currently, it is impossible to properly type nested CSS properties
+# defined similar as in SCSS, it will be possible when the following PEP is
+# implemented and supported by type checkers: https://peps.python.org/pep-0728/
+GlobalStyles = Mapping[str, "CSSProperties | GlobalStyles"]
+"""CSS styles for elements or components which are defined by setting the ``styles``
+class property.
+
+Example usage:
+
+    class Page(Component[AnyChildren, NoAttrs]):
+        styles = {
+            "body": {
+                "background-color": "red",
+            },
+        }
+"""
```

### Comparing `ludic-0.2.2/ludic/format.py` & `ludic-0.3.0/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/styles.py` & `ludic-0.3.0/ludic/styles/collect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from collections.abc import Mapping
-from typing import Any
+from collections.abc import Mapping, MutableMapping
+from typing import TYPE_CHECKING, Any
 
-from ludic.base import ELEMENT_REGISTRY
-from ludic.css import CSSProperties
-from ludic.types import BaseElement, GlobalStyles
+from .themes import Theme, get_default_theme
+from .types import CSSProperties, GlobalStyles
 
-GLOBAL_STYLES_CACHE: GlobalStyles = {}
+if TYPE_CHECKING:
+    from ludic.types import BaseElement
+
+GLOBAL_STYLES_CACHE: MutableMapping[str, GlobalStyles] = {}
 
 
 def format_styles(styles: GlobalStyles, separator: str = "\n") -> str:
     """Format styles from all registered elements.
 
     Args:
         styles (GlobalStyles): Styles to format.
@@ -34,64 +36,71 @@
 
         if content:
             result.append(f"{" ".join(parents)} {{ {" ".join(content)} }}")
 
     return separator.join(result)
 
 
-def collect_from_components(*components: type[BaseElement]) -> GlobalStyles:
+def from_components(
+    *components: type["BaseElement"], theme: Theme | None = None
+) -> GlobalStyles:
     """Global styles collector from given components.
 
     Example usage:
 
         class Page(Component[AnyChildren, NoAttrs]):
 
             @override
-            def render(self) -> BaseElement:
+            def render(self) -> html:
                 return html(
                     head(
                         title("An example Example"),
                         styles(collect_from_components()),
                     ),
                     body(
                         *self.children,
                     ),
                 )
 
     This would render an HTML page containing the ``<style>`` element
     with the styles the given components.
     """
-    styles: dict[str, CSSProperties | GlobalStyles] = {}
+    all_styles: dict[str, CSSProperties | GlobalStyles] = {}
+    theme = theme or get_default_theme()
+
     for component in components:
-        if not component.styles:
+        styles = getattr(component, "styles", {})
+
+        if not isinstance(styles, Mapping):
             continue
+        elif hasattr(styles, "theme"):
+            styles.theme = theme
 
-        for key, value in component.styles.items():
+        for key, value in styles.items():
             if isinstance(value, Mapping):
-                styles[key] = value
-    return styles
+                all_styles[key] = value
 
+    return all_styles
 
-def collect_from_loaded(cache: bool = False) -> GlobalStyles:
+
+def from_loaded(cache: bool = False, theme: Theme | None = None) -> GlobalStyles:
     """Global styles collector from loaded components.
 
     Args:
         cache (bool): Whether to cache the result Default is False.
 
     Returns:
         GlobalStyles: Collected styles from loaded components.
     """
+    from ludic.base import ELEMENT_REGISTRY
+
     global GLOBAL_STYLES_CACHE
+    theme = theme or get_default_theme()
 
-    if cache and GLOBAL_STYLES_CACHE:
-        return GLOBAL_STYLES_CACHE
+    if cache and GLOBAL_STYLES_CACHE.get(theme.name):
+        return GLOBAL_STYLES_CACHE[theme.name]
 
-    loaded = (
-        element
-        for elements in ELEMENT_REGISTRY.values()
-        for element in elements
-        if element.styles
-    )
-    result = collect_from_components(*loaded)
+    loaded = (element for elements in ELEMENT_REGISTRY.values() for element in elements)
+    result = from_components(*loaded, theme=theme)
     if cache:
-        GLOBAL_STYLES_CACHE = result
+        GLOBAL_STYLES_CACHE[theme.name] = result
     return result
```

### Comparing `ludic-0.2.2/ludic/types.py` & `ludic-0.3.0/ludic/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from collections.abc import Iterable, Mapping
 from typing import TypedDict
 
 from .base import (
     AnyChildren,
     Attrs,
     BaseElement,
-    Blank,
     ComplexChildren,
-    Component,
-    ComponentStrict,
     Element,
     ElementStrict,
-    GlobalStyles,
     JavaScript,
     NoAttrs,
     NoChildren,
     PrimitiveChildren,
     Safe,
     TAttrs,
     TChildren,
     TChildrenArgs,
 )
+from .components import Blank, Component, ComponentStrict
+from .styles import CSSProperties, GlobalStyles, Theme
 
 JSONType = (
     Mapping[str, "JSONType"] | Iterable["JSONType"] | str | int | float | bool | None
 )
 Headers = Mapping[str, JSONType]
 HXHeaders = TypedDict(
     "HXHeaders",
@@ -47,22 +45,24 @@
 __all__ = (
     "AnyChildren",
     "Attrs",
     "BaseElement",
     "ComplexChildren",
     "Component",
     "ComponentStrict",
+    "CSSProperties",
     "Element",
     "ElementStrict",
     "GlobalStyles",
     "Headers",
     "HXHeaders",
     "JavaScript",
     "NoAttrs",
     "NoChildren",
     "PrimitiveChildren",
     "Safe",
     "TAttrs",
     "TChildren",
     "TChildrenArgs",
+    "Theme",
     "Blank",
 )
```

### Comparing `ludic-0.2.2/ludic/utils.py` & `ludic-0.3.0/ludic/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,20 @@
         cls_or_obj (Any): The element to get the generic arguments of.
 
     Returns:
         dict[str, Any] | None: The generic arguments or :obj:`None`.
     """
     from ludic.base import BaseElement
 
+    if hints := getattr(cls_or_obj, "__annotations__", None):
+        children = hints.get("children")
+        attrs = hints.get("attrs")
+        if attrs and children:
+            return (children, attrs)
+
     for base in getattr(cls_or_obj, "__orig_bases__", []):
         if issubclass(get_origin(base), BaseElement):
             return get_args(base)
     return None
 
 
 def get_element_attrs_annotations(
```

### Comparing `ludic-0.2.2/ludic/catalog/forms.py` & `ludic-0.3.0/ludic/catalog/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """An experimental module for creating HTML forms."""
 
 from collections.abc import Callable, Mapping
 from dataclasses import dataclass
 from typing import Any, Literal, get_type_hints, override
 
 from ludic.attrs import Attrs, FormAttrs, InputAttrs, TextAreaAttrs
-from ludic.html import div, form, input, label, textarea
+from ludic.html import div, form, input, label, style, textarea
 from ludic.types import (
     BaseElement,
     ComplexChildren,
     Component,
     NoChildren,
     PrimitiveChildren,
     TAttrs,
@@ -76,15 +76,14 @@
         return self.parse(value)
 
 
 class FieldAttrs(Attrs, total=False):
     """Shared attributes between custom form fields."""
 
     label: str
-    class_div: str
 
 
 class InputFieldAttrs(FieldAttrs, InputAttrs):
     """Attributes of the component ``InputField``.
 
     The attributes are subclassed from :class:`FieldAttrs` and :class:`InputAttrs`.
     """
@@ -96,14 +95,37 @@
     The attributes are subclassed from :class:`FieldAttrs` and :class:`TextAreaAttrs`.
     """
 
 
 class FormField(Component[TChildren, TAttrs]):
     """Base class for form fields."""
 
+    classes = ["form-field"]
+    styles = style.use(
+        lambda theme: {
+            ".form-field": {
+                "label": {
+                    "display": "block",
+                    "margin-top": "12px",
+                    "margin-bottom": "8px",
+                    "font-weight": "bold",
+                },
+                "input": {
+                    "width": "100%",
+                    "padding": "10px",
+                    "margin": "5px 0",
+                    "border": f"1px solid {theme.colors.light.darken(0.2)}",
+                    "border-radius": "4px",
+                    "box-sizing": "border-box",
+                    "font-size": "1em",
+                },
+            }
+        }
+    )
+
     def create_label(self, text: PrimitiveChildren, for_: str = "") -> label:
         if for_:
             return label(text, for_=for_)
         else:
             return label(text)
 
 
@@ -117,15 +139,15 @@
             attrs["id"] = self.attrs["name"]
 
         elements: list[ComplexChildren] = []
         if text := self.attrs.get("label"):
             elements.append(self.create_label(text=text, for_=attrs.get("id", "")))
         elements.append(input(**attrs))
 
-        return div(*elements, class_=self.attrs.get("class_div", "form-group"))
+        return div(*elements)
 
 
 class TextAreaField(FormField[PrimitiveChildren, TextAreaFieldAttrs]):
     """Represents the HTML ``textarea`` element with an optional ``label`` element."""
 
     @override
     def render(self) -> div:
@@ -134,20 +156,22 @@
             attrs["id"] = self.attrs["name"]
 
         elements: list[ComplexChildren] = []
         if text := self.attrs.get("label"):
             elements.append(self.create_label(text=text, for_=attrs.get("id", "")))
         elements.append(textarea(self.children[0], **attrs))
 
-        return div(*elements, class_=self.attrs.get("class_div", "form-group"))
+        return div(*elements)
 
 
 class Form(Component[ComplexChildren, FormAttrs]):
     """A component helper for creating HTML forms."""
 
+    classes = ["form"]
+
     @override
     def render(self) -> form:
         return form(*self.children, **self.attrs)
 
 
 def create_fields(attrs: Any, spec: type[TAttrs]) -> tuple[ComplexChildren, ...]:
     """Create form fields from the given attributes.
```

### Comparing `ludic-0.2.2/ludic/catalog/lists.py` & `ludic-0.3.0/ludic/catalog/items.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 from collections.abc import Iterable
 from typing import override
 
 from ludic.attrs import GlobalAttrs
-from ludic.base import Component
 from ludic.html import dd, dl, dt
-from ludic.types import PrimitiveChildren
+from ludic.types import Component, PrimitiveChildren
 
 from .utils import attr_to_camel
 
 
 class Key(Component[PrimitiveChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``dt`` element."""
 
+    classes = ["key"]
+    styles = {
+        "dt.key": {
+            "font-weight": "bold",
+            "margin-bottom": "10px",
+        },
+    }
+
     @override
     def render(self) -> dt:
         return dt(*self.children, **self.attrs)
 
 
 class Value(Component[PrimitiveChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``dd`` element."""
 
+    classes = ["value"]
+    styles = {
+        "dd.value": {
+            "margin-left": "0",
+            "margin-bottom": "20px",
+        },
+    }
+
     @override
     def render(self) -> dd:
         return dd(*self.children, **self.attrs)
 
 
 class PairsAttrs(GlobalAttrs, total=False):
     """Attributes of the component ``Pairs``."""
@@ -52,14 +67,24 @@
     Or alternatively:
 
         Pairs(
             items={"name": "John", "age": 42}.items(),
         )
     """
 
+    classes = ["pairs"]
+    styles = {
+        "dl.pairs": {
+            "margin-top": "20px",
+            "margin-bottom": "20px",
+        },
+    }
+
     @override
     def render(self) -> dl:
         from_items: list[Key | Value] = []
+
         for key, value in self.attrs.get("items", ()):
             from_items.append(Key(attr_to_camel(key)))
             from_items.append(Value(value))
+
         return dl(*from_items, *self.children, **self.attrs_for(dl))
```

### Comparing `ludic-0.2.2/ludic/catalog/navigation.py` & `ludic-0.3.0/ludic/catalog/navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import override
 
 from ludic.attrs import GlobalAttrs
-from ludic.base import Component, PrimitiveChildren
 from ludic.html import li, ul
+from ludic.types import Component, PrimitiveChildren
 
 from .typography import Link
 
 
 class NavItemAttrs(GlobalAttrs):
     to: str
 
@@ -31,10 +31,12 @@
 
         Navigation(
             NavItem("Home", to="/"),
             NavItem("About", to="/about"),
         )
     """
 
+    classes = ["navigation"]
+
     @override
     def render(self) -> ul:
-        return ul(*self.children, class_="navigation", **self.attrs_for(ul))
+        return ul(*self.children, **self.attrs_for(ul))
```

### Comparing `ludic-0.2.2/ludic/catalog/tables.py` & `ludic-0.3.0/ludic/catalog/tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, Literal, cast, get_type_hints, override
 
 from typing_extensions import TypeVar
 
 from ludic.attrs import GlobalAttrs
-from ludic.html import table, tbody, td, th, thead, tr
+from ludic.html import style, table, tbody, td, th, thead, tr
 from ludic.types import (
     AnyChildren,
     BaseElement,
     Component,
     ComponentStrict,
     PrimitiveChildren,
     TAttrs,
@@ -58,31 +58,51 @@
     def __call__(self, value: Any) -> PrimitiveChildren:
         return self.parse(value)
 
 
 class TableRow(Component[AnyChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``tr`` element."""
 
-    def get_text(self, index: int) -> str:
+    classes = ["table-row"]
+    styles = style.use(
+        lambda theme: {
+            "tr.table-row td": {
+                "border": f"1px solid {theme.colors.light.darken(0.2)}",
+                "padding": "12px",
+            }
+        }
+    )
+
+    def get_value(self, index: int) -> PrimitiveChildren | None:
         if len(self.children) > index:
             child = self.children[index]
-            return child.text if isinstance(child, BaseElement) else str(child)
-        return ""
+            return child.text if isinstance(child, BaseElement) else child
+        return None
 
     @override
     def render(self) -> tr:
         return tr(
             *(child if isinstance(child, td) else td(child) for child in self.children),
             **self.attrs,
         )
 
 
 class TableHead(Component[AnyChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``tr`` element."""
 
+    classes = ["table-head"]
+    styles = style.use(
+        lambda theme: {
+            "tr.table-head th": {
+                "border": f"1px solid {theme.colors.light.darken(0.2)}",
+                "padding": "12px",
+            }
+        }
+    )
+
     @property
     def header(self) -> tuple[PrimitiveChildren, ...]:
         return tuple(
             child.text if isinstance(child, BaseElement) else str(child)
             for child in self.children
             if self.children
         )
@@ -95,63 +115,84 @@
         )
 
 
 THead = TypeVar("THead", bound=BaseElement, default=TableHead)
 TRow = TypeVar("TRow", bound=BaseElement, default=TableRow)
 
 
-class TableType(ComponentStrict[THead, *tuple[TRow, ...], GlobalAttrs]):
-    """A component rendering as the HTML ``table`` element.
-
-    The component allows specifying the table head and rows types:
-
-        TableType[PersonHead, PersonRow](
-            PersonHead("Name", "Age"),
-            PersonRow("John", 42),
-            PersonRow("Jane", 23),
-        )
-    """
-
-    @override
-    def render(self) -> table:
-        return table(thead(self.children[0]), tbody(*self.children[1:]), **self.attrs)
+class TableAttrs(GlobalAttrs):
+    head_attrs: GlobalAttrs
+    body_attrs: GlobalAttrs
 
 
-class Table(TableType[TableHead, TableRow]):
+class Table(ComponentStrict[THead, *tuple[TRow, ...], TableAttrs]):
     """A component rendering as the HTML ``table`` element.
 
-    The component only allows :class:`TableHead` and :class:`TableRow` types.
+    The component allows :class:`TableHead` and :class:`TableRow` types by default.
 
     Example:
 
         Table(
             TableHead("Name", "Age"),
             TableRow("John", 42),
             TableRow("Jane", 23),
         )
+
+    You can also specify different types of header and body:
+
+        Table[PersonHead, PersonRow](
+            PersonHead("Name", "Age"),
+            PersonRow("John", 42),
+        )
     """
 
+    classes = ["table"]
+    styles = style.use(
+        lambda theme: {
+            "table.table": {
+                "width": "100%",  # type: ignore
+                "border-collapse": "collapse",  # type: ignore
+                "thead": {
+                    "background-color": theme.colors.light,
+                },
+                "button.btn": {
+                    "margin": "0 5px",
+                },
+            }
+        }
+    )
+
     @property
     def header(self) -> tuple[PrimitiveChildren, ...]:
-        return self.children[0].header
+        if isinstance(self.children[0], TableHead):
+            return self.children[0].header
+        return ()
 
     def getlist(self, key: str) -> list[PrimitiveChildren | None]:
         result: list[PrimitiveChildren | None] = []
 
         for idx, head in enumerate(self.header):
             if key != head:
                 continue
 
             rows: list[TableRow] = cast(list[TableRow], self.children[1:])
             for row in rows:
-                if value := row.get_text(idx):
+                if value := row.get_value(idx):
                     result.append(value)
 
         return result
 
+    @override
+    def render(self) -> table:
+        return table(
+            thead(self.children[0], **self.attrs.get("head_attrs", {})),
+            tbody(*self.children[1:], **self.attrs.get("body_attrs", {})),
+            **self.attrs_for(table),
+        )
+
 
 def create_rows(
     attrs_list: list[TAttrs], spec: type[TAttrs], include_id_column: bool = False
 ) -> tuple[TableHead, *tuple[TableRow, ...]]:
     """Create table rows from the given attributes.
 
     Example:
```

### Comparing `ludic-0.2.2/ludic/catalog/typography.py` & `ludic-0.3.0/ludic/catalog/typography.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Example usage:
 
         Link("Hello, World!", to="https://example.com")
     """
 
     @override
     def render(self) -> a:
-        return a(self.children[0], href=self.attrs["to"], **self.attrs_for(a))
+        return a(self.children[0], href=self.attrs["to"])
 
 
 class Paragraph(Component[AnyChildren, GlobalAttrs]):
     """Simple component simulating a paragraph.
 
     There is basically just an alias for the :class:`p` element.
```

### Comparing `ludic-0.2.2/ludic/web/app.py` & `ludic-0.3.0/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/datastructures.py` & `ludic-0.3.0/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/endpoints.py` & `ludic-0.3.0/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/exceptions.py` & `ludic-0.3.0/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/parsers.py` & `ludic-0.3.0/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/requests.py` & `ludic-0.3.0/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/responses.py` & `ludic-0.3.0/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/ludic/web/routing.py` & `ludic-0.3.0/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/tests/test_elements.py` & `ludic-0.3.0/tests/test_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ludic.css import CSSProperties
 from ludic.html import (
     a,
     b,
     button,
     div,
     i,
     label,
@@ -12,14 +11,15 @@
     table,
     tbody,
     td,
     th,
     thead,
     tr,
 )
+from ludic.styles import CSSProperties
 
 
 def test_empty_element() -> None:
     dom = div()
     assert dom.to_html() == "<div />"
     assert dom.to_string() == "<div />"
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cfas71fk_/tmpt84mtcza_TarContainer/0/54.py", line 165, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-from ludic.css import CSSProperties from ludic.html import ( a, b, button, div,
-i, label, p, script, span, table, tbody, td, th, thead, tr, ) def
+from ludic.html import ( a, b, button, div, i, label, p, script, span, table,
+tbody, td, th, thead, tr, ) from ludic.styles import CSSProperties def
 test_empty_element() -> None: dom = div() assert dom.to_html() == "
 " assert dom.to_string() == "
 " dom2 = p("") assert dom2.to_html() == "
 " assert dom2.to_string() == "
 " dom3 = script() assert dom3.to_html() == "
 " assert dom3.to_string() == "
```

### Comparing `ludic-0.2.2/tests/test_examples.py` & `ludic-0.3.0/tests/test_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,7 +96,18 @@
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         response = client.get("/load/0")
         assert response.status_code == 200
         assert b"Content Loaded" in response.content
 
     app.routes.clear()
+
+
+def test_infinite_scroll() -> None:
+    import examples.infinite_scroll as _  # noqa
+
+    with TestClient(app) as client:
+        assert client.get("/").status_code == 200
+        assert client.get("/contacts/").status_code == 200
+        assert client.get("/contacts/?page=2").status_code == 200
+
+    app.routes.clear()
```

### Comparing `ludic-0.2.2/tests/test_exceptions.py` & `ludic-0.3.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/tests/test_formatting.py` & `ludic-0.3.0/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/tests/test_styles.py` & `ludic-0.3.0/tests/test_styles.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,14 +104,14 @@
         "@layer state { .alert { background-color: brown; } p { padding: 10px; } }\n"
         "</style>"
     )
 
 
 def test_styles_collection() -> None:
     assert style.from_components(A, B).to_html() == (
-        "<style>\n"
+        '<style type="text/css">\n'
         "a { color: red; }\n"
         ".content { background: #ffe; padding: 10px; }\n"
         ".content > p { color: blue; font-size: 20px; }\n"
         "a.test { color: blue; }\n"
         "</style>"
     )
```

### Comparing `ludic-0.2.2/tests/test_types.py` & `ludic-0.3.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/.gitignore` & `ludic-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/LICENCE` & `ludic-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.2.2/README.md` & `ludic-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ## Features
 
 - Seamless **&lt;/&gt; htmx** integration for rapid web development in **pure Python**
 - **Type-Guided components** utilizing Python's typing system
 - Uses the power of **Starlette** and **Async** for high-performance web development
 - Build HTML with the ease and power of Python **f-strings**
+- Add CSS styling to your components with **themes**
 
 ## Ideals
 
 This framework allows HTML generation in Python while utilizing Python's typing system. Our goal is to enable the creation of dynamic web applications with reusable components, all while offering a greater level of type safety than raw HTML.
 
 **Key Ideas:**
 
@@ -49,15 +50,15 @@
     TableHead("Id", "Name"),
     TableRow("1", "John"),
     TableRow("2", "Jane"),
     TableRow("3", "Bob"),
 )
 ```
 
-This structure can be type-checked thanks to Python's rich type system. Additionally, this `Table` component could have **dynamic properties** like sorting or even modification of data on the server.
+This structure can be type-checked thanks to Python's rich type system. Additionally, this `Table` component could have **dynamic properties** like sorting or filtering.
 
 ## Requirements
 
 Python 3.12+
 
 ## Installation
 
@@ -81,20 +82,22 @@
 from ludic.html import a
 from ludic.types import Attrs, Component
 
 class LinkAttrs(Attrs):
     to: str
 
 class Link(Component[str, LinkAttrs]):
+    classes = ["link"]
+
     @override
     def render(self) -> a:
         return a(
             *self.children,
             href=self.attrs["to"],
-            style={"color": "#abc"},
+            style={"color": self.theme.colors.primary},
         )
 ```
 
 Now you can use it like this:
 
 ```python
 link = Link("Hello, World!", to="/home")
```

### Comparing `ludic-0.2.2/pyproject.toml` & `ludic-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -77,10 +77,28 @@
 
 [tool.mypy]
 python_version = "3.12"
 strict = true
 disallow_subclassing_any = false
 
 [tool.pytest.ini_options]
+testpaths = "tests"
+norecursedirs = ".git docs .pytest_cache .mypy_cache .ruff_cache"
 filterwarnings = [
     "ignore:The \\'app\\' shortcut is now deprecated. Use the explicit style \\'transport=WSGITransport\\(app=\\.\\.\\.\\)\\' instead\\.",
 ]
+
+[tool.coverage.run]
+omit = ["tests/**"]
+
+[tool.coverage.paths]
+source = ["ludic", "examples"]
+
+[tool.coverage.report]
+show_missing = true
+precision = 2
+exclude_lines = [
+    "pragma: no cover",
+    "raise NotImplementedError",
+    "if TYPE_CHECKING:",
+    "pass"
+]
```

### Comparing `ludic-0.2.2/PKG-INFO` & `ludic-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
@@ -41,14 +41,15 @@
 
 ## Features
 
 - Seamless **&lt;/&gt; htmx** integration for rapid web development in **pure Python**
 - **Type-Guided components** utilizing Python's typing system
 - Uses the power of **Starlette** and **Async** for high-performance web development
 - Build HTML with the ease and power of Python **f-strings**
+- Add CSS styling to your components with **themes**
 
 ## Ideals
 
 This framework allows HTML generation in Python while utilizing Python's typing system. Our goal is to enable the creation of dynamic web applications with reusable components, all while offering a greater level of type safety than raw HTML.
 
 **Key Ideas:**
 
@@ -79,15 +80,15 @@
     TableHead("Id", "Name"),
     TableRow("1", "John"),
     TableRow("2", "Jane"),
     TableRow("3", "Bob"),
 )
 ```
 
-This structure can be type-checked thanks to Python's rich type system. Additionally, this `Table` component could have **dynamic properties** like sorting or even modification of data on the server.
+This structure can be type-checked thanks to Python's rich type system. Additionally, this `Table` component could have **dynamic properties** like sorting or filtering.
 
 ## Requirements
 
 Python 3.12+
 
 ## Installation
 
@@ -111,20 +112,22 @@
 from ludic.html import a
 from ludic.types import Attrs, Component
 
 class LinkAttrs(Attrs):
     to: str
 
 class Link(Component[str, LinkAttrs]):
+    classes = ["link"]
+
     @override
     def render(self) -> a:
         return a(
             *self.children,
             href=self.attrs["to"],
-            style={"color": "#abc"},
+            style={"color": self.theme.colors.primary},
         )
 ```
 
 Now you can use it like this:
 
 ```python
 link = Link("Hello, World!", to="/home")
```

