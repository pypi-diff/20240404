# Comparing `tmp/automagic-rest-1.0.0.tar.gz` & `tmp/automagic-rest-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/www-dev/tallen/automagic-rest/dist/.tmp-7tvfsaqf/automagic-rest-1.0.0.tar", last modified: Tue Nov 21 15:53:16 2023, max compression
+gzip compressed data, was "/var/www-dev/tallen/api/venv/src/automagic-rest/dist/.tmp-dtz7i0h6/automagic-rest-1.1.0.tar", last modified: Wed Apr  3 22:13:59 2024, max compression
```

## Comparing `automagic-rest-1.0.0.tar` & `automagic-rest-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.755272 automagic-rest-1.0.0/
--rwx------   0 tallen   (86646) wrds     (60359)      601 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/.gitignore
--rw-------   0 tallen   (86646) wrds     (60359)     1550 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/LICENSE
--rw-r--r--   0 tallen   (86646) wrds     (60359)     9535 2023-11-21 15:53:16.755272 automagic-rest-1.0.0/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)     8045 2022-04-22 18:08:58.000000 automagic-rest-1.0.0/README.md
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.753272 automagic-rest-1.0.0/automagic_rest/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/automagic_rest/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)      411 2023-11-21 15:53:16.000000 automagic-rest-1.0.0/automagic_rest/_version.py
--rw-------   0 tallen   (86646) wrds     (60359)      102 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/automagic_rest/apps.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.754272 automagic-rest-1.0.0/automagic_rest/management/
--rw-r--r--   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/automagic_rest/management/__init__.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.754272 automagic-rest-1.0.0/automagic_rest/management/commands/
--rw-r--r--   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/automagic_rest/management/commands/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)    12892 2022-04-22 18:06:04.000000 automagic-rest-1.0.0/automagic_rest/management/commands/build_data_models.py
--rw-------   0 tallen   (86646) wrds     (60359)     1421 2023-11-21 15:44:50.000000 automagic-rest-1.0.0/automagic_rest/pagination.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.751272 automagic-rest-1.0.0/automagic_rest/templates/
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.754272 automagic-rest-1.0.0/automagic_rest/templates/automagic_rest/
--rw-r--r--   0 tallen   (86646) wrds     (60359)      326 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/automagic_rest/templates/automagic_rest/models.html
--rw-r--r--   0 tallen   (86646) wrds     (60359)      356 2022-01-19 22:08:09.000000 automagic-rest-1.0.0/automagic_rest/templates/automagic_rest/urls.html
--rw-------   0 tallen   (86646) wrds     (60359)     8750 2023-11-21 15:44:50.000000 automagic-rest-1.0.0/automagic_rest/views.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:53:16.754272 automagic-rest-1.0.0/automagic_rest.egg-info/
--rw-r--r--   0 tallen   (86646) wrds     (60359)     9535 2023-11-21 15:53:16.000000 automagic-rest-1.0.0/automagic_rest.egg-info/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)      605 2023-11-21 15:53:16.000000 automagic-rest-1.0.0/automagic_rest.egg-info/SOURCES.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2023-11-21 15:53:16.000000 automagic-rest-1.0.0/automagic_rest.egg-info/dependency_links.txt
--rw-------   0 tallen   (86646) wrds     (60359)       85 2023-11-21 15:53:16.000000 automagic-rest-1.0.0/automagic_rest.egg-info/requires.txt
--rw-------   0 tallen   (86646) wrds     (60359)       15 2023-11-21 15:53:16.000000 automagic-rest-1.0.0/automagic_rest.egg-info/top_level.txt
--rw-------   0 tallen   (86646) wrds     (60359)     1661 2023-11-21 15:52:32.000000 automagic-rest-1.0.0/pyproject.toml
--rw-------   0 tallen   (86646) wrds     (60359)       38 2023-11-21 15:53:16.755272 automagic-rest-1.0.0/setup.cfg
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.199513 automagic-rest-1.1.0/
+-rwx------   0 tallen   (86646) wrds     (60359)      601 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/.gitignore
+-rw-------   0 tallen   (86646) wrds     (60359)     1550 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/LICENSE
+-rw-r--r--   0 tallen   (86646) wrds     (60359)     9535 2024-04-03 22:13:59.198513 automagic-rest-1.1.0/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)     8045 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/README.md
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.196513 automagic-rest-1.1.0/automagic_rest/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)      411 2024-04-03 22:13:59.000000 automagic-rest-1.1.0/automagic_rest/_version.py
+-rw-------   0 tallen   (86646) wrds     (60359)      102 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/apps.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.197513 automagic-rest-1.1.0/automagic_rest/management/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/management/__init__.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.198513 automagic-rest-1.1.0/automagic_rest/management/commands/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/management/commands/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)    12595 2024-04-03 22:13:19.000000 automagic-rest-1.1.0/automagic_rest/management/commands/build_data_models.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1421 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/pagination.py
+-rw-------   0 tallen   (86646) wrds     (60359)      507 2024-04-03 22:13:19.000000 automagic-rest-1.1.0/automagic_rest/settings.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.194513 automagic-rest-1.1.0/automagic_rest/templates/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.198513 automagic-rest-1.1.0/automagic_rest/templates/automagic_rest/
+-rw-------   0 tallen   (86646) wrds     (60359)      326 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/templates/automagic_rest/models.html
+-rw-------   0 tallen   (86646) wrds     (60359)      356 2023-11-21 15:25:40.000000 automagic-rest-1.1.0/automagic_rest/templates/automagic_rest/urls.html
+-rw-------   0 tallen   (86646) wrds     (60359)     8962 2024-04-03 22:13:19.000000 automagic-rest-1.1.0/automagic_rest/views.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2024-04-03 22:13:59.198513 automagic-rest-1.1.0/automagic_rest.egg-info/
+-rw-r--r--   0 tallen   (86646) wrds     (60359)     9535 2024-04-03 22:13:59.000000 automagic-rest-1.1.0/automagic_rest.egg-info/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)      632 2024-04-03 22:13:59.000000 automagic-rest-1.1.0/automagic_rest.egg-info/SOURCES.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2024-04-03 22:13:59.000000 automagic-rest-1.1.0/automagic_rest.egg-info/dependency_links.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       85 2024-04-03 22:13:59.000000 automagic-rest-1.1.0/automagic_rest.egg-info/requires.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       15 2024-04-03 22:13:59.000000 automagic-rest-1.1.0/automagic_rest.egg-info/top_level.txt
+-rw-------   0 tallen   (86646) wrds     (60359)     1661 2024-04-03 20:34:33.000000 automagic-rest-1.1.0/pyproject.toml
+-rw-------   0 tallen   (86646) wrds     (60359)       38 2024-04-03 22:13:59.199513 automagic-rest-1.1.0/setup.cfg
```

### Comparing `automagic-rest-1.0.0/.gitignore` & `automagic-rest-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `automagic-rest-1.0.0/LICENSE` & `automagic-rest-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automagic-rest-1.0.0/PKG-INFO` & `automagic-rest-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automagic-rest
-Version: 1.0.0
+Version: 1.1.0
 Summary: Automagic REST: Django REST Framework Code Generator for Underlying PostgreSQL DBs
 Author-email: Tim Allen <flipper@peregrinesalon.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wharton/automagic-rest
 Project-URL: Repository, https://github.com/wharton/automagic-rest
 Project-URL: Documentation, https://github.com/wharton/automagic-rest
 Keywords: django,automagic-rest,rest,drf,django-rest-framework,djangorestframework
```

