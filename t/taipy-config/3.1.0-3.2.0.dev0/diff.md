# Comparing `tmp/taipy-config-3.1.0.tar.gz` & `tmp/taipy-config-3.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-3.1.0.tar", last modified: Mon Mar  4 15:20:12 2024, max compression
+gzip compressed data, was "taipy-config-3.2.0.dev0.tar", last modified: Thu Apr  4 01:11:41 2024, max compression
```

## Comparing `taipy-config-3.1.0.tar` & `taipy-config-3.2.0.dev0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.437669 taipy-config-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-04 15:20:00.000000 taipy-config-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-04 15:20:10.000000 taipy-config-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-04 15:20:12.437669 taipy-config-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-04 15:20:00.000000 taipy-config-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:20:12.437669 taipy-config-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-04 15:20:10.000000 taipy-config-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.429669 taipy-config-3.1.0/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.429669 taipy-config-3.1.0/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.429669 taipy-config-3.1.0/taipy/_cli/_base_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/_cli/_base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/_cli/_base_cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/_cli/_run_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/_cli/_scaffold_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.429669 taipy-config-3.1.0/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.429669 taipy-config-3.1.0/taipy/config/_config_comparator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_config_comparator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_config_comparator/_comparator_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_config_comparator/_config_comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.429669 taipy-config-3.1.0/taipy/config/_serializer/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_serializer/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_serializer/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/_serializer/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.433669 taipy-config-3.1.0/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.433669 taipy-config-3.1.0/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.433669 taipy-config-3.1.0/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/common/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    42877 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.433669 taipy-config-3.1.0/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.433669 taipy-config-3.1.0/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/config/setup.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-04 15:20:00.000000 taipy-config-3.1.0/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.433669 taipy-config-3.1.0/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:12.437669 taipy-config-3.1.0/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-04 15:20:12.000000 taipy-config-3.1.0/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-04 15:20:12.000000 taipy-config-3.1.0/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:20:12.000000 taipy-config-3.1.0/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:20:10.000000 taipy-config-3.1.0/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-04 15:20:12.000000 taipy-config-3.1.0/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:20:12.000000 taipy-config-3.1.0/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.408273 taipy-config-3.2.0.dev0/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.408273 taipy-config-3.2.0.dev0/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.408273 taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/_abstract_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/_taipy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/_run_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/_cli/_scaffold_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.408273 taipy-config-3.2.0.dev0/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.412273 taipy-config-3.2.0.dev0/taipy/config/_config_comparator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_config_comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_config_comparator/_comparator_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_config_comparator/_config_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.412273 taipy-config-3.2.0.dev0/taipy/config/_serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_serializer/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_serializer/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/_serializer/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.412273 taipy-config-3.2.0.dev0/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.412273 taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.412273 taipy-config-3.2.0.dev0/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/common/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46078 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/config/setup.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-04 01:11:27.000000 taipy-config-3.2.0.dev0/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:11:41.416272 taipy-config-3.2.0.dev0/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-04 01:11:41.000000 taipy-config-3.2.0.dev0/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-04 01:11:41.000000 taipy-config-3.2.0.dev0/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:11:41.000000 taipy-config-3.2.0.dev0/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:11:39.000000 taipy-config-3.2.0.dev0/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 01:11:41.000000 taipy-config-3.2.0.dev0/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 01:11:41.000000 taipy-config-3.2.0.dev0/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-3.1.0/LICENSE` & `taipy-config-3.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/PKG-INFO` & `taipy-config-3.2.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 3.1.0
+Version: 3.2.0.dev0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-3.1.0/README.md` & `taipy-config-3.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/setup.py` & `taipy-config-3.2.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/__init__.py` & `taipy-config-3.2.0.dev0/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/_cli/__init__.py` & `taipy-config-3.2.0.dev0/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/_cli/_base_cli/__init__.py` & `taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,9 +4,7 @@
 # the License. You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
-
-from ._cli import _CLI
```

### Comparing `taipy-config-3.1.0/taipy/_cli/_base_cli/_cli.py` & `taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/_taipy_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import argparse
 from typing import Dict
 
 
