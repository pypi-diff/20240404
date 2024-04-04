# Comparing `tmp/pytest-helm-templates-0.0.1a0.tar.gz` & `tmp/pytest-helm-templates-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-helm-templates-0.0.1a0.tar", last modified: Thu Apr  4 01:53:53 2024, max compression
+gzip compressed data, was "pytest-helm-templates-0.0.1a1.tar", last modified: Thu Apr  4 14:05:37 2024, max compression
```

## Comparing `pytest-helm-templates-0.0.1a0.tar` & `pytest-helm-templates-0.0.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:53:53.553878 pytest-helm-templates-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 01:53:53.553878 pytest-helm-templates-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:53:53.545878 pytest-helm-templates-0.0.1a0/pytest_helm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:53:53.549878 pytest-helm-templates-0.0.1a0/pytest_helm_templates/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates/commands/template_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates/helm_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:53:53.549878 pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 01:53:53.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-04 01:53:53.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:53:53.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 01:53:53.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 01:53:53.000000 pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 01:53:53.553878 pytest-helm-templates-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-04 01:53:12.000000 pytest-helm-templates-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.388186 pytest-helm-templates-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 14:05:37.388186 pytest-helm-templates-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.380186 pytest-helm-templates-0.0.1a1/pytest_helm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.380186 pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/template_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/helm_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.380186 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 14:05:37.388186 pytest-helm-templates-0.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/setup.py
```

### Comparing `pytest-helm-templates-0.0.1a0/LICENSE` & `pytest-helm-templates-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a0/PKG-INFO` & `pytest-helm-templates-0.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Pytest fixtures for unit testing the output of helm templates
 Home-page: https://github.com/tdg5/pytest-helm-templates
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Framework :: Pytest
```

### Comparing `pytest-helm-templates-0.0.1a0/README.md` & `pytest-helm-templates-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a0/pyproject.toml` & `pytest-helm-templates-0.0.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a0/pytest_helm_templates/commands/template_command.py` & `pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/template_command.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a0/pytest_helm_templates/helm_runner.py` & `pytest-helm-templates-0.0.1a1/pytest_helm_templates/helm_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 import textwrap
 from os import path
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Dict, List, Optional
+from typing import IO, Any, Dict, List, Optional, Tuple, Union
 
 import yaml
 
 from pytest_helm_templates.commands import TemplateCommand
 
 
 class HelmRunner:
@@ -25,15 +25,15 @@
         name: str,
         api_versions: Optional[List[str]] = None,
         dry_run: Optional[str] = None,
         is_upgrade: Optional[bool] = None,
         kube_version: Optional[str] = None,
         namespace: Optional[str] = None,
         repo: Optional[str] = None,
-        values: Optional[List[str]] = None,
+        values: Optional[List[Union[Dict[str, Any], str]]] = None,
         version: Optional[str] = None,
     ) -> str:
         """
         This function is a bit hacky in that it requires creating a copy of
         NOTES.txt that's embedded in a YAML template, as such, it depends on a
         local chart. `helm template` doesn't currently return NOTES.txt, and
         otherwise NOTES.txt is only rendered during `helm install`.
@@ -98,36 +98,58 @@
         include_crds: Optional[bool] = None,
         is_upgrade: Optional[bool] = None,
         kube_version: Optional[str] = None,
         namespace: Optional[str] = None,
         repo: Optional[str] = None,
         show_only: Optional[List[str]] = None,
         skip_tests: Optional[bool] = None,
-        values: Optional[List[str]] = None,
+        values: Optional[List[Union[Dict[str, Any], str]]] = None,
         version: Optional[str] = None,
     ) -> List[Dict]:
         chart_path = Path(chart) if not self.cwd else Path(self.cwd).joinpath(chart)
-        helm_arguments = TemplateCommand.helm_arguments(
-            api_versions=api_versions,
-            chart=str(chart_path),
-            dry_run=dry_run,
-            include_crds=include_crds,
-            is_upgrade=is_upgrade,
-            kube_version=kube_version,
-            namespace=namespace,
-            name=name,
-            repo=repo,
-            show_only=show_only,
-            skip_tests=skip_tests,
-            values=values,
-            version=version,
-        )
-        templates_yaml = self._run(helm_arguments)
+
+        _values = []
+        temp_files: List[IO] = []
+        try:
+            if values:
+                for values_instance in values:
+                    if isinstance(values_instance, str):
+                        _values.append(values_instance)
+                    else:
+                        temp_file_path, temp_file = self._reify_values(values_instance)
+                        _values.append(temp_file_path)
+                        temp_files.append(temp_file)
+            helm_arguments = TemplateCommand.helm_arguments(
+                api_versions=api_versions,
+                chart=str(chart_path),
+                dry_run=dry_run,
+                include_crds=include_crds,
+                is_upgrade=is_upgrade,
+                kube_version=kube_version,
+                namespace=namespace,
+                name=name,
+                repo=repo,
+                show_only=show_only,
+                skip_tests=skip_tests,
+                values=_values,
+                version=version,
+            )
+            templates_yaml = self._run(helm_arguments)
+        finally:
+            for temp_file in temp_files:
+                temp_file.close()
+
         return list(yaml.safe_load_all(templates_yaml))
 
+    def _reify_values(self, values: Dict) -> Tuple[str, IO]:
+        temp_file = NamedTemporaryFile(delete=False, mode="w")
+        temp_file.write(yaml.safe_dump(values))
+        temp_file.flush()
+        return temp_file.name, temp_file
+
     def _run(self, helm_arguments: List[str]) -> str:
         completed_process = subprocess.run(
             helm_arguments,
             capture_output=True,
             cwd=self.cwd,
             env=self.env,
         )
```

### Comparing `pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/PKG-INFO` & `pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Pytest fixtures for unit testing the output of helm templates
 Home-page: https://github.com/tdg5/pytest-helm-templates
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Framework :: Pytest
```

### Comparing `pytest-helm-templates-0.0.1a0/pytest_helm_templates.egg-info/requires.txt` & `pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a0/setup.py` & `pytest-helm-templates-0.0.1a1/setup.py`

 * *Files identical despite different names*

