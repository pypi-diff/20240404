# Comparing `tmp/pipestat-0.8.3a1.tar.gz` & `tmp/pipestat-0.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestat-0.8.3a1.tar", last modified: Thu Mar 14 16:13:06 2024, max compression
+gzip compressed data, was "pipestat-0.9.0a1.tar", last modified: Thu Apr  4 17:46:46 2024, max compression
```

## Comparing `pipestat-0.8.3a1.tar` & `pipestat-0.9.0a1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.439207 pipestat-0.8.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-14 16:13:06.439207 pipestat-0.8.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.431207 pipestat-0.8.3a1/pipestat/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.431207 pipestat-0.8.3a1/pipestat/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.431207 pipestat-0.8.3a1/pipestat/backends/db_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/db_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/db_backend/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/db_backend/db_parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/db_backend/dbbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.431207 pipestat-0.8.3a1/pipestat/backends/file_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/file_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30131 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/backends/file_backend/filebackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.435207 pipestat-0.8.3a1/pipestat/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/glossary.html
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/glossary_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/jinja_templates/status_table_no_links.html
--rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    37505 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.435207 pipestat-0.8.3a1/pipestat/pipestatreader/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/pipestatreader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/pipestatreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/pipestatreader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    58153 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.435207 pipestat-0.8.3a1/pipestat/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/schemas/pipestat_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/schemas/status_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pipestat/schemas/status_table_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.439207 pipestat-0.8.3a1/pipestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-14 16:13:06.000000 pipestat-0.8.3a1/pipestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-14 16:13:06.000000 pipestat-0.8.3a1/pipestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 16:13:06.000000 pipestat-0.8.3a1/pipestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 16:13:06.000000 pipestat-0.8.3a1/pipestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-14 16:13:06.000000 pipestat-0.8.3a1/pipestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 16:13:06.000000 pipestat-0.8.3a1/pipestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.439207 pipestat-0.8.3a1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/requirements/requirements-db-backend.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/requirements/requirements-pipestatreader.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 16:13:06.439207 pipestat-0.8.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:13:06.439207 pipestat-0.8.3a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/tests/test_db_only_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/tests/test_parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    86565 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/tests/test_pipestat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-03-14 16:12:55.000000 pipestat-0.8.3a1/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/db_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/db_parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/dbbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/file_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/file_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30130 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/file_backend/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/glossary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/glossary_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status_table_no_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37635 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/pipestatreader/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58267 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/pipestat_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/status_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/status_table_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/pipestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-db-backend.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-pipestatreader.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_db_only_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87713 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_pipestat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_status.py
```

### Comparing `pipestat-0.8.3a1/LICENSE` & `pipestat-0.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/PKG-INFO` & `pipestat-0.9.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.8.3a1
+Version: 0.9.0a1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonschema
 Requires-Dist: logmuse>=0.2.5
-Requires-Dist: oyaml
-Requires-Dist: ubiquerg>=0.6.1
+Requires-Dist: pyyaml
+Requires-Dist: ubiquerg>=0.8.0
 Requires-Dist: yacman>=0.9.3
 Requires-Dist: pandas
 Requires-Dist: eido
 Requires-Dist: jinja2
 Provides-Extra: dbbackend
 Requires-Dist: psycopg>=3.1.13; extra == "dbbackend"
 Requires-Dist: pydantic<3.0.0,>=2.5.3; extra == "dbbackend"
```

### Comparing `pipestat-0.8.3a1/README.md` & `pipestat-0.9.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/argparser.py` & `pipestat-0.9.0a1/pipestat/argparser.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/backends/abstract.py` & `pipestat-0.9.0a1/pipestat/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/backends/db_backend/db_helpers.py` & `pipestat-0.9.0a1/pipestat/backends/db_backend/db_helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/backends/db_backend/db_parsed_schema.py` & `pipestat-0.9.0a1/pipestat/backends/db_backend/db_parsed_schema.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/backends/db_backend/dbbackend.py` & `pipestat-0.9.0a1/pipestat/backends/db_backend/dbbackend.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         else:
             _LOGGER.info(f" rm_record flag False, aborting Removing '{record_identifier}' record")
 
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: str,
-        force_overwrite: bool = False,
+        force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
     ) -> Union[List[str], bool]:
         """
         Update the value of a result in a current namespace.
 
         This method overwrites any existing data and creates the required
          hierarchical mapping structure if needed.
```

### Comparing `pipestat-0.8.3a1/pipestat/backends/file_backend/filebackend.py` & `pipestat-0.9.0a1/pipestat/backends/file_backend/filebackend.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         else:
             _LOGGER.info(f" rm_record flag False, aborting Removing '{record_identifier}' record")
 
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: Optional[str] = None,
-        force_overwrite: bool = False,
+        force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
     ) -> Union[List[str], bool]:
         """
         Update the value of a result in a current namespace.
 
         This method overwrites any existing data and creates the required
          hierarchical mapping structure if needed.