-class _CLI:
+class _TaipyParser:
     """Argument parser for Taipy application."""
 
     # The conflict_handler is set to "resolve" to override conflict arguments
     _subparser_action = None
     _parser = argparse.ArgumentParser(conflict_handler="resolve")
 
     _sub_taipyparsers: Dict[str, argparse.ArgumentParser] = {}
@@ -48,20 +48,14 @@
             return groupparser
 
         groupparser = cls._parser.add_argument_group(title=title, description=description)
         cls._arg_groups[title] = groupparser
         return groupparser
 
     @classmethod
-    def _parse(cls):
-        """Parse and return only known arguments."""
-        args, _ = cls._parser.parse_known_args()
-        return args
-
-    @classmethod
     def _remove_argument(cls, arg: str):
         """Remove an argument from the parser. Note that the `arg` must be without --.
 
         Source: https://stackoverflow.com/questions/32807319/disable-remove-argument-in-argparse
         """
         for action in cls._parser._actions:
             opts = action.option_strings
```

### Comparing `taipy-config-3.1.0/taipy/_cli/_help_cli.py` & `taipy-config-3.2.0.dev0/taipy/_cli/_base_cli/_abstract_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,36 +6,59 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import sys
+from abc import abstractmethod
+from difflib import SequenceMatcher
+from typing import List, Optional
 
-from taipy._cli._base_cli import _CLI
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from ._taipy_parser import _TaipyParser
 
-class _HelpCLI:
-    __logger = _TaipyLogger._get_logger()
+
+class _AbstractCLI:
+    _logger = _TaipyLogger._get_logger()
+
+    _COMMAND_NAME: Optional[str] = None
+    _ARGUMENTS: List[str] = []
+    SIMILARITY_THRESHOLD = 0.8
 
     @classmethod
+    @abstractmethod
     def create_parser(cls):
-        create_parser = _CLI._add_subparser("help", help="Show the Taipy help message.", add_help=False)
-        create_parser.add_argument(
-            "command", nargs="?", type=str, const="", default="", help="Show the help message of the command."
-        )
+        raise NotImplementedError
 
     @classmethod
-    def parse_arguments(cls):
-        args = _CLI._parse()
+    @abstractmethod
+    def handle_command(cls):
+        raise NotImplementedError
+
+    @classmethod
+    def _parse_arguments(cls):
+        args, unknown_args = _TaipyParser._parser.parse_known_args()
+
+        if getattr(args, "which", None) != cls._COMMAND_NAME:
+            return
 
-        if getattr(args, "which", None) == "help":
-            if args.command:
-                if args.command in _CLI._sub_taipyparsers.keys():
-                    _CLI._sub_taipyparsers.get(args.command).print_help()
-                else:
-                    cls.__logger.error(f"{args.command} is not a valid command.")
-            else:
-                _CLI._parser.print_help()
+        if unknown_args:
+            _TaipyParser._sub_taipyparsers.get(cls._COMMAND_NAME).print_help()
+            for unknown_arg in unknown_args:
+                if not unknown_arg.startswith("-"):
+                    continue
+
+                error_message = f"Unknown arguments: {unknown_arg}."
+                similar_args = [
+                    arg
+                    for arg in cls._ARGUMENTS
+                    if SequenceMatcher(None, unknown_arg, arg).ratio() > cls.SIMILARITY_THRESHOLD
+                ]
+                if similar_args:
+                    error_message += f" Did you mean: {' or '.join(similar_args)}?"
+                cls._logger.error(error_message)
+            cls._logger.error("Please refer to the help message above for more information.")
+            sys.exit(1)
 
-            sys.exit(0)
+        return args
```

### Comparing `taipy-config-3.1.0/taipy/_cli/_run_cli.py` & `taipy-config-3.2.0.dev0/taipy/_cli/_run_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,52 +8,56 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import subprocess
 import sys
 
-from taipy._cli._base_cli import _CLI
+from ._base_cli._abstract_cli import _AbstractCLI
+from ._base_cli._taipy_parser import _TaipyParser
 
 
-class _RunCLI:
+class _RunCLI(_AbstractCLI):
+    _COMMAND_NAME = "run"
+
     @classmethod
     def create_parser(cls):
