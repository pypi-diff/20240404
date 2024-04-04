# Comparing `tmp/pdm_dockerize-0.3.1.tar.gz` & `tmp/pdm_dockerize-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_dockerize-0.3.1.tar", last modified: Fri Dec 22 02:20:11 2023, max compression
+gzip compressed data, was "pdm_dockerize-0.4.0.tar", last modified: Thu Apr  4 17:57:42 2024, max compression
```

## Comparing `pdm_dockerize-0.3.1.tar` & `pdm_dockerize-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0     1070 2023-12-22 02:19:52.459755 pdm_dockerize-0.3.1/LICENSE
--rw-r--r--   0        0        0     3819 2023-12-22 02:19:52.459755 pdm_dockerize-0.3.1/README.md
--rw-r--r--   0        0        0     3996 2023-12-22 02:20:11.863801 pdm_dockerize-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        6 2023-12-22 02:20:11.863801 pdm_dockerize-0.3.1/src/pdm_dockerize/VERSION
--rw-r--r--   0        0        0      321 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/__init__.py
--rw-r--r--   0        0        0     2510 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/commands.py
--rw-r--r--   0        0        0      447 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/config.py
--rw-r--r--   0        0        0     8445 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/entrypoint.py
--rw-r--r--   0        0        0      596 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/filters.py
--rw-r--r--   0        0        0     3724 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/installer.py
--rw-r--r--   0        0        0        0 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/src/pdm_dockerize/py.typed
--rw-r--r--   0        0        0      288 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[exclude-all].sh
--rw-r--r--   0        0        0      547 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh
--rw-r--r--   0        0        0      458 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[include-all-but-prefix].sh
--rw-r--r--   0        0        0      689 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh
--rw-r--r--   0        0        0      430 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[include-list].sh
--rw-r--r--   0        0        0      442 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[include-prefix-except].sh
--rw-r--r--   0        0        0      288 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[no-filter].sh
--rw-r--r--   0        0        0      299 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_pythonpath_explicit_src_layout.sh
--rw-r--r--   0        0        0      299 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_pythonpath_implicit_src_layout.sh
--rw-r--r--   0        0        0      793 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[args-placeholder-with-defaults].sh
--rw-r--r--   0        0        0      666 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[args-placeholder].sh
--rw-r--r--   0        0        0      428 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[call-with-arguments].sh
--rw-r--r--   0        0        0      390 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[call].sh
--rw-r--r--   0        0        0      353 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[cmd-as-dict].sh
--rw-r--r--   0        0        0      385 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[cmd-as-list].sh
--rw-r--r--   0        0        0      353 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[cmd-as-str].sh
--rw-r--r--   0        0        0      391 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[composite-inline].sh
--rw-r--r--   0        0        0      382 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[composite].sh
--rw-r--r--   0        0        0      397 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[env].sh
--rw-r--r--   0        0        0      503 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[env_file-override-precedance].sh
--rw-r--r--   0        0        0      481 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[env_file-override].sh
--rw-r--r--   0        0        0      503 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[env_file-precedance].sh
--rw-r--r--   0        0        0      481 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[env_file].sh
--rw-r--r--   0        0        0      288 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[no_script].sh
--rw-r--r--   0        0        0      526 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[pre-post].sh
--rw-r--r--   0        0        0      401 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[shared-env].sh
--rw-r--r--   0        0        0      481 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[shared-env_file].sh
--rw-r--r--   0        0        0      353 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[shell].sh
--rw-r--r--   0        0        0      596 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[whitespaces].sh
--rw-r--r--   0        0        0      353 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist.sh
--rw-r--r--   0        0        0      353 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist_to_target.sh
--rw-r--r--   0        0        0     1059 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     5379 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/test_entrypoint.py
--rw-r--r--   0        0        0      953 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/test_filters.py
--rw-r--r--   0        0        0     4011 2023-12-22 02:19:52.463755 pdm_dockerize-0.3.1/tests/test_pdm_dockerize.py
--rw-r--r--   0        0        0     5090 1970-01-01 00:00:00.000000 pdm_dockerize-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4591 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/README.md
+-rw-r--r--   0        0        0     4026 2024-04-04 17:57:42.411753 pdm_dockerize-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-04 17:57:42.407753 pdm_dockerize-0.4.0/src/pdm_dockerize/VERSION
+-rw-r--r--   0        0        0      321 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/commands.py
+-rw-r--r--   0        0        0      638 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/config.py
+-rw-r--r--   0        0        0     9236 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/entrypoint.py
+-rw-r--r--   0        0        0      596 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/filters.py
+-rw-r--r--   0        0        0     3534 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/installer.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-all].sh
+-rw-r--r--   0        0        0      575 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh
+-rw-r--r--   0        0        0      486 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all-but-prefix].sh
+-rw-r--r--   0        0        0      717 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh
+-rw-r--r--   0        0        0      458 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-list].sh
+-rw-r--r--   0        0        0      470 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-prefix-except].sh
+-rw-r--r--   0        0        0      316 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[no-filter].sh
+-rw-r--r--   0        0        0      440 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_global_env.sh
+-rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_global_env_file.sh
+-rw-r--r--   0        0        0      329 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_pythonpath_explicit_src_layout.sh
+-rw-r--r--   0        0        0      329 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_pythonpath_implicit_src_layout.sh
+-rw-r--r--   0        0        0      821 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder-with-defaults].sh
+-rw-r--r--   0        0        0      694 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder].sh
+-rw-r--r--   0        0        0      456 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[call-with-arguments].sh
+-rw-r--r--   0        0        0      418 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[call].sh
+-rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-dict].sh
+-rw-r--r--   0        0        0      413 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-list].sh
+-rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-str].sh
+-rw-r--r--   0        0        0      419 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[composite-inline].sh
+-rw-r--r--   0        0        0      410 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[composite].sh
+-rw-r--r--   0        0        0      470 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env].sh
+-rw-r--r--   0        0        0      593 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override-precedance].sh
+-rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override].sh
+-rw-r--r--   0        0        0      593 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-precedance].sh
+-rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file].sh
+-rw-r--r--   0        0        0      316 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[no_script].sh
+-rw-r--r--   0        0        0      554 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[pre-post].sh
+-rw-r--r--   0        0        0      474 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env].sh
+-rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env_file].sh
+-rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shell].sh
+-rw-r--r--   0        0        0      624 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[whitespaces].sh
+-rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist.sh
+-rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist_to_target.sh
+-rw-r--r--   0        0        0     1662 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     6305 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/test_entrypoint.py
+-rw-r--r--   0        0        0      953 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/test_filters.py
+-rw-r--r--   0        0        0     4011 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/test_pdm_dockerize.py
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 pdm_dockerize-0.4.0/PKG-INFO
```

### Comparing `pdm_dockerize-0.3.1/LICENSE` & `pdm_dockerize-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.3.1/README.md` & `pdm_dockerize-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -153,10 +153,39 @@
 Most of the time, you will look like this
 
 ```toml
 [tool.pdm.dockerize]
 include = ["uvicorn"]
 ```
 
