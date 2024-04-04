# Comparing `tmp/django-template-partials-23.4.tar.gz` & `tmp/django-template-partials-24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-template-partials-23.4.tar", last modified: Mon Nov 20 09:40:00 2023, max compression
+gzip compressed data, was "django-template-partials-24.1.tar", last modified: Thu Apr  4 12:26:16 2024, max compression
```

## Comparing `django-template-partials-23.4.tar` & `django-template-partials-24.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1418 2023-10-08 09:18:58.608494 django-template-partials-23.4/.github/workflows/package-tests.yml
--rw-r--r--   0        0        0       23 2023-10-08 09:06:53.252564 django-template-partials-23.4/.gitignore
--rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-23.4/.vscode/settings.json
--rw-r--r--   0        0        0     2374 2023-11-20 09:36:52.531215 django-template-partials-23.4/CHANGELOG.md
--rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-23.4/LICENSE
--rw-r--r--   0        0        0     5905 2023-10-08 09:11:10.167518 django-template-partials-23.4/README.md
--rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-23.4/justfile
--rw-r--r--   0        0        0     1090 2023-11-20 09:20:35.702726 django-template-partials-23.4/pyproject.toml
--rw-r--r--   0        0        0      121 2023-11-20 09:37:43.853833 django-template-partials-23.4/src/template_partials/__init__.py
--rw-r--r--   0        0        0     2170 2023-11-20 09:15:23.735606 django-template-partials-23.4/src/template_partials/apps.py
--rw-r--r--   0        0        0     2013 2023-10-08 09:16:01.840154 django-template-partials-23.4/src/template_partials/loader.py
--rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-23.4/src/template_partials/templatetags/__init__.py
--rw-r--r--   0        0        0     4396 2023-10-08 09:17:53.629675 django-template-partials-23.4/src/template_partials/templatetags/partials.py
--rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-23.4/tests/__init__.py
--rw-r--r--   0        0        0      804 2023-11-20 09:36:58.594009 django-template-partials-23.4/tests/settings.py
--rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-23.4/tests/templates/base.html
--rw-r--r--   0        0        0      161 2023-10-08 09:11:10.169756 django-template-partials-23.4/tests/templates/debug.html
--rw-r--r--   0        0        0      286 2023-10-08 09:11:10.170054 django-template-partials-23.4/tests/templates/example.html
--rw-r--r--   0        0        0     4332 2023-11-20 09:15:23.736358 django-template-partials-23.4/tests/tests.py
--rw-r--r--   0        0        0      374 2023-10-08 09:06:53.253993 django-template-partials-23.4/tox.ini
--rw-r--r--   0        0        0     6843 1970-01-01 00:00:00.000000 django-template-partials-23.4/PKG-INFO
+-rw-r--r--   0        0        0      295 2024-04-04 12:06:18.310243 django-template-partials-24.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1418 2024-04-04 12:06:18.311243 django-template-partials-24.1/.github/workflows/package-tests.yml
+-rw-r--r--   0        0        0       23 2023-10-08 09:06:53.252564 django-template-partials-24.1/.gitignore
+-rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-24.1/.vscode/settings.json
+-rw-r--r--   0        0        0     2516 2024-04-04 12:23:18.997066 django-template-partials-24.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-24.1/LICENSE
+-rw-r--r--   0        0        0     5905 2023-10-08 09:11:10.167518 django-template-partials-24.1/README.md
+-rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-24.1/justfile
+-rw-r--r--   0        0        0     1090 2023-11-20 09:20:35.702726 django-template-partials-24.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-04 12:23:58.394079 django-template-partials-24.1/src/template_partials/__init__.py
+-rw-r--r--   0        0        0     2170 2024-04-04 12:06:18.312180 django-template-partials-24.1/src/template_partials/apps.py
+-rw-r--r--   0        0        0     2329 2024-04-04 12:20:35.190731 django-template-partials-24.1/src/template_partials/loader.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-24.1/src/template_partials/templatetags/__init__.py
+-rw-r--r--   0        0        0     4396 2023-10-08 09:17:53.629675 django-template-partials-24.1/src/template_partials/templatetags/partials.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-24.1/tests/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-04 12:06:18.313184 django-template-partials-24.1/tests/settings.py
+-rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-24.1/tests/templates/base.html
+-rw-r--r--   0        0        0      161 2023-10-08 09:11:10.169756 django-template-partials-24.1/tests/templates/debug.html
+-rw-r--r--   0        0        0      286 2023-10-08 09:11:10.170054 django-template-partials-24.1/tests/templates/example.html
+-rw-r--r--   0        0        0     5464 2024-04-04 12:20:35.190920 django-template-partials-24.1/tests/tests.py
+-rw-r--r--   0        0        0      374 2023-10-08 09:06:53.253993 django-template-partials-24.1/tox.ini
+-rw-r--r--   0        0        0     6843 1970-01-01 00:00:00.000000 django-template-partials-24.1/PKG-INFO
```

### Comparing `django-template-partials-23.4/.github/workflows/package-tests.yml` & `django-template-partials-24.1/.github/workflows/package-tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       fail-fast: false
       matrix:
         python-version:
           - "3.11"
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install -e .[tests]
       - name: Run tests with coverage
         run: |
@@ -36,15 +36,15 @@
 #         python-version:
 #           - "3.10"
 #           - "3.11"
 #           - "3.12"
 #     steps:
 #       - uses: actions/checkout@v4
 #       - name: Set up Python ${{ matrix.python-version }}