-        run_parser = _CLI._add_subparser("run", help="Run a Taipy application.")
+        run_parser = _TaipyParser._add_subparser(cls._COMMAND_NAME, help="Run a Taipy application.")
         run_parser.add_argument(
             "application_main_file",
         )
 
         sub_run_parser = run_parser.add_subparsers(title="subcommands")
         sub_run_parser.add_parser(
             "external-args",
             help="""
                 Arguments defined after this keyword will be considered as external arguments
                 to be passed to the application
             """,
         )
 
     @classmethod
-    def parse_arguments(cls):
-        args = _CLI._parse()
-
-        if getattr(args, "which", None) == "run":
-            all_args = sys.argv[3:]  # First 3 args are always (1) Python executable, (2) run, (3) Python file
-
-            external_args = []
-            try:
-                external_args_index = all_args.index("external-args")
-            except ValueError:
-                pass
-            else:
-                external_args.extend(all_args[external_args_index + 1 :])
-                all_args = all_args[:external_args_index]
-
-            taipy_args = [f"--taipy-{arg[2:]}" if arg.startswith("--") else arg for arg in all_args]
-
-            subprocess.run(
-                [sys.executable, args.application_main_file, *(external_args + taipy_args)],
-                stdout=sys.stdout,
-                stderr=sys.stdout,
-            )
+    def handle_command(cls):
+        args, _ = _TaipyParser._parser.parse_known_args()
+        if getattr(args, "which", None) != "run":
+            return
+
+        all_args = sys.argv[3:]  # First 3 args are always (1) Python executable, (2) run, (3) Python file
+
+        external_args = []
+        try:
+            external_args_index = all_args.index("external-args")
+        except ValueError:
+            pass
+        else:
+            external_args.extend(all_args[external_args_index + 1 :])
+            all_args = all_args[:external_args_index]
+
+        taipy_args = [f"--taipy-{arg[2:]}" if arg.startswith("--") else arg for arg in all_args]
+
+        subprocess.run(
+            [sys.executable, args.application_main_file, *(external_args + taipy_args)],
+            stdout=sys.stdout,
+            stderr=sys.stdout,
+        )
 
-            sys.exit(0)
+        sys.exit(0)
```

### Comparing `taipy-config-3.1.0/taipy/_cli/_scaffold_cli.py` & `taipy-config-3.2.0.dev0/taipy/_cli/_scaffold_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,32 +11,40 @@
 
 import pathlib
 import sys
 
 from cookiecutter.main import cookiecutter
 
 import taipy
-from taipy._cli._base_cli import _CLI
 
+from ._base_cli._abstract_cli import _AbstractCLI
+from ._base_cli._taipy_parser import _TaipyParser
 
-class _ScaffoldCLI:
+
+class _ScaffoldCLI(_AbstractCLI):
     __TAIPY_PATH = pathlib.Path(taipy.__file__).parent.resolve() / "templates"
+    _TEMPLATE_MAP = {str(x.name): str(x) for x in __TAIPY_PATH.iterdir() if x.is_dir() and not x.name.startswith("_")}
 
-    _TEMPLATE_MAP = {str(x.name): str(x) for x in __TAIPY_PATH.iterdir() if x.is_dir()}
+    _COMMAND_NAME = "create"
+    _ARGUMENTS = ["--template"]
 
     @classmethod
     def create_parser(cls):
-        create_parser = _CLI._add_subparser("create", help="Create a new Taipy application.")
+        create_parser = _TaipyParser._add_subparser(
+            cls._COMMAND_NAME,
+            help="Create a new Taipy application using pre-defined templates.",
+        )
         create_parser.add_argument(
             "--template",
             choices=list(cls._TEMPLATE_MAP.keys()),
             default="default",
             help="The Taipy template to create new application.",
         )
 
     @classmethod
-    def parse_arguments(cls):
-        args = _CLI._parse()
+    def handle_command(cls):
+        args = cls._parse_arguments()
+        if not args:
+            return
 
