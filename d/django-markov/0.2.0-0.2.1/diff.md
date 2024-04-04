# Comparing `tmp/django_markov-0.2.0.tar.gz` & `tmp/django_markov-0.2.1.tar.gz`

## Comparing `django_markov-0.2.0.tar` & `django_markov-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/admin.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/apps.py
--rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/py.typed
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/text_models.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/urls.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/views.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0001_initial.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0003_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/settings.py
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/test_models.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/urls.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.0/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 django_markov-0.2.0/LICENSE
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 django_markov-0.2.0/README.md
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 django_markov-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 django_markov-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/admin.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/apps.py
+-rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/py.typed
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/text_models.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/urls.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/views.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0003_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/settings.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/test_models.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/urls.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 django_markov-0.2.1/README.md
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 django_markov-0.2.1/PKG-INFO
```

### Comparing `django_markov-0.2.0/src/django_markov/models.py` & `django_markov-0.2.1/src/django_markov/models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/src/django_markov/migrations/0001_initial.py` & `django_markov-0.2.1/src/django_markov/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py` & `django_markov-0.2.1/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/src/django_markov/migrations/0003_markovtextmodel_compiled.py` & `django_markov-0.2.1/src/django_markov/migrations/0003_markovtextmodel_compiled.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/tests/settings.py` & `django_markov-0.2.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/tests/test_models.py` & `django_markov-0.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/tests/urls.py` & `django_markov-0.2.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.0/LICENSE` & `django_markov-0.2.1/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-BSD License
-
-Copyright (c) 2024, Daniel Andrlik
-All rights reserved.
+Copyright 2024 Daniel Andrlik
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice, this
-  list of conditions and the following disclaimer in the documentation and/or
-  other materials provided with the distribution.
+1. Redistributions of source code must retain the above copyright notice, this
+list of conditions and the following disclaimer.
 
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from this
-  software without specific prior written permission.
+2. Redistributions in binary form must reproduce the above copyright notice,
+this list of conditions and the following disclaimer in the documentation and/or
+other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors
+may be used to endorse or promote products derived from this software without
+specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
-OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
-OF THE POSSIBILITY OF SUCH DAMAGE.
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `django_markov-0.2.0/README.md` & `django_markov-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 django-markov is a reusable Django app that enables you to create Markov text models, and store
 them in the database. Those models can then be used to generate Markov chain sentences.
 It relies on the excellent [markovify](https://github.com/jsvine/markovify) by [Jeremy Singer-Vine](https://github.com/jsvine)
 and [spacy](https://spacy.io).
 
 ![PyPI - Version](https://img.shields.io/pypi/v/django-markov)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-markov)
 ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/django/django-markov)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![security: bandit](https://img.shields.io/badge/security-bandit-brightgreen.svg)](https://github.com/PyCQA/bandit)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andrlik/django-markov/ci.yml?branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/andrlik/django-markov/badge.svg?branch=main)](https://coveralls.io/github/andrlik/django-markov?branch=main)
 
 
 This project is extracted from [django-quotes](https://github.com/andrlik/django-quotes). Once I realized I needed it for another project, but without
 the quotes, I spent an afternoon splitting it out.
```

### Comparing `django_markov-0.2.0/pyproject.toml` & `django_markov-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "django-markov"
-version = "0.2.0"
+version = "0.2.1"
 description = "django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences."
 authors = [
     { name = "Daniel Andrlik", email = "daniel@andrlik.org" }
 ]
 dependencies = [
-    "django>=5.0.3",
+    "django>=4.2",
     "markovify>=0.9.4",
     "spacy>=3.7.4",
 ]
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">= 3.11"
 classifiers = [
@@ -22,14 +22,29 @@
 ]
 
 [project.urls]
 Repository = "https://github.com/andrlik/django-markov"
 Documentation = "https://andrlik.github.io/django-markov"
 Homepage = "https://andrlik.github.io/django-markov"
 
+[project.optional-dependencies]
+test = [
+    "pytest-django",
+    "pytest-cov",
+    "pytest-sugar",
+    "pytest-asyncio",
+    "django-coverage",
+    "django-coverage-plugin",
+    "argon2-cffi",
+    "django-environ",
+    "pytest-mock",
+    "faker",
+    "django-extensions",
+]
+
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
@@ -54,14 +69,15 @@
     "django-coverage>=1.2.4",
     "django-coverage-plugin>=3.1.0",
     "argon2-cffi>=23.1.0",
     "django-environ>=0.11.2",
     "django-extensions>=3.2.3",
     "pytest-mock>=3.14.0",
     "faker>=24.4.0",
+    "bandit[toml]>=1.7.8",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/django_markov"]
@@ -208,15 +224,15 @@
   "--reuse-db"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.bumpversion]
-current_version = "0.2.0"
+current_version = "0.2.1"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
@@ -241,7 +257,10 @@
 [[tool.bumpversion.files]]
 filename = "CHANGELOG.md"
 search = "{current_version}...HEAD"
 replace = "{current_version}...{new_version}"
 
 [tool.django-stubs]
 django-settings-module = "tests.settings"
+
+[tool.bandit]
+exclude_dirs = ["tests", "conftest.py", "src/django_markov/migrations"]
```

### Comparing `django_markov-0.2.0/PKG-INFO` & `django_markov-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 Metadata-Version: 2.3
 Name: django-markov
-Version: 0.2.0
+Version: 0.2.1
 Summary: django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences.
 Project-URL: Repository, https://github.com/andrlik/django-markov
 Project-URL: Documentation, https://andrlik.github.io/django-markov
 Project-URL: Homepage, https://andrlik.github.io/django-markov
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
-Requires-Dist: django>=5.0.3
+Requires-Dist: django>=4.2
 Requires-Dist: markovify>=0.9.4
 Requires-Dist: spacy>=3.7.4
+Provides-Extra: test
+Requires-Dist: argon2-cffi; extra == 'test'
+Requires-Dist: django-coverage; extra == 'test'
+Requires-Dist: django-coverage-plugin; extra == 'test'
+Requires-Dist: django-environ; extra == 'test'
+Requires-Dist: django-extensions; extra == 'test'
+Requires-Dist: faker; extra == 'test'
+Requires-Dist: pytest-asyncio; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-django; extra == 'test'
+Requires-Dist: pytest-mock; extra == 'test'
+Requires-Dist: pytest-sugar; extra == 'test'
 Description-Content-Type: text/markdown
 
 # django-markov
 
 django-markov is a reusable Django app that enables you to create Markov text models, and store
 them in the database. Those models can then be used to generate Markov chain sentences.
 It relies on the excellent [markovify](https://github.com/jsvine/markovify) by [Jeremy Singer-Vine](https://github.com/jsvine)
 and [spacy](https://spacy.io).
 
 ![PyPI - Version](https://img.shields.io/pypi/v/django-markov)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-markov)
 ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/django/django-markov)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![security: bandit](https://img.shields.io/badge/security-bandit-brightgreen.svg)](https://github.com/PyCQA/bandit)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andrlik/django-markov/ci.yml?branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/andrlik/django-markov/badge.svg?branch=main)](https://coveralls.io/github/andrlik/django-markov?branch=main)
 
 
 This project is extracted from [django-quotes](https://github.com/andrlik/django-quotes). Once I realized I needed it for another project, but without
 the quotes, I spent an afternoon splitting it out.
```

