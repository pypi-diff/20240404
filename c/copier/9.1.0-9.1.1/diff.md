# Comparing `tmp/copier-9.1.0.tar.gz` & `tmp/copier-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier-9.1.0.tar", max compression
+gzip compressed data, was "copier-9.1.1.tar", max compression
```

## Comparing `copier-9.1.0.tar` & `copier-9.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1076 2023-11-27 10:41:54.680331 copier-9.1.0/LICENSE
--rw-r--r--   0        0        0     6516 2023-11-27 10:41:54.680331 copier-9.1.0/README.md
--rw-r--r--   0        0        0      189 2023-11-27 10:42:10.300549 copier-9.1.0/copier/__init__.py
--rw-r--r--   0        0        0      198 2023-11-27 10:41:54.680331 copier-9.1.0/copier/__main__.py
--rw-r--r--   0        0        0    12877 2023-11-27 10:41:54.680331 copier-9.1.0/copier/cli.py
--rw-r--r--   0        0        0     3957 2023-11-27 10:41:54.680331 copier-9.1.0/copier/errors.py
--rw-r--r--   0        0        0    41605 2023-11-27 10:41:54.680331 copier-9.1.0/copier/main.py
--rw-r--r--   0        0        0        1 2023-11-27 10:41:54.680331 copier-9.1.0/copier/py.typed
--rw-r--r--   0        0        0     2652 2023-11-27 10:41:54.680331 copier-9.1.0/copier/subproject.py
--rw-r--r--   0        0        0    17749 2023-11-27 10:41:54.680331 copier-9.1.0/copier/template.py
--rw-r--r--   0        0        0     6377 2023-11-27 10:41:54.680331 copier-9.1.0/copier/tools.py
--rw-r--r--   0        0        0     1477 2023-11-27 10:41:54.680331 copier-9.1.0/copier/types.py
--rw-r--r--   0        0        0    17874 2023-11-27 10:41:54.680331 copier-9.1.0/copier/user_data.py
--rw-r--r--   0        0        0     7211 2023-11-27 10:41:54.680331 copier-9.1.0/copier/vcs.py
--rw-r--r--   0        0        0     3584 2023-11-27 10:42:10.300549 copier-9.1.0/pyproject.toml
--rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 copier-9.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-01-16 15:39:49.634070 copier-9.1.1/LICENSE
+-rw-r--r--   0        0        0     6517 2024-01-16 15:39:49.634070 copier-9.1.1/README.md
+-rw-r--r--   0        0        0      189 2024-01-16 15:40:00.778215 copier-9.1.1/copier/__init__.py
+-rw-r--r--   0        0        0      198 2024-01-16 15:39:49.634070 copier-9.1.1/copier/__main__.py
+-rw-r--r--   0        0        0    12867 2024-01-16 15:39:49.634070 copier-9.1.1/copier/cli.py
+-rw-r--r--   0        0        0     3957 2024-01-16 15:39:49.634070 copier-9.1.1/copier/errors.py
+-rw-r--r--   0        0        0    41633 2024-01-16 15:39:49.634070 copier-9.1.1/copier/main.py
+-rw-r--r--   0        0        0        1 2024-01-16 15:39:49.634070 copier-9.1.1/copier/py.typed
+-rw-r--r--   0        0        0     2652 2024-01-16 15:39:49.634070 copier-9.1.1/copier/subproject.py
+-rw-r--r--   0        0        0    17754 2024-01-16 15:39:49.634070 copier-9.1.1/copier/template.py
+-rw-r--r--   0        0        0     6558 2024-01-16 15:39:49.634070 copier-9.1.1/copier/tools.py
+-rw-r--r--   0        0        0     1477 2024-01-16 15:39:49.634070 copier-9.1.1/copier/types.py
+-rw-r--r--   0        0        0    17874 2024-01-16 15:39:49.634070 copier-9.1.1/copier/user_data.py
+-rw-r--r--   0        0        0     7253 2024-01-16 15:39:49.634070 copier-9.1.1/copier/vcs.py
+-rw-r--r--   0        0        0     3794 2024-01-16 15:40:00.778215 copier-9.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7962 1970-01-01 00:00:00.000000 copier-9.1.1/PKG-INFO
```

### Comparing `copier-9.1.0/LICENSE` & `copier-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `copier-9.1.0/README.md` & `copier-9.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     ```
 
 ## Basic concepts
 
 Copier is composed of these main concepts:
 
 1. **Templates**. They lay out how to generate the subproject.
