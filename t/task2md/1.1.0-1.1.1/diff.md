# Comparing `tmp/task2md-1.1.0.tar.gz` & `tmp/task2md-1.1.1.tar.gz`

## Comparing `task2md-1.1.0.tar` & `task2md-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 task2md-1.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.1.0/.markdownlint.yaml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.1.0/.python-version
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.1.0/.releaserc
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.1.0/.vale.ini
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.1.0/.yamllint
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.1.0/Taskfile.project.yml
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.1.0/Taskfile.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.1.0/lychee.toml
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.1.0/mkdocs.yml
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.1.0/requirements.lock
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/cli.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task2md.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/file.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/header.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/task.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/task/variable.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.1.0/docs/util/dir.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/__init__.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/__init__.py
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/file.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/header.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/index.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/task.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/template/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/util/__init__.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.1.0/src/task2md/util/dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/test_dir.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/test_file.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/test_task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/files/empty.yml
--rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/files/lint.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/__init__.py
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_file.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_header.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_index.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_task.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/task/test_variable.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.1.0/tests/util/test_dir.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.1.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.1.0/LICENSE
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.1.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 task2md-1.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.1.1/.markdownlint.yaml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.1.1/.python-version
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.1.1/.releaserc
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.1.1/.vale.ini
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.1.1/.yamllint
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.1.1/Taskfile.project.yml
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.1.1/Taskfile.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.1.1/lychee.toml
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.1.1/requirements.lock
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/cli.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task2md.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/file.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/header.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/task.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/variable.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/util/dir.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/__init__.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/__init__.py
+-rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/file.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/header.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/index.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/task.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/util/__init__.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/util/dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/test_dir.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/test_file.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/test_task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/files/empty.yml
+-rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/files/lint.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/__init__.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_file.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_header.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_index.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_task.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_variable.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/util/test_dir.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.1.1/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.1.1/PKG-INFO
```

### Comparing `task2md-1.1.0/.gitlab-ci.yml` & `task2md-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/.pre-commit-config.yaml` & `task2md-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/Taskfile.project.yml` & `task2md-1.1.1/Taskfile.project.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/Taskfile.yml` & `task2md-1.1.1/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/requirements-dev.lock` & `task2md-1.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/src/task2md/task2md.py` & `task2md-1.1.1/src/task2md/task2md.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from task2md.template.file import File
 from task2md.template.index import Index
 from task2md.util.dir import Dir
 
 
 @click.group()
-@click.version_option("1.1.0", prog_name="task2md")
+@click.version_option("1.1.1", prog_name="task2md")
 def cli() -> None:
     """A CLI tool to generate markdown documentation files from Task files."""
     pass
 
 
 @cli.command()
 @click.option(
@@ -68,14 +68,15 @@
 
                 index_file.task_files.append(task_file)
 
                 click.echo(
                     f"Task documentation generated: {task_file.get_filename()}.md"
                 )
             filename = "index"
+            index_file.task_files.sort()
             index_file.generate(out_dir)
             click.echo("Index documentation generated: index.md")
 
         except ValueError as ve:
             raise click.ClickException(
                 "Error on reading or writing file {} :\n {}".format(filename, str(ve))
             )
```

### Comparing `task2md-1.1.0/src/task2md/template/file.py` & `task2md-1.1.1/src/task2md/template/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -244,7 +244,15 @@
         """
         output = ""
 
         for task in self.tasks:
             output += task.to_md(self.get_filename())
 
         return output
+
+    def __lt__(self, other: "File") -> bool:
+        """A custom comparison function for sorting by name
+
+        Returns:
+            str: True if object is lower than other
+        """
+        return bool(self.get_filename() < other.get_filename())
```

### Comparing `task2md-1.1.0/src/task2md/template/header.py` & `task2md-1.1.1/src/task2md/template/header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/src/task2md/template/index.py` & `task2md-1.1.1/src/task2md/template/index.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/src/task2md/template/task.py` & `task2md-1.1.1/src/task2md/template/task.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/src/task2md/template/variable.py` & `task2md-1.1.1/src/task2md/template/variable.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/src/task2md/util/dir.py` & `task2md-1.1.1/src/task2md/util/dir.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/test_dir.py` & `task2md-1.1.1/tests/test_dir.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/test_file.py` & `task2md-1.1.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/test_task2md.py` & `task2md-1.1.1/tests/test_task2md.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/files/lint.yml` & `task2md-1.1.1/tests/files/lint.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/task/test_file.py` & `task2md-1.1.1/tests/task/test_file.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/task/test_header.py` & `task2md-1.1.1/tests/task/test_header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/task/test_index.py` & `task2md-1.1.1/tests/task/test_index.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/task/test_task.py` & `task2md-1.1.1/tests/task/test_task.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/tests/task/test_variable.py` & `task2md-1.1.1/tests/task/test_variable.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/LICENSE` & `task2md-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/README.md` & `task2md-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `task2md-1.1.0/pyproject.toml` & `task2md-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "task2md"
-version = "1.1.0"
+version = "1.1.1"
 description = "A program to generate markdown documentation files from Task files"
 authors = [
     { name = "FX Soubirou", email = "soubirou@yahoo.fr" }
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
```

### Comparing `task2md-1.1.0/PKG-INFO` & `task2md-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: task2md
-Version: 1.1.0
+Version: 1.1.1
 Summary: A program to generate markdown documentation files from Task files
 Project-URL: Homepage, https://gitlab.com/op_so/task/task2md
 Project-URL: Documentation, https://op_so.gitlab.io/task/task2md/
 Author-email: FX Soubirou <soubirou@yahoo.fr>
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