```

### Comparing `pipestat-0.8.3a1/pipestat/cli.py` & `pipestat-0.9.0a1/pipestat/cli.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/const.py` & `pipestat-0.9.0a1/pipestat/const.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/exceptions.py` & `pipestat-0.9.0a1/pipestat/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,24 @@
             if cli
             else "It needs to be supplied to the object constructor"
         )
         txt += f" or via '{ENV_VARS['schema']}' environment variable."
         super(SchemaNotFoundError, self).__init__(txt)
 
 
+class SchemaValidationErrorDuringReport(SchemaError):
+    """Adds clarity to JSON schema validation errors by providing additional information to error message."""
+
+    def __init__(self, msg, record_identifier, result_identifier, result):
+
+        txt = msg  # original schema validation error
+        txt += f"\nRecord identifier {record_identifier} \nResult_identifier {result_identifier} \nReported result: {result}"
+        super(SchemaValidationErrorDuringReport, self).__init__(txt)
+
+
 class MissingConfigDataError(PipestatError):
     """Exception for invalid config file."""
 
     def __init__(self, msg):
         spacing = " " if msg[-1] in ["?", ".", "\n"] else "; "
         suggest = "For config format documentation please see: http://pipestat.databio.org/en/latest/db_config/"
         super(MissingConfigDataError, self).__init__(msg + spacing + suggest)
```

### Comparing `pipestat-0.8.3a1/pipestat/helpers.py` & `pipestat-0.9.0a1/pipestat/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,47 +7,51 @@
 
 import jsonschema
 from json import dumps
 from pathlib import Path
 from shutil import make_archive
 from typing import Any, Dict, Optional, Tuple, Union, List
 
-from oyaml import safe_load, dump
-from ubiquerg import expandpath
-
-from zipfile import ZipFile, ZIP_DEFLATED
+from yaml import dump
+from .exceptions import SchemaValidationErrorDuringReport
 
 from .const import (
     PIPESTAT_GENERIC_CONFIG,
     SCHEMA_PROP_KEY,
     SCHEMA_TYPE_KEY,
     CLASSES_BY_TYPE,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def validate_type(value, schema, strict_type=False):
+def validate_type(value, schema, strict_type=False, record_identifier=None):
     """
     Validate reported result against a partial schema, in case of failure try
     to cast the value into the required class.
 
     Does not support objects of objects.
 
     :param any value: reported value
     :param dict schema: partial jsonschema schema to validate
         against, e.g. {"type": "integer"}
     :param bool strict_type: whether the value should validate as is
+    :param str record_identifier: used for clarifying error messages
     """
 
     try:
         jsonschema.validate(value, schema)
     except jsonschema.exceptions.ValidationError as e:
         if strict_type:
-            raise
+            raise SchemaValidationErrorDuringReport(
+                msg=str(e),
+                record_identifier=record_identifier,
+                result_identifier=schema,
+                result=value,
+            )
         _LOGGER.debug(f"{str(e)}")
         if schema[SCHEMA_TYPE_KEY] != "object":
             value = CLASSES_BY_TYPE[schema[SCHEMA_TYPE_KEY]](value)
         else:
             for prop, prop_dict in schema[SCHEMA_PROP_KEY].items():
                 try:
                     cls_fun = CLASSES_BY_TYPE[prop_dict[SCHEMA_TYPE_KEY]]
@@ -59,35 +63,14 @@
                         f"Casted the reported result into required " f"type: {str(cls_fun)}"
                     )
         jsonschema.validate(value, schema)
     else:
         _LOGGER.debug(f"Value '{value}' validated successfully against a schema")
 
 
