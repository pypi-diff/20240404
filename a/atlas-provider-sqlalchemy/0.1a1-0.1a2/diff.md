# Comparing `tmp/atlas_provider_sqlalchemy-0.1a1.tar.gz` & `tmp/atlas_provider_sqlalchemy-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas_provider_sqlalchemy-0.1a1.tar", max compression
+gzip compressed data, was "atlas_provider_sqlalchemy-0.1a2.tar", max compression
```

## Comparing `atlas_provider_sqlalchemy-0.1a1.tar` & `atlas_provider_sqlalchemy-0.1a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4291 2023-10-15 19:52:15.799588 atlas_provider_sqlalchemy-0.1a1/README.md
--rw-r--r--   0        0        0        0 2023-09-30 14:11:17.638329 atlas_provider_sqlalchemy-0.1a1/cli/__init__.py
--rw-r--r--   0        0        0     3249 2023-10-15 22:46:54.065418 atlas_provider_sqlalchemy-0.1a1/cli/main.py
--rw-r--r--   0        0        0      541 2023-10-15 22:56:11.303187 atlas_provider_sqlalchemy-0.1a1/pyproject.toml
--rw-r--r--   0        0        0     4831 1970-01-01 00:00:00.000000 atlas_provider_sqlalchemy-0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     3417 2023-10-25 17:43:20.718520 atlas_provider_sqlalchemy-0.1a2/README.md
+-rw-r--r--   0        0        0        0 2023-10-25 17:21:50.982376 atlas_provider_sqlalchemy-0.1a2/cli/__init__.py
+-rw-r--r--   0        0        0     3389 2023-10-25 16:59:26.289056 atlas_provider_sqlalchemy-0.1a2/cli/main.py
+-rw-r--r--   0        0        0      541 2023-10-25 17:43:27.135158 atlas_provider_sqlalchemy-0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 atlas_provider_sqlalchemy-0.1a2/PKG-INFO
```

### Comparing `atlas_provider_sqlalchemy-0.1a1/README.md` & `atlas_provider_sqlalchemy-0.1a2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 # DRAFT
 
 # atlas-provider-sqlalchemy
 Atlas provider for sqlalchemy
 