-        if getattr(args, "which", None) == "create":
-            cookiecutter(cls._TEMPLATE_MAP[args.template])
-            sys.exit(0)
+        cookiecutter(cls._TEMPLATE_MAP[args.template])
+        sys.exit(0)
```

### Comparing `taipy-config-3.1.0/taipy/config/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_config.py` & `taipy-config-3.2.0.dev0/taipy/config/_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_config_comparator/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/_config_comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_config_comparator/_comparator_result.py` & `taipy-config-3.2.0.dev0/taipy/config/_config_comparator/_comparator_result.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_config_comparator/_config_comparator.py` & `taipy-config-3.2.0.dev0/taipy/config/_config_comparator/_config_comparator.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_init.py` & `taipy-config-3.2.0.dev0/taipy/config/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_serializer/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_serializer/_base_serializer.py` & `taipy-config-3.2.0.dev0/taipy/config/_serializer/_base_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_serializer/_json_serializer.py` & `taipy-config-3.2.0.dev0/taipy/config/_serializer/_json_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/_serializer/_toml_serializer.py` & `taipy-config-3.2.0.dev0/taipy/config/_serializer/_toml_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/_checker.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/_checkers/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/_checkers/_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/issue.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/issue.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/checker/issue_collector.py` & `taipy-config-3.2.0.dev0/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/_classproperty.py` & `taipy-config-3.2.0.dev0/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/_config_blocker.py` & `taipy-config-3.2.0.dev0/taipy/config/common/_config_blocker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/_repr_enum.py` & `taipy-config-3.2.0.dev0/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/_template_handler.py` & `taipy-config-3.2.0.dev0/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/_validate_id.py` & `taipy-config-3.2.0.dev0/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/frequency.py` & `taipy-config-3.2.0.dev0/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/scope.py` & `taipy-config-3.2.0.dev0/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/common/typing.py` & `taipy-config-3.2.0.dev0/taipy/config/common/typing.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/config.py` & `taipy-config-3.2.0.dev0/taipy/config/config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/config.pyi` & `taipy-config-3.2.0.dev0/taipy/config/config.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,47 +23,51 @@
 from .common.scope import Scope
 from .global_app.global_app_config import GlobalAppConfig
 from .section import Section
 from .unique_section import UniqueSection
 
 class Config:
     """Configuration singleton."""
-
     @_Classproperty
     def unique_sections(cls) -> Dict[str, UniqueSection]:
         """Return all unique sections."""
+
     @_Classproperty
     def sections(cls) -> Dict[str, Dict[str, Section]]:
         """Return all non unique sections."""
+
     @_Classproperty
     def global_config(cls) -> GlobalAppConfig:
         """Return configuration values related to the global application as a `GlobalAppConfig^`."""
+
     @classmethod
     @_ConfigBlocker._check()
     def load(cls, filename):
         """Load a configuration file.
 
         The current Python configuration is replaced and the Config compilation is triggered.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     def export(cls, filename):
         """Export a configuration.
 
         The export is done in a toml file.
 
         The exported configuration is taken from the Python code configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
             If *filename* already exists, it is overwritten.
         """
+
     @classmethod
     def backup(cls, filename):
         """Backup a configuration.
 
         The backup is done in a toml file.
 
         The backed up configuration is a compilation from the three possible methods to configure
@@ -71,93 +75,112 @@
         configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
             If *filename* already exists, it is overwritten.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def restore(cls, filename):
         """Restore a configuration file and replace the current applied configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def override(cls, filename):
         """Load a configuration from a file and overrides the current config.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     def block_update(cls):
         """Block update on the configuration signgleton."""
+
     @classmethod
     def unblock_update(cls):
         """Unblock update on the configuration signgleton."""
+
     @classmethod
     @_ConfigBlocker._check()
     def configure_global_app(cls, **properties) -> GlobalAppConfig:
         """Configure the global application.
 
         Parameters:
             **properties (Dict[str, Any]): A dictionary of additional properties.
         Returns:
             The global application configuration.
         """