-#         uses: actions/setup-python@v4
+#         uses: actions/setup-python@v5
 #         with:
 #           python-version: ${{ matrix.python-version }}
 #       - name: Install dependencies
 #         run: |
 #           python -m pip install --upgrade pip setuptools wheel
 #           python -m pip install --upgrade 'tox>=4.0.0rc3'
 #       - name: Run tox targets for ${{ matrix.python-version }}
```

### Comparing `django-template-partials-23.4/CHANGELOG.md` & `django-template-partials-24.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGELOG
 
+## 24.1 (2024-04-04)
+
+* Fixed a bug in how the partial loader called down to the cached loader when
+  present.
+
+  Thanks to Marco Garbelini.
+
 ## 23.4 (2023-11-20)
 
 * Fixed a bug automatically wrapping the template loaders when another installed
   app had already instantiated the template engine.
 
   Thanks to Jannis Vajen.
```

### Comparing `django-template-partials-23.4/LICENSE` & `django-template-partials-24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.4/README.md` & `django-template-partials-24.1/README.md`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.4/pyproject.toml` & `django-template-partials-24.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.4/src/template_partials/apps.py` & `django-template-partials-24.1/src/template_partials/apps.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.4/src/template_partials/loader.py` & `django-template-partials-24.1/src/template_partials/loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.template.loaders import cached
 from django.template import TemplateDoesNotExist
 from django.template.loaders.base import Loader as BaseLoader
 
 
 class Loader(BaseLoader):
     """
     Wrapper class that takes a list of template loaders as an argument and attempts
@@ -29,16 +30,21 @@
 
         - Split the template_name into template_name, partial_name.
         - Use self.loaders to find the template. Raise if not found.
         - If partial_name is not None. Check for defined partial. Raise if not found.
         """
         template_name, _, partial_name = template_name.partition("#")
 
-        # May raise TemplateDoesNotExist
-        template = super().get_template(template_name, skip)
+        # Find template from child loaders.
+        # The cached loader requires special handling.
+        # May raise TemplateDoesNotExist.
+        if len(self.loaders) == 1 and isinstance(self.loaders[0], cached.Loader):
+            template = self.loaders[0].get_template(template_name, skip)
+        else:
+            template = super().get_template(template_name, skip)
 
         if not partial_name:
             return template
 
         try:
             partial_contents = template.origin.partial_contents
         except AttributeError:
```

### Comparing `django-template-partials-23.4/src/template_partials/templatetags/partials.py` & `django-template-partials-24.1/src/template_partials/templatetags/partials.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.4/tests/settings.py` & `django-template-partials-24.1/tests/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from re import U
-
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
         "DIRS": [],
         "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
```

### Comparing `django-template-partials-23.4/tests/tests.py` & `django-template-partials-24.1/tests/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 
             # Compile and render the template
             engine = engines["django"]
             t = engine.from_string(template)
             rendered = t.render()
 
             # Check for deprecation warning
-            self.assertTrue(any(issubclass(warn.category, DeprecationWarning) for warn in w))
+            self.assertTrue(
+                any(issubclass(warn.category, DeprecationWarning) for warn in w)
+            )
 
         # Check the rendered content
         self.assertEqual("DEPRECATED TEST CONTENT", rendered.strip())
 
     def test_partialdef_tag_with_inline(self):
         template = """
         {% load partials %}
@@ -107,21 +109,46 @@
         class LazyExceptionObject:
             def __str__(self):
                 raise Exception("Test exception")
 
         engine = engines["django"]
         template = engine.get_template("debug.html")
         try:
-            template.render({'exception': LazyExceptionObject()})
+            template.render({"exception": LazyExceptionObject()})
         except Exception as e:
-            self.assertEqual(e.template_debug['message'], "Test exception")
-            self.assertEqual(e.template_debug['line'], 4)
+            self.assertEqual(e.template_debug["message"], "Test exception")
+            self.assertEqual(e.template_debug["line"], 4)
 
     def test_template_source(self):
         """Partials defer to their source template for source code."""
         engine = engines["django"]
         partial = engine.get_template("example.html#test-partial")
         source_template = engine.get_template("example.html")
         self.assertEqual(
             partial.template.source,
             source_template.template.source,
         )
+
+    def test_chained_exception_forwarded(self):
+        """TemplateDoesNotExist exceptions are chained with the tried attribute."""
+        engine = engines["django"]
+        with self.assertRaises(django.template.TemplateDoesNotExist) as ex:
+            engine.get_template("not_there.html#not-a-partial")
+
+        self.assertTrue(len(ex.exception.tried) > 0)
+        origin, _ = ex.exception.tried[0]
+        self.assertEqual(origin.template_name, "not_there.html")
+
+
+class ChildCachedLoaderTest(TestCase):
+    def test_child_cached_loader(self):
+        wrap_loaders("django")
+        engine = engines["django"].engine
+        partial_loader = engine.template_loaders[0]
+        self.assertEqual(type(partial_loader).__module__, "template_partials.loader")
+        cached_loader = partial_loader.loaders[0]
+        self.assertEqual(
+            type(cached_loader).__module__, "django.template.loaders.cached"
+        )
+        self.assertEqual(len(cached_loader.get_template_cache), 0)
+        engine.get_template("example.html")
+        self.assertEqual(len(cached_loader.get_template_cache), 1)
```

### Comparing `django-template-partials-23.4/PKG-INFO` & `django-template-partials-24.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-template-partials
-Version: 23.4
+Version: 24.1
 Summary: django-template-partials
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-template-partials Version: 23.4 Summary:
+Metadata-Version: 2.1 Name: django-template-partials Version: 24.1 Summary:
 django-template-partials Author-email: Carlton Gibson
 noumenal.es> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.2
```