+### Controlling environment
+
+`pdm-dockerize` respects defined environment variables:
+- scripts `env` variables are properly set
+- shared `_.env` variables are properly set
+- scripts `env_file` are properly loaded
+- shared `_.env_file` are properly loaded
+
+In addition, you can define some docker-only environment variables using the `tool.pdm.dockerize.env` table
+or some docker-only `.env` files using `tool.pdm.dockerize.env_file`
+
+#### Defining docker-only environment variables
+
+Those environment variables will only be effective in the docker entrypoint.
+
+```toml
+[tool.pdm.dockerize.env]
+VAR = "value"
+```
+
+#### Loading docker-only environment files
+
+This file will only be loaded in the docker entrypoint.
+
+```toml
+[tool.pdm.dockerize]
+env_file = "docker.env"
+```
+
 ## Contributing
 
 Read the [dedicated contributing guidelines](./CONTRIBUTING.md).
```

### Comparing `pdm_dockerize-0.3.1/pyproject.toml` & `pdm_dockerize-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Code Generators",
     "Typing :: Typed",
 ]
 dependencies = [
-    "pdm>=2.11",
+    "pdm>=2.13",
 ]
-version = "0.3.1"
+version = "0.4.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/noirbizarre/pdm-dockerize"
 Documentation = "https://github.com/noirbizarre/pdm-dockerize#readme"
