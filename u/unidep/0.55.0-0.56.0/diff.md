# Comparing `tmp/unidep-0.55.0.tar.gz` & `tmp/unidep-0.56.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidep-0.55.0.tar", last modified: Wed Feb 21 20:37:32 2024, max compression
+gzip compressed data, was "unidep-0.56.0.tar", last modified: Thu Apr  4 12:37:26 2024, max compression
```

## Comparing `unidep-0.55.0.tar` & `unidep-0.56.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:37:32.004429 unidep-0.55.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-21 20:37:18.000000 unidep-0.55.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    62629 2024-02-21 20:37:32.004429 unidep-0.55.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    61008 2024-02-21 20:37:18.000000 unidep-0.55.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-21 20:37:18.000000 unidep-0.55.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 20:37:32.004429 unidep-0.55.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:37:32.000429 unidep-0.55.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-02-21 20:37:18.000000 unidep-0.55.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-02-21 20:37:18.000000 unidep-0.55.0/tests/test_conda_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-02-21 20:37:18.000000 unidep-0.55.0/tests/test_parse_yaml_local_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    71402 2024-02-21 20:37:18.000000 unidep-0.55.0/tests/test_unidep.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-02-21 20:37:18.000000 unidep-0.55.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-02-21 20:37:18.000000 unidep-0.55.0/tests/test_version_conflicts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:37:32.000429 unidep-0.55.0/unidep/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    42571 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    20303 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_conda_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    13056 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    21968 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_dependencies_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_hatch_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_pytest_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6916 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_setuptools_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/platform_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-02-21 20:37:18.000000 unidep-0.55.0/unidep/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:37:32.004429 unidep-0.55.0/unidep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    62629 2024-02-21 20:37:31.000000 unidep-0.55.0/unidep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-21 20:37:31.000000 unidep-0.55.0/unidep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 20:37:31.000000 unidep-0.55.0/unidep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-21 20:37:31.000000 unidep-0.55.0/unidep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-21 20:37:31.000000 unidep-0.55.0/unidep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-21 20:37:31.000000 unidep-0.55.0/unidep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.834399 unidep-0.56.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-04 12:37:16.000000 unidep-0.56.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    62612 2024-04-04 12:37:26.834399 unidep-0.56.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    60991 2024-04-04 12:37:16.000000 unidep-0.56.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-04 12:37:16.000000 unidep-0.56.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:37:26.834399 unidep-0.56.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.830399 unidep-0.56.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_conda_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_parse_yaml_local_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71403 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_unidep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_version_conflicts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.830399 unidep-0.56.0/unidep/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42572 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20304 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_conda_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13056 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22028 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_dependencies_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_hatch_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_pytest_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6917 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_setuptools_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/platform_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.834399 unidep-0.56.0/unidep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    62612 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/top_level.txt
```

### Comparing `unidep-0.55.0/LICENSE` & `unidep-0.56.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unidep-0.55.0/PKG-INFO` & `unidep-0.56.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidep
-Version: 0.55.0
+Version: 0.56.0
 Summary: Unified Conda and Pip requirements management.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/unidep
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
@@ -144,21 +144,22 @@
 
 Both files contain the following keys:
 
 - **name** (Optional): For documentation, not used in the output.
 - **channels**: List of conda channels for packages, such as `conda-forge`.
 - **dependencies**: Mix of Conda and Pip packages.
 - **local_dependencies** (Optional): List of paths to other `requirements.yaml` or `pyproject.toml` files to include.
-- **platforms** (Optional): List of platforms that are supported (used in `conda-lock`).
 - **optional_dependencies** (Optional): Dictionary with lists of optional dependencies.
+- **platforms** (Optional): List of platforms that are supported (used in `conda-lock`).
 
 Whether you use a `requirements.yaml` or `pyproject.toml` file, the same information can be specified in either.
 Choose the format that works best for your project.
 
 ### Example