### Comparing `automagic-rest-1.0.0/README.md` & `automagic-rest-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `automagic-rest-1.0.0/automagic_rest/management/commands/build_data_models.py` & `automagic-rest-1.1.0/automagic_rest/management/commands/build_data_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections import namedtuple
 
 from glob import glob
-import keyword
 import os
 from re import sub
 
 from django.core.management.base import BaseCommand
 from django.db import connections
 from django.template.loader import render_to_string
 
+from automagic_rest.settings import get_reserved_words_to_append_underscore
+
 # Map PostgreSQL column types to Django ORM field type
 # Please note: "blank=True, null=True" must be typed
 # exactly, as it will be stripped out for primary keys
 # The first column in the table is always marked as the
 # primary key.
 COLUMN_FIELD_MAP = {
     "smallint": "IntegerField({}blank=True, null=True{})",
@@ -33,32 +34,27 @@
     "text": "TextField({}blank=True, null=True{})",
     "uuid": "UUIDField({}blank=True, null=True{})",
     "interval": "DurationField({}blank=True, null=True{})",
     "json": "JSONField({}blank=True, null=True{})",
     "jsonb": "JSONField({}blank=True, null=True{})",
 }
 
-# Created a reserved words list that can not be used for Django field
-# names. Start with the Python reserved words list, and add any additional
-# fields reserved by DRF or Automagic REST.
-# We will then append `_var` to any fields with these names, and map to
-# the underlying database column in the models.
-RESERVED_WORDS = keyword.kwlist
-
-# Additional reserved words for Django REST Framework
-RESERVED_WORDS.append("format")
+# Words that can't be used as column names
+RESERVED_WORDS = get_reserved_words_to_append_underscore()
 
 
 def fetch_result_with_blank_row(cursor):
     """
     Gets all the rows, and appends a blank row so that the final
     model and column are written in the loop.
     """
     results = cursor.fetchall()