-def read_yaml_data(path: Union[str, Path], what: str) -> Tuple[str, Dict[str, Any]]:
-    """
-    Safely read YAML file and log message
-
-    :param str path: YAML file to read
-    :param str what: context
-    :return (str, dict): absolute path to the read file and the read data
-    """
-    if isinstance(path, Path):
-        test = lambda p: p.is_file()
-    elif isinstance(path, str):
-        path = expandpath(path)
-        test = os.path.isfile
-    else:
-        raise TypeError(f"Alleged path to YAML file to read is neither path nor string: {path}")
-    assert test(path), FileNotFoundError(f"File not found: {path}")
-    _LOGGER.debug(f"Reading {what} from '{path}'")
-    with open(path, "r") as f:
-        return path, safe_load(f)
-
-
 def mk_list_of_str(x):
     """
     Make sure the input is a list of strings
     :param str | list[str] | falsy x: input to covert
     :return list[str]: converted input
     :raise TypeError: if the argument cannot be converted
     """
@@ -96,49 +79,22 @@
     if isinstance(x, str):
         return [x]
     raise TypeError(
         f"String or list of strings required as input. Got: " f"{x.__class__.__name__}"
     )
 
 
-def mk_abs_via_cfg(
-    path: Optional[str],
-    cfg_path: Optional[str],
-) -> Optional[str]:
-    """
-    Helper function to ensure a path is absolute.
-
-    Assumes a relative path is relative to cfg_path, or to current working directory if cfg_path is None.
-
-    : param str path: The path to make absolute.
-    : param str cfg_path: Relative paths will be relative the containing folder of this pat
-    """
-    if path is None:
-        return path
-    assert isinstance(path, str), TypeError("Path is expected to be a str")
-    if os.path.isabs(path):
-        return path
-    if cfg_path is None:
-        rel_to_cwd = os.path.join(os.getcwd(), path)
+def make_subdirectories(path):
+    """Takes an absolute file path and creates subdirectories to file if they do not exist"""
+
+    if path:
         try:
-            os.makedirs(os.path.dirname(rel_to_cwd))
+            os.makedirs(os.path.dirname(path))
         except FileExistsError:
             pass
-        if os.path.exists(rel_to_cwd) or os.access(os.path.dirname(rel_to_cwd), os.W_OK):
-            return rel_to_cwd
-        else:
-            raise OSError(f"File not found: {path}")
-    joined = os.path.join(os.path.dirname(cfg_path), path)
-    try:
-        os.makedirs(os.path.dirname(joined))
-    except FileExistsError:
-        pass
-    if os.path.isabs(joined):
-        return joined
-    raise OSError(f"Could not make this path absolute: {path}")
 
 
 def init_generic_config():
     """
     Create generic config file for DB Backend
     """
     try:
