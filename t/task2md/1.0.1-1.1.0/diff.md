# Comparing `tmp/task2md-1.0.1.tar.gz` & `tmp/task2md-1.1.0.tar.gz`

## Comparing `task2md-1.0.1.tar` & `task2md-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 task2md-1.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.0.1/.markdownlint.yaml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.0.1/.python-version
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.0.1/.releaserc
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.0.1/.vale.ini
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.0.1/.yamllint
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.0.1/Taskfile.project.yml
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.0.1/Taskfile.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.0.1/lychee.toml
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.0.1/mkdocs.yml
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.0.1/requirements-dev.lock
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.0.1/requirements.lock
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/cli.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task2md.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/file.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/header.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/task.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/variable.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/util/dir.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/__init__.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/__init__.py
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/file.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/header.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/task.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/util/__init__.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/util/dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/test_dir.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/test_file.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/test_task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/files/empty.yml
--rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/files/lint.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/__init__.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_file.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_header.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_task.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_variable.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/util/test_dir.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.0.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.0.1/LICENSE
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.0.1/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 task2md-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.1.0/.markdownlint.yaml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.1.0/.python-version
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.1.0/.releaserc
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.1.0/.vale.ini
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.1.0/.yamllint
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.1.0/Taskfile.project.yml
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.1.0/Taskfile.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.1.0/lychee.toml
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.1.0/requirements.lock
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/cli.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task2md.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/file.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/header.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/task.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/variable.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/util/dir.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/__init__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/__init__.py
+-rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/file.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/header.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/index.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/task.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/util/__init__.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/util/dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/test_dir.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/test_file.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/test_task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/files/empty.yml
+-rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/files/lint.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/__init__.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_file.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_header.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_index.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_task.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_variable.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/util/test_dir.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.1.0/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.1.0/PKG-INFO
```

### Comparing `task2md-1.0.1/.gitlab-ci.yml` & `task2md-1.1.0/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -25,10 +25,11 @@
     - rye sync
     - rye run pytest --version
     - mkdir -p reports/cov
   script:
     - rye run test
 
 gitlab-release:
+  retry: 1
   before_script:
     - npx semantic-release --dry-run --no-ci
     - if [ -s .VERSION ]; then task 00:project-set-version VERSION=$(cat .VERSION); fi
```

### Comparing `task2md-1.0.1/.pre-commit-config.yaml` & `task2md-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/Taskfile.project.yml` & `task2md-1.1.0/Taskfile.project.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/Taskfile.yml` & `task2md-1.1.0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/requirements-dev.lock` & `task2md-1.1.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/src/task2md/task2md.py` & `task2md-1.1.0/src/task2md/task2md.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
 import os
 from typing import List
 
 import click
 
-from task2md.task.file import File
+from task2md.template.file import File
+from task2md.template.index import Index
 from task2md.util.dir import Dir
 
 
 @click.group()