-    results.append(("__BLANK__", "__BLANK__", "__BLANK__", "integer", "__BLANK__", 0, 0))
+    results.append(
+        ("__BLANK__", "__BLANK__", "__BLANK__", "integer", "__BLANK__", 0, 0)
+    )
     desc = cursor.description
     nt_result = namedtuple("Result", [col[0] for col in desc])
 
     return [nt_result(*row) for row in results]
 
 
 class Command(BaseCommand):
@@ -77,29 +73,35 @@
             help='The database to use. Defaults to the "my_pg_data" database.',
         )
         parser.add_argument(
             "--owner",
             action="store",
             dest="owner",
             default="my_pg_user",
-            help='Select schemata from this PostgreSQL owner user. Defaults to the "wrdsadmn" owner.',
+            help=(
+                'Select schemata from this PostgreSQL owner user. Defaults to the '
+                '"wrdsadmn" owner.'
+            ),
         )
         parser.add_argument(
             "--path",
             action="store",
             dest="path",
             default="data_path",
             help="The path where to place the model files.",
         )
         parser.add_argument(
             "--verbose",
             action="store_true",
             dest="verbose",
             default=False,
-            help="""Sets verbose mode; displays each model built, instead of just schemata.""",
+            help=(
+                "Sets verbose mode; displays each model built, instead of just "
+                "schemata."
+            ),
         )
 
     def get_db(self, options):
         """
         Returns the Django name of the PostgreSQL database we will connect to.
         """
         return options.get("database")
@@ -235,15 +237,15 @@
     def write_schema_files(self, root_path, context):
         """
         Write out the current schema model.
         """
         with open(
             f"""{root_path}/models/{context["schema_name"]}.py""", "w"
         ) as f:
-            output = render_to_string(f"automagic_rest/models.html", context)
+            output = render_to_string("automagic_rest/models.html", context)
             f.write(output)
 
     def handle(self, *args, **options):
         verbose = options.get("verbose")
         max_digits_default = self.get_max_digits_default()
         decimal_places_default = self.get_decimal_places_default()
         # Get the provided root path and create directories
@@ -297,20 +299,16 @@
                     print(f"{model_count}: {row.table_name}")
                 context["tables"][row.table_name] = []
                 primary_key_has_been_set = False
                 context["routes"].append(f"""{row.schema_name}.{row.table_name}""")
 
             # If the column name is a Python reserved word, append an underscore
             # to follow the Python convention
-            if row.column_name in RESERVED_WORDS or row.column_name.endswith("_"):
-                if row.column_name.endswith("_"):
-                    under_score = ""
-                else:
-                    under_score = "_"
-                column_name = "{}{}var".format(row.column_name, under_score)
+            if row.column_name in RESERVED_WORDS:
+                column_name = f"{row.column_name}_"
                 db_column = ", db_column='{}'".format(row.column_name)
             else:
                 column_name = row.column_name
                 db_column = ""
 
             # For decimals, add the max_length and decimal places
             if row.data_type == "numeric":