+
 #### Example `requirements.yaml`
 
 Example of a `requirements.yaml` file:
 
 ```yaml
 name: example_environment
 channels:
@@ -171,22 +172,22 @@
   - conda: mumps                 # conda-only
   # Use platform selectors
   - conda: cuda-toolkit =11.8    # [linux64]
 local_dependencies:
   - ../other-project-using-unidep     # include other projects that use unidep
   - ../common-requirements.yaml       # include other requirements.yaml files
   - ../project-not-managed-by-unidep  # 🚨 Skips its dependencies!
-platforms:  # (Optional) specify platforms that are supported (used in conda-lock)
-  - linux-64
-  - osx-arm64
-optional_dependencies:  # (Optional) specify optional dependencies
+optional_dependencies:
   test:
     - pytest
   full:
-    - ../other-local-dep[test]  # include its optional dependencies
+    - ../other-local-dep[test]  # include its optional 'test' dependencies
+platforms:  # (Optional) specify platforms that are supported (used in conda-lock)
+  - linux-64
+  - osx-arm64
 ```
 
 > [!IMPORTANT]
 > `unidep` can process this during `pip install` and create a Conda installable `environment.yaml` or `conda-lock.yml` file, and more!
 
 > [!NOTE]
 > For a more in-depth example containing multiple installable projects, see the [`example`](example/) directory.
@@ -206,22 +207,22 @@
     { conda = "cuda-toolkit =11.8:linux64" }         # Use platform selectors by appending `:linux64`
 ]
 local_dependencies = [
     "../other-project-using-unidep",   # include other projects that use unidep
     "../common-requirements.yaml"      # include other requirements.yaml files
     "../project-not-managed-by-unidep" # 🚨 Skips its dependencies!
 ]
+optional_dependencies = {
+    test = ["pytest"],
+    full = ["../other-local-dep[test]"]  # include its optional 'test' dependencies
+}
 platforms = [ # (Optional) specify platforms that are supported (used in conda-lock)
     "linux-64",
     "osx-arm64"
 ]