-1. **Questionaries**. They are configured in the template. Answers are used to generate
+1. **Questionnaires**. They are configured in the template. Answers are used to generate
    projects.
 1. **Projects**. This is where your real program lives. But it is usually generated
    and/or updated from a template.
 
 Copier targets these main human audiences:
 
 1.  **Template creators**. Programmers that repeat code too much and prefer a tool to do
```

### Comparing `copier-9.1.0/copier/cli.py` & `copier-9.1.1/copier/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Command line entrypoint. This module declares the Copier CLI applications.
+"""Command line entrypoint. This module declares the Copier CLI applications.
 
 Basically, there are 3 different commands you can run:
 
 -   [`copier`][copier.cli.CopierApp], the main app, which is a shortcut for the
     `copy` and `update` subapps.
 
     If the destination project is found and has [an answers
@@ -193,16 +192,15 @@
 
         updates_without_cli_overrides = {
             k: v for k, v in file_updates.items() if k not in self.data
         }
         self.data.update(updates_without_cli_overrides)
 
     def _worker(self, src_path: OptStr = None, dst_path: str = ".", **kwargs) -> Worker:
-        """
-        Run Copier's internal API using CLI switches.
+        """Run Copier's internal API using CLI switches.
 
         Arguments:
             src_path: The source path of the template to generate the project from.
             dst_path: The path to generate the project to.
             **kwargs: Arguments passed to [Worker][copier.main.Worker].
         """
         return Worker(
```

### Comparing `copier-9.1.0/copier/errors.py` & `copier-9.1.1/copier/errors.py`

 * *Files identical despite different names*

### Comparing `copier-9.1.0/copier/main.py` & `copier-9.1.1/copier/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             If it is `None`, the default value will be obtained from
             [copier.template.Template.answers_relpath][].
 
         vcs_ref:
             Specify the VCS tag/commit to use in the template.
 
         data:
-            Answers to the questionary defined in the template.
+            Answers to the questionnaire defined in the template.
 
         exclude:
             User-chosen additional [file exclusion patterns][exclude].
 
         use_prereleases:
             Consider prereleases when detecting the *latest* one?
 
@@ -367,16 +367,14 @@
             expected_contents:
                 Used to compare existing file contents with them. Allows to know if
                 rendering is needed.
         """
         assert not dst_relpath.is_absolute()
         assert not expected_contents or not is_dir, "Dirs cannot have expected content"
         dst_abspath = Path(self.subproject.local_abspath, dst_relpath)
-        if dst_relpath != Path(".") and self.match_exclude(dst_relpath):
-            return False
         previous_is_symlink = dst_abspath.is_symlink()
         try:
             previous_content: Union[bytes, Path]
             if previous_is_symlink:
                 previous_content = readlink(dst_abspath)
             else:
                 previous_content = dst_abspath.read_bytes()
@@ -405,15 +403,15 @@
                 quiet=self.quiet,
                 file_=sys.stderr,
             )
             return True
         return self._solve_render_conflict(dst_relpath)
 
     def _ask(self) -> None:
-        """Ask the questions of the questionary and record their answers."""
+        """Ask the questions of the questionnaire and record their answers."""
         result = AnswersMap(
             user_defaults=self.user_defaults,
             init=self.data,
             last=self.subproject.last_answers,
             metadata=self.template.metadata,
         )
 
@@ -622,15 +620,15 @@
                 src_mode = src_abspath.lstat().st_mode
                 dst_abspath.lchmod(src_mode)
 
     def _render_folder(self, src_abspath: Path) -> None:
         """Recursively render a folder.
 
         Args:
-            src_path:
+            src_abspath:
                 Folder to be rendered. It must be an absolute path within
                 the template.
         """
         assert src_abspath.is_absolute()
         src_relpath = src_abspath.relative_to(self.template_copy_root)
         dst_relpath = self._render_path(src_relpath)
         if dst_relpath is None:
@@ -672,14 +670,17 @@
                 return None
             # {{ _copier_conf.answers_file }} becomes the full path; in that case,
             # restore part to be just the end leaf
             if str(self.answers_relpath) == part:
                 part = Path(part).name
             rendered_parts.append(part)
         result = Path(*rendered_parts)
+        # Skip excluded paths.
+        if result != Path(".") and self.match_exclude(relpath):
+            return None
         if not is_template:
             templated_sibling = (
                 self.template.local_abspath
                 / f"{result}{self.template.templates_suffix}"
             )
             if templated_sibling.exists():
                 return None
```

### Comparing `copier-9.1.0/copier/subproject.py` & `copier-9.1.1/copier/subproject.py`

 * *Files identical despite different names*

### Comparing `copier-9.1.0/copier/template.py` & `copier-9.1.1/copier/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     class _Loader(yaml.FullLoader):
         """Intermediate class to avoid monkey-patching main loader."""
 
     YamlIncludeConstructor.add_to_loader_class(
         loader_class=_Loader, base_dir=conf_path.parent
     )
 
-    with open(conf_path) as f:
+    with conf_path.open("rb") as f:
         try:
             flattened_result = lflatten(yaml.load_all(f, Loader=_Loader))
         except yaml.parser.ParserError as e:
             raise InvalidConfigFileError(conf_path, quiet) from e
 
     merged_options = defaultdict(list)
     for option in (
```

### Comparing `copier-9.1.0/copier/tools.py` & `copier-9.1.1/copier/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,18 +189,25 @@
 
 
 def _re_octal_replace(match: re.Match) -> str:
     return bytes([int(match.group(1), 8), int(match.group(2), 8)]).decode("utf8")
 
 
 def normalize_git_path(path: str) -> str:
-    # A filename like âñ will be reported by Git
-    # as "\\303\\242\\303\\261" (octal notation).
-    # This can be disabled with `git config core.quotepath off`.
+    r"""Convert weird characters returned by Git to normal UTF-8 path strings.
 
+    A filename like âñ will be reported by Git as "\\303\\242\\303\\261" (octal notation).
+    This can be disabled with `git config core.quotepath off`.
+
+    Args:
+        path: The Git path to normalize.
+
+    Returns:
+        str: The normalized Git path.
+    """
     # Remove surrounding quotes
     if path[0] == path[-1] == '"':
         path = path[1:-1]
     # Repair double-quotes
     path = path.replace('\\"', '"')
     # Convert octal to utf8
     return _re_octal.sub(_re_octal_replace, path)
```

### Comparing `copier-9.1.0/copier/types.py` & `copier-9.1.1/copier/types.py`

 * *Files identical despite different names*

### Comparing `copier-9.1.0/copier/user_data.py` & `copier-9.1.1/copier/user_data.py`

 * *Files identical despite different names*

### Comparing `copier-9.1.0/copier/vcs.py` & `copier-9.1.1/copier/vcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 from plumbum.machines import LocalCommand
 
 from .errors import DirtyLocalWarning, ShallowCloneWarning
 from .types import OptBool, OptStr, OptStrOrPath, StrOrPath
 
 
 def get_git(context_dir: OptStrOrPath = None) -> LocalCommand:
-    """Gets `git` command, or fails if it's not available"""
+    """Gets `git` command, or fails if it's not available."""
     command = local["git"]
     if context_dir:
         command = command["-C", context_dir]
     return command
 
 
 def get_git_version() -> Version:
+    """Get the installed git version."""
     git = get_git()
 
     return Version(re.findall(r"\d+\.\d+\.\d+", git("version"))[0])
 
 
 GIT_PREFIX = ("git@", "git://", "git+", "https://github.com/", "https://gitlab.com/")
 GIT_POSTFIX = ".git"
```

### Comparing `copier-9.1.0/pyproject.toml` & `copier-9.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [tool.poetry]
 name = "copier"
 # This version is a placeholder autoupdated by poetry-dynamic-versioning
-version = "9.1.0"
+version = "9.1.1"
 description = "A library for rendering project templates."
 license = "MIT"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 authors = ["Ben Felder <ben@felder.io>"]
 homepage = "https://github.com/copier-org/copier"
 repository = "https://github.com/copier-org/copier"
 readme = "README.md"
 
 [tool.poetry.scripts]
 copier = "copier.__main__:copier_app_run"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/copier-org/copier/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0" # HACK https://github.com/PyCQA/isort/issues/1945
+python = ">=3.8"
 colorama = ">=0.4.6"
 decorator = ">=5.1.1"
-dunamai = ">=1.7.0"
+# HACK Remove markers when https://github.com/mtkennerly/dunamai/issues/74 is fixed
+dunamai = { version = ">=1.7.0", markers = "python_version < '4'" }
 funcy = ">=1.17"
-jinja2 = ">=3.1.1"
+jinja2 = ">=3.1.3"
 jinja2-ansible-filters = ">=1.3.1"
 packaging = ">=23.0"
 pathspec = ">=0.9.0"
 plumbum = ">=1.6.9"
 pydantic = ">=2.4.2"
 pygments = ">=2.7.1"
 pyyaml = ">=5.3.1"
@@ -70,15 +71,15 @@
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
 
 [tool.poetry.group.build]
 # Helper group just for helping nix to build properly
 optional = true
 
 [tool.poetry.group.build.dependencies]
-poetry-dynamic-versioning = ">=1.1.0"
+poetry-dynamic-versioning = { version = ">=1.1.0", markers = "python_version < '4'" }
 
 [tool.poe.tasks.clean]
 script = "devtasks:clean"
 help = "remove build/python artifacts"
 
 [tool.poe.tasks.coverage]
 cmd = "pytest --cov-report html --cov copier copier tests"
@@ -105,40 +106,40 @@
 help = "run the type (mypy) checker on the codebase"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 vcs = "git"
 
-[tool.black]
-target-version = ["py38"]
+[tool.ruff.lint]
+extend-select = ["B", "D", "E", "F", "I", "UP"]
+extend-ignore = ['B028', "B904", "D105", "D107", "E501"]
+
+[tool.ruff.lint.per-file-ignores]
+"tests/**" = ["D"]
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
+known-first-party = ["copier"]
 
-[tool.isort]
-profile = "black"
-combine_as_imports = true
-known_first_party = ["copier"]
+[tool.ruff.lint.pydocstyle]
+convention = "google"
 
 [tool.mypy]
 ignore_missing_imports = true
 plugins = ["pydantic.mypy"]
 warn_no_return = false
 
-[tool.pydocstyle]
-match_dir = "^copier"
-add_ignore = ["D105", "D107"]
-
 [tool.pytest.ini_options]
 addopts = "-n auto -ra"
-markers = [
-    "impure: needs network or is not 100% reproducible"
-]
+markers = ["impure: needs network or is not 100% reproducible"]
 
 [tool.commitizen]
 annotated_tag = true
 changelog_incremental = true
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "9.1.0"
+version = "9.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.7.0", "poetry-dynamic-versioning>=1.1.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `copier-9.1.0/PKG-INFO` & `copier-9.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: copier
-Version: 9.1.0
+Version: 9.1.1
 Summary: A library for rendering project templates.
 Home-page: https://github.com/copier-org/copier
 License: MIT
 Author: Ben Felder
 Author-email: ben@felder.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6)
 Requires-Dist: decorator (>=5.1.1)
-Requires-Dist: dunamai (>=1.7.0)
+Requires-Dist: dunamai (>=1.7.0) ; python_version < "4"
 Requires-Dist: funcy (>=1.17)
-Requires-Dist: jinja2 (>=3.1.1)
+Requires-Dist: jinja2 (>=3.1.3)
 Requires-Dist: jinja2-ansible-filters (>=1.3.1)
 Requires-Dist: packaging (>=23.0)
 Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: plumbum (>=1.6.9)
 Requires-Dist: pydantic (>=2.4.2)
 Requires-Dist: pygments (>=2.7.1)
 Requires-Dist: pyyaml (>=5.3.1)
@@ -131,15 +131,15 @@
     ```
 
 ## Basic concepts
 
 Copier is composed of these main concepts:
 
 1. **Templates**. They lay out how to generate the subproject.
-1. **Questionaries**. They are configured in the template. Answers are used to generate
+1. **Questionnaires**. They are configured in the template. Answers are used to generate
    projects.
 1. **Projects**. This is where your real program lives. But it is usually generated
    and/or updated from a template.
 
 Copier targets these main human audiences:
 
 1.  **Template creators**. Programmers that repeat code too much and prefer a tool to do
```

