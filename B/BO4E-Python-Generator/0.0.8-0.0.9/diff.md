# Comparing `tmp/bo4e_python_generator-0.0.8.tar.gz` & `tmp/bo4e_python_generator-0.0.9.tar.gz`

## Comparing `bo4e_python_generator-0.0.8.tar` & `bo4e_python_generator-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,44 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/README.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/domain-specific-terms.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/requirements.in
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/requirements.txt
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/src/_bo4e_generator_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/src/bo4e_generator/__init__.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/src/bo4e_generator/__main__.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/src/bo4e_generator/parser.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/src/bo4e_generator/py.typed
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/src/bo4e_generator/schema.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/.gitignore
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/README.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/domain-specific-terms.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/requirements.in
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/_bo4e_generator_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/__init__.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/__main__.py
+-rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/parser.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/py.typed
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/schema.py
+-rw-r--r--   0        0        0    16417 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/sqlparser.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/custom_templates/BaseModel.jinja2
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/custom_templates/Config.jinja2
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/custom_templates/Enum.jinja2
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/src/bo4e_generator/custom_templates/ManyLinks.jinja2
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 bo4e_python_generator-0.0.9/PKG-INFO
```

### Comparing `bo4e_python_generator-0.0.8/.pre-commit-config.yaml` & `bo4e_python_generator-0.0.9/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.1.1
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
```

### Comparing `bo4e_python_generator-0.0.8/README.md` & `bo4e_python_generator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/requirements.txt` & `bo4e_python_generator-0.0.9/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile requirements.in
 #
 annotated-types==0.6.0
     # via pydantic
 argcomplete==3.1.2
     # via datamodel-code-generator
-black==24.1.1
+black==24.2.0
     # via datamodel-code-generator
 click==8.1.7
     # via
     #   -r requirements.in
     #   black
-datamodel-code-generator==0.25.3
+colorama==0.4.6
+    # via click
+datamodel-code-generator==0.25.4
     # via -r requirements.in
 dnspython==2.4.2
     # via email-validator
 email-validator==2.0.0.post2
     # via pydantic
 genson==1.2.2
     # via datamodel-code-generator
@@ -39,17 +41,15 @@
     #   black
     #   datamodel-code-generator
 pathspec==0.11.2
     # via black
 platformdirs==3.11.0
     # via black
 pydantic[email]==2.4.2
-    # via
-    #   datamodel-code-generator
-    #   pydantic
+    # via datamodel-code-generator
 pydantic-core==2.10.1
     # via pydantic
 pyyaml==6.0.1
     # via datamodel-code-generator
 typing-extensions==4.8.0
     # via
     #   pydantic
```

### Comparing `bo4e_python_generator-0.0.8/tox.ini` & `bo4e_python_generator-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/dependabot.yml` & `bo4e_python_generator-0.0.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/codeql-analysis.yml` & `bo4e_python_generator-0.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/coverage.yml` & `bo4e_python_generator-0.0.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/dependabot_automerge.yml` & `bo4e_python_generator-0.0.9/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/formatting.yml` & `bo4e_python_generator-0.0.9/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/packaging_test.yml` & `bo4e_python_generator-0.0.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/python-publish.yml` & `bo4e_python_generator-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/pythonlint.yml` & `bo4e_python_generator-0.0.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/.github/workflows/unittests.yml` & `bo4e_python_generator-0.0.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/dev_requirements/requirements-packaging.txt` & `bo4e_python_generator-0.0.9/dev_requirements/requirements-packaging.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,72 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile requirements-packaging.in
+#    pip-compile '.\dev_requirements\requirements-packaging.in'
 #
-bleach==6.0.0
-    # via readme-renderer
-build==1.0.3
-    # via -r dev_requirements/requirements-packaging.in
-certifi==2023.7.22
+build==1.2.1
+    # via -r .\dev_requirements\requirements-packaging.in
+certifi==2024.2.2
     # via requests
-cffi==1.15.1
-    # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
-cryptography==41.0.4
-    # via secretstorage
+colorama==0.4.6
+    # via build
 docutils==0.20.1
     # via readme-renderer
-idna==3.4
+idna==3.6
     # via requests
