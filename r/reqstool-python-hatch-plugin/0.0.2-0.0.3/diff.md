# Comparing `tmp/reqstool_python_hatch_plugin-0.0.2.tar.gz` & `tmp/reqstool_python_hatch_plugin-0.0.3.tar.gz`

## Comparing `reqstool_python_hatch_plugin-0.0.2.tar` & `reqstool_python_hatch_plugin-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/workflows/check_release.yml
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/workflows/publish_gh_pages.yml
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/workflows/publish_pypi_prod.yml
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.github/workflows/publish_pypi_test.yml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/antora-playbook.yml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/antora.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/pages/description.adoc
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/pages/installation.adoc
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/pages/license.adoc
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/pages/usage.adoc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/src/reqstool_python_hatch_plugin/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/src/reqstool_python_hatch_plugin/hooks.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/src/reqstool_python_hatch_plugin/build_hook/hook.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/tests/unit/conftest.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/tests/unit/reqstool_python_hatch_plugin/test_hooks.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/LICENSE
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/README.md
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/workflows/check_release.yml
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/workflows/publish_gh_pages.yml
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/workflows/publish_pypi_prod.yml
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.github/workflows/publish_pypi_test.yml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/antora-playbook.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/antora.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/pages/description.adoc
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/pages/installation.adoc
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/pages/license.adoc
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/pages/usage.adoc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/src/reqstool_python_hatch_plugin/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/src/reqstool_python_hatch_plugin/hooks.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/src/reqstool_python_hatch_plugin/build_hook/hook.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/tests/unit/conftest.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/tests/unit/reqstool_python_hatch_plugin/test_hooks.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 reqstool_python_hatch_plugin-0.0.3/PKG-INFO
```

### Comparing `reqstool_python_hatch_plugin-0.0.2/.github/dependabot.yml` & `reqstool_python_hatch_plugin-0.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/.github/workflows/build.yml` & `reqstool_python_hatch_plugin-0.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/.github/workflows/lint.yml` & `reqstool_python_hatch_plugin-0.0.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/.github/workflows/publish_gh_pages.yml` & `reqstool_python_hatch_plugin-0.0.3/.github/workflows/publish_gh_pages.yml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - name: Checkout repository
         uses: actions/checkout@v4
       - name: Configure Pages
-        uses: actions/configure-pages@v4
+        uses: actions/configure-pages@v5
       - name: Install Node.js
         uses: actions/setup-node@v4
         with:
           node-version: "18"
       - name: Install Antora
         run: npm i antora
       - name: Install Asciidoctor Kroki extension
```

### Comparing `reqstool_python_hatch_plugin-0.0.2/.github/workflows/publish_pypi_prod.yml` & `reqstool_python_hatch_plugin-0.0.3/.github/workflows/publish_pypi_prod.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/.github/workflows/publish_pypi_test.yml` & `reqstool_python_hatch_plugin-0.0.3/.github/workflows/publish_pypi_test.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/docs/antora-playbook.yml` & `reqstool_python_hatch_plugin-0.0.3/docs/antora-playbook.yml`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/docs/modules/ROOT/pages/installation.adoc` & `reqstool_python_hatch_plugin-0.0.3/docs/modules/ROOT/pages/installation.adoc`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/src/reqstool_python_hatch_plugin/build_hook/hook.py` & `reqstool_python_hatch_plugin-0.0.3/src/reqstool_python_hatch_plugin/build_hook/hook.py`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/.gitignore` & `reqstool_python_hatch_plugin-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/LICENSE` & `reqstool_python_hatch_plugin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reqstool_python_hatch_plugin-0.0.2/README.md` & `reqstool_python_hatch_plugin-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 
 ### Configuration
 
 The plugin can be configured through the `pyproject.toml` file. Configure plugin in `pyproject.toml`as follows;
 
 ```
 [tool.hatch.build.targets.wheel.hooks.decorators]
-dependencies = ["reqstool-hatch-plugin == <version>"]
+dependencies = ["reqstool-python-hatch-plugin == <version>"]
 path = ["src","tests"]
 
 ```
-It specifies that the reqstool-hatch-plugin is a dependency for the build process, and it should be of a specific version. 
+It specifies that the reqstool-python-hatch-plugin is a dependency for the build process, and it should be of a specific version. 
 
 Further it defines the paths where the plugin should be applied. In this case, it specifies that the plugin should be applied to files in the src and tests directories.
```

### Comparing `reqstool_python_hatch_plugin-0.0.2/pyproject.toml` & `reqstool_python_hatch_plugin-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Development Status :: 4 - Beta",
 ]
 
 
 requires-python = ">=3.10"
 
 dependencies = [
-    "reqstool-python-decorators == 0.0.3",
+    "reqstool-python-decorators == 0.0.4",
     "ruamel.yaml==0.18.6",
     "hatchling>=1.20.0",
 ]
 
 packages = [{ include = "reqstool_python_hatch_plugin", from = "src" }]
 
 [project.scripts]
```

### Comparing `reqstool_python_hatch_plugin-0.0.2/PKG-INFO` & `reqstool_python_hatch_plugin-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: reqstool-python-hatch-plugin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hatch plugin to process reqstool-python-decorators when building with Hatch
 Project-URL: Source, https://github.com/Luftfartsverket/reqstool-python-hatch-plugin.git
 Author-email: LFV <sysdev@lfv.se>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: hatchling>=1.20.0
-Requires-Dist: reqstool-python-decorators==0.0.3
+Requires-Dist: reqstool-python-decorators==0.0.4
 Requires-Dist: ruamel-yaml==0.18.6
 Description-Content-Type: text/markdown
 
 
 [![Commit Activity](https://img.shields.io/github/commit-activity/m/Luftfartsverket/reqstool-python-hatch-plugin?label=commits&style=for-the-badge)](https://github.com/Luftfartsverket/reqstool-python-hatch-plugin/pulse)
 [![GitHub Issues](https://img.shields.io/github/issues/Luftfartsverket/reqstool-python-hatch-plugin?style=for-the-badge&logo=github)](https://github.com/Luftfartsverket/reqstool-python-hatch-plugin/issues)
 [![License](https://img.shields.io/github/license/Luftfartsverket/reqstool-python-hatch-plugin?style=for-the-badge&logo=opensourceinitiative)](https://opensource.org/license/mit/)
@@ -48,14 +48,14 @@
 
 ### Configuration
 
 The plugin can be configured through the `pyproject.toml` file. Configure plugin in `pyproject.toml`as follows;
 
 ```
 [tool.hatch.build.targets.wheel.hooks.decorators]
-dependencies = ["reqstool-hatch-plugin == <version>"]
+dependencies = ["reqstool-python-hatch-plugin == <version>"]
 path = ["src","tests"]
 
 ```
-It specifies that the reqstool-hatch-plugin is a dependency for the build process, and it should be of a specific version. 
+It specifies that the reqstool-python-hatch-plugin is a dependency for the build process, and it should be of a specific version. 
 
 Further it defines the paths where the plugin should be applied. In this case, it specifies that the plugin should be applied to files in the src and tests directories.
```