+
     @classmethod
     def check(cls) -> IssueCollector:
         """Check configuration.
 
         This method logs issue messages and returns an issue collector.
 
         Returns:
             Collector containing the info, warning and error issues.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def _register_default(cls, default_section: Section):
         """"""
+
     @classmethod
     @_ConfigBlocker._check()
     def _register(cls, section):
         """"""
+
     @classmethod
     def _override_env_file(cls):
         """"""
+
     @classmethod
     def _compile_configs(cls):
         """"""
+
     @classmethod
     def _to_json(cls, _config: _Config) -> str:
         """"""
+
     @classmethod
     def _from_json(cls, config_as_str: str) -> _Config:
         """"""
+
     @_Classproperty
     def job_config(cls) -> JobConfig:
         """"""
+
     @_Classproperty
     def data_nodes(cls) -> Dict[str, DataNodeConfig]:
         """"""
+
     @_Classproperty
     def tasks(cls) -> Dict[str, TaskConfig]:
         """"""
+
     @_Classproperty
     def scenarios(cls) -> Dict[str, ScenarioConfig]:
         """"""
+
     @_Classproperty
     def migration_functions(cls) -> Dict[str, MigrationConfig]:
         """"""
+
     @_Classproperty
     def core(cls) -> Dict[str, CoreSection]:
         """"""
+
     @staticmethod
     def configure_scenario(
         id: str,
         task_configs: Optional[List[TaskConfig]] = None,
         additional_data_node_configs: Optional[List[DataNodeConfig]] = None,
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
@@ -186,14 +209,15 @@
             sequences (Optional[Dict[str, List[TaskConfig]]]): Dictionary of sequence descriptions.
                 The default value is None.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new scenario configuration.
         """