-optional_dependencies = { # (Optional) specify optional dependencies
-    test = ["pytest"],
-    full = ["../other-local-dep[test]"]  # include its optional dependencies
-}
 ```
 
 This data structure is *identical* to the `requirements.yaml` format, with the exception of the `name` field and the [platform selectors](#platform-selectors).
 In the `requirements.yaml` file, one can use e.g., `# [linux64]`, which in the `pyproject.toml` file is `:linux64` at the end of the package name.
 
 See [Build System Integration](#jigsaw-build-system-integration) for more information on how to set up `unidep` with different build systems (Setuptools or Hatchling).
 
@@ -232,17 +233,17 @@
 ### Key Points
 
 - Standard names (e.g., `- numpy`) are assumed to be the same for Conda and Pip.
 - Use a dictionary with `conda: <package>` *and* `pip: <package>` to specify different names across platforms.
 - Use `pip:` to specify packages that are only available through Pip.
 - Use `conda:` to specify packages that are only available through Conda.
 - Use `# [selector]` (YAML only) or `package:selector` to specify platform-specific dependencies.
-- Use `platforms:` to specify the platforms that are supported.
 - Use `local_dependencies:` to include other `requirements.yaml` or `pyproject.toml` files and merge them into one. Also allows projects that are not managed by `unidep` to be included, but be aware that this skips their dependencies!
 - Use `optional_dependencies:` to specify optional dependencies. Can be installed like `unidep install ".[test]"` or `pip install ".[test]"`.
+- Use `platforms:` to specify the platforms that are supported. If omitted, all platforms are assumed to be supported.
 
 > *We use the YAML notation here, but the same information can be specified in `pyproject.toml` as well.*
 
 ### Supported Version Pinnings
 
 UniDep supports a range of version pinning operators (the same as Conda):
```

### Comparing `unidep-0.55.0/README.md` & `unidep-0.56.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,21 +101,22 @@
 
 Both files contain the following keys:
 
 - **name** (Optional): For documentation, not used in the output.
 - **channels**: List of conda channels for packages, such as `conda-forge`.
 - **dependencies**: Mix of Conda and Pip packages.
 - **local_dependencies** (Optional): List of paths to other `requirements.yaml` or `pyproject.toml` files to include.
-- **platforms** (Optional): List of platforms that are supported (used in `conda-lock`).
 - **optional_dependencies** (Optional): Dictionary with lists of optional dependencies.
+- **platforms** (Optional): List of platforms that are supported (used in `conda-lock`).
 
 Whether you use a `requirements.yaml` or `pyproject.toml` file, the same information can be specified in either.
 Choose the format that works best for your project.
 
 ### Example
+
 #### Example `requirements.yaml`
 
 Example of a `requirements.yaml` file:
 
 ```yaml
 name: example_environment
 channels:
@@ -128,22 +129,22 @@
   - conda: mumps                 # conda-only
   # Use platform selectors
   - conda: cuda-toolkit =11.8    # [linux64]
 local_dependencies:
   - ../other-project-using-unidep     # include other projects that use unidep
   - ../common-requirements.yaml       # include other requirements.yaml files
   - ../project-not-managed-by-unidep  # 🚨 Skips its dependencies!
-platforms:  # (Optional) specify platforms that are supported (used in conda-lock)
-  - linux-64
-  - osx-arm64
-optional_dependencies:  # (Optional) specify optional dependencies
+optional_dependencies:
   test:
     - pytest
   full:
-    - ../other-local-dep[test]  # include its optional dependencies
+    - ../other-local-dep[test]  # include its optional 'test' dependencies
+platforms:  # (Optional) specify platforms that are supported (used in conda-lock)
+  - linux-64
+  - osx-arm64
 ```
 
 > [!IMPORTANT]
 > `unidep` can process this during `pip install` and create a Conda installable `environment.yaml` or `conda-lock.yml` file, and more!
 
 > [!NOTE]
 > For a more in-depth example containing multiple installable projects, see the [`example`](example/) directory.
@@ -163,22 +164,22 @@
     { conda = "cuda-toolkit =11.8:linux64" }         # Use platform selectors by appending `:linux64`
 ]
 local_dependencies = [
     "../other-project-using-unidep",   # include other projects that use unidep
     "../common-requirements.yaml"      # include other requirements.yaml files
     "../project-not-managed-by-unidep" # 🚨 Skips its dependencies!
 ]
+optional_dependencies = {
+    test = ["pytest"],
+    full = ["../other-local-dep[test]"]  # include its optional 'test' dependencies
+}
 platforms = [ # (Optional) specify platforms that are supported (used in conda-lock)
     "linux-64",
     "osx-arm64"
 ]