@@ -60,14 +60,15 @@
 [tool.pdm.dev-dependencies]
 test = [
     "pdm[pytest]",
     "pytest>=7.1.2",
     "pytest-sugar>=0.9.5",
     "pytest-cov>=3.0.0",
     "syrupy>=3.0.6",
+    "shellcheck-py>=0.9.0.6",
 ]
 lint = [
     "black>=23.7.0",
     "codespell>=2.2.6",
     "mypy>=1.5.1",
     "ruff>=0.1.7",
     "tomli; python_version<'3.11'",
```

### Comparing `pdm_dockerize-0.3.1/src/pdm_dockerize/commands.py` & `pdm_dockerize-0.4.0/src/pdm_dockerize/commands.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.3.1/src/pdm_dockerize/entrypoint.py` & `pdm_dockerize-0.4.0/src/pdm_dockerize/entrypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 
     def as_script(self) -> str:
         """Render the `sh` entrypoint"""
         out = io.StringIO()
 
         out.write("#!/usr/bin/env sh\n\n")
         out.write("set -eu\n\n")
-        out.write("dirname=$(dirname $0)\n")
+        out.write('dirname=$(dirname "$0")\n')
         out.write('cmd=${1:-""}\n')
-        out.write("[ $cmd ] && shift\n")
-        out.write("cd $dirname > /dev/null\n")
+        out.write('[ "$cmd" ] && shift\n')
+        out.write('cd "$dirname" > /dev/null\n')
         out.write("\n")
         out.write(self.export_env())
         out.write("\n")
         out.write(self.usage())
         out.write("\n")
         out.write("case $cmd in\n")
 
@@ -80,16 +80,30 @@
     def export_env(self) -> str:
         """Export the environment variables"""
         out = io.StringIO()
         path = ["$(pwd)/bin", "$PATH"]
         pythonpath = ["$(pwd)/lib"]
         if package_dir := self.get_package_dir():
             pythonpath.insert(0, package_dir)
-        out.write(f"export PYTHONPATH={':'.join(pythonpath)}\n")
-        out.write(f"export PATH={':'.join(path)}\n")
+        out.write(self.export_var("PYTHONPATH", ":".join(f'"{p}"' for p in pythonpath)))
+        out.write(self.export_var("PATH", ":".join(f'"{p}"' for p in path)))
+        if env := self.settings.get("env"):
+            for name, value in env.items():
+                out.write(self.export_var(name, str(value)))
+        if env_file := self.settings.get("env_file"):
+            out.write(self.source_env(env_file))
+        return out.getvalue()
+
+    def export_var(self, name: str, value: str, indent: int = 0) -> str:
+        prefix = INDENT * indent
+        out = io.StringIO()
+        if not value.startswith('"') or not value.endswith('"'):
+            value = f'"{value}"'
+        out.write(f"{prefix}{name}={value}\n")
+        out.write(f"{prefix}export {name}\n")
         return out.getvalue()
 
     def get_package_dir(self) -> str | None:
         """An optional directory containing the project sources"""
         # TODO: find a better way to identify package-dir
         build_system = self.project.backend.build_system()
         if not build_system.get("build-backend") == "pdm.backend":
@@ -137,38 +151,40 @@
         return out.getvalue()
 
     def script_for(self, task: Task, params: str | None = None) -> str:
         """Render the script part for a single task"""
         out = io.StringIO()
         opts = exec_opts(self.runner.global_options, task.options)
         if (envfile := opts.get("env_file")) and isinstance(envfile, str):
-            out.write(self.source_env(envfile))
+            out.write(self.source_env(envfile, indent=2))
 
-        for var, value in opts.get("env", {}).items():
-            out.write(f'{2 * INDENT}{var}="{value}"\n')
+        for var, value in (opts.get("env") or {}).items():
+            out.write(self.export_var(var, value, indent=2))
 
         if isinstance(envfile, dict) and (override := envfile.get("override")):
-            out.write(self.source_env(override))
+            out.write(self.source_env(override, indent=2))
 
         if task.kind == "call":
             out.write(self.call_script(task))
         elif task.kind == "cmd":
             out.write(self.cmd_script(task, params))
         elif task.kind == "composite":
             out.write(self.composite_script(task, params))
         else:
             out.write(self.shell_script(task, params))
         return out.getvalue()
 
-    def source_env(self, envfile: str) -> str:
+    def source_env(self, envfile: str, indent: int = 0) -> str:
         out = io.StringIO()
-        out.write(f"{2 * INDENT}set -o allexport\n")
-        out.write(f"{2 * INDENT}[ -f {envfile} ] && . {envfile} ")
+        prefix = indent * INDENT
+        out.write(f"{prefix}set -o allexport\n")
+        out.write(f"{prefix}# shellcheck source=/dev/null\n")
+        out.write(f"{prefix}[ -f {envfile} ] && . {envfile} ")
         out.write(f"|| echo '{envfile} is ignored as it does not exist.'\n")
-        out.write(f"{2 * INDENT}set +o allexport\n")
+        out.write(f"{prefix}set +o allexport\n")
         return out.getvalue()
 
     def cmd_script(self, task: Task, params: str | None = None) -> str:
         if isinstance(task.args, str):
             script, interpolated = self.interpolate(task.args)
             script = " ".join(shlex.split(script, posix=False))
         else:
```

### Comparing `pdm_dockerize-0.3.1/src/pdm_dockerize/filters.py` & `pdm_dockerize-0.4.0/src/pdm_dockerize/filters.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.3.1/src/pdm_dockerize/installer.py` & `pdm_dockerize-0.4.0/src/pdm_dockerize/installer.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable
 
 from installer.destinations import Scheme
 from installer.records import RecordEntry
 from pdm.compat import Distribution
 from pdm.installers import Synchronizer
-from pdm.installers.installers import InstallDestination, _get_kind, _install_wheel
+from pdm.installers.installers import InstallDestination, PackageWheelSource, install
 from pdm.installers.manager import InstallManager
 
 from . import filters
 
 if TYPE_CHECKING:
     from installer.scripts import ScriptSection
     from pdm.environments import BaseEnvironment
@@ -38,23 +38,21 @@
         prepared = candidate.prepare(self.environment)
         additional_metadata = None
         if (direct_url := prepared.direct_url()) is not None:
             additional_metadata = {"direct_url.json": json.dumps(direct_url, indent=2).encode()}
         destination = FilteringDestination(
             scheme_dict=self.environment.get_paths(),
             interpreter=str(self.environment.interpreter.executable),
-            script_kind=_get_kind(self.environment),
+            script_kind=self.environment.script_kind,
             include=self.include,
             exclude=self.exclude,
         )
-        dist_info = _install_wheel(
-            wheel=str(prepared.build()),
-            destination=destination,
-            additional_metadata=additional_metadata,
-        )
+
+        source = PackageWheelSource(prepared.get_cached_package())
+        dist_info = install(source, destination, additional_metadata)
         return Distribution.at(dist_info)
 
 
 class DockerizeSynchronizer(Synchronizer):
     """A `Synchronizer` using the `DockerizeInstallManager`"""
 
     def get_manager(self) -> InstallManager:
@@ -63,26 +61,22 @@
 
 class FilteringDestination(InstallDestination):
     """An `InstallDestination` filtering installed binaries"""
 
     def __init__(
         self,
         *args: Any,
-        link_to: str | None = None,
-        link_method: LinkMethod | None = None,
-        link_individual: bool = False,
+        link_method: LinkMethod = "copy",
         include: list[str] | None = None,
         exclude: list[str] | None = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             *args,
-            link_to=link_to,
             link_method=link_method,
-            link_individual=link_individual,
             **kwargs,
         )
 
         self.include = include or []
         self.exclude = exclude or []
 
     def write_script(
```

### Comparing `pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh` & `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env sh
 
 set -eu
 
-dirname=$(dirname $0)
+dirname=$(dirname "$0")
 cmd=${1:-""}
-[ $cmd ] && shift
-cd $dirname > /dev/null
+[ "$cmd" ] && shift
+cd "$dirname" > /dev/null
 
-export PYTHONPATH=$(pwd)/lib
-export PATH=$(pwd)/bin:$PATH
+PYTHONPATH="$(pwd)/lib"
+export PYTHONPATH
+PATH="$(pwd)/bin":"$PATH"
+export PATH
 
 usage() {
     echo "Available commands"
     echo "=================="
     echo "test:something: pytest something"
     echo "ns:task2: ns:task2"
     echo "ns:task3: ns:task3"
```

### Comparing `pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh` & `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env sh
 
 set -eu
 
-dirname=$(dirname $0)
+dirname=$(dirname "$0")
 cmd=${1:-""}
-[ $cmd ] && shift
-cd $dirname > /dev/null
+[ "$cmd" ] && shift
+cd "$dirname" > /dev/null
 
-export PYTHONPATH=$(pwd)/lib
-export PATH=$(pwd)/bin:$PATH
+PYTHONPATH="$(pwd)/lib"
+export PYTHONPATH
+PATH="$(pwd)/bin":"$PATH"
+export PATH
 
 usage() {
     echo "Available commands"
     echo "=================="
     echo "test: pytest"
     echo "test:something: pytest something"
     echo "ns:task1: ns:task1"
```

### Comparing `pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[args-placeholder-with-defaults].sh` & `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder-with-defaults].sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env sh
 
 set -eu
 
-dirname=$(dirname $0)
+dirname=$(dirname "$0")
 cmd=${1:-""}
-[ $cmd ] && shift
-cd $dirname > /dev/null
+[ "$cmd" ] && shift
+cd "$dirname" > /dev/null
 
-export PYTHONPATH=$(pwd)/lib
-export PATH=$(pwd)/bin:$PATH
+PYTHONPATH="$(pwd)/lib"
+export PYTHONPATH
+PATH="$(pwd)/bin":"$PATH"
+export PATH
 
 usage() {
     echo "Available commands"
     echo "=================="
     echo "cmd: cmd.before {args:default value} cmd.after"
     echo "shell: shell.before {args:default value} shell.after"
     echo "composite: cmd --something ➤ shell {args:default value}"
```

### Comparing `pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[args-placeholder].sh` & `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder].sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env sh
 
 set -eu
 
-dirname=$(dirname $0)
+dirname=$(dirname "$0")
 cmd=${1:-""}
-[ $cmd ] && shift
-cd $dirname > /dev/null
+[ "$cmd" ] && shift
+cd "$dirname" > /dev/null
 
-export PYTHONPATH=$(pwd)/lib
-export PATH=$(pwd)/bin:$PATH
+PYTHONPATH="$(pwd)/lib"
+export PYTHONPATH
+PATH="$(pwd)/bin":"$PATH"
+export PATH
 
 usage() {
     echo "Available commands"
     echo "=================="
     echo "cmd: cmd.before {args} cmd.after"
     echo "shell: shell.before {args} shell.after"
     echo "composite: cmd --something ➤ shell {args}"
```

### Comparing `pdm_dockerize-0.3.1/tests/__snapshots__/test_entrypoint/test_serilization[whitespaces].sh` & `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[whitespaces].sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env sh
 
 set -eu
 
-dirname=$(dirname $0)
+dirname=$(dirname "$0")
 cmd=${1:-""}
-[ $cmd ] && shift
-cd $dirname > /dev/null
+[ "$cmd" ] && shift
+cd "$dirname" > /dev/null
 
-export PYTHONPATH=$(pwd)/lib
-export PATH=$(pwd)/bin:$PATH
+PYTHONPATH="$(pwd)/lib"
+export PYTHONPATH
+PATH="$(pwd)/bin":"$PATH"
+export PATH
 
 usage() {
     echo "Available commands"
     echo "=================="
     echo "cmd: whitespaces…"
     echo "shell: whitespaces…"
     echo "composite: whitespaces…"
```

### Comparing `pdm_dockerize-0.3.1/tests/test_entrypoint.py` & `pdm_dockerize-0.4.0/tests/test_entrypoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from pdm_dockerize.entrypoint import ProjectEntrypoint
 
 if TYPE_CHECKING:
     from pdm.project import Project
     from syrupy import SnapshotAssertion
 
+    from tests.conftest import ShellcheckFixture
+
 
 def entrypoint_for(project: Project, hooks: HookManager | None = None) -> str:
     return str(ProjectEntrypoint(project, hooks or HookManager(project)))
 
 
 CASES = {
     "no_script": {},
@@ -92,18 +94,25 @@
         "shell": {"shell": "shell.before {args:default value} shell.after"},
         "composite": {"composite": ["cmd --something", "shell {args:default value}"]},
     },
 }
 
 
 @pytest.mark.parametrize("scripts", [pytest.param(scripts, id=id) for id, scripts in CASES.items()])
-def test_serilization(project: Project, snapshot: SnapshotAssertion, scripts: dict[str, Any]):
+def test_serialization(
+    project: Project,
+    snapshot: SnapshotAssertion,
+    scripts: dict[str, Any],
+    shellcheck: ShellcheckFixture,
+):
     project.pyproject.settings["dockerize"] = {"include": "*"}
     project.pyproject.settings["scripts"] = scripts
-    assert entrypoint_for(project) == snapshot
+    entrypoint = entrypoint_for(project)
+    assert entrypoint == snapshot
+    shellcheck(entrypoint)
 
 
 @dataclass
 class FilterCase:
     id: str
     include: str | list[str] | None = None
     exclude: str | list[str] | None = None
@@ -153,7 +162,31 @@
         "build-backend": "pdm.backend",
     }
     pkg_dir = project.root / "src/pkg"
     pkg_dir.mkdir(parents=True, exist_ok=True)
     pkg_init = pkg_dir / "__init__.py"
     pkg_init.write_text("")
     assert entrypoint_for(project) == snapshot
+
+
+def test_global_env(
+    project: Project,
+    snapshot: SnapshotAssertion,
+    shellcheck: ShellcheckFixture,
+):
+    project.pyproject.settings["dockerize"] = {"include": "*", "env": {"VAR": 42, "LAST": "value"}}
+    project.pyproject.settings["scripts"] = {"hello": "echo 'Hello'"}
+    entrypoint = entrypoint_for(project)
+    assert entrypoint == snapshot
+    shellcheck(entrypoint)
+
+
+def test_global_env_file(
+    project: Project,
+    snapshot: SnapshotAssertion,
+    shellcheck: ShellcheckFixture,
+):
+    project.pyproject.settings["dockerize"] = {"include": "*", "env_file": "docker.env"}
+    project.pyproject.settings["scripts"] = {"hello": "echo 'Hello'"}
+    entrypoint = entrypoint_for(project)
+    assert entrypoint == snapshot
+    shellcheck(entrypoint)
```

### Comparing `pdm_dockerize-0.3.1/tests/test_filters.py` & `pdm_dockerize-0.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.3.1/tests/test_pdm_dockerize.py` & `pdm_dockerize-0.4.0/tests/test_pdm_dockerize.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.3.1/PKG-INFO` & `pdm_dockerize-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-dockerize
-Version: 0.3.1
+Version: 0.4.0
 Summary: Help generating docker images from PDM projects
 Author-Email: Axel Haustant <noirbizarre@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://github.com/noirbizarre/pdm-dockerize
 Project-URL: Documentation, https://github.com/noirbizarre/pdm-dockerize#readme
 Project-URL: Repository, https://github.com/noirbizarre/pdm-dockerize
 Project-URL: Issues, https://github.com/noirbizarre/pdm-dockerize/issues
 Requires-Python: >=3.8.1
-Requires-Dist: pdm>=2.11
+Requires-Dist: pdm>=2.13
 Description-Content-Type: text/markdown
 
 # pdm-dockerize
 
 [![CI](https://github.com/noirbizarre/pdm-dockerize/actions/workflows/ci.yml/badge.svg)](https://github.com/noirbizarre/pdm-dockerize/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/noirbizarre/pdm-dockerize/main.svg)](https://results.pre-commit.ci/latest/github/noirbizarre/pdm-dockerize/main)
 [![PyPI](https://img.shields.io/pypi/v/pdm-dockerize)](https://pypi.org/project/pdm-dockerize/)
@@ -182,10 +182,39 @@
 Most of the time, you will look like this
 
 ```toml
 [tool.pdm.dockerize]
 include = ["uvicorn"]
 ```
 
+### Controlling environment
+
+`pdm-dockerize` respects defined environment variables:
+- scripts `env` variables are properly set
+- shared `_.env` variables are properly set
+- scripts `env_file` are properly loaded
+- shared `_.env_file` are properly loaded
+
+In addition, you can define some docker-only environment variables using the `tool.pdm.dockerize.env` table
+or some docker-only `.env` files using `tool.pdm.dockerize.env_file`
+
+#### Defining docker-only environment variables
+
+Those environment variables will only be effective in the docker entrypoint.
+
+```toml
+[tool.pdm.dockerize.env]
+VAR = "value"
+```
+
+#### Loading docker-only environment files
+
+This file will only be loaded in the docker entrypoint.
+
+```toml
+[tool.pdm.dockerize]
+env_file = "docker.env"
+```
+
 ## Contributing
 
 Read the [dedicated contributing guidelines](./CONTRIBUTING.md).
```