+
     @staticmethod
     def set_default_scenario_configuration(
         task_configs: Optional[List[TaskConfig]] = None,
         additional_data_node_configs: List[DataNodeConfig] = None,
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         sequences: Optional[Dict[str, List[TaskConfig]]] = None,
@@ -223,41 +247,43 @@
                 `taipy.compare_scenarios()^` more more details.
             sequences (Optional[Dict[str, List[TaskConfig]]]): Dictionary of sequences. The default value is None.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new default scenario configuration.
         """
+
     @staticmethod
     def set_default_data_node_configuration(
         storage_type: str, scope: Optional[Scope] = None, validity_period: Optional[timedelta] = None, **properties
     ) -> "DataNodeConfig":
         """Set the default values for data node configurations.
 
         This function creates the _default data node configuration_ object,
         where all data node configuration objects will find their default
         values when needed.
 
         Parameters:
             storage_type (str): The default storage type for all data node configurations.
                 The possible values are *"pickle"* (the default value), *"csv"*, *"excel"*,
-                *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"* or
-                *"generic"*.
+                *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"*, *"generic"*,
+                or *"s3_object"*.
             scope (Optional[Scope^]): The default scope for all data node configurations.<br/>
                 The default value is `Scope.SCENARIO`.
             validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
                 considered up-to-date. Once the validity period has passed, the data node is considered stale and
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The default data node configuration.
         """
+
     @classmethod
     def configure_data_node_from(
         cls,
         source_configuration: "DataNodeConfig",
         id: str,
         **properties,
     ) -> "DataNodeConfig":
@@ -268,14 +294,15 @@
             id (str): The unique identifier of the new data node configuration.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.<br/>
                 The default properties are the properties of the source data node configuration.
 
         Returns:
             The new data node configuration.
         """
+
     @classmethod
     def configure_data_node(
         cls,
         id: str,
         storage_type: Optional[str] = None,
         scope: Optional[Scope] = None,
         validity_period: Optional[timedelta] = None,
@@ -300,14 +327,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new data node configuration.
         """
+
     @classmethod
     def configure_csv_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         encoding: Optional[str] = None,
         has_header: Optional[bool] = None,
@@ -333,14 +361,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new CSV data node configuration.
         """
+
     @classmethod
     def configure_json_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         encoding: Optional[str] = None,
         encoder: Optional[json.JSONEncoder] = None,
@@ -364,14 +393,15 @@
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new JSON data node configuration.
         """
+
     @classmethod
     def configure_parquet_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         engine: Optional[str] = None,
         compression: Optional[str] = None,
@@ -408,14 +438,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Parquet data node configuration.
         """
+
     @classmethod
     def configure_excel_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         has_header: Optional[bool] = None,
         sheet_name: Optional[Union[List[str], str]] = None,
@@ -442,14 +473,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Excel data node configuration.
         """
+
     @classmethod
     def configure_generic_data_node(
         cls,
         id: str,
         read_fct: Optional[Callable] = None,
         write_fct: Optional[Callable] = None,
         read_fct_args: Optional[List] = None,
@@ -476,14 +508,15 @@
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new Generic data node configuration.
         """
+
     @classmethod
     def configure_in_memory_data_node(
         cls,
         id: str,
         default_data: Optional[Any] = None,
         scope: Optional[Scope] = None,
         validity_period: Optional[timedelta] = None,
@@ -491,26 +524,29 @@
     ) -> "DataNodeConfig":
         """Configure a new *in-memory* data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new in_memory data node configuration.
             default_data (Optional[any]): The default data of the data nodes instantiated from
                 this in_memory data node configuration.
+                If provided, note that the default_data will be stored as a configuration attribute.
+                So it is designed to handle small data values like parameters, and it must be Json serializable.
             scope (Optional[Scope^]): The scope of the in_memory data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
             validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
                 considered up-to-date. Once the validity period has passed, the data node is considered stale and
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new *in-memory* data node configuration.
         """
+
     @classmethod
     def configure_pickle_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         default_data: Optional[Any] = None,
         scope: Optional[Scope] = None,
@@ -520,26 +556,29 @@
         """Configure a new pickle data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new pickle data node configuration.
             default_path (Optional[str]): The path of the pickle file.
             default_data (Optional[any]): The default data of the data nodes instantiated from
                 this pickle data node configuration.
+                If provided, note that the default_data will be stored as a configuration attribute.
+                So it is designed to handle small data values like parameters, and it must be Json serializable.
             scope (Optional[Scope^]): The scope of the pickle data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
             validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
                 considered up-to-date. Once the validity period has passed, the data node is considered stale and
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new pickle data node configuration.
         """
+
     @classmethod
     def configure_sql_table_data_node(
         cls,
         id: str,
         db_name: str,
         db_engine: str,
         table_name: str,
@@ -589,22 +628,24 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new SQL data node configuration.
         """
+
     @classmethod
     def configure_sql_data_node(
         cls,
         id: str,
         db_name: str,
         db_engine: str,
         read_query: str,
         write_query_builder: Callable,
+        append_query_builder: Optional[Callable] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_host: Optional[str] = None,
         db_port: Optional[int] = None,
         db_driver: Optional[str] = None,
         sqlite_folder_path: Optional[str] = None,
         sqlite_file_extension: Optional[str] = None,
@@ -619,15 +660,17 @@
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
             db_name (str): The database name, or the name of the SQLite database file.
             db_engine (str): The database engine. Possible values are *"sqlite"*, *"mssql"*, *"mysql"*,
                 or *"postgresql"*.
             read_query (str): The SQL query string used to read the data from the database.
             write_query_builder (Callable): A callback function that takes the data as an input parameter
-                and returns a list of SQL queries.
+                and returns a list of SQL queries to be executed when writing data to the data node.
+            append_query_builder (Optional[Callable]): A callback function that takes the data as an input parameter
+                and returns a list of SQL queries to be executed when appending data to the data node.
             db_username (Optional[str]): The database username. Required by the *"mssql"*, *"mysql"*, and
                 *"postgresql"* engines.
             db_password (Optional[str]): The database password. Required by the *"mssql"*, *"mysql"*, and
                 *"postgresql"* engines.
             db_host (Optional[str]): The database host.<br/>
                 The default value is "localhost".
             db_port (Optional[int]): The database port.<br/>
@@ -648,14 +691,15 @@
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new SQL data node configuration.
         """
+
     @classmethod
     def configure_mongo_collection_data_node(
         cls,
         id: str,
         db_name: str,
         collection_name: str,
         custom_document: Optional[Any] = None,
@@ -697,14 +741,53 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Mongo collection data node configuration.
         """
+
+    @classmethod
+    def configure_s3_object_data_node(
+        cls,
+        id: str,
+        aws_access_key: str,
+        aws_secret_access_key: str,
+        aws_s3_bucket_name: str,
+        aws_s3_object_key: str,
+        aws_region: Optional[str] = None,
+        aws_s3_object_parameters: Optional[Dict[str, Any]] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new S3 object data node configuration.
+
+        Parameters:
+            id (str): The unique identifier of the new S3 Object data node configuration.
+            aws_access_key (str): Amazon Web Services ID for to identify account.
+            aws_secret_access_key (str): Amazon Web Services access key to authenticate programmatic requests.
+            aws_s3_bucket_name (str): The bucket in S3 to read from and to write the data to.
+            aws_region (Optional[str]): Self-contained geographic area where Amazon Web Services (AWS)
+                infrastructure is located.
+            aws_s3_object_parameters (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into AWS S3 bucket access string.
+            scope (Optional[Scope^]): The scope of the S3 Object data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
+        Returns:
+            The new S3 object data node configuration.
+        """
+
     @staticmethod
     def configure_task(
         id: str,
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
@@ -725,14 +808,15 @@
                 been made on inputs.<br/>
                 The default value is False.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new task configuration.
         """
+
     @staticmethod
     def set_default_task_configuration(
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
         **properties,
@@ -755,34 +839,36 @@
                 been made on inputs.<br/>
                 The default value is False.
             **properties (dict[str, any]): A keyworded variable length list of additional
                 arguments.
         Returns:
             The default task configuration.
         """
+
     @staticmethod
     def configure_job_executions(
         mode: Optional[str] = None, max_nb_of_workers: Optional[Union[int, str]] = None, **properties
     ) -> "JobConfig":
         """Configure job execution.
 
         Parameters:
             mode (Optional[str]): The job execution mode.
-                Possible values are: *"standalone"* (the default value) or *"development"*.
-            max_nb_of_workers (Optional[int, str]): Parameter used only in default *"standalone"* mode.
+                Possible values are: *"standalone"* or *"development"*.
+            max_nb_of_workers (Optional[int, str]): Parameter used only in *"standalone"* mode.
                 This indicates the maximum number of jobs able to run in parallel.<br/>
-                The default value is 1.<br/>
+                The default value is 2.<br/>
                 A string can be provided to dynamically set the value using an environment
                 variable. The string must follow the pattern: `ENV[&lt;env_var&gt;]` where
                 `&lt;env_var&gt;` is the name of an environment variable.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new job execution configuration.
         """
+
     @staticmethod
     def add_migration_function(
         target_version: str,
         config: Union[Section, str],
         migration_fct: Callable,
         **properties,
     ):
@@ -793,34 +879,39 @@
             config (Union[Section, str]): The configuration or the `id` of the config that needs to migrate.
             migration_fct (Callable): Migration function that takes an entity as input and returns a new entity
                 that is compatible with the target production version.
             **properties (Dict[str, Any]): A keyworded variable length list of additional arguments.
         Returns:
             `MigrationConfig^`: The Migration configuration.
         """
+
     @staticmethod
     def configure_core(
         root_folder: Optional[str] = None,
         storage_folder: Optional[str] = None,
+        taipy_storage_folder: Optional[str] = None,
         repository_type: Optional[str] = None,
         repository_properties: Optional[Dict[str, Union[str, int]]] = None,
         read_entity_retry: Optional[int] = None,
         mode: Optional[str] = None,
         version_number: Optional[str] = None,
         force: Optional[bool] = None,
         **properties,
     ) -> "CoreSection":
         """Configure the Core service.
 
         Parameters:
             root_folder (Optional[str]): Path of the base folder for the taipy application.
                 The default value is "./taipy/"
-            storage_folder (Optional[str]): Folder name used to store Taipy data. The default value is ".data/".
-                It is used in conjunction with the `root_folder` field. That means the storage path is
-                <root_folder><storage_folder> (The default path is "./taipy/.data/").
+            storage_folder (str): Folder name used to store user data. The default value is "user_data/". It is used in
+                conjunction with the *root_folder* attribute. That means the storage path is
+                <root_folder><storage_folder> (The default path is "./taipy/user_data/").
+            taipy_storage_folder (str): Folder name used to store Taipy data. The default value is ".taipy/". It is
+                used in conjunction with the *root_folder* attribute. That means the storage path is
+                <root_folder><storage_folder> (The default path is "./taipy/.taipy/").
             repository_type (Optional[str]): The type of the repository to be used to store Taipy data.
                 The default value is "filesystem".
             repository_properties (Optional[Dict[str, Union[str, int]]]): A dictionary of additional properties
                 to be used by the repository.
             read_entity_retry (Optional[int]): Number of retries to read an entity from the repository
                 before return failure. The default value is 3.
             mode (Optional[str]): Indicates the mode of the version management system.
```

### Comparing `taipy-config-3.1.0/taipy/config/exceptions/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/exceptions/exceptions.py` & `taipy-config-3.2.0.dev0/taipy/config/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/global_app/__init__.py` & `taipy-config-3.2.0.dev0/taipy/config/global_app/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/global_app/global_app_config.py` & `taipy-config-3.2.0.dev0/taipy/config/global_app/global_app_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/section.py` & `taipy-config-3.2.0.dev0/taipy/config/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
 
     _DEFAULT_KEY = "default"
     _ID_KEY = "id"
 
     def __init__(self, id, **properties):
         self.id = _validate_id(id)
-        self._properties = properties or dict()
+        self._properties = properties or {}
 
     @abstractmethod
     def __copy__(self):
         raise NotImplementedError
 
     @property
     @abstractmethod
```

### Comparing `taipy-config-3.1.0/taipy/config/unique_section.py` & `taipy-config-3.2.0.dev0/taipy/config/unique_section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/config/version.py` & `taipy-config-3.2.0.dev0/taipy/config/version.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/logger/__init__.py` & `taipy-config-3.2.0.dev0/taipy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-3.1.0/taipy/logger/_taipy_logger.py` & `taipy-config-3.2.0.dev0/taipy/logger/_taipy_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,11 +30,11 @@
             logging.config.fileConfig(config_filename)
             cls.__logger = logging.getLogger("Taipy")
         else:
             cls.__logger = logging.getLogger("Taipy")
             cls.__logger.setLevel(logging.INFO)
             ch = logging.StreamHandler(sys.stdout)
             ch.setLevel(logging.INFO)
-            formatter = logging.Formatter("[%(asctime)s][%(name)s][%(levelname)s] %(message)s", "%Y-%m-%d %H:%M:%S")
-            ch.setFormatter(formatter)
+            f = logging.Formatter("[%(asctime)s.%(msecs)03d][%(name)s][%(levelname)s] %(message)s", "%Y-%m-%d %H:%M:%S")
+            ch.setFormatter(f)
             cls.__logger.addHandler(ch)
         return cls.__logger
```

### Comparing `taipy-config-3.1.0/taipy_config.egg-info/PKG-INFO` & `taipy-config-3.2.0.dev0/taipy_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 3.1.0
+Version: 3.2.0.dev0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-3.1.0/taipy_config.egg-info/SOURCES.txt` & `taipy-config-3.2.0.dev0/taipy_config.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 setup.py
 taipy/__init__.py
 taipy/_cli/__init__.py
 taipy/_cli/_help_cli.py
 taipy/_cli/_run_cli.py
 taipy/_cli/_scaffold_cli.py
 taipy/_cli/_base_cli/__init__.py
-taipy/_cli/_base_cli/_cli.py
+taipy/_cli/_base_cli/_abstract_cli.py
+taipy/_cli/_base_cli/_taipy_parser.py
 taipy/config/__init__.py
 taipy/config/_config.py
 taipy/config/_init.py
 taipy/config/config.py
 taipy/config/config.pyi
 taipy/config/section.py
 taipy/config/setup.requirements.txt
```