-@click.version_option("1.0.1", prog_name="task2md")
+@click.version_option("1.1.0", prog_name="task2md")
 def cli() -> None:
     """A CLI tool to generate markdown documentation files from Task files."""
     pass
 
 
 @cli.command()
 @click.option(
@@ -56,25 +57,31 @@
 
         except OSError as error:
             raise click.ClickException(
                 "Output directory can not be created!\n" + str(error)
             )
 
         try:
+            index_file = Index()
             for filename in task_files:
                 task_file = File(path=f"{in_dir}/{filename}")
                 task_file.generate(out_dir)
 
+                index_file.task_files.append(task_file)
+
                 click.echo(
                     f"Task documentation generated: {task_file.get_filename()}.md"
                 )
+            filename = "index"
+            index_file.generate(out_dir)
+            click.echo("Index documentation generated: index.md")
 
         except ValueError as ve:
             raise click.ClickException(
-                "Error on reading file {} :\n {}".format(filename, str(ve))
+                "Error on reading or writing file {} :\n {}".format(filename, str(ve))
             )
 
 
 @cli.command()
 @click.option(
     "-i",
     "--input",
```

### Comparing `task2md-1.0.1/src/task2md/task/file.py` & `task2md-1.1.0/src/task2md/template/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import re
 from pathlib import Path
 from typing import Any, Dict, List
 
 import yaml
 from pydantic import BaseModel
 
-from task2md.task.header import Header
-from task2md.task.task import Task
-from task2md.task.variable import Variable
+from task2md.template.header import Header
+from task2md.template.task import Task
+from task2md.template.variable import Variable
 from task2md.util.dir import Dir
 
 
 class File(BaseModel):
     """File Task content class"""
 
     path: str = ""
@@ -38,15 +38,15 @@
         Args:
             dir (Dir): The dir object
         """
         self.load()
         self.parse()
         output = self.to_md()
 
-        output_filename = dir.path + "/" + self.get_filename() + ".md"
+        output_filename = f"{dir.path}/{self.get_filename()}.md"
 
         with open(output_filename, "w") as f:
             f.write(output)
 
     def load(self) -> None:
         """Load file content from path"""
         with open(self.path) as f:
@@ -119,17 +119,17 @@
             str: Markdown content
         """
         output = ""
         # Tag
         output += self.tags_to_md()
 
         # Top
-        output += "---\n\n# " + self.get_filename() + "\n\n"
+        output += f"---\n\n# {self.get_filename()}\n\n"
         output += self.header.description + "\n\n"
-        output += '!!! info "' + self.get_filename() + ' template details"\n\n'
+        output += f'!!! info "{self.get_filename()} template details"\n\n'
         output += self.header_to_md()
 
         # Tasks list
         output += "## :material-list-box: List of tasks\n"
         output += self.tasks_list_to_md() + "\n"
 
         # Global variables
@@ -203,17 +203,18 @@
         """
         output = """
 | Tasks | Description |
 | ----- | ----------- |
 """
         for task in self.tasks:
             file_name = self.get_filename()
+            escape_task_desc = task.desc.replace("|", r"\|")
             output += (
                 f"| [`{file_name}:{task.name}`](#{file_name}{task.name})"
-                f" | {task.desc} |\n"
+                f" | {escape_task_desc} |\n"
             )
 
         return output
 
     def global_variables_to_md(self) -> str:
         """Return the global variables to a markdown table
```

### Comparing `task2md-1.0.1/src/task2md/task/header.py` & `task2md-1.1.0/src/task2md/template/header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/src/task2md/task/task.py` & `task2md-1.1.0/src/task2md/template/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import re
 from typing import ClassVar, List
 
 from pydantic import BaseModel
 
 
 class Argument(BaseModel):
+    """Task argument class"""
+
     label: str = ""
     value: str = ""
 
 
 class Task(BaseModel):
     """Task class"""
```

### Comparing `task2md-1.0.1/src/task2md/util/dir.py` & `task2md-1.1.0/src/task2md/util/dir.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/tests/test_dir.py` & `task2md-1.1.0/tests/test_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,40 +5,39 @@
 from shutil import rmtree
 
 from click.testing import CliRunner
 
 from task2md import task2md
 
 
-class TestDir:
+class TestFile:
     def get_output_content(self, output_path: str) -> str:
         file_out = pathlib.Path(output_path)
         with open(file_out) as f:
             return f.read()
 
-    def test_dir_help(self) -> None:
+    def test_file_help(self) -> None:
         runner = CliRunner()
-        result = runner.invoke(task2md.cli, ["dir", "--help"])
+        result = runner.invoke(task2md.cli, ["file", "--help"])
         assert result.exit_code == 0
-        assert "dir [OPTIONS]" in result.stdout
+        assert "file [OPTIONS]" in result.stdout
 
-    def test_dir_missing_option(self) -> None:
+    def test_file_missing_option(self) -> None:
         runner = CliRunner()
-        result = runner.invoke(task2md.cli, ["dir"])
+        result = runner.invoke(task2md.cli, ["file"])
         assert result.exit_code == 2
         assert "Error: Missing option" in result.stdout
 
-    def test_dir_short_options_default_dir(self) -> None:
+    def test_file_short_options_default_dir(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
             task2md.cli,
-            ["dir", "-i", "tests/files"],
+            ["file", "-i", "tests/files/lint.yml"],
         )
         assert result.exit_code == 0
-        assert "Task documentation generated: empty.md" in result.stdout
         assert "Task documentation generated: lint.md" in result.stdout
         output = self.get_output_content("lint.md")
         assert "tags:" in output
         assert "  - lint" in output
         assert " * :material-check-circle: Status: stable" in output
         assert " * :material-license: License: MIT" in output
         assert "| [`lint:all`](#lintall) " in output
@@ -51,69 +50,74 @@
         assert "| Arguments | Description |" in output
         assert "| Fix files (optional, by default no) |" in output
         assert "| `MEX " in output
         assert "Notes:" in output
         assert "starting by dot" in output
         assert '!!! info "Requirements:' in output
         assert "    - yamllint or docker" in output
-        os.remove("empty.md")
         os.remove("lint.md")
 
-    def test_dir_long_options_default_dir(self) -> None:
+    def test_file_long_options_default_dir(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
             task2md.cli,
-            ["dir", "--input", "tests/files"],
+            ["file", "--input", "tests/files/lint.yml"],
         )
         assert result.exit_code == 0
-        assert "Task documentation generated: empty.md" in result.stdout
         assert "Task documentation generated: lint.md" in result.stdout
         output = self.get_output_content("lint.md")
         assert "| `IMAGE_HADOLINT` |" in output
-        os.remove("empty.md")
         os.remove("lint.md")
 
-    def test_dir_dir_create_short_options(self) -> None:
+    def test_file_dir_create_short_options(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
             task2md.cli,
-            ["dir", "-i", "tests/files", "-d", ".tmp-not-exist"],
+            ["file", "-i", "tests/files/lint.yml", "-d", ".tmp-not-exist"],
         )
         assert result.exit_code == 0
-        assert "Task documentation generated: empty.md" in result.stdout
         assert "Task documentation generated: lint.md" in result.stdout
         assert os.path.exists(".tmp-not-exist/lint.md")
         output = self.get_output_content(".tmp-not-exist/lint.md")
         assert "| `IMAGE_HADOLINT` |" in output
         rmtree(".tmp-not-exist")
 
-    def test_dir_dir_create_long_options(self) -> None:
+    def test_file_dir_create_long_options(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
             task2md.cli,
-            ["dir", "--input", "tests/files", "--dir", ".tmp-not-exist"],
+            ["file", "--input", "tests/files/lint.yml", "--dir", ".tmp-not-exist"],
         )
         assert result.exit_code == 0
-        assert "Task documentation generated: empty.md" in result.stdout
         assert "Task documentation generated: lint.md" in result.stdout
         assert os.path.exists(".tmp-not-exist/lint.md")
         output = self.get_output_content(".tmp-not-exist/lint.md")
         assert "| `IMAGE_HADOLINT` |" in output
         rmtree(".tmp-not-exist")
 
-    def test_dir_not_found(self) -> None:
+    def test_file_not_found(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
             task2md.cli,
-            ["dir", "--input", "tests/not-exist"],
+            ["file", "--input", "tests/files/not-exist.yml"],
         )
         assert result.exit_code == 2
-        assert "Directory 'tests/not-exist' does not exist" in result.stdout
+        assert "File 'tests/files/not-exist.yml' does not exist" in result.stdout
 
-    def test_dir_no_yml_file(self) -> None:
+    def test_file_wrong_file(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
             task2md.cli,
-            ["dir", "--input", "tests"],
+            ["file", "--input", "/bin/sh"],
+        )
+        assert result.exit_code == 1
+        assert "Error on reading file /bin/sh" in result.stdout
+
+    def test_file_empty(self) -> None:
+        runner = CliRunner()
+        result = runner.invoke(
+            task2md.cli,
+            ["file", "-i", "tests/files/empty.yml"],
         )
         assert result.exit_code == 0
-        assert "No yaml file found in: tests" in result.stdout
+        assert "Task documentation generated: empty.md" in result.stdout
+        os.remove("empty.md")
```

### Comparing `task2md-1.0.1/tests/test_task2md.py` & `task2md-1.1.0/tests/test_task2md.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/tests/files/lint.yml` & `task2md-1.1.0/tests/files/lint.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/tests/task/test_file.py` & `task2md-1.1.0/tests/task/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 
-from task2md.task.file import File
+from task2md.template.file import File
 
 HEADER_FULL = """
 #
 # @description: A set of tasks to lint different types of files.
 # @tags: lint, docker, CI
 # @authors: FX Soubirou <soubirou@yahoo.fr>, FXS <fxs@example.com>
 # File :material-bookmark-check:/:material-bookmark-remove:
@@ -107,34 +107,30 @@
         f = File(content=empty)
         f.parse()
         assert f.yaml == {}
         assert f.global_variables == []
         assert f.parsed is True
 
     def test_file_get_filename(self) -> None:
-        f = File(content="")
-        f.path = "my_dir/lint.yml"
+        f = File(content="", path="my_dir/lint.yml")
         assert f.get_filename() == "lint"
         assert f.parsed is False
 
     def test_file_get_filename_no_extension(self) -> None:
-        f = File(content="")
-        f.path = "my_dir/lint"
+        f = File(content="", path="my_dir/lint")
         assert f.get_filename() == "lint"
         assert f.parsed is False
 
     def test_file_get_filename_no_dir(self) -> None:
-        f = File(content="")
-        f.path = "lint.yml"
+        f = File(content="", path="lint.yml")
         assert f.get_filename() == "lint"
         assert f.parsed is False
 
     def test_file_header(self) -> None:
-        f = File(content=HEADER_FULL)
-        f.path = "my_dir/lint.yml"
+        f = File(content=HEADER_FULL, path="my_dir/lint.yml")
         f.parse()
         assert f.global_variables == []
         assert f.header.license == "MIT"
         assert (
             f.header.description == "A set of tasks to lint different types of files."
         )
         assert f.header.tags == ["lint", "docker", "CI"]
@@ -230,22 +226,21 @@
         assert (
             "    * :material-home: Home: [https://gitlab.com/op_so/task/task-templates](https://gitlab.com/op_so/task/task-templates)"
             in output
         )
         assert "    * :material-license: License: MIT" in output
 
     def test_file_tasks_list_to_md(self) -> None:
-        f = File(content=TASKS)
-        f.path = "my_dir/lint.yml"
+        f = File(content=TASKS, path="my_dir/lint.yml")
         f.parse()
         output = f.tasks_list_to_md()
 
         assert TASKS_LIST_HEADER in output
         assert (
-            '| [`lint:all`](#lintall) | Linter for files, markdown, yaml extensions. Arguments: [FIX|F=y|Y] [MEX|M="#node_modules"] (*) |'
+            r'| [`lint:all`](#lintall) | Linter for files, markdown, yaml extensions. Arguments: [FIX\|F=y\|Y] [MEX\|M="#node_modules"] (*) |'
             in output
         )
         assert "| [`lint:file`](#lintfile) | Linter for files" in output
 
     def test_file_global_variables_to_md(self) -> None:
         f = File(content=VARS4)
         f.parse()
@@ -254,16 +249,15 @@
 
         assert VARS_HEADER in output
         assert "| `IMAGE_DEFAULT` |" in output
         assert "| Default image for # lint:vale task |" in output
         assert "| `hadolint/hadolint` |" in output
 
     def test_file_to_md(self) -> None:
-        f = File(content=(HEADER_FULL + VARS4))
-        f.path = "my_dir/lint.yml"
+        f = File(content=(HEADER_FULL + VARS4), path="my_dir/lint.yml")
         f.parse()
         output = f.to_md()
 
         assert "tags:" in output
         assert "  - lint" in output
         assert "# lint" in output
         assert "A set of tasks to lint different types of files." in output
```

### Comparing `task2md-1.0.1/tests/task/test_header.py` & `task2md-1.1.0/tests/task/test_header.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 
-from task2md.task.header import Header
+from task2md.template.header import Header
 
 VARS_HEADER_FULL = """
 #
 # @description: A set of tasks to lint different types of files.
 # @tags: lint, docker, CI
 # @authors: FX Soubirou <soubirou@yahoo.fr>, FXS <fxs@example.com>
 # File :material-bookmark-check:/:material-bookmark-remove:
```

### Comparing `task2md-1.0.1/tests/task/test_task.py` & `task2md-1.1.0/tests/task/test_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 
-from task2md.task.task import Task
+from task2md.template.task import Task
 
 TASK1 = """[LINT] Linter for files.
 Usage: task lint:all [FIX|F=<y|Y>] [MEX|M='"#node_modules"']
 
 Arguments:
   FIX |  F:  Fix files (optional, by default no)
   MEX | M: Makdown exlude directories with single quotes example: MEX='"#node_modules" "#.node_cache"' (see: https://github.com/DavidAnson/markdownlint-cli2)
```

### Comparing `task2md-1.0.1/tests/task/test_variable.py` & `task2md-1.1.0/tests/task/test_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from task2md.task.variable import Variable
+from task2md.template.variable import Variable
 
 
 class TestVariable:
     def test_variable_blank(self) -> None:
         v = Variable()
         assert v.name == ""
         assert v.value == ""
```

### Comparing `task2md-1.0.1/LICENSE` & `task2md-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/README.md` & `task2md-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `task2md-1.0.1/pyproject.toml` & `task2md-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "task2md"
-version = "1.0.1"
+version = "1.1.0"
 description = "A program to generate markdown documentation files from Task files"
 authors = [
     { name = "FX Soubirou", email = "soubirou@yahoo.fr" }
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
```

### Comparing `task2md-1.0.1/PKG-INFO` & `task2md-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: task2md
-Version: 1.0.1
+Version: 1.1.0
 Summary: A program to generate markdown documentation files from Task files
 Project-URL: Homepage, https://gitlab.com/op_so/task/task2md
 Project-URL: Documentation, https://op_so.gitlab.io/task/task2md/
 Author-email: FX Soubirou <soubirou@yahoo.fr>
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

