# Comparing `tmp/shell-jobrunner-2.6.4.tar.gz` & `tmp/shell-jobrunner-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-jobrunner-2.6.4.tar", last modified: Tue Mar 26 19:02:17 2024, max compression
+gzip compressed data, was "shell-jobrunner-2.6.5.tar", last modified: Wed Apr  3 22:16:45 2024, max compression
```

## Comparing `shell-jobrunner-2.6.4.tar` & `shell-jobrunner-2.6.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.882058 shell-jobrunner-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.870058 shell-jobrunner-2.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.874058 shell-jobrunner-2.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-26 19:02:17.882058 shell-jobrunner-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    28040 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/cover.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/format.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.878058 shell-jobrunner-2.6.4/jobrunner/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/binutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.878058 shell-jobrunner-2.6.4/jobrunner/db/
--rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/db/sqlite_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.878058 shell-jobrunner-2.6.4/jobrunner/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/mail/chat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29846 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.878058 shell-jobrunner-2.6.4/jobrunner/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.878058 shell-jobrunner-2.6.4/jobrunner/service/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/service/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.882058 shell-jobrunner-2.6.4/jobrunner/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/chatmail_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/db_sqlite_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/info_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.882058 shell-jobrunner-2.6.4/jobrunner/test/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/await_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      293 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/dump_json_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/integration_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/interrupt_running_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      236 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/send_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/integration/smoke_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/main_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/test/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/jobrunner/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/maketags
--rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-26 19:02:17.882058 shell-jobrunner-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:02:17.882058 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-26 19:02:17.000000 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-26 19:02:17.000000 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:02:17.000000 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 19:02:17.000000 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 19:02:17.000000 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 19:02:17.000000 shell-jobrunner-2.6.4/shell_jobrunner.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      305 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/test-docker-helper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4284 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/test-docker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-03-26 19:02:09.000000 shell-jobrunner-2.6.4/test.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.961683 shell-jobrunner-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.949683 shell-jobrunner-2.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.953683 shell-jobrunner-2.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-03 22:16:45.961683 shell-jobrunner-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    28040 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/cover.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.957682 shell-jobrunner-2.6.5/jobrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/binutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.957682 shell-jobrunner-2.6.5/jobrunner/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/db/sqlite_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.957682 shell-jobrunner-2.6.5/jobrunner/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/mail/chat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29846 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.957682 shell-jobrunner-2.6.5/jobrunner/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.957682 shell-jobrunner-2.6.5/jobrunner/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/service/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.957682 shell-jobrunner-2.6.5/jobrunner/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/chatmail_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/db_sqlite_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/info_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.961683 shell-jobrunner-2.6.5/jobrunner/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/await_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      293 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/dump_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/integration_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/interrupt_running_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      236 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/send_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/integration/smoke_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/test/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/jobrunner/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/maketags
+-rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 22:16:45.961683 shell-jobrunner-2.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:16:45.961683 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-03 22:16:45.000000 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-03 22:16:45.000000 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:16:45.000000 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 22:16:45.000000 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 22:16:45.000000 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 22:16:45.000000 shell-jobrunner-2.6.5/shell_jobrunner.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      305 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/test-docker-helper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4284 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/test-docker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-04-03 22:16:40.000000 shell-jobrunner-2.6.5/test.sh
```

### Comparing `shell-jobrunner-2.6.4/.github/workflows/check.yml` & `shell-jobrunner-2.6.5/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/.github/workflows/codeql-analysis.yml` & `shell-jobrunner-2.6.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/.github/workflows/dependency-review.yml` & `shell-jobrunner-2.6.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/.github/workflows/python-publish.yml` & `shell-jobrunner-2.6.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/.gitignore` & `shell-jobrunner-2.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/CONTRIBUTING.md` & `shell-jobrunner-2.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/LICENSE` & `shell-jobrunner-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/Makefile` & `shell-jobrunner-2.6.5/Makefile`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/PKG-INFO` & `shell-jobrunner-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-jobrunner
-Version: 2.6.4
+Version: 2.6.5
 Summary: Shell-based job runner with logging
 Home-page: https://github.com/wwade/jobrunner
 Project-URL: Source, https://github.com/wwade/jobrunner
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shell-jobrunner-2.6.4/Pipfile.lock` & `shell-jobrunner-2.6.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/README.rst` & `shell-jobrunner-2.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/argparse.py` & `shell-jobrunner-2.6.5/jobrunner/argparse.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/compat.py` & `shell-jobrunner-2.6.5/jobrunner/compat.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/config.py` & `shell-jobrunner-2.6.5/jobrunner/config.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/db/__init__.py` & `shell-jobrunner-2.6.5/jobrunner/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from ..service import service
 from ..utils import (
     FileLock,
     cmp_,
     dateTimeFromJson,
     dateTimeToJson,
     doMsg,
+    humanTimeDeltaSecs,
     pidDebug,
     safeSleep,
     sprint,
     utcNow,
 )
 
 NUM_RECENT = 100
@@ -767,20 +768,15 @@
             if wkspace:
                 sprint(os.path.basename(wkspace) + ":")
             else:
                 sprint("Outside of any workspace:")
             for res in ["pass", "fail"]:
                 if wkspace in perWs and res in perWs[wkspace]:
                     j = perWs[wkspace][res]
-                    sec = int((unow - j.stopTime).total_seconds())
-                    tmHour = sec / (60 * 60)
-                    sec -= tmHour * 60 * 60
-                    tmMin = sec / 60
-                    sec -= tmMin * 60
-                    diffTime = "%d:%02d:%02d" % (tmHour, tmMin, sec)
+                    diffTime = humanTimeDeltaSecs(unow, j.stopTime)
                     sprint(
                         "  last %s, \033[97m%s\033[0m ago" %
                         (res, diffTime))
                     sprint("    " + str(j))
             if wkspace in remind:
                 sprint("  reminders:")
                 for j in remind[wkspace]:
```