-importlib-metadata==6.7.0
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.2.3
+jaraco-classes==3.4.0
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
-keyring==23.13.1
+jaraco-context==4.3.0
+    # via keyring
+jaraco-functools==4.0.0
+    # via keyring
+keyring==25.1.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.1.0
-    # via jaraco-classes
-packaging==23.2
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+nh3==0.2.17
+    # via readme-renderer
+packaging==24.0
     # via build
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-pycparser==2.21
-    # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-readme-renderer==37.3
+pywin32-ctypes==0.2.2
+    # via keyring
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.4.2
+rich==13.7.1
     # via twine
-secretstorage==3.3.3
-    # via keyring
-six==1.16.0
-    # via bleach
 twine==5.0.0
-    # via -r dev_requirements/requirements-packaging.in
-urllib3==2.0.6
+    # via -r .\dev_requirements\requirements-packaging.in
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-webencodings==0.5.1
-    # via bleach
-zipp==3.15.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `bo4e_python_generator-0.0.8/src/bo4e_generator/__main__.py` & `bo4e_python_generator-0.0.9/src/bo4e_generator/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 import shutil
 from pathlib import Path
 from typing import Optional
 
 import click
 
-from bo4e_generator.parser import bo4e_init_file_content, bo4e_version_file_content, parse_bo4e_schemas
+from bo4e_generator.parser import OutputType, bo4e_init_file_content, bo4e_version_file_content, parse_bo4e_schemas
 from bo4e_generator.schema import get_namespace, get_version
+from bo4e_generator.sqlparser import format_code
 
 
 def resolve_paths(input_directory: Path, output_directory: Path) -> tuple[Path, Path]:
     """
     Resolve the input and output paths. The data-model-parser have problems with handling relative paths.
     """
     if not input_directory.is_absolute():
@@ -22,36 +23,36 @@
         output_directory = output_directory.resolve()
     return input_directory, output_directory
 
 
 def generate_bo4e_schemas(
     input_directory: Path,
     output_directory: Path,
-    pydantic_v1: bool = False,
+    output_type: OutputType,
     clear_output: bool = False,
     target_version: Optional[str] = None,
 ):
     """
     Generate all BO4E schemas from the given input directory and save them in the given output directory.
     """
     input_directory, output_directory = resolve_paths(input_directory, output_directory)
     namespace = get_namespace(input_directory)
-    file_contents = parse_bo4e_schemas(input_directory, namespace, pydantic_v1)
+    file_contents = parse_bo4e_schemas(input_directory, namespace, output_type)
     version = get_version(target_version, namespace)
     file_contents[Path("__version__.py")] = bo4e_version_file_content(version)
     file_contents[Path("__init__.py")] = bo4e_init_file_content(namespace, version)
     if clear_output and output_directory.exists():
         shutil.rmtree(output_directory)
 
     for relative_file_path, file_content in file_contents.items():
         file_path = output_directory / relative_file_path
         file_path.parent.mkdir(parents=True, exist_ok=True)
-        file_path.write_text(file_content, "utf-8")
+        file_content = format_code(file_content)
+        file_path.write_text(file_content, encoding="utf-8")
         print(f"Created {file_path}")
-
     print("Done.")
 
 
 @click.command()
 @click.option(
     "--input-dir",
     "-i",
@@ -63,20 +64,21 @@
     "--output-dir",
     "-o",
     type=click.Path(exists=False, file_okay=False, path_type=Path),
     help="Output directory for the generated python files.",
     required=True,
 )
 @click.option(
-    "--pydantic-v1/--pydantic-v2",
-    "-p1/-p2",
-    is_flag=True,
-    help="Generate pydantic v1 models instead of pydantic v2 models.",
+    "--output-type",
+    "-ot",
+    type=click.Choice(list(map(lambda x: x.name, OutputType)), case_sensitive=False),
+    # Taken from https://github.com/pallets/click/issues/605#issuecomment-889462570
+    help="Output type for the generated python files.",
     required=False,
-    default=False,
+    default=OutputType.PYDANTIC_V2,
 )
 @click.option(
     "--clear-output",
     help="Clear the output directory before saving the schemas. "
     "Otherwise, if e.g. schemas got deleted, they will not be removed from the output directory. "
     "Note: Generated output files will always overwrite existing files.",
     is_flag=True,
@@ -88,18 +90,18 @@
     help="Optionally set the target BO4E version. If not defined, it tries to read it from `_version`. "
     "If it can't be found, it will be set to 'unknown'.",
     type=str,
     default=None,
 )
 @click.version_option(package_name="BO4E-Python-Generator")
 def main(
-    input_dir: Path, output_dir: Path, pydantic_v1: bool, clear_output: bool, target_version: Optional[str] = None
+    input_dir: Path, output_dir: Path, clear_output: bool, output_type: OutputType, target_version: Optional[str] = None
 ):
     """
     CLI entry point for the bo4e-generator.
     """
-    generate_bo4e_schemas(input_dir, output_dir, pydantic_v1, clear_output, target_version)
+    generate_bo4e_schemas(input_dir, output_dir, output_type, clear_output, target_version)
 
 
 if __name__ == "__main__":
     # pylint: disable=no-value-for-parameter
     main()
```