```

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/footer_index.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/footer_index.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/glossary_table.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/glossary_table.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/head.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/head.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/index.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/logo.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/logo.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/navbar.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/navbar_links.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/navbar_links.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/navbar_list_parent.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/object.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/object.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/project_object.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/project_object.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/sample.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/sample.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/status_table.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/status_table.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/jinja_templates/status_table_no_links.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/parsed_schema.py` & `pipestat-0.9.0a1/pipestat/parsed_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Abstraction of a parse of a schema definition"""
 
 import copy
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, Mapping, Optional, Union
-
+import yacman
 from .const import (
     CANONICAL_TYPES,
     CLASSES_BY_TYPE,
     RECORD_IDENTIFIER,
     SCHEMA_DESC_KEY,
     SCHEMA_ITEMS_KEY,
     SCHEMA_PROP_KEY,
     SCHEMA_TYPE_KEY,
 )
 from .exceptions import SchemaError
-from .helpers import read_yaml_data
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 NULL_MAPPING_VALUE = {}
 SCHEMA_PIPELINE_NAME_KEY = "pipeline_name"
@@ -72,15 +71,15 @@
     _PROJECT_KEY = "project"
     _SAMPLES_KEY = "samples"
     _STATUS_KEY = "status"
 
     def __init__(self, data: Union[Dict[str, Any], Path, str]) -> None:
         # initial validation and parse
         if not isinstance(data, dict):
-            _, data = read_yaml_data(data, "schema")
+            data = yacman.load_yaml(data)
 
         # Keep a copy of the original schema
         self.original_schema = copy.deepcopy(data)
         # Create a copy of a resolved schema
         if "$defs" in data.keys():
             self.resolved_schema = replace_JSON_refs(copy.deepcopy(data), data)
             self.resolved_schema.pop("$defs")
@@ -165,28 +164,43 @@
     def __str__(self):
         """
         Generate string representation of the object.
 
         :return str: string representation of the object
         """
         res = f"{self.__class__.__name__} ({self._pipeline_name})"
+
+        def add_props(props):
+            res = ""
+            if len(props) == 0:
+                res += "\n - None"
+            else:
+                for k, v in props:
+                    res += f"\n - {k} : {v}"
+            return res
+
         if self._project_level_data is not None:
-            res += "\n Project Level Data:"
-            for k, v in self._project_level_data.items():
-                res += f"\n -  {k} : {v}"
+            res += "\n Project-level properties:"
+            res += add_props(self._project_level_data.items())
         if self._sample_level_data is not None:
-            res += "\n Sample Level Data:"
-            for k, v in self._sample_level_data.items():
-                res += f"\n -  {k} : {v}"
+            res += "\n Sample-level properties:"
+            res += add_props(self._sample_level_data.items())
         if self._status_data is not None:
-            res += "\n Status Data:"
-            for k, v in self._status_data.items():
-                res += f"\n -  {k} : {v}"
+            res += "\n Status properties:"
+            res += add_props(self._status_data.items())
         return res
 
+    def __repr__(self):
+        """
+        Generate string representation of the object.
+
+        :return str: string representation of the object
+        """
+        return self.__str__()
+
     @property
     def pipeline_name(self):
         """Return the declared name for the pipeline for which this schema's written."""
         return self._pipeline_name
 
     @property
     def project_level_data(self):
@@ -269,39 +283,42 @@
         spec = s.setdefault(k, {})
         spec.setdefault(SCHEMA_PROP_KEY, {}).update(curr_type_spec[SCHEMA_PROP_KEY])
         spec.setdefault("required", []).extend(curr_type_spec["required"])
         spec[SCHEMA_TYPE_KEY] = curr_type_spec[SCHEMA_TYPE_KEY]
     return s
 
 
-def replace_JSON_refs(s: Dict[str, Any], data: Dict[str, Any]) -> Dict[str, Any]:
+def replace_JSON_refs(
+    target_schema: Dict[str, Any], source_schema: Dict[str, Any]
+) -> Dict[str, Any]:
     """
-    Recursively search and replace the $refs if they exist in schema, s, and if their corresponding $defs exist in
-    source schema, data
-
-    :param dict s: schema to replace types in
-    :param dict data: source schema
-    :return dict s: schema with types replaced
+    Recursively search and replace the $refs if they exist in schema, target_schema, and if their corresponding $defs
+    exist in source schema, source_schema. If $defs  exist in the target schema and target_schema is the same as
+    source_schema then deepcopy should be used such that target_schema = copy.deepcopy(source_schema)
+
+    :param dict target_schema: schema to replace types in
+    :param dict source_schema: source schema
+    :return dict target_schema: schema with types replaced
     """
 
-    for k, v in list(s.items()):
+    for k, v in list(target_schema.items()):
         if isinstance(v, dict):
-            replace_JSON_refs(s[k], data)
+            replace_JSON_refs(target_schema[k], source_schema)
         if "$ref" == k:
             split_value = v.split("/")
             if len(split_value) != 3:
                 raise SchemaError(
                     msg=f"$ref exists in source schema but path,{v} ,not valid, e.g. '#/$defs/file' "
                 )
-            if split_value[1] in data and split_value[2] in data[split_value[1]]:
-                result = data[split_value[1]][split_value[2]]
+            if split_value[1] in source_schema and split_value[2] in source_schema[split_value[1]]:
+                result = source_schema[split_value[1]][split_value[2]]
             else:
                 result = None
             if result is not None:
                 for key, value in result.items():
-                    s.update({key: value})
-                del s["$ref"]
+                    target_schema.update({key: value})
+                del target_schema["$ref"]
             else:
                 raise SchemaError(
                     msg=f"Could not find {split_value[1]} and {split_value[2]} in $def"
                 )
-    return s
+    return target_schema
```