-## Run
-From the root directory of your project run:
-```shell
-pipx run --spec git+https://github.com/noamtamir/atlas-provider-sqlalchemy.git atlas-provider-sqlalchemy --dialect dialect
-```
-`dialect: postgresql|mysql|oracle|sqlite|mssql` (or any other dialect supported by sqlalchemy)    
-Optionally add  `--path path/to/models` if you need to run it from a different directory. All paths are relative to the directory this is run in.
-
-# atlas-provider-sqlalchemy
-
 Load [SQLAlchemy](https://www.sqlalchemy.org/) models into an [Atlas](https://atlasgo.io) project.
 
 ### Use-cases
 1. **Declarative migrations** - use a Terraform-like `atlas schema apply --env sqlalchemy` to apply your SQLAlchemy schema to the database.
 2. **Automatic migration planning** - use `atlas migrate diff --env sqlalchemy` to automatically plan a migration from the current database version to the SQLAlchemy schema.
 
 ### Installation
@@ -25,119 +15,102 @@
 ```bash
 curl -sSf https://atlasgo.sh | sh
 ```
 See [atlasgo.io](https://atlasgo.io/getting-started#installation) for more installation options.
 
 Install the provider by running:
 ```bash
-pipx install git+https://github.com/noamtamir/atlas-provider-sqlalchemy.git
+pip install atlas-provider-sqlalchemy
 ```
-([Pipx documentation](https://pypa.github.io/pipx/) )
 
 
 #### Standalone 
 
 If all of your SQLAlchemy models exist in a single package, 
 you can use the provider directly to load your SQLAlchemy schema into Atlas.
 
 In your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
   program = [
     "atlas-provider-sqlalchemy",
-    "--dialect", "mysql", // mysql | mariadb | postgresql | sqlite | mssql
+    "--dialect", "mysql", // postgresql | mysql | oracle | sqlite | mssql
   ]
 }
 
 env "sqlalchemy" {
   src = data.external_schema.sqlalchemy.url
   dev = "docker://mysql/8/dev"
 }
 ```
 
 #### As Python Script 
 ...   
 If you want to use the provider as a python script, you can use the provider as follows:
 
-Create a new file named `load.py` with the following contents:
+Create a new file named `load_models.py` with the following contents:
 
 ```python
 # import all models
 from models import User, Task;
-...
-const load_models = require("@ariga/atlas-provider-sequelize");
-
-print(load_models("mysql", [User, Task]));
+from ariga_provider_sqlalchemy import print_ddl
+print_ddl("mysql", [User, Task])
 ```
 
 Next, in your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
     program = [
         "python",
-        "load.py",
-        "mysql"
+        "load_models.py"
     ]
 }
 
 env "sqlalchemy" {
     src = data.external_schema.sqlalchemy.url
     dev = "docker://mysql/8/dev"
-    migration {
-        dir = "file://migrations"
-    }
-    format {
-        migrate {
-            diff = "{{ sql . \"  \" }}"
-        }
-    }
 }
 ```
 
 ### Usage
 
 Once you have the provider installed, you can use it to apply your SQLAlchemy schema to the database:
 
 #### Apply
 
-You can use the `atlas schema apply` command to plan and apply a migration of your database to
-your current SQLAlchemy schema. This works by inspecting the target database and comparing it to the
-SQLAlchemy schema and creating a migration plan. Atlas will prompt you to confirm the migration plan
-before applying it to the database.
+You can use the `atlas schema apply` command to plan and apply a migration of your database to your current SQLAlchemy schema. This works by inspecting the target database and comparing it to the SQLAlchemy schema and creating a migration plan. Atlas will prompt you to confirm the migration plan before applying it to the database.
 
 ```bash
-atlas schema apply --env sequelize -u "mysql://root:password@localhost:3306/mydb"
+atlas schema apply --env sqlalchemy -u "mysql://root:password@localhost:3306/mydb"
 ```
 Where the `-u` flag accepts the [URL](https://atlasgo.io/concepts/url) to the
 target database.
 
 #### Diff
 
 Atlas supports a [version migration](https://atlasgo.io/concepts/declarative-vs-versioned#versioned-migrations) 
 workflow, where each change to the database is versioned and recorded in a migration file. You can use the
 `atlas migrate diff` command to automatically generate a migration file that will migrate the database
 from its latest revision to the current Sequelize schema.
 
 ```bash
-atlas migrate diff --env sequelize 
+atlas migrate diff --env sqlalchemy 
 ````
 
-### Typescript
-for typescript support, see the [ts-atlas-provider-sequelize](https://github.com/ariga/atlas-provider-sequelize/tree/master/ts) README.
-
 ### Supported Databases
 
 The provider supports the following databases:
 * MySQL
 * MariaDB
 * PostgreSQL
 * SQLite
 * Microsoft SQL Server
+* Oracle
 
 ### Issues
 
 Please report any issues or feature requests in the [ariga/atlas](https://github.com/ariga/atlas/issues) repository.
 
 ### License
```

### Comparing `atlas_provider_sqlalchemy-0.1a1/cli/main.py` & `atlas_provider_sqlalchemy-0.1a2/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import importlib.util
 import inspect
 import typer
 from pathlib import Path
 from sqlalchemy import create_mock_engine
 from sqlalchemy.orm import DeclarativeBase
-from typing import Type, Set
+from typing import Type, Set, List
 
 
 COMMON_VENV_NAMES = [
     '.env',
     '.venv',
     'env',
     'venv',
@@ -94,9 +94,12 @@
 
 
 @app.command()
 def load(dialect: str = typer.Option(default=...), path: str = '', debug: bool = False):
     run(dialect, path, debug)
 
 
+def print_ddl(dialect_driver: str, models: List[Type[DeclarativeBase]]):
+    dump_ddl(dialect_driver=dialect_driver, Base=models[0])
+
 if __name__ == "__main__":
     app(prog_name='atlas-provider-sqlalchemy')
```

### Comparing `atlas_provider_sqlalchemy-0.1a1/pyproject.toml` & `atlas_provider_sqlalchemy-0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atlas-provider-sqlalchemy"
-version = "0.1a1"
+version = "0.1a2"
 description = ""
 authors = ["noamtamir <noam.tamir@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `atlas_provider_sqlalchemy-0.1a1/PKG-INFO` & `atlas_provider_sqlalchemy-0.1a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-provider-sqlalchemy
-Version: 0.1a1
+Version: 0.1a2
 Summary: 
 Author: noamtamir
 Author-email: noam.tamir@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,24 +15,14 @@
 Description-Content-Type: text/markdown
 
 # DRAFT
 
 # atlas-provider-sqlalchemy
 Atlas provider for sqlalchemy
 
-## Run
-From the root directory of your project run:
-```shell
-pipx run --spec git+https://github.com/noamtamir/atlas-provider-sqlalchemy.git atlas-provider-sqlalchemy --dialect dialect
-```
-`dialect: postgresql|mysql|oracle|sqlite|mssql` (or any other dialect supported by sqlalchemy)    
-Optionally add  `--path path/to/models` if you need to run it from a different directory. All paths are relative to the directory this is run in.
-
-# atlas-provider-sqlalchemy
-
 Load [SQLAlchemy](https://www.sqlalchemy.org/) models into an [Atlas](https://atlasgo.io) project.
 
 ### Use-cases
 1. **Declarative migrations** - use a Terraform-like `atlas schema apply --env sqlalchemy` to apply your SQLAlchemy schema to the database.
 2. **Automatic migration planning** - use `atlas migrate diff --env sqlalchemy` to automatically plan a migration from the current database version to the SQLAlchemy schema.
 
 ### Installation
@@ -41,119 +31,102 @@
 ```bash
 curl -sSf https://atlasgo.sh | sh
 ```
 See [atlasgo.io](https://atlasgo.io/getting-started#installation) for more installation options.
 
 Install the provider by running:
 ```bash
-pipx install git+https://github.com/noamtamir/atlas-provider-sqlalchemy.git
+pip install atlas-provider-sqlalchemy
 ```
-([Pipx documentation](https://pypa.github.io/pipx/) )
 
 
 #### Standalone 
 
 If all of your SQLAlchemy models exist in a single package, 
 you can use the provider directly to load your SQLAlchemy schema into Atlas.
 
 In your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
   program = [
     "atlas-provider-sqlalchemy",
-    "--dialect", "mysql", // mysql | mariadb | postgresql | sqlite | mssql
+    "--dialect", "mysql", // postgresql | mysql | oracle | sqlite | mssql
   ]
 }
 
 env "sqlalchemy" {
   src = data.external_schema.sqlalchemy.url
   dev = "docker://mysql/8/dev"
 }
 ```
 
 #### As Python Script 
 ...   
 If you want to use the provider as a python script, you can use the provider as follows:
 
-Create a new file named `load.py` with the following contents:
+Create a new file named `load_models.py` with the following contents:
 
 ```python
 # import all models
 from models import User, Task;
-...
-const load_models = require("@ariga/atlas-provider-sequelize");
-
-print(load_models("mysql", [User, Task]));
+from ariga_provider_sqlalchemy import print_ddl
+print_ddl("mysql", [User, Task])
 ```
 
 Next, in your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
     program = [
         "python",
-        "load.py",
-        "mysql"
+        "load_models.py"
     ]
 }
 
 env "sqlalchemy" {
     src = data.external_schema.sqlalchemy.url
     dev = "docker://mysql/8/dev"
-    migration {
-        dir = "file://migrations"
-    }
-    format {
-        migrate {
-            diff = "{{ sql . \"  \" }}"
-        }
-    }
 }
 ```
 
 ### Usage
 
 Once you have the provider installed, you can use it to apply your SQLAlchemy schema to the database:
 
 #### Apply
 
-You can use the `atlas schema apply` command to plan and apply a migration of your database to
-your current SQLAlchemy schema. This works by inspecting the target database and comparing it to the
-SQLAlchemy schema and creating a migration plan. Atlas will prompt you to confirm the migration plan
-before applying it to the database.
+You can use the `atlas schema apply` command to plan and apply a migration of your database to your current SQLAlchemy schema. This works by inspecting the target database and comparing it to the SQLAlchemy schema and creating a migration plan. Atlas will prompt you to confirm the migration plan before applying it to the database.
 
 ```bash
-atlas schema apply --env sequelize -u "mysql://root:password@localhost:3306/mydb"
+atlas schema apply --env sqlalchemy -u "mysql://root:password@localhost:3306/mydb"
 ```
 Where the `-u` flag accepts the [URL](https://atlasgo.io/concepts/url) to the
 target database.
 
 #### Diff
 
 Atlas supports a [version migration](https://atlasgo.io/concepts/declarative-vs-versioned#versioned-migrations) 
 workflow, where each change to the database is versioned and recorded in a migration file. You can use the
 `atlas migrate diff` command to automatically generate a migration file that will migrate the database
 from its latest revision to the current Sequelize schema.
 
 ```bash
-atlas migrate diff --env sequelize 
+atlas migrate diff --env sqlalchemy 
 ````
 
-### Typescript
-for typescript support, see the [ts-atlas-provider-sequelize](https://github.com/ariga/atlas-provider-sequelize/tree/master/ts) README.
-
 ### Supported Databases
 
 The provider supports the following databases:
 * MySQL
 * MariaDB
 * PostgreSQL
 * SQLite
 * Microsoft SQL Server
+* Oracle
 
 ### Issues
 
 Please report any issues or feature requests in the [ariga/atlas](https://github.com/ariga/atlas/issues) repository.
 
 ### License
```