### Comparing `bo4e_python_generator-0.0.8/src/bo4e_generator/parser.py` & `bo4e_python_generator-0.0.9/src/bo4e_generator/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 """
 Contains code to generate pydantic v2 models from json schemas.
 Since the used tool doesn't support all features we need, we monkey patch some functions.
 """
 
 import itertools
 import re
+import shutil
+from enum import Enum
 from pathlib import Path
-from typing import Sequence, Tuple, Type
+from typing import Any, Sequence, Type
 
 import datamodel_code_generator.parser.base
 import datamodel_code_generator.reference
 from datamodel_code_generator import DataModelType, PythonVersion
 from datamodel_code_generator.imports import IMPORT_DATETIME
 from datamodel_code_generator.model import DataModelSet, get_data_model_types
 from datamodel_code_generator.model.enum import Enum as _Enum
 from datamodel_code_generator.parser.jsonschema import JsonSchemaParser
 from datamodel_code_generator.types import DataType, StrictTypes, Types
 
 from bo4e_generator.schema import SchemaMetadata
+from bo4e_generator.sqlparser import adapt_parse_for_sql, remove_pydantic_field_import, write_many_many_links
+
+
+class OutputType(str, Enum):
+    """
+    enum to specify the output type
+    """
+
+    PYDANTIC_V2 = "pydantic_v2"
+    PYDANTIC_V1 = "pydantic_v1"
+    SQL_MODEL = "sql_model"
 
 
 def get_bo4e_data_model_types(
     data_model_type: DataModelType,
     target_python_version: PythonVersion,
     namespace: dict[str, SchemaMetadata],
     monkey_patch_enum_type: bool = True,
@@ -90,15 +103,15 @@
     Originally, this function would create something like "from ..enum import typ" and a field definition like
     "typ: Annotated[typ.Typ | None, Field(alias='_typ')] = None".
     This is in general a valid way to do it, but pydantic somehow doesn't like it. It will throw an error if you
     attempt to import an enum this way. Looks something like "'Typ' has no attribute 'Typ'".
     Anyway, this monkey patch changes the imports to "from ..enum.typ import Typ" which resolves the issue.
     """
 
-    def relative(current_module: str, reference: str) -> Tuple[str, str]:
+    def relative(current_module: str, reference: str) -> tuple[str, str]:
         """Find relative module path."""
 
         current_module_path = current_module.split(".") if current_module else []
         *reference_path, name = reference.split(".")
 
         if current_module_path == reference_path:
             return "", ""
@@ -166,48 +179,61 @@
     """
     Remove the future import from the generated code.
     """
     return re.sub(r"from __future__ import annotations\n\n", "", python_code)
 
 
 def parse_bo4e_schemas(
-    input_directory: Path, namespace: dict[str, SchemaMetadata], pydantic_v1: bool = False
+    input_directory: Path, namespace: dict[str, SchemaMetadata], output_type: OutputType
 ) -> dict[Path, str]:
     """
     Generate all BO4E schemas from the given input directory. Returns all file contents as dictionary:
     file path (relative to arbitrary output directory) => file content.
     """
     data_model_types = get_bo4e_data_model_types(
-        DataModelType.PydanticBaseModel if pydantic_v1 else DataModelType.PydanticV2BaseModel,
+        (
+            DataModelType.PydanticBaseModel
+            if output_type is OutputType.PYDANTIC_V1.name
+            else DataModelType.PydanticV2BaseModel
+        ),
         target_python_version=PythonVersion.PY_311,
         namespace=namespace,
     )
     monkey_patch_relative_import()