### Comparing `shell-jobrunner-2.6.4/jobrunner/db/sqlite_db.py` & `shell-jobrunner-2.6.5/jobrunner/db/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/info.py` & `shell-jobrunner-2.6.5/jobrunner/info.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/logging.py` & `shell-jobrunner-2.6.5/jobrunner/logging.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/mail/chat.py` & `shell-jobrunner-2.6.5/jobrunner/mail/chat.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/main.py` & `shell-jobrunner-2.6.5/jobrunner/main.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/plugins.py` & `shell-jobrunner-2.6.5/jobrunner/plugins.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/service/__init__.py` & `shell-jobrunner-2.6.5/jobrunner/service/__init__.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/chatmail_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/chatmail_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/config_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/config_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/db_sqlite_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/db_sqlite_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/helpers.py` & `shell-jobrunner-2.6.5/jobrunner/test/helpers.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/info_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/info_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/integration/integration_lib.py` & `shell-jobrunner-2.6.5/jobrunner/test/integration/integration_lib.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/integration/interrupt_running_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/integration/interrupt_running_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/integration/smoke_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/integration/smoke_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/main_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/main_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/plugin_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/plugin_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/test/service_test.py` & `shell-jobrunner-2.6.5/jobrunner/test/service_test.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/jobrunner/utils.py` & `shell-jobrunner-2.6.5/jobrunner/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,29 +34,29 @@
 LOG = logging.getLogger(__name__)
 
 
 def strForEach(value):
     try:
         return text_type(value)
     except (UnicodeDecodeError, UnicodeEncodeError):
-        LOG.debug("%r", value, exc_info=1)
+        LOG.debug("%r", value, exc_info=True)
         return f"{value!r}"
 
 
 def sprint(*args, **kwargs):
     """sprint: "safe" print - ignore IOError"""
     try:
         print(*list(map(strForEach, args)), **kwargs)
     except IOError:
-        LOG.debug("sprint ignore IOError", exc_info=1)
+        LOG.debug("sprint ignore IOError", exc_info=True)
     except (UnicodeEncodeError, UnicodeDecodeError):
         print("codec error", repr(args))
-        LOG.debug("%r", args, exc_info=1)
+        LOG.debug("%r", args, exc_info=True)
     except BaseException:
-        LOG.debug("sprint caught error", exc_info=1)
+        LOG.debug("sprint caught error", exc_info=True)
         raise
 
 
 class ModState(object):
     def __init__(self) -> None:
         self._plugins: Optional[Plugins] = None
 
@@ -86,15 +86,15 @@
 
 @contextmanager
 def lockedSection(jobs):
     jobs.lock()
     try:
         yield
     except BaseException:
-        LOG.debug("lockedSection exception", exc_info=1)
+        LOG.debug("lockedSection exception", exc_info=True)
         raise
     finally:
         jobs.unlock()
 
 
 @contextmanager
 def maybeUnlock(jobs):
@@ -349,15 +349,27 @@
             subprocess.check_call(cmd)
         except subprocess.CalledProcessError as error:
             LOG.debug("cmd %r => error=%s", cmd, error, exc_info=True)
             return error.output
     return None
 
 
-def autoDecode(byteArray):
+def autoDecode(byteArray: bytes) -> str:
     detected = chardet.detect(byteArray)
+    if not detected:
+        return byteArray.decode()
+
     encoding = detected["encoding"]
     if detected["confidence"] < 0.8:  # very arbitrary
         LOG.debug("char encoding below confidence level 0.8 (%r). "
                   "Fall back to UTF-8.", detected)
         encoding = "utf-8"
+
     return byteArray.decode(encoding)
+
+
+def humanTimeDeltaSecs(a: datetime.datetime, b: datetime.datetime) -> str:
+    """
+    Returns a human readable string for the time difference a - b.
+    """
+    seconds = round((a - b).total_seconds(), 0)
+    return f"{datetime.timedelta(seconds=seconds)}"
```

### Comparing `shell-jobrunner-2.6.4/pylintrc` & `shell-jobrunner-2.6.5/pylintrc`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/setup.cfg` & `shell-jobrunner-2.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/shell_jobrunner.egg-info/PKG-INFO` & `shell-jobrunner-2.6.5/shell_jobrunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-jobrunner
-Version: 2.6.4
+Version: 2.6.5
 Summary: Shell-based job runner with logging
 Home-page: https://github.com/wwade/jobrunner
 Project-URL: Source, https://github.com/wwade/jobrunner
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shell-jobrunner-2.6.4/shell_jobrunner.egg-info/SOURCES.txt` & `shell-jobrunner-2.6.5/shell_jobrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/test-docker.py` & `shell-jobrunner-2.6.5/test-docker.py`

 * *Files identical despite different names*

### Comparing `shell-jobrunner-2.6.4/test.sh` & `shell-jobrunner-2.6.5/test.sh`

 * *Files identical despite different names*