### Comparing `pipestat-0.8.3a1/pipestat/pipestat.py` & `pipestat-0.9.0a1/pipestat/pipestat.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from abc import ABC
 from collections.abc import MutableMapping
 
 from jsonschema import validate
 from yacman import FutureYAMLConfigManager as YAMLConfigManager
 from yacman.yacman_future import select_config
+from ubiquerg import mkabs
+from yacman import load_yaml
+
 
 from typing import Optional, Union, Dict, Any, List, Iterator
 
 
 from .exceptions import (
     ColumnNotFoundError,
     NoBackendSpecifiedError,
@@ -20,15 +23,20 @@
     PipestatDependencyError,
     PipestatDatabaseError,
     RecordNotFoundError,
     SchemaNotFoundError,
 )
 from pipestat.backends.file_backend.filebackend import FileBackend
 from .reports import HTMLReportBuilder, _create_stats_objs_summaries
-from .helpers import validate_type, mk_abs_via_cfg, read_yaml_data, default_formatter, zip_report
+from .helpers import (
+    validate_type,
+    default_formatter,
+    zip_report,
+    make_subdirectories,
+)
 from .const import (
     PKG_NAME,
     DEFAULT_PIPELINE_NAME,
     ENV_VARS,
     CFG_DATABASE_KEY,
     SCHEMA_PATH,
     STATUS_SCHEMA,
@@ -169,15 +177,15 @@
         elif self.cfg["config_path"] is not None:
             self.cfg[CONFIG_KEY] = YAMLConfigManager.from_yaml_file(
                 filepath=self.cfg["config_path"]
             )
         else:
             self.cfg[CONFIG_KEY] = YAMLConfigManager()
 
-        _, cfg_schema = read_yaml_data(CFG_SCHEMA, "config schema")
+        cfg_schema = load_yaml(CFG_SCHEMA)
         validate(self.cfg[CONFIG_KEY].exp, cfg_schema)
 
         self.cfg[SCHEMA_PATH] = self.cfg[CONFIG_KEY].priority_get(
             "schema_path", env_var=ENV_VARS["schema"], override=schema_path
         )
         self.process_schema(schema_path)
 
@@ -203,24 +211,25 @@
 
         self.cfg[DB_ONLY_KEY] = database_only
 
         self.cfg[PIPELINE_TYPE] = self.cfg[CONFIG_KEY].priority_get(
             "pipeline_type", default="sample", override=pipeline_type
         )
 
-        self.cfg[FILE_KEY] = mk_abs_via_cfg(
+        self.cfg[FILE_KEY] = mkabs(
             self.resolve_results_file_path(
                 self.cfg[CONFIG_KEY].priority_get(
                     "results_file_path",
                     env_var=ENV_VARS["results_file"],
                     override=results_file_path,
                 )
             ),
             self.cfg["config_path"],
         )
+        make_subdirectories(self.cfg[FILE_KEY])
 
         self.cfg[RESULT_FORMATTER] = result_formatter
 
         self.cfg[MULTI_PIPELINE] = multi_pipelines
 
         self.cfg["multi_result_files"] = None
 
@@ -337,17 +346,16 @@
             self.cfg[DB_ONLY_KEY] = False
 
         flag_file_dir = self.cfg[CONFIG_KEY].priority_get(
             "flag_file_dir",
             override=flag_file_dir,
             default=os.path.dirname(self.cfg[FILE_KEY]),
         )
-        self.cfg[STATUS_FILE_DIR] = mk_abs_via_cfg(
-            flag_file_dir, self.config_path or self.cfg[FILE_KEY]
-        )
+        self.cfg[STATUS_FILE_DIR] = mkabs(flag_file_dir, self.config_path or self.cfg[FILE_KEY])
+        make_subdirectories(self.cfg[STATUS_FILE_DIR])
 
         self.backend = FileBackend(
             self.cfg[FILE_KEY],
             record_identifier,
             self.cfg[PIPELINE_NAME],
             self.cfg[PIPELINE_TYPE],
             self.cfg[SCHEMA_KEY],
@@ -497,26 +505,24 @@
             self.cfg[SCHEMA_KEY] = None
             self.cfg[STATUS_SCHEMA_KEY] = None
             self.cfg[STATUS_SCHEMA_SOURCE_KEY] = None
             # return None
             # raise SchemaNotFoundError("PipestatManager creation failed; no schema")
         else:
             # Main schema
-            schema_to_read = mk_abs_via_cfg(self._schema_path, self.cfg["config_path"])
+            schema_to_read = mkabs(self._schema_path, self.cfg["config_path"])
             self._schema_path = schema_to_read
             parsed_schema = ParsedSchema(schema_to_read)
             self.cfg[SCHEMA_KEY] = parsed_schema
 
             # Status schema
             self.cfg[STATUS_SCHEMA_KEY] = parsed_schema.status_data
             if not self.cfg[STATUS_SCHEMA_KEY]:
-                (
-                    self.cfg[STATUS_SCHEMA_SOURCE_KEY],
-                    self.cfg[STATUS_SCHEMA_KEY],
-                ) = read_yaml_data(path=STATUS_SCHEMA, what="default status schema")
+                self.cfg[STATUS_SCHEMA_SOURCE_KEY] = STATUS_SCHEMA
+                self.cfg[STATUS_SCHEMA_KEY] = load_yaml(filepath=STATUS_SCHEMA)
             else:
                 self.cfg[STATUS_SCHEMA_SOURCE_KEY] = schema_to_read
 
     @require_backend
     def remove(
         self,
         record_identifier: str = None,
@@ -541,15 +547,15 @@
         )
 
     @require_backend
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: Optional[str] = None,
-        force_overwrite: bool = False,
+        force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
         strict_type: bool = True,
     ) -> Union[List[str], bool]:
         """
         Report a result.
 
         :param Dict[str, any] values: dictionary of result-value pairs
@@ -579,14 +585,15 @@
                         f"Can't report a result for attribute '{r}'; it is not defined in the output schema."
                     )
 
                 validate_type(
                     value=values[r],
                     schema=self.result_schemas[r],
                     strict_type=strict_type,
+                    record_identifier=record_identifier,
                 )
 
         reported_results = self.backend.report(
             values=values,
             record_identifier=r_id,
             force_overwrite=force_overwrite,
             result_formatter=result_formatter,
@@ -688,15 +695,15 @@
                     try:
                         return result[0]
                     except IndexError:
                         raise RecordNotFoundError(
                             f"Results '{columns}' for '{record_identifier}' not found"
                         )
                 try:
-                    return result[0][result_identifier]
+                    return result[0][columns[0]]
                 except IndexError:
                     raise RecordNotFoundError(
                         f"Results '{columns}' for '{record_identifier}' not found"
                     )
             else:
                 raise RecordNotFoundError(
                     f"Results '{columns}' for '{record_identifier}' not found"
@@ -809,15 +816,16 @@
         if self.file and self.cfg["unresolved_result_path"] != self.file:
             if "{record_identifier}" in self.cfg["unresolved_result_path"]:
                 # assume there are multiple result files in sub-directories
                 self.cfg["multi_result_files"] = True
                 results_directory = self.cfg["unresolved_result_path"].split(
                     "{record_identifier}"
                 )[0]
-                results_directory = mk_abs_via_cfg(results_directory, self.cfg["config_path"])
+                results_directory = mkabs(results_directory, self.cfg["config_path"])
+                make_subdirectories(results_directory)
                 self.backend.aggregate_multi_results(results_directory)
 
     @require_backend
     def table(
         self,
     ) -> List[str]:
         """
```

### Comparing `pipestat-0.8.3a1/pipestat/pipestatreader/README.md` & `pipestat-0.9.0a1/pipestat/pipestatreader/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/pipestatreader/reader.py` & `pipestat-0.9.0a1/pipestat/pipestatreader/reader.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat/reports.py` & `pipestat-0.9.0a1/pipestat/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from datetime import timedelta
 from eido import read_schema
 from json import dumps
 from logging import getLogger
 from peppy.const import AMENDMENTS_KEY
 from typing import List
 from copy import deepcopy
-from .helpers import mk_abs_via_cfg
+
+from ubiquerg import mkabs
 
 from ._version import __version__
 from .const import (
     PIPELINE_NAME,
     PKG_NAME,
     OUTPUT_DIR,
     OBJECT_TYPES,
@@ -30,15 +31,15 @@
     PIPELINE_TYPE,
     PROJECT_NAME,
     TEMPLATES_DIRNAME,
     PROFILE_COLNAMES,
     STATUS_FILE_DIR,
     FILE_KEY,
 )
-
+from .helpers import make_subdirectories
 
 _LOGGER = getLogger(PKG_NAME)
 
 
 class HTMLReportBuilder(object):
     """Generate HTML summary report for project/samples"""
 
@@ -505,20 +506,21 @@
         """
         if not os.path.exists(self.pipeline_reports):
             os.makedirs(self.pipeline_reports)
         html_page = os.path.join(self.pipeline_reports, f"{sample_name}.html".lower())
 
         if self.prj.cfg["multi_result_files"] is True:
             self.prj.cfg["record_identifier"] = sample_name
-            temp_result_file_path = mk_abs_via_cfg(
+            temp_result_file_path = mkabs(
                 self.prj.resolve_results_file_path(self.prj.cfg["unresolved_result_path"]),
                 self.prj.cfg["config_path"],
             )
+            make_subdirectories(temp_result_file_path)
             self.prj.backend.status_file_dir = os.path.dirname(
-                mk_abs_via_cfg(temp_result_file_path, self.prj.cfg["config_path"])
+                mkabs(temp_result_file_path, self.prj.cfg["config_path"])
             )
 
         flag = self.prj.get_status(record_identifier=sample_name)
 
         if not flag:
             button_class = "btn btn-secondary"
             flag = "Missing"
@@ -1214,20 +1216,21 @@
             sample_name = sample["record_identifier"]
             psm = project
             sample_names.append(sample_name)
             # status and status style
             try:
                 if psm.cfg["multi_result_files"] is True:
                     psm.cfg["record_identifier"] = sample_name
-                    temp_result_file_path = mk_abs_via_cfg(
+                    temp_result_file_path = mkabs(
                         psm.resolve_results_file_path(psm.cfg["unresolved_result_path"]),
                         psm.cfg["config_path"],
                     )
+                    make_subdirectories(temp_result_file_path)
                     psm.backend.status_file_dir = os.path.dirname(
-                        mk_abs_via_cfg(temp_result_file_path, psm.cfg["config_path"])
+                        mkabs(temp_result_file_path, psm.cfg["config_path"])
                     )
                 status = psm.get_status(record_identifier=sample_name)
                 statuses.append(status)
                 status_metadata = psm.status_schema[status]
                 status_styles.append(_rgb2hex(*status_metadata["color"]))
                 status_descs.append(status_metadata["description"])
             except Exception as e:
```

### Comparing `pipestat-0.8.3a1/pipestat/schemas/pipestat_config_schema.yaml` & `pipestat-0.9.0a1/pipestat/schemas/pipestat_config_schema.yaml`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/pipestat.egg-info/PKG-INFO` & `pipestat-0.9.0a1/pipestat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.8.3a1
+Version: 0.9.0a1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonschema
 Requires-Dist: logmuse>=0.2.5
-Requires-Dist: oyaml
-Requires-Dist: ubiquerg>=0.6.1
+Requires-Dist: pyyaml
+Requires-Dist: ubiquerg>=0.8.0
 Requires-Dist: yacman>=0.9.3
 Requires-Dist: pandas
 Requires-Dist: eido
 Requires-Dist: jinja2
 Provides-Extra: dbbackend
 Requires-Dist: psycopg>=3.1.13; extra == "dbbackend"
 Requires-Dist: pydantic<3.0.0,>=2.5.3; extra == "dbbackend"
```

### Comparing `pipestat-0.8.3a1/pipestat.egg-info/SOURCES.txt` & `pipestat-0.9.0a1/pipestat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/setup.py` & `pipestat-0.9.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/tests/test_db_only_mode.py` & `pipestat-0.9.0a1/tests/test_db_only_mode.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.8.3a1/tests/test_init.py` & `pipestat-0.9.0a1/tests/test_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from tempfile import mkdtemp
 
-import oyaml
 import pytest
 import os
 from yaml import dump
 
 from pipestat import PipestatManager, SamplePipestatManager, ProjectPipestatManager
 from pipestat.exceptions import *
 from pipestat.parsed_schema import SCHEMA_PIPELINE_NAME_KEY
```

### Comparing `pipestat-0.8.3a1/tests/test_parsed_schema.py` & `pipestat-0.9.0a1/tests/test_parsed_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Tests of the parsed schema class"""
 
 from functools import partial
 from pathlib import Path
 from typing import *
 import pytest
-import oyaml
+import yaml
 from pipestat.const import SAMPLE_NAME, STATUS, RECORD_IDENTIFIER
-from pipestat.exceptions import SchemaError
+from pipestat.exceptions import SchemaError, SchemaValidationErrorDuringReport
 from pipestat.parsed_schema import (
     NULL_MAPPING_VALUE,
     ParsedSchema,
     SCHEMA_PIPELINE_NAME_KEY,
 )
 from .conftest import COMMON_CUSTOM_STATUS_DATA, DEFAULT_STATUS_DATA, get_data_file_path
+from pipestat.helpers import validate_type
 
 TEMP_SCHEMA_FILENAME = "schema.tmp.yaml"
 
 
 def write_yaml(data: Mapping[str, Any], path: Path) -> Path:
     with open(path, "w") as fH:
-        oyaml.dump(data, fH)
+        yaml.dump(data, fH)
     return path
 
 
 # This is to mirror the signature of write_yaml, serving schema as dict.
 def echo_data(data: Mapping[str, Any], path: Path) -> Mapping[str, Any]:
     return data
 
 
 def read_yaml(path: Union[str, Path]) -> Dict[str, Any]:
     with open(path, "r") as fh:
-        return oyaml.safe_load(fh)
+        return yaml.safe_load(fh)
 
 
 @pytest.fixture(scope="function", params=[lambda p: p, read_yaml])
 def prepare_schema_from_file(request):
     return request.param
 
 
@@ -271,7 +272,21 @@
     print(schema.resolved_schema)
 
     # Schema without refs and defs
     schema2 = ParsedSchema(output_schema_no_refs)
     print(schema2.original_schema)
     print(schema2.resolved_schema)
     print("done")
+
+
+def test_JSON_schema_validation_exception(output_schema_as_JSON_schema):
+    # schema with defs and refs
+    schema = ParsedSchema(output_schema_as_JSON_schema)
+    sample_level_data = schema.sample_level_data
+
+    # This should pass without exception
+    validate_type(value=5, schema=sample_level_data["number_of_things"])
+
+    with pytest.raises(SchemaValidationErrorDuringReport):
+        validate_type(
+            value="string", schema=sample_level_data["number_of_things"], strict_type=True
+        )
```

### Comparing `pipestat-0.8.3a1/tests/test_pipestat.py` & `pipestat-0.9.0a1/tests/test_pipestat.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,14 +587,45 @@
             assert str(list(val.keys())[0]) in list(retrieved_val.keys())
             # Test Retrieve Whole Record
             assert isinstance(psm.retrieve_one(record_identifier=rec_id), Mapping)
 
     @pytest.mark.parametrize(
         ["rec_id", "val"],
         [
+            ("sample1", {"number_of_things": 2}),
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["file", "db"])
+    def test_retrieve_one_single_result_as_list(
+        self,
+        rec_id,
+        val,
+        config_file_path,
+        results_file_path,
+        schema_file_path,
+        backend,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            psm = SamplePipestatManager(**args)
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+            assert psm.retrieve_one(
+                record_identifier=rec_id, result_identifier="number_of_things"
+            ) == psm.retrieve_one(record_identifier=rec_id, result_identifier=["number_of_things"])
+
+    @pytest.mark.parametrize(
+        ["rec_id", "val"],
+        [
             ("sample1", {"name_of_something": "test_name"}),
             ("sample1", {"number_of_things": 2}),
         ],
     )
     @pytest.mark.parametrize("backend", ["file", "db"])
     def test_retrieve_getitem(
         self,
```

### Comparing `pipestat-0.8.3a1/tests/test_status.py` & `pipestat-0.9.0a1/tests/test_status.py`

 * *Files identical despite different names*