+
+    additional_arguments: dict[str, Any] = {}
+
+    if output_type is OutputType.SQL_MODEL.name:
+        # adapt input for SQLModel classes
+        namespace, additional_arguments, input_directory, links = adapt_parse_for_sql(input_directory, namespace)
+
     parser = JsonSchemaParser(
         input_directory,
         data_model_type=data_model_types.data_model,
         data_model_root_type=data_model_types.root_model,
         data_model_field_type=data_model_types.field_model,
         data_type_manager_type=data_model_types.data_type_manager,
         dump_resolve_reference_action=data_model_types.dump_resolve_reference_action,
-        # use_annotated=not pydantic_v1,
+        # use_annotated=OutputType is not OutputType.PYDANTIC_V1.name,
         use_double_quotes=True,
         use_schema_description=True,
         use_subclass_enum=True,
         use_standard_collections=True,
         use_union_operator=True,
+        use_field_description=True,
         set_default_enum_member=True,
         snake_case_field=True,
         field_constraints=True,
         capitalise_enum_members=True,
         base_path=input_directory,
         remove_special_field_name_prefix=True,
         allow_extra_fields=False,
         allow_population_by_field_name=True,
         use_default_kwarg=True,
+        **additional_arguments,
     )
     parse_result = parser.parse()
     if not isinstance(parse_result, dict):
         raise ValueError(f"Unexpected type of parse result: {type(parse_result)}")
     file_contents = {}
     for schema_metadata in namespace.values():
         module_path = schema_metadata.module_path_with_extension
@@ -219,12 +245,23 @@
             raise KeyError(
                 f"Could not find module {'.'.join(module_path)} in results: "
                 f"{list(parse_result.keys())}"  # type: ignore[union-attr]
                 # Item "str" of "str | dict[tuple[str, ...], Result]" has no attribute "keys"
                 # Somehow, mypy is not good enough to understand the instance-check above
             )
 
-        file_contents[schema_metadata.output_file] = remove_future_import(parse_result.pop(module_path).body)
+        python_code = remove_future_import(parse_result.pop(module_path).body)
+        if output_type is OutputType.SQL_MODEL.name:
+            # remove pydantic field
+            python_code = remove_pydantic_field_import(python_code)
+
+        file_contents[schema_metadata.output_file] = python_code
 
     file_contents.update({Path(*module_path): result.body for module_path, result in parse_result.items()})
 
+    # add SQLModel classes for many-to-many relationships in "many.py"
+    if output_type is OutputType.SQL_MODEL.name:
+        shutil.rmtree(input_directory)  # remove intermediate dir of schemas
+        if links:
+            file_contents[Path("many.py")] = write_many_many_links(links)
+
     return file_contents
```

### Comparing `bo4e_python_generator-0.0.8/src/bo4e_generator/schema.py` & `bo4e_python_generator-0.0.9/src/bo4e_generator/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     Create a namespace for the bo4e classes.
     """
 
     namespace: dict[str, SchemaMetadata] = {}
     for file_path in input_directory.rglob("*.json"):
         relative_path = file_path.relative_to(input_directory)
         module_path = tuple(camel_to_snake(part) for part in relative_path.with_suffix("").parts)
-        schema_text = file_path.read_text()
+        schema_text = file_path.read_text(encoding="utf-8")
         schema_parsed = json.loads(schema_text)
         class_name = schema_parsed["title"].replace(" ", "_")
 
         namespace[class_name] = SchemaMetadata(
             module_path=module_path,
             input_file=file_path,
             output_file=Path(*module_path).with_suffix(".py"),
```

### Comparing `bo4e_python_generator-0.0.8/.gitignore` & `bo4e_python_generator-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/pyproject.toml` & `bo4e_python_generator-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bo4e_python_generator-0.0.8/PKG-INFO` & `bo4e_python_generator-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: BO4E-Python-Generator
-Version: 0.0.8
+Version: 0.0.9
 Summary: This tool auto generates (customizable) pydantic v2 Code to implement the BO4E-Schemas.
 Project-URL: Changelog, https://github.com/Hochfrequenz/python_template_repository/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/python_template_repository
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: MIT
 Keywords: bo4e,code-generator
 Classifier: Development Status :: 4 - Beta
```