-optional_dependencies = { # (Optional) specify optional dependencies
-    test = ["pytest"],
-    full = ["../other-local-dep[test]"]  # include its optional dependencies
-}
 ```
 
 This data structure is *identical* to the `requirements.yaml` format, with the exception of the `name` field and the [platform selectors](#platform-selectors).
 In the `requirements.yaml` file, one can use e.g., `# [linux64]`, which in the `pyproject.toml` file is `:linux64` at the end of the package name.
 
 See [Build System Integration](#jigsaw-build-system-integration) for more information on how to set up `unidep` with different build systems (Setuptools or Hatchling).
 
@@ -189,17 +190,17 @@
 ### Key Points
 
 - Standard names (e.g., `- numpy`) are assumed to be the same for Conda and Pip.
 - Use a dictionary with `conda: <package>` *and* `pip: <package>` to specify different names across platforms.
 - Use `pip:` to specify packages that are only available through Pip.
 - Use `conda:` to specify packages that are only available through Conda.
 - Use `# [selector]` (YAML only) or `package:selector` to specify platform-specific dependencies.
-- Use `platforms:` to specify the platforms that are supported.
 - Use `local_dependencies:` to include other `requirements.yaml` or `pyproject.toml` files and merge them into one. Also allows projects that are not managed by `unidep` to be included, but be aware that this skips their dependencies!
 - Use `optional_dependencies:` to specify optional dependencies. Can be installed like `unidep install ".[test]"` or `pip install ".[test]"`.
+- Use `platforms:` to specify the platforms that are supported. If omitted, all platforms are assumed to be supported.
 
 > *We use the YAML notation here, but the same information can be specified in `pyproject.toml` as well.*
 
 ### Supported Version Pinnings
 
 UniDep supports a range of version pinning operators (the same as Conda):
```

### Comparing `unidep-0.55.0/pyproject.toml` & `unidep-0.56.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 max-complexity = 18
 
 [tool.mypy]
 python_version = "3.7"
 
 # Use bump-my-version, e.g., call `bump-my-version bump minor`
 [tool.bumpversion]
-current_version = "0.55.0"
+current_version = "0.56.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "v{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "unidep/_version.py"
```

### Comparing `unidep-0.55.0/tests/test_cli.py` & `unidep-0.56.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """unidep CLI tests."""
+
 from __future__ import annotations
 
 import os
 import re
 import shutil
 import subprocess
 import textwrap
```

### Comparing `unidep-0.55.0/tests/test_conda_lock.py` & `unidep-0.56.0/tests/test_conda_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """unidep conda-lock tests."""
+
 from __future__ import annotations
 
 import shutil
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 from unittest.mock import patch
```

### Comparing `unidep-0.55.0/tests/test_parse_yaml_local_dependencies.py` & `unidep-0.56.0/tests/test_parse_yaml_local_dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """unidep's YAML parsing of the `local_dependencies` list."""
+
 from __future__ import annotations
 
 import shutil
 import textwrap
+from contextlib import nullcontext
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from ruamel.yaml import YAML
 
 from unidep import (
@@ -279,26 +281,26 @@
     toml_or_yaml: Literal["toml", "yaml"],
     tmp_path: Path,
 ) -> None:
     example_folder = tmp_path / "example"
     shutil.copytree(REPO_ROOT / "example", example_folder)
 
     # Add an extra project
-    extra_project = example_folder / "project69"
+    extra_project = example_folder / "extra_project"
     extra_project.mkdir(exist_ok=True, parents=True)
     (extra_project / "requirements.yaml").write_text(
         "local_dependencies: [../setup_py_project]",
     )
 
     # Add a line to project1 local_dependencies
     setup_py_project_req = example_folder / "setup_py_project" / "requirements.yaml"
     yaml = YAML(typ="safe")
     with setup_py_project_req.open("r") as f:
         requirements = yaml.load(f)
-    requirements["local_dependencies"].append("../project69")
+    requirements["local_dependencies"].append("../extra_project")
     with setup_py_project_req.open("w") as f:
         yaml.dump(requirements, f)
 
     setup_py_project_req = maybe_as_toml(toml_or_yaml, setup_py_project_req)
     found_files = find_requirements_files(example_folder)
     assert len(found_files) == 6
 
@@ -310,51 +312,62 @@
 
     local_dependencies = parse_local_dependencies(
         *found_files,
         check_pip_installable=True,
         verbose=True,
     )
     assert local_dependencies
+    # extra_project is not `pip installable` so it should not be included in the values()
     assert local_dependencies == {
         example_folder / "setup_py_project": [
             example_folder / "hatch_project",
             example_folder / "setuptools_project",
         ],
         example_folder / "setuptools_project": [
             example_folder / "hatch_project",
         ],
         example_folder / "pyproject_toml_project": [
             example_folder / "hatch_project",
         ],
+        example_folder / "extra_project": [
+            example_folder / "hatch_project",
+            example_folder / "setup_py_project",
+            example_folder / "setuptools_project",
+        ],
+        example_folder: [
+            example_folder / "hatch_project",
+            example_folder / "setup_py_project",
+            example_folder / "setuptools_project",
+        ],
     }
 
 
 @pytest.mark.parametrize("toml_or_yaml", ["toml", "yaml"])
 def test_parse_local_dependencies_pip_installable_with_non_installable_project(
     toml_or_yaml: Literal["toml", "yaml"],
     tmp_path: Path,
 ) -> None:
     example_folder = tmp_path / "example"
     shutil.copytree(REPO_ROOT / "example", example_folder)
 
     # Add an extra project
-    extra_project = example_folder / "project4"
+    extra_project = example_folder / "extra_project"
     extra_project.mkdir(exist_ok=True, parents=True)
     r_extra = extra_project / "requirements.yaml"
     r_extra.write_text("local_dependencies: [../setup_py_project]")
     r_extra = maybe_as_toml(toml_or_yaml, r_extra)
 
     # Add a line to hatch_project local_dependencies which should
-    # make hatch_project depend on setup_py_project, via project4! However, project4 is
+    # make hatch_project depend on setup_py_project, via extra_project! However, extra_project is
     # not `pip installable` so we're testing that path.
     setup_py_project_req = example_folder / "hatch_project" / "requirements.yaml"
     yaml = YAML(typ="safe")
     with setup_py_project_req.open("r") as f:
         requirements = yaml.load(f)
-    requirements["local_dependencies"] = ["../project4"]
+    requirements["local_dependencies"] = ["../extra_project"]
     with setup_py_project_req.open("w") as f:
         yaml.dump(requirements, f)
 
     found_files = find_requirements_files(example_folder)
     assert len(found_files) == 6
 
     local_dependencies = parse_local_dependencies(
@@ -377,14 +390,19 @@
             example_folder / "setup_py_project",
             example_folder / "setuptools_project",
         ],
         example_folder / "setuptools_project": [
             example_folder / "hatch_project",
             example_folder / "setup_py_project",
         ],
+        example_folder / "extra_project": [
+            example_folder / "hatch_project",
+            example_folder / "setup_py_project",
+            example_folder / "setuptools_project",
+        ],
     }
 
 
 def test_local_non_unidep_managed_dependency(tmp_path: Path) -> None:
     project1 = tmp_path / "project1"
     project1.mkdir(exist_ok=True, parents=True)
     project2 = tmp_path / "project2"
@@ -448,7 +466,54 @@
 
     local_dependencies = parse_local_dependencies(
         r1,
         verbose=True,
         raise_if_missing=False,
     )
     assert local_dependencies == {}
+
+
+@pytest.mark.parametrize("unidep_managed", [True, False])
+def test_parse_local_dependencies_without_local_deps_themselves(
+    tmp_path: Path,
+    unidep_managed: bool,  # noqa: FBT001
+) -> None:
+    project1 = tmp_path / "project1"
+    project1.mkdir(exist_ok=True, parents=True)
+    r1 = project1 / "requirements.yaml"
+    r1.write_text(
+        textwrap.dedent(
+            """\
+            local_dependencies:
+                - ../project2
+            """,
+        ),
+    )
+
+    project2 = tmp_path / "project2"
+    project2.mkdir(exist_ok=True, parents=True)
+    r2 = project2 / "pyproject.toml"
+    txt = textwrap.dedent(
+        """\
+            [build-system]
+            requires = ["setuptools", "wheel"]
+            """,
+    )
+    if unidep_managed:
+        txt += '[tool.unidep]\ndependencies = ["numpy"]'
+    r2.write_text(txt)
+    ctx = (
+        pytest.warns(UserWarning, match="not managed by unidep")
+        if not unidep_managed
+        else nullcontext()
+    )
+    with ctx:
+        local_dependencies = parse_local_dependencies(
+            r1,
+            verbose=True,
+            raise_if_missing=True,
+        )
+    assert local_dependencies == {project1: [project2]}
+
+    r2.write_text("")
+    with pytest.raises(RuntimeError, match="is not pip installable"):
+        parse_local_dependencies(r1, verbose=True, raise_if_missing=True)
```

### Comparing `unidep-0.55.0/tests/test_unidep.py` & `unidep-0.56.0/tests/test_unidep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """unidep tests."""
+
 from __future__ import annotations
 
 import textwrap
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
```

### Comparing `unidep-0.55.0/tests/test_utils.py` & `unidep-0.56.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the unidep.utils module."""
+
 from __future__ import annotations
 
 import sys
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
```

### Comparing `unidep-0.55.0/tests/test_version_conflicts.py` & `unidep-0.56.0/tests/test_version_conflicts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the version conflict resolution logic."""
+
 from __future__ import annotations
 
 import pytest
 
 from unidep._conflicts import (
     VersionConflictError,
     _combine_pinning_within_platform,
```

### Comparing `unidep-0.55.0/unidep/__init__.py` & `unidep-0.56.0/unidep/__init__.py`

 * *Files identical despite different names*

### Comparing `unidep-0.55.0/unidep/_cli.py` & `unidep-0.56.0/unidep/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 """unidep - Unified Conda and Pip requirements management.
 
 This module provides a command-line tool for managing conda environment.yaml files.
 """
+
 from __future__ import annotations
 
 import argparse
 import functools
 import importlib.util
 import json
 import os
```

### Comparing `unidep-0.55.0/unidep/_conda_env.py` & `unidep-0.56.0/unidep/_conda_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """unidep - Unified Conda and Pip requirements management.
 
 Conda environment file generation functions.
 """
+
 from __future__ import annotations
 
 import sys
 from collections import defaultdict
 from copy import deepcopy
 from typing import TYPE_CHECKING, NamedTuple, cast
```

### Comparing `unidep-0.55.0/unidep/_conda_lock.py` & `unidep-0.56.0/unidep/_conda_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """unidep - Unified Conda and Pip requirements management.
 
 This module provides the `unidep conda-lock` CLI command, used in `unidep._cli`.
 """
+
 from __future__ import annotations
 
 import shutil
 import subprocess
 import sys
 import tempfile
 import urllib.request
```

### Comparing `unidep-0.55.0/unidep/_conflicts.py` & `unidep-0.56.0/unidep/_conflicts.py`

 * *Files identical despite different names*

### Comparing `unidep-0.55.0/unidep/_dependencies_parsing.py` & `unidep-0.56.0/unidep/_dependencies_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,14 +479,18 @@
     return identifier
 
 
 # Alias for backwards compatibility
 parse_yaml_requirements = parse_requirements
 
 
+def _is_same_path(path1: Path, path2: Path) -> bool:
+    return path1.resolve() == path2.resolve()
+
+
 def _extract_local_dependencies(
     path: Path,
     base_path: Path,
     processed: set[Path],
     dependencies: dict[str, set[str]],
     *,
     check_pip_installable: bool = True,
@@ -535,27 +539,25 @@
                 )
                 raise RuntimeError(msg) from None
             continue
 
         project_path = str(requirements_path.parent)
         if project_path == str(base_path):
             continue
-        if not check_pip_installable or (
-            is_pip_installable(base_path)
-            and is_pip_installable(requirements_path.parent)
-        ):
+        if not check_pip_installable or is_pip_installable(requirements_path.parent):
             dependencies[str(base_path)].add(project_path)
         if verbose:
             print(f"🔗 Adding `{requirements_path}` from `local_dependencies`")
         _extract_local_dependencies(
             requirements_path,
             base_path,
             processed,
             dependencies,
             check_pip_installable=check_pip_installable,
+            verbose=verbose,
         )
 
 
 def parse_local_dependencies(
     *paths: Path,
     check_pip_installable: bool = True,
     verbose: bool = False,
```

### Comparing `unidep-0.55.0/unidep/_hatch_integration.py` & `unidep-0.56.0/unidep/_hatch_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """unidep - Unified Conda and Pip requirements management.
 
 This module contains the Hatchling integration.
 """
+
 from __future__ import annotations
 
 from pathlib import Path
 
 from hatchling.metadata.plugin.interface import MetadataHookInterface
 from hatchling.plugin import hookimpl
```

### Comparing `unidep-0.55.0/unidep/_pytest_plugin.py` & `unidep-0.56.0/unidep/_pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """unidep - Unified Conda and Pip requirements management.
 
 Pytest plugin for running only tests of changed files.
 
 WARNING: Still experimental and not documented.
 """
+
 from __future__ import annotations
 
 import logging
 import os
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING
```

### Comparing `unidep-0.55.0/unidep/_setuptools_integration.py` & `unidep-0.56.0/unidep/_setuptools_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 """unidep - Unified Conda and Pip requirements management.
 
 This module provides setuptools integration for unidep.
 """
+
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, NamedTuple
 
 from unidep._conflicts import resolve_conflicts
```

### Comparing `unidep-0.55.0/unidep/platform_definitions.py` & `unidep-0.56.0/unidep/platform_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """unidep - Unified Conda and Pip requirements management.
 
 Types and definitions for platforms, selectors, and markers.
 """
+
 from __future__ import annotations
 
 import sys
 from typing import NamedTuple, cast
 
 if sys.version_info >= (3, 8):
     from typing import Literal, get_args
```

### Comparing `unidep-0.55.0/unidep/utils.py` & `unidep-0.56.0/unidep/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """unidep - Unified Conda and Pip requirements management.
 
 This module provides utility functions used throughout the package.
 """
+
 from __future__ import annotations
 
 import codecs
 import platform
 import re
 import sys
 import warnings
@@ -72,28 +73,34 @@
     return codecs.decode(string, "unicode_escape")
 
 
 def is_pip_installable(folder: str | Path) -> bool:  # pragma: no cover
     """Determine if the project is pip installable.
 
     Checks for existence of setup.py or [build-system] in pyproject.toml.
+    If the `toml` library is available, it is used to parse the `pyproject.toml` file.
+    If the `toml` library is not available, the function checks for the existence of
+    a line starting with "[build-system]". This does not handle the case where
+    [build-system] is inside of a multi-line literal string.
     """
     path = Path(folder)
     if (path / "setup.py").exists():
         return True
 
-    # When toml makes it into the standard library, we can use that instead
-    # For now this is good enough, except it doesn't handle the case where
-    # [build-system] is inside of a multi-line literal string.
     pyproject_path = path / "pyproject.toml"
     if pyproject_path.exists():
-        with pyproject_path.open("r") as file:
-            for line in file:
-                if line.strip().startswith("[build-system]"):
-                    return True
+        if HAS_TOML:
+            with pyproject_path.open("rb") as file:
+                pyproject_data = tomllib.load(file)
+                return "build-system" in pyproject_data
+        else:
+            with pyproject_path.open("r") as file:
+                for line in file:
+                    if line.strip().startswith("[build-system]"):
+                        return True
     return False
 
 
 class UnsupportedPlatformError(Exception):
     """Raised when the current platform is not supported."""
```

### Comparing `unidep-0.55.0/unidep.egg-info/PKG-INFO` & `unidep-0.56.0/unidep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidep
-Version: 0.55.0
+Version: 0.56.0
 Summary: Unified Conda and Pip requirements management.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/unidep
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
@@ -144,21 +144,22 @@
 
 Both files contain the following keys:
 
 - **name** (Optional): For documentation, not used in the output.
 - **channels**: List of conda channels for packages, such as `conda-forge`.
 - **dependencies**: Mix of Conda and Pip packages.
 - **local_dependencies** (Optional): List of paths to other `requirements.yaml` or `pyproject.toml` files to include.
-- **platforms** (Optional): List of platforms that are supported (used in `conda-lock`).
 - **optional_dependencies** (Optional): Dictionary with lists of optional dependencies.
+- **platforms** (Optional): List of platforms that are supported (used in `conda-lock`).
 
 Whether you use a `requirements.yaml` or `pyproject.toml` file, the same information can be specified in either.
 Choose the format that works best for your project.
 
 ### Example
+
 #### Example `requirements.yaml`
 
 Example of a `requirements.yaml` file:
 
 ```yaml
 name: example_environment
 channels:
@@ -171,22 +172,22 @@
   - conda: mumps                 # conda-only
   # Use platform selectors
   - conda: cuda-toolkit =11.8    # [linux64]
 local_dependencies:
   - ../other-project-using-unidep     # include other projects that use unidep
   - ../common-requirements.yaml       # include other requirements.yaml files
   - ../project-not-managed-by-unidep  # 🚨 Skips its dependencies!
-platforms:  # (Optional) specify platforms that are supported (used in conda-lock)
-  - linux-64
-  - osx-arm64
-optional_dependencies:  # (Optional) specify optional dependencies
+optional_dependencies:
   test:
     - pytest
   full:
-    - ../other-local-dep[test]  # include its optional dependencies
+    - ../other-local-dep[test]  # include its optional 'test' dependencies
+platforms:  # (Optional) specify platforms that are supported (used in conda-lock)
+  - linux-64
+  - osx-arm64
 ```
 
 > [!IMPORTANT]
 > `unidep` can process this during `pip install` and create a Conda installable `environment.yaml` or `conda-lock.yml` file, and more!
 
 > [!NOTE]
 > For a more in-depth example containing multiple installable projects, see the [`example`](example/) directory.
@@ -206,22 +207,22 @@
     { conda = "cuda-toolkit =11.8:linux64" }         # Use platform selectors by appending `:linux64`
 ]
 local_dependencies = [
     "../other-project-using-unidep",   # include other projects that use unidep
     "../common-requirements.yaml"      # include other requirements.yaml files
     "../project-not-managed-by-unidep" # 🚨 Skips its dependencies!
 ]
+optional_dependencies = {
+    test = ["pytest"],
+    full = ["../other-local-dep[test]"]  # include its optional 'test' dependencies
+}
 platforms = [ # (Optional) specify platforms that are supported (used in conda-lock)
     "linux-64",
     "osx-arm64"
 ]
-optional_dependencies = { # (Optional) specify optional dependencies
-    test = ["pytest"],
-    full = ["../other-local-dep[test]"]  # include its optional dependencies
-}
 ```
 
 This data structure is *identical* to the `requirements.yaml` format, with the exception of the `name` field and the [platform selectors](#platform-selectors).
 In the `requirements.yaml` file, one can use e.g., `# [linux64]`, which in the `pyproject.toml` file is `:linux64` at the end of the package name.
 
 See [Build System Integration](#jigsaw-build-system-integration) for more information on how to set up `unidep` with different build systems (Setuptools or Hatchling).
 
@@ -232,17 +233,17 @@
 ### Key Points
 
 - Standard names (e.g., `- numpy`) are assumed to be the same for Conda and Pip.
 - Use a dictionary with `conda: <package>` *and* `pip: <package>` to specify different names across platforms.
 - Use `pip:` to specify packages that are only available through Pip.
 - Use `conda:` to specify packages that are only available through Conda.
 - Use `# [selector]` (YAML only) or `package:selector` to specify platform-specific dependencies.
-- Use `platforms:` to specify the platforms that are supported.
 - Use `local_dependencies:` to include other `requirements.yaml` or `pyproject.toml` files and merge them into one. Also allows projects that are not managed by `unidep` to be included, but be aware that this skips their dependencies!
 - Use `optional_dependencies:` to specify optional dependencies. Can be installed like `unidep install ".[test]"` or `pip install ".[test]"`.
+- Use `platforms:` to specify the platforms that are supported. If omitted, all platforms are assumed to be supported.
 
 > *We use the YAML notation here, but the same information can be specified in `pyproject.toml` as well.*
 
 ### Supported Version Pinnings
 
 UniDep supports a range of version pinning operators (the same as Conda):
```

### Comparing `unidep-0.55.0/unidep.egg-info/SOURCES.txt` & `unidep-0.56.0/unidep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

