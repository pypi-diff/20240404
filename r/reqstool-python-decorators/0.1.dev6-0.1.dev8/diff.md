# Comparing `tmp/reqstool_python_decorators-0.1.dev6.tar.gz` & `tmp/reqstool_python_decorators-0.1.dev8.tar.gz`

## Comparing `reqstool_python_decorators-0.1.dev6.tar` & `reqstool_python_decorators-0.1.dev8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.github/dependabot.yml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.github/workflows/build.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.github/workflows/publish_development.yml
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.github/workflows/publish_pages.yml
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.github/workflows/publish_production.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/antora-playbook.yml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/antora.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/pages/description.adoc
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/pages/installation.adoc
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/pages/licence.adoc
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/pages/usage.adoc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/src/reqstool_python_decorators/__init__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/src/reqstool_python_decorators/decorators/decorators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/src/reqstool_python_decorators/processors/__init__.py
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/src/reqstool_python_decorators/processors/decorator_processor.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/tests/resources/test_decorators/requirements_decorators.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/tests/resources/test_decorators/svc_decorators.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/tests/unit/conftest.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/tests/unit/reqstool_decorators/processors/test_processors.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/README.md
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/pyproject.toml
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev6/PKG-INFO
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.github/dependabot.yml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.github/workflows/publish_development.yml
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.github/workflows/publish_pages.yml
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.github/workflows/publish_production.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/antora-playbook.yml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/antora.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/pages/description.adoc
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/pages/installation.adoc
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/pages/licence.adoc
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/pages/usage.adoc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/src/reqstool_python_decorators/__init__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/src/reqstool_python_decorators/decorators/decorators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/src/reqstool_python_decorators/processors/__init__.py
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/src/reqstool_python_decorators/processors/decorator_processor.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/tests/resources/test_decorators/requirements_decorators.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/tests/resources/test_decorators/svc_decorators.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/tests/unit/conftest.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/tests/unit/reqstool_decorators/processors/test_processors.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/README.md
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/pyproject.toml
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 reqstool_python_decorators-0.1.dev8/PKG-INFO
```

### Comparing `reqstool_python_decorators-0.1.dev6/.github/dependabot.yml` & `reqstool_python_decorators-0.1.dev8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/.github/workflows/build.yml` & `reqstool_python_decorators-0.1.dev8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/.github/workflows/lint.yml` & `reqstool_python_decorators-0.1.dev8/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/.github/workflows/publish_development.yml` & `reqstool_python_decorators-0.1.dev8/.github/workflows/publish_development.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/.github/workflows/publish_pages.yml` & `reqstool_python_decorators-0.1.dev8/.github/workflows/publish_pages.yml`

 * *Files 0% similar despite different names*

```diff
@@ -37,13 +37,13 @@
       - name: Install Asciidoctor Kroki extension
         run: npm i asciidoctor asciidoctor-kroki
       - name: Generate Site
         run: npx antora docs/antora-playbook.yml
       - name: Create site folders
         run: mkdir -p docs/build/site
       - name: Upload Artifacts
-        uses: actions/upload-pages-artifact@v2
+        uses: actions/upload-pages-artifact@v3
         with:
           path: docs/build/site
       - name: Deploy to GitHub Pages
         id: deployment
         uses: actions/deploy-pages@v2
```

### Comparing `reqstool_python_decorators-0.1.dev6/.github/workflows/publish_production.yml` & `reqstool_python_decorators-0.1.dev8/.github/workflows/publish_production.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/docs/antora-playbook.yml` & `reqstool_python_decorators-0.1.dev8/docs/antora-playbook.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/docs/modules/ROOT/pages/usage.adoc` & `reqstool_python_decorators-0.1.dev8/docs/modules/ROOT/pages/usage.adoc`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/src/reqstool_python_decorators/processors/decorator_processor.py` & `reqstool_python_decorators-0.1.dev8/src/reqstool_python_decorators/processors/decorator_processor.py`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/tests/unit/reqstool_decorators/processors/test_processors.py` & `reqstool_python_decorators-0.1.dev8/tests/unit/reqstool_decorators/processors/test_processors.py`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/.gitignore` & `reqstool_python_decorators-0.1.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/LICENSE` & `reqstool_python_decorators-0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/README.md` & `reqstool_python_decorators-0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/pyproject.toml` & `reqstool_python_decorators-0.1.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reqstool_python_decorators-0.1.dev6/PKG-INFO` & `reqstool_python_decorators-0.1.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reqstool-python-decorators
-Version: 0.1.dev6
+Version: 0.1.dev8
 Summary: Reqstool Python Decorators
 Project-URL: Source, https://github.com/Luftfartsverket/reqstool-python-decorators.git
 Author-email: LFV SYSDEV <sysdev@lfv.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