@@ -318,22 +316,25 @@
                 if max_digits is None:
                     max_digits = max_digits_default
 
                 decimal_places = row.numeric_scale
                 if decimal_places is None:
                     decimal_places = decimal_places_default
 
-                db_column += f", max_digits={max_digits}, decimal_places={decimal_places}"
+                db_column += (
+                    f", max_digits={max_digits}, decimal_places={decimal_places}"
+                )
 
             if row.data_type in COLUMN_FIELD_MAP:
                 if primary_key_has_been_set:
                     field_map = COLUMN_FIELD_MAP[row.data_type].format("", db_column)
                 else:
-                    # We'll make the first column the primary key, since once is required in the Django ORM
-                    # and this is read-only. Primary keys can not be set to NULL in Django.
+                    # We'll make the first column the primary key, since once is
+                    # required in the Django ORM and this is read-only. Primary keys can
+                    # not be set to NULL in Django.
                     field_map = (
                         COLUMN_FIELD_MAP[row.data_type]
                         .format("primary_key=True", db_column)
                         .replace("blank=True, null=True", "")
                     )
                     primary_key_has_been_set = True
             else:
@@ -345,9 +346,9 @@
             context["tables"][row.table_name].append(
                 f"""{column_name} = models.{field_map}"""
             )
 
         # Pop off the final false row, and write the URLs file.
         context["routes"].pop()
         with open(f"{root_path}/urls.py", "w") as f:
-            output = render_to_string(f"automagic_rest/urls.html", context)
+            output = render_to_string("automagic_rest/urls.html", context)
             f.write(output)
```

### Comparing `automagic-rest-1.0.0/automagic_rest/pagination.py` & `automagic-rest-1.1.0/automagic_rest/pagination.py`

 * *Files identical despite different names*

### Comparing `automagic-rest-1.0.0/automagic_rest/views.py` & `automagic-rest-1.1.0/automagic_rest/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from rest_framework.viewsets import ReadOnlyModelViewSet
 from rest_framework_filters.backends import (
     ComplexFilterBackend,
     RestFrameworkFilterBackend,
 )
 
 from .pagination import estimate_count, CountEstimatePagination
+from .settings import get_reserved_words_to_append_underscore
 
 
 def split_basename(basename):
     """
     Splits a base name into schema and table names.
     """
     parts = basename.split(".")
@@ -230,26 +231,27 @@
         return index_columns
 
     def get_positions(self):
         """
         Return a dict of keyed column names and their ordinal positions as values.
         """
 
+        RESERVED_WORDS = get_reserved_words_to_append_underscore()
         positions = {}
 
         cursor = connections[self.db_name].cursor()
-
         cursor.execute(
             """
             SELECT column_name, ordinal_position
             FROM information_schema.columns
             WHERE table_schema = %(table_schema)s
             AND table_name = %(table_name)s
             """,
             {"table_schema": self.schema_name, "table_name": self.table_name},
         )
 
         for row in cursor.fetchall():
             # 0 = column_name, 1 = ordinal_position
-            positions[row[0]] = row[1]
+            column_name = f"{row[0]}_" if row[0] in RESERVED_WORDS else row[0]
+            positions[column_name] = row[1]
 
         return positions
```

### Comparing `automagic-rest-1.0.0/automagic_rest.egg-info/PKG-INFO` & `automagic-rest-1.1.0/automagic_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automagic-rest
-Version: 1.0.0
+Version: 1.1.0
 Summary: Automagic REST: Django REST Framework Code Generator for Underlying PostgreSQL DBs
 Author-email: Tim Allen <flipper@peregrinesalon.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wharton/automagic-rest
 Project-URL: Repository, https://github.com/wharton/automagic-rest
 Project-URL: Documentation, https://github.com/wharton/automagic-rest
 Keywords: django,automagic-rest,rest,drf,django-rest-framework,djangorestframework
```

### Comparing `automagic-rest-1.0.0/pyproject.toml` & `automagic-rest-1.1.0/pyproject.toml`

 * *Files identical despite different names*

