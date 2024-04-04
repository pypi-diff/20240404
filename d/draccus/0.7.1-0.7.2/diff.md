# Comparing `tmp/draccus-0.7.1.tar.gz` & `tmp/draccus-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draccus-0.7.1.tar", last modified: Tue Nov 28 00:06:48 2023, max compression
+gzip compressed data, was "draccus-0.7.2.tar", last modified: Thu Apr  4 03:55:12 2024, max compression
```

## Comparing `draccus-0.7.1.tar` & `draccus-0.7.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.197963 draccus-0.7.1/
--rw-r--r--   0 dlwh       (501) staff       (20)     1179 2023-11-09 05:37:34.000000 draccus-0.7.1/LICENSE
--rw-r--r--   0 dlwh       (501) staff       (20)    23768 2023-11-28 00:06:48.197649 draccus-0.7.1/PKG-INFO
--rw-r--r--   0 dlwh       (501) staff       (20)    21142 2023-11-09 05:37:34.000000 draccus-0.7.1/README.md
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.189934 draccus-0.7.1/draccus/
--rw-r--r--   0 dlwh       (501) staff       (20)      481 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     7765 2023-11-17 17:59:54.000000 draccus-0.7.1/draccus/argparsing.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1113 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/cfgparsing.py
--rw-r--r--   0 dlwh       (501) staff       (20)     6592 2023-11-28 00:05:42.000000 draccus-0.7.1/draccus/choice_types.py
--rw-r--r--   0 dlwh       (501) staff       (20)      846 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/fields.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3262 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/help_formatter.py
--rw-r--r--   0 dlwh       (501) staff       (20)      849 2023-06-22 17:52:39.000000 draccus-0.7.1/draccus/options.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.191481 draccus-0.7.1/draccus/parsers/
--rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.7.1/draccus/parsers/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2244 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/parsers/config_parsers.py
--rw-r--r--   0 dlwh       (501) staff       (20)    13048 2023-11-28 00:05:42.000000 draccus-0.7.1/draccus/parsers/decoding.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3771 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/parsers/encoding.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2845 2023-06-22 18:34:03.000000 draccus-0.7.1/draccus/parsers/registry_utils.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3725 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/parsers/yaml_loader.py
--rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.7.1/draccus/py.typed
--rw-r--r--   0 dlwh       (501) staff       (20)    10850 2023-11-28 00:05:42.000000 draccus-0.7.1/draccus/utils.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.192666 draccus-0.7.1/draccus/wrappers/
--rw-r--r--   0 dlwh       (501) staff       (20)       88 2023-06-22 00:25:09.000000 draccus-0.7.1/draccus/wrappers/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4176 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/wrappers/choice_wrapper.py
--rw-r--r--   0 dlwh       (501) staff       (20)     7378 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/wrappers/dataclass_wrapper.py
--rw-r--r--   0 dlwh       (501) staff       (20)    10207 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/wrappers/docstring.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2199 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/wrappers/field_metavar.py
--rw-r--r--   0 dlwh       (501) staff       (20)    13149 2023-11-28 00:05:42.000000 draccus-0.7.1/draccus/wrappers/field_wrapper.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2113 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/wrappers/suppressing_argparse.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2123 2023-11-09 05:37:34.000000 draccus-0.7.1/draccus/wrappers/wrapper.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.196915 draccus-0.7.1/draccus.egg-info/
--rw-r--r--   0 dlwh       (501) staff       (20)    23768 2023-11-28 00:06:48.000000 draccus-0.7.1/draccus.egg-info/PKG-INFO
--rw-r--r--   0 dlwh       (501) staff       (20)     1463 2023-11-28 00:06:48.000000 draccus-0.7.1/draccus.egg-info/SOURCES.txt
--rw-r--r--   0 dlwh       (501) staff       (20)        1 2023-11-28 00:06:48.000000 draccus-0.7.1/draccus.egg-info/dependency_links.txt
--rw-r--r--   0 dlwh       (501) staff       (20)       93 2023-11-28 00:06:48.000000 draccus-0.7.1/draccus.egg-info/requires.txt
--rw-r--r--   0 dlwh       (501) staff       (20)       41 2023-11-28 00:06:48.000000 draccus-0.7.1/draccus.egg-info/top_level.txt
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.192932 draccus-0.7.1/examples/
--rw-r--r--   0 dlwh       (501) staff       (20)     2007 2023-11-09 05:37:34.000000 draccus-0.7.1/examples/choice_class_demo.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1609 2023-11-09 05:37:34.000000 draccus-0.7.1/examples/demo.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1852 2023-11-28 00:06:16.000000 draccus-0.7.1/pyproject.toml
--rw-r--r--   0 dlwh       (501) staff       (20)       38 2023-11-28 00:06:48.198010 draccus-0.7.1/setup.cfg
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.196227 draccus-0.7.1/tests/
--rw-r--r--   0 dlwh       (501) staff       (20)        1 2023-06-25 05:13:38.000000 draccus-0.7.1/tests/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     6231 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/conftest.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-11-28 00:06:48.196521 draccus-0.7.1/tests/draccus_choice_plugins/
--rw-r--r--   0 dlwh       (501) staff       (20)      207 2023-06-26 06:28:19.000000 draccus-0.7.1/tests/draccus_choice_plugins/gpt.py
--rw-r--r--   0 dlwh       (501) staff       (20)      437 2023-11-28 00:05:42.000000 draccus-0.7.1/tests/draccus_choice_plugins/model_config.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2153 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/test_argparse_choice_types.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2245 2023-11-28 00:05:42.000000 draccus-0.7.1/tests/test_argparse_choice_types_plugin.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4432 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/test_base.py
--rw-r--r--   0 dlwh       (501) staff       (20)      735 2023-06-22 18:07:30.000000 draccus-0.7.1/tests/test_bools.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1496 2023-11-27 23:44:09.000000 draccus-0.7.1/tests/test_choice_types.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3727 2023-07-04 07:55:11.000000 draccus-0.7.1/tests/test_decoding.py
--rw-r--r--   0 dlwh       (501) staff       (20)      761 2023-07-25 06:09:01.000000 draccus-0.7.1/tests/test_default_args.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3105 2023-06-22 17:52:37.000000 draccus-0.7.1/tests/test_docstrings.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1681 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/test_enums.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2433 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/test_inheritance.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4112 2023-11-28 00:05:42.000000 draccus-0.7.1/tests/test_lists.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3136 2023-06-22 17:34:00.000000 draccus-0.7.1/tests/test_optional.py
--rw-r--r--   0 dlwh       (501) staff       (20)      463 2023-06-22 00:25:09.000000 draccus-0.7.1/tests/test_optional_union.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2516 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/test_preferred_help.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1172 2023-06-22 18:59:25.000000 draccus-0.7.1/tests/test_tuples.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1340 2023-11-28 00:05:42.000000 draccus-0.7.1/tests/test_union.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2348 2023-06-22 17:38:04.000000 draccus-0.7.1/tests/test_utils.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1797 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/test_yaml_inclusion.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4656 2023-11-09 05:37:34.000000 draccus-0.7.1/tests/testutils.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.416240 draccus-0.7.2/
+-rw-r--r--   0 dlwh       (501) staff       (20)     1179 2023-11-09 05:37:34.000000 draccus-0.7.2/LICENSE
+-rw-r--r--   0 dlwh       (501) staff       (20)    23796 2024-04-04 03:55:12.415944 draccus-0.7.2/PKG-INFO
+-rw-r--r--   0 dlwh       (501) staff       (20)    21142 2023-11-09 05:37:34.000000 draccus-0.7.2/README.md
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.402360 draccus-0.7.2/draccus/
+-rw-r--r--   0 dlwh       (501) staff       (20)      481 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     7762 2023-12-22 21:08:59.000000 draccus-0.7.2/draccus/argparsing.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1115 2023-12-22 20:35:01.000000 draccus-0.7.2/draccus/cfgparsing.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     6592 2023-12-22 21:00:27.000000 draccus-0.7.2/draccus/choice_types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      846 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/fields.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3262 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/help_formatter.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      849 2023-06-22 17:52:39.000000 draccus-0.7.2/draccus/options.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.405006 draccus-0.7.2/draccus/parsers/
+-rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.7.2/draccus/parsers/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2244 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/parsers/config_parsers.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    16165 2023-12-24 07:17:29.000000 draccus-0.7.2/draccus/parsers/decoding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3771 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/parsers/encoding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3024 2023-12-24 20:24:14.000000 draccus-0.7.2/draccus/parsers/registry_utils.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3725 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/parsers/yaml_loader.py
+-rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.7.2/draccus/py.typed
+-rw-r--r--   0 dlwh       (501) staff       (20)    12254 2023-12-24 20:24:29.000000 draccus-0.7.2/draccus/utils.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.407570 draccus-0.7.2/draccus/wrappers/
+-rw-r--r--   0 dlwh       (501) staff       (20)       88 2023-06-22 00:25:09.000000 draccus-0.7.2/draccus/wrappers/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4176 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/wrappers/choice_wrapper.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     7356 2023-12-24 07:14:39.000000 draccus-0.7.2/draccus/wrappers/dataclass_wrapper.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    10207 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/wrappers/docstring.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2199 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/wrappers/field_metavar.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    13149 2023-11-28 00:05:42.000000 draccus-0.7.2/draccus/wrappers/field_wrapper.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2113 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/wrappers/suppressing_argparse.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2123 2023-11-09 05:37:34.000000 draccus-0.7.2/draccus/wrappers/wrapper.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.415290 draccus-0.7.2/draccus.egg-info/
+-rw-r--r--   0 dlwh       (501) staff       (20)    23796 2024-04-04 03:55:12.000000 draccus-0.7.2/draccus.egg-info/PKG-INFO
+-rw-r--r--   0 dlwh       (501) staff       (20)     1463 2024-04-04 03:55:12.000000 draccus-0.7.2/draccus.egg-info/SOURCES.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)        1 2024-04-04 03:55:12.000000 draccus-0.7.2/draccus.egg-info/dependency_links.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)      121 2024-04-04 03:55:12.000000 draccus-0.7.2/draccus.egg-info/requires.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)       41 2024-04-04 03:55:12.000000 draccus-0.7.2/draccus.egg-info/top_level.txt
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.408357 draccus-0.7.2/examples/
+-rw-r--r--   0 dlwh       (501) staff       (20)     2007 2023-11-09 05:37:34.000000 draccus-0.7.2/examples/choice_class_demo.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1609 2023-11-09 05:37:34.000000 draccus-0.7.2/examples/demo.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1880 2024-04-04 03:53:33.000000 draccus-0.7.2/pyproject.toml
+-rw-r--r--   0 dlwh       (501) staff       (20)       38 2024-04-04 03:55:12.416297 draccus-0.7.2/setup.cfg
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.414299 draccus-0.7.2/tests/
+-rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-12-23 07:37:50.000000 draccus-0.7.2/tests/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     6231 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/conftest.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-04 03:55:12.414771 draccus-0.7.2/tests/draccus_choice_plugins/
+-rw-r--r--   0 dlwh       (501) staff       (20)      207 2023-06-26 06:28:19.000000 draccus-0.7.2/tests/draccus_choice_plugins/gpt.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      437 2023-11-28 00:05:42.000000 draccus-0.7.2/tests/draccus_choice_plugins/model_config.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2153 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/test_argparse_choice_types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2245 2023-11-28 00:05:42.000000 draccus-0.7.2/tests/test_argparse_choice_types_plugin.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4815 2023-12-24 07:14:39.000000 draccus-0.7.2/tests/test_base.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      821 2023-12-23 07:25:55.000000 draccus-0.7.2/tests/test_bools.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1539 2023-12-23 08:39:41.000000 draccus-0.7.2/tests/test_choice_types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3724 2023-12-24 07:14:36.000000 draccus-0.7.2/tests/test_decoding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      803 2023-12-23 08:41:16.000000 draccus-0.7.2/tests/test_default_args.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3105 2023-06-22 17:52:37.000000 draccus-0.7.2/tests/test_docstrings.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1681 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/test_enums.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2433 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/test_inheritance.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4112 2023-11-28 00:05:42.000000 draccus-0.7.2/tests/test_lists.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3136 2023-06-22 17:34:00.000000 draccus-0.7.2/tests/test_optional.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      463 2023-06-22 00:25:09.000000 draccus-0.7.2/tests/test_optional_union.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2516 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/test_preferred_help.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1313 2023-12-23 08:11:15.000000 draccus-0.7.2/tests/test_tuples.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3027 2023-12-23 08:41:06.000000 draccus-0.7.2/tests/test_union.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2348 2023-06-22 17:38:04.000000 draccus-0.7.2/tests/test_utils.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1797 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/test_yaml_inclusion.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4656 2023-11-09 05:37:34.000000 draccus-0.7.2/tests/testutils.py
```

### Comparing `draccus-0.7.1/LICENSE` & `draccus-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/PKG-INFO` & `draccus-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.7.1
+Version: 0.7.2
 Summary: A slightly opinionated framework for simple dataclass-based configurations based on Pyrallis.
 Author-email: David Hall <dlwh@cs.stanford.edu>, Siddharth Karamcheti <skaramcheti@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2019 Fabrice Normandin
         Copyright (c) 2021 Elad Richardson
         Copyright (c) 2023 David Hall
@@ -38,19 +38,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mergedeep
-Requires-Dist: pyyaml
-Requires-Dist: pyyaml-include
-Requires-Dist: toml
-Requires-Dist: typing-inspect
+Requires-Dist: mergedeep~=1.3
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: pyyaml-include~=1.4
+Requires-Dist: toml~=0.10
+Requires-Dist: typing-inspect~=0.9.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
```

### Comparing `draccus-0.7.1/README.md` & `draccus-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/argparsing.py` & `draccus-0.7.2/draccus/argparsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from typing import Dict, Generic, Optional, Sequence, Text, Type, TypeVar, Union
 
 import mergedeep
 
 from draccus import cfgparsing, utils
 from draccus.help_formatter import SimpleHelpFormatter
 from draccus.parsers import decoding
-from draccus.utils import Dataclass, PyrallisException
+from draccus.utils import Dataclass, DraccusException
 from draccus.wrappers import DataclassWrapper
 from draccus.wrappers.docstring import HelpOrder
 from draccus.wrappers.suppressing_argparse import SuppressingArgumentParser
 
 logger = getLogger(__name__)
 
 T = TypeVar("T")
@@ -85,22 +85,22 @@
 
         new_wrapper = dataclass_wrapper_class(dataclass, default=default, preferred_help=self.preferred_help)
         new_wrapper.register_actions(parser=self.parser)
 
     def _assert_preferred_help(self):
         """Checks that `self.prefer_help` is valid."""
         if self.preferred_help not in {"inline", "above", "below"}:
-            raise PyrallisException(
+            raise DraccusException(
                 f"Value `prefer_help = {self.preferred_help}` not supported; must be one of < inline | above | below >"
             )
 
     def _assert_no_conflicts(self):
         """Checks for a field name that conflicts with utils.CONFIG_ARG"""
         if utils.CONFIG_ARG in [field.name for field in dataclasses.fields(self.config_class)]:
-            raise PyrallisException(f"{utils.CONFIG_ARG} is a reserved word for draccus")
+            raise DraccusException(f"{utils.CONFIG_ARG} is a reserved word for draccus")
 
     def parse_args(self, args=None, namespace=None) -> T:
         args, argv = self.parse_known_args(args, namespace)
         if argv:
             msg = gettext("unrecognized arguments: %s")
             self.parser.error(msg % " ".join(argv))
         return args
```

### Comparing `draccus-0.7.1/draccus/cfgparsing.py` & `draccus-0.7.2/draccus/cfgparsing.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def load(t: Type[Dataclass], stream):
     dictionary = load_config(stream)
     return decode(t, dictionary)
 
 
 def dump(config: Dataclass, stream=None, omit_defaults: bool = False, **kwargs):
     """
-    Dump the config file to yaml.
+    Dump the config object to yaml.
     optionally omit any value that still has a default value
     """
     config_dict = encode(config)
     if omit_defaults:
         defaults_dict = encode(utils.get_defaults_dict(config))
         config_dict = utils.remove_matching(config_dict, defaults_dict)
     return save_config(config_dict, stream, **kwargs)
```

### Comparing `draccus-0.7.1/draccus/choice_types.py` & `draccus-0.7.2/draccus/choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/fields.py` & `draccus-0.7.2/draccus/fields.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/help_formatter.py` & `draccus-0.7.2/draccus/help_formatter.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/options.py` & `draccus-0.7.2/draccus/options.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/parsers/config_parsers.py` & `draccus-0.7.2/draccus/parsers/config_parsers.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/parsers/decoding.py` & `draccus-0.7.2/draccus/parsers/decoding.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,87 @@
 """ Functions for decoding dataclass fields from "raw" values (e.g. from json).
 """
-import traceback
+import functools
 import typing
 from collections import OrderedDict
-from dataclasses import MISSING, Field, fields, is_dataclass
+from dataclasses import MISSING, fields, is_dataclass
 from functools import lru_cache, partial
 from logging import getLogger
 from pathlib import Path
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Optional, Protocol, Sequence, Set, Tuple, Type, TypeVar, Union
 
 from draccus.choice_types import CHOICE_TYPE_KEY, ChoiceType
 from draccus.parsers.registry_utils import RegistryFunc, withregistry
 from draccus.utils import (
+    DecodingError,
     ParsingError,
     canonicalize_union,
     format_error,
     get_type_arguments,
     has_generic_arg,
     is_choice_type,
     is_dict,
     is_enum,
     is_list,
     is_set,
     is_tuple,
     is_union,
+    stringify_type,
 )
 
 logger = getLogger(__name__)
 
 T = TypeVar("T")
+T_co = TypeVar("T_co", covariant=True)
 K = TypeVar("K")
 V = TypeVar("V")
 Dataclass = TypeVar("Dataclass")
 
 
+class DecodingFunction(Protocol[T_co]):
+    def __call__(self, raw_value: Any, path: Sequence[str]) -> T_co:
+        ...
+
+
 @withregistry
 def decode(cls: Type[T], raw_value: Any) -> T:
     cls = canonicalize_union(cls)
-    return get_decoding_fn(cls)(raw_value)  # type: ignore
+    return get_decoding_fn(cls)(raw_value, ())  # type: ignore
+
+
+def decode_from_init(cls: Type[T], raw_value: Any, path: Sequence[str]) -> T:
+    """Decodes a value into an atomic type (e.g. str, int, float, etc.)."""
+    try:
+        return cls(raw_value)  # type: ignore
+    except Exception as e:
+        raise DecodingError(path, f"Couldn't parse '{raw_value}' into a {stringify_type(cls)}") from e
 
 
-# Dictionary mapping from types/type annotations to their decoding functions.
 for t in [str, float, int, bytes]:
-    decode.register(t, t)
+    decode.register(t, partial(decode_from_init, t))
 
 
 @decode.register(bool)
-def decode_bool(raw_value: Any) -> bool:
+def decode_bool(raw_value: Any, path) -> bool:
     # only accept yaml 1.2 bools
     if raw_value is True or raw_value == "true":
         return True
     elif raw_value is False or raw_value == "false":
         return False
     else:
-        raise ValueError(f"Couldn't parse '{raw_value}' as a bool")
+        raise DecodingError(path, f"Couldn't parse '{raw_value}' into a bool")
 
 
-def decode_dataclass(cls: Type[Dataclass], d: Dict[str, Any]) -> Dataclass:
+def decode_dataclass(cls: Type[Dataclass], d: Dict[str, Any], path: Sequence[str] = ()) -> Dataclass:
     """Parses an instance of the dataclass `cls` from the dict `d`."""
-    if d is None:
-        return None
+    # if d is None:
+    #     return None
+
+    path = tuple(path)
+
     obj_dict: Dict[str, Any] = d.copy()
 
     init_args: Dict[str, Any] = {}
     non_init_args: Dict[str, Any] = {}
 
     logger.debug(f"from_dict for {cls}")
 
@@ -72,49 +90,65 @@
         if name not in obj_dict:
             if field.default is MISSING and field.default_factory is MISSING:
                 logger.warning(f"Couldn't find the field '{name}' in the dict with keys {list(d.keys())}")
             continue
 
         raw_value = obj_dict.pop(name)
         try:
-            field_value = decode_field(field, raw_value)
+            field_type = field.type
+            logger.debug(f"Decode name = {name}, type = {field_type}")
+            field_value = get_decoding_fn(field_type)(raw_value, (*path, name))  # type: ignore
         except ParsingError as e:
             raise e
+        except DecodingError as e:
+            raise e
         except Exception as e:
-            raise ParsingError(
+            raise DecodingError(
+                (*path, name),
                 f"Failed when parsing value='{raw_value}' into field \"{cls}.{name}\" of type"
-                f' {field.type}.\n\tUnderlying error is "{format_error(e)}"'
+                f' {field.type}.\n\tUnderlying error is "{format_error(e)}"',
             ) from e
 
         if field.init:
             init_args[name] = field_value
         else:
             non_init_args[name] = field_value
 
     extra_args = obj_dict
 
     # If there are arguments left over in the dict after taking all fields.
     if extra_args:
-        raise ParsingError(f"The fields {extra_args} do not belong to the class")
+        formatted_keys = ", ".join(f"`{k}`" for k in extra_args.keys())
+        raise DecodingError(path, f"The fields {formatted_keys} are not valid for {stringify_type(cls)}")
+
+    # see if there are missing required fields
+    missing_fields = []
+    for field in fields(cls):  # type: ignore
+        if field.init and field.name not in init_args and field.default is MISSING and field.default_factory is MISSING:
+            missing_fields.append(field.name)
+
+    if missing_fields:
+        formatted_keys = ", ".join(f"`{k}`" for k in missing_fields)
+        raise DecodingError(path, f"Missing required field(s) {formatted_keys} for {stringify_type(cls)}")
 
     init_args.update(extra_args)
     try:
         instance = cls(**init_args)  # type: ignore
     except TypeError as e:
-        raise ParsingError(f"Couldn't instantiate class {cls} using the given arguments.") from e
+        raise ParsingError(f"Couldn't instantiate class {stringify_type(cls)} using the given arguments.") from e
     except ValueError as e:
-        raise ParsingError(f"Couldn't instantiate class {cls} using the given arguments.") from e
+        raise ParsingError(f"Couldn't instantiate class {stringify_type(cls)} using the given arguments.") from e
 
     for name, value in non_init_args.items():
         logger.debug(f"Setting non-init field '{name}' on the instance.")
         setattr(instance, name, value)
     return instance
 
 
-def decode_choice_class(cls: Type[T], raw_value: Any) -> T:
+def decode_choice_class(cls: Type[T], raw_value: Any, path: Sequence[str]) -> T:
     """Decodes a value into an subtype of a choice class following the ChoiceType protocol."""
     assert issubclass(cls, ChoiceType)
 
     try:
         cls.get_choice_name(cls)
         # we already know what type we're looking for, so we can just use that
         return decode_dataclass(cls, raw_value)  # type: ignore
@@ -132,45 +166,37 @@
         choice_type = default
     else:
         choice_type = raw_value[CHOICE_TYPE_KEY]
 
     try:
         subcls = cls.get_choice_class(choice_type)
     except KeyError as e:
-        raise ParsingError(f"Couldn't find a choice class for '{choice_type}' in {cls}") from e
+        raise DecodingError(path, f"Couldn't find a choice class for '{choice_type}' in {cls}") from e
 
     raw_value = raw_value.copy()
     if CHOICE_TYPE_KEY in raw_value:
         raw_value.pop(CHOICE_TYPE_KEY)
 
     # return decode(subcls, raw_value)
-    return decode_dataclass(subcls, raw_value)
-
-
-def decode_field(field: Field, raw_value: Any) -> Any:
-    """Converts a "raw" value (e.g. from json file) to the type of the `field`."""
-    name = field.name
-    field_type = field.type
-    logger.debug(f"Decode name = {name}, type = {field_type}")
-    return decode(field_type, raw_value)
+    return decode_dataclass(subcls, raw_value, path)
 
 
 def has_custom_decoder(cls: Type[T]):
     cached_func: RegistryFunc = decode.dispatch(cls)
 
     if cached_func is not None:
         # If supports subclasses, pass the actual type
         if cached_func.include_subclasses:
             return partial(cached_func.func, cls)
         else:
             return cached_func.func
 
 
 @lru_cache(maxsize=100)
-def get_decoding_fn(cls: Type[T]) -> Callable[[Any], T]:
+def get_decoding_fn(cls: Type[T]) -> DecodingFunction[T]:
     """Fetches/Creates a decoding function for the given type annotation.
 
     This decoding function can then be used to create an instance of the type
     when deserializing dicts.
 
     This function inspects the type annotation and creates the right decoding
     function recursively in a "dynamic-programming-ish" fashion.
@@ -181,15 +207,31 @@
     # Start by trying the dispatch mechanism
     cached_func: RegistryFunc = decode.dispatch(cls)
     if cached_func is not None:
         # If supports subclasses, pass the actual type
         if cached_func.include_subclasses:
             return partial(cached_func.func, cls)
         else:
-            return cached_func.func
+            fn = cached_func.func
+
+            # we want to support the old interface where the decoding function
+            # takes only one argument, so we wrap it here
+            @functools.wraps(fn)
+            def backwards_compat_call(raw_value: Any, path: Sequence[str] = ()) -> T:
+                try:
+                    return fn(raw_value, path)
+                except TypeError:
+                    try:
+                        return fn(raw_value)
+                    except Exception as e:  # pylint: disable=broad-except
+                        raise DecodingError(
+                            path, f"Couldn't parse '{raw_value}' into a {stringify_type(cls)}: {e}"
+                        ) from e
+
+            return backwards_compat_call
 
     elif is_choice_type(cls):
         return partial(decode_choice_class, cls)
 
     elif is_dataclass(cls):
         return partial(decode_dataclass, cls)
 
@@ -231,86 +273,109 @@
 
     elif is_union(cls):
         logger.debug(f"Decoding a Union field: {cls}")
         args = get_type_arguments(cls)
         return decode_union(*args)
 
     elif is_enum(cls):
-        return lambda key: cls[key]
+        return partial(decode_enum, cls)
 
     import typing_inspect as tpi
 
     if tpi.is_typevar(cls):
         bound = tpi.get_bound(cls)
         logger.debug(f"Decoding a typevar: {cls}, bound type is {bound}.")
         if bound is not None:
             return get_decoding_fn(bound)
 
     raise Exception(f"No decoding function for type {cls}, consider using draccus.decode.register")
 
 
-def decode_optional(t: Type[T]) -> Callable[[Optional[Any]], Optional[T]]:
+def decode_enum(cls: Type[T], raw_value: Any, path) -> T:
+    """Decodes a value into an enum."""
+    if not is_enum(cls):
+        raise Exception(f"Expected an enum type, got {cls}")
+
+    try:
+        return cls[raw_value]  # type: ignore
+    except ValueError as e:
+        raise DecodingError(path, f"Couldn't parse '{raw_value}' into an enum of type {cls}") from e
+
+
+def decode_optional(t: Type[T]) -> DecodingFunction[Optional[T]]:
     decode = get_decoding_fn(t)  # type: ignore
 
-    def _decode_optional(val: Optional[Any]) -> Optional[T]:
-        return val if val is None else decode(val)
+    def _decode_optional(raw_value: Any, path: Sequence[str] = ()) -> Optional[T]:
+        return raw_value if raw_value is None else decode(raw_value, path)
 
     return _decode_optional
 
 
-def try_functions(funcs: Dict[Any, Callable[[Any], T]]) -> Callable[[Any], Union[T, Any]]:
-    """Tries to use the functions in succession, else returns the same value unchanged."""
-    if len(funcs) == 0:
+@typing.no_type_check
+def decode_union(*types: Type[T]) -> DecodingFunction[T]:
+    types = list(types)
+    is_optional = type(None) in types
+    # Partition the Union into None and non-None types.
+    while type(None) in types:
+        types.remove(type(None))
+
+    decoding_fns = {t: get_decoding_fn(t) for t in types}
+    # Try using each of the non-None types, in succession
+
+    if len(decoding_fns) == 0:
         raise ValueError("Must provide at least one function to try")
-    elif len(funcs) == 1:
-        return next(iter(funcs.values()))
+    elif len(decoding_fns) == 1 and not is_optional:
+        return next(iter(decoding_fns.values()))
+
+    def _try_functions(val: Any, path: Sequence[str] = ()) -> T:
+        if is_optional and val is None:
+            return None
 
-    def _try_functions(val: Any) -> Union[T, Any]:
         exceptions = {}
-        for descriptor, func in funcs.items():
+        for descriptor, func in decoding_fns.items():
             try:
-                return func(val)
+                return func(val, path)
             except Exception as e:
                 exceptions[descriptor] = e
 
-        message = "Failed to decode value using any of the following functions:\n"
+        message = "Could not decode the value into any of the given types:\n"
         for descriptor, ex in exceptions.items():
-            message += f"\t{descriptor}: {traceback.format_exception(type(ex), ex, ex.__traceback__)}"
+            if isinstance(ex, DecodingError):
+                ex = ex.strip_prefix(path)
+            descriptor = stringify_type(descriptor)
+            submessage = str(ex).split("\n")
+            # indent the submessage by (4 + len(descriptor) + 1) spaces
+            first_line = True
+            for line in submessage:
+                if first_line:
+                    first_line = False
+                    message += f"    {descriptor}: {line.strip()}"
+                    message += "\n"
+                else:
+                    message += f"{' ' * (5 + len(str(descriptor)))}{line}\n"
 
-        raise Exception(message) from exceptions[next(iter(exceptions))]
+        raise DecodingError(path, message) from exceptions[next(iter(exceptions))]
 
     return _try_functions
 
 
-@typing.no_type_check
-def decode_union(*types: Type[T]) -> Callable[[Any], Union[T, Any]]:
-    types = list(types)
-    optional = type(None) in types
-    # Partition the Union into None and non-None types.
-    while type(None) in types:
-        types.remove(type(None))
-
-    decoding_fns = {t: (decode_optional(t) if optional else get_decoding_fn(t)) for t in types}
-    # Try using each of the non-None types, in succession. Worst case, return the value.
-    return try_functions(decoding_fns)
-
-
-def decode_list(t: Type[T]) -> Callable[[List[Any]], List[T]]:
+def decode_list(t: Type[T]) -> DecodingFunction[List[T]]:
     decode_item = get_decoding_fn(t)  # type: ignore
 
-    def _decode_list(val: List[Any]) -> List[T]:
+    def _decode_list(raw_value: List[Any], path: Sequence[str]) -> List[T]:
+        path = tuple(path)
         # assert type(val) == list
-        if not isinstance(val, list):
-            raise Exception(f"The given value='{val}' is not of a valid input")
-        return [decode_item(v) for v in val]
+        if not isinstance(raw_value, list):
+            raise Exception(f"The given value='{raw_value}' is not of a valid input for a list type")
+        return [decode_item(v, (*path, str(i))) for i, v in enumerate(raw_value)]
 
     return _decode_list
 
 
-def decode_tuple(*tuple_item_types: Type[T]) -> Callable[[List[T]], Tuple[T, ...]]:
+def decode_tuple(*tuple_item_types: Type[T]) -> DecodingFunction[Tuple[T, ...]]:
     """Makes a parsing function for creating tuples."""
     # Get the decoding function for each item type
     has_ellipsis = False
     if Ellipsis in tuple_item_types:
         ellipsis_index = tuple_item_types.index(Ellipsis)
         decoding_fn_index = ellipsis_index - 1
         decoding_fn = get_decoding_fn(tuple_item_types[decoding_fn_index])  # type: ignore
@@ -320,64 +385,67 @@
         decoding_fn = no_op  # Functionality will be the same as Tuple[Any,...]
     else:
         decoding_fns = [get_decoding_fn(t) for t in tuple_item_types]  # type: ignore
 
     # Note, if there are more values than types in the tuple type, then the
     # last type is used.
 
-    def _decode_tuple(val: typing.Sequence[Any]) -> Tuple[T, ...]:
-        if val is None:
-            raise TypeError("Value must not be None for conversion to a tuple")
+    def _decode_tuple(raw_value: typing.Sequence[Any], path) -> Tuple[T, ...]:
+        path = tuple(path)
+        if raw_value is None:
+            raise DecodingError("Value must not be None for conversion to a tuple", path)
         if has_ellipsis:
-            return tuple(decoding_fn(v) for v in val)
+            return tuple(decoding_fn(v, (*path, str(i))) for i, v in enumerate(raw_value))
         else:
-            if len(decoding_fns) != len(val):
-                err_msg = f"Trying to decode {len(val)} values for a predfined {len(decoding_fns)}-Tuple"
-                raise TypeError(err_msg)
-            return tuple(decoding_fns[i](v) for i, v in enumerate(val))
+            if len(decoding_fns) != len(raw_value):
+                # err_msg = f"Trying to decode {len(raw_value)} values for a predfined {len(decoding_fns)}-Tuple"
+                err_msg = f"Expected {len(decoding_fns)} items, got {len(raw_value)}"
+                raise DecodingError(path, err_msg)
+            return tuple(decoding_fns[i](v, (*path, str(i))) for i, v in enumerate(raw_value))
 
     return _decode_tuple
 
 
-def decode_set(item_type: Type[T]) -> Callable[[List[T]], Set[T]]:
+def decode_set(item_type: Type[T]) -> DecodingFunction[Set[T]]:
     """Makes a parsing function for creating sets with items of type `item_type`."""
     # Get the parsers fn for a list of items of type `item_type`.
     parse_list_fn = decode_list(item_type)
 
-    def _decode_set(val: List[Any]) -> Set[T]:
-        return set(parse_list_fn(val))
+    def _decode_set(raw_value: List[Any], path) -> Set[T]:
+        return set(parse_list_fn(raw_value, path))
 
     return _decode_set
 
 
-def decode_dict(K_: Type[K], V_: Type[V]) -> Callable[[List[Tuple[Any, Any]]], Dict[K, V]]:
+def decode_dict(K_: Type[K], V_: Type[V]) -> DecodingFunction[Dict[K, V]]:
     """Creates a decoding function for a dict type. Works with OrderedDict too."""
     decode_k = get_decoding_fn(K_)  # type: ignore
-    decode_v: Callable[[Any], V] = get_decoding_fn(V_)  # type: ignore
+    decode_v: DecodingFunction[V] = get_decoding_fn(V_)  # type: ignore
 
-    def _decode_dict(val: Union[Dict[Any, Any], List[Tuple[Any, Any]]]) -> Dict[K, V]:
+    def _decode_dict(raw_value: Union[Dict[Any, Any], List[Tuple[Any, Any]]], path) -> Dict[K, V]:
         result: Dict[K, V] = {}
         items: Iterable[Tuple[Any, Any]]
-        if isinstance(val, list):
+        if isinstance(raw_value, list):
             result = OrderedDict()
-            items = val
-        elif isinstance(val, OrderedDict):
+            items = raw_value
+        elif isinstance(raw_value, OrderedDict):
             # NOTE(ycho): Needed to propagate `OrderedDict` type
             result = OrderedDict()
-            items = val.items()
+            items = raw_value.items()
         else:
-            items = val.items()
+            items = raw_value.items()
         for k, v in items:
-            k_ = decode_k(k)
-            v_ = decode_v(v)
+            k_ = decode_k(k, (*tuple(path), f"key={k}"))
+            v_ = decode_v(v, (*tuple(path), k))
             result[k_] = v_
         return result
 
     return _decode_dict
 
 
-def no_op(v: T) -> T:
+def no_op(raw_value: T, path) -> T:
     """Decoding function that gives back the value as-is."""
-    return v
+    del path
+    return raw_value
 
 
-decode.register(Path, Path)
+decode.register(Path, partial(decode_from_init, Path))
```

### Comparing `draccus-0.7.1/draccus/parsers/encoding.py` & `draccus-0.7.2/draccus/parsers/encoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/parsers/registry_utils.py` & `draccus-0.7.2/draccus/parsers/registry_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import get_cache_token
 from dataclasses import dataclass
 from functools import _find_impl, update_wrapper  # type: ignore
 from typing import Callable, Optional
 
+from draccus.utils import canonicalize_union
+
 
 @dataclass
 class RegistryFunc:
     # The function saved in the registry
     func: Callable
     # Whether the function should be registered for subclasses as well
     include_subclasses: bool
@@ -18,14 +20,16 @@
 
     registry = {}
     dispatch_cache = weakref.WeakKeyDictionary()
     cache_token = None
 
     def dispatch(cls) -> Optional[RegistryFunc]:
         nonlocal cache_token
+        # Python 3.10: you can't have weak refs to x|y union types, so we need to canonicalize
+        cls = canonicalize_union(cls)
         if cache_token is not None:
             current_token = get_cache_token()
             if cache_token != current_token:
                 dispatch_cache.clear()
                 cache_token = current_token
         if cls in dispatch_cache:
             impl = dispatch_cache[cls]
```

### Comparing `draccus-0.7.1/draccus/parsers/yaml_loader.py` & `draccus-0.7.2/draccus/parsers/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/utils.py` & `draccus-0.7.2/draccus/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,22 +60,47 @@
 
 T = TypeVar("T")
 
 Dataclass = TypeVar("Dataclass", bound=DataclassInstance)
 DataclassType = Type[Dataclass]
 
 
-class PyrallisException(Exception):
+class DraccusException(Exception):
     pass
 
 
-class ParsingError(PyrallisException):
+class ParsingError(DraccusException):
     pass
 
 
+class DecodingError(ParsingError):
+    key_path: Sequence[str]
+    message: str
+
+    def strip_prefix(self, prefix: Sequence[str]) -> "DecodingError":
+        if len(self.key_path) < len(prefix):
+            return self
+        if not all(self.key_path[i] == prefix[i] for i in range(len(prefix))):
+            raise ValueError(f"Prefix {prefix} is not a prefix of {self.key_path}")
+        return DecodingError(self.key_path[len(prefix) :], self.message)
+
+    def __init__(self, key_path: Sequence[str], message: str):
+        self.key_path = key_path
+        self.message = message
+        super().__init__(key_path, message)
+
+    def __str__(self):
+        if len(self.key_path) == 0:
+            return self.message
+
+        key_path = ".".join(self.key_path)
+
+        return f"`{key_path}`: {self.message}"
+
+
 def get_item_type(container_type: Type[Container[T]]) -> Type[T]:
     """Returns the `type` of the items in the provided container `type`.
 
     When no type annotation is found, or no item type is found, returns
     `typing.Any`.
     NOTE: If a type with multiple arguments is passed, only the first type
     argument is returned.
@@ -365,17 +390,16 @@
     # giving your class an __iter__ method gives you membership checking
     # and the ability to easily convert to another iterable
     def __iter__(cls):
         yield from cls.members
 
 
 def canonicalize_union(t: Type):
-    if sys.version_info >= (3, 10):
-        if isinstance(t, types.UnionType):
-            return Union[t.__args__]
+    if sys.version_info >= (3, 10) and isinstance(t, types.UnionType):
+        return Union[tuple(canonicalize_union(u) for u in t.__args__)]
     # recursively canonicalize
     args = get_args(t)
     if args:
         args = tuple(canonicalize_union(arg) for arg in args)
         origin = tpi.get_origin(t)
         if origin is not None:
             origin = raw_to_typing.get(origin, origin)
@@ -392,11 +416,35 @@
     dict: Dict,
     list: List,
     tuple: Tuple,
     set: Set,
 }
 
 
+def stringify_type(tpe: Type):
+    origin = tpi.get_origin(tpe)
+    if tpe is float:
+        return "float"
+    elif tpe is int:
+        return "int"
+    elif tpe is bool:
+        return "bool"
+    elif tpe is str:
+        return "str"
+    elif tpe is list:
+        return "list"
+    elif origin is list or origin is List:
+        return f"list[{stringify_type(get_args(tpe)[0])}]"
+
+    # TODO: more types
+    else:
+        # strip any package names/get plain name
+        try:
+            return tpe.__name__
+        except Exception:
+            return str(tpe)
+
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `draccus-0.7.1/draccus/wrappers/choice_wrapper.py` & `draccus-0.7.2/draccus/wrappers/choice_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/wrappers/dataclass_wrapper.py` & `draccus-0.7.2/draccus/wrappers/dataclass_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from logging import getLogger
 from typing import Dict, List, Optional, Type, Union, cast
 
 from draccus.utils import Dataclass, DataclassType
 
 from .. import utils
 from ..choice_types import ChoiceType
-
-# from ..parsers.decoding import get_decoding_fn, has_custom_decoder
+from ..parsers.decoding import has_custom_decoder
 from . import docstring
 from .choice_wrapper import ChoiceWrapper
 from .field_wrapper import FieldWrapper
 from .wrapper import AggregateWrapper, Wrapper
 
 logger = getLogger(__name__)
 
@@ -150,18 +149,18 @@
     parent: Optional[Wrapper],
     field: dataclasses.Field,
     preferred_help: str = docstring.HelpOrder.inline,
 ) -> Optional[Wrapper]:
     if not field.init:
         return None
 
-    # elif has_custom_decoder(field.type):
-    #     field_wrapper = field_wrapper_class(field, parent=self, prefix=self.prefix)
-    #     logger.debug(f"wrapped field at {field_wrapper.dest} has a default value of {field_wrapper.default}")
-    #     return field_wrapper
+    elif has_custom_decoder(field.type):
+        field_wrapper = FieldWrapper(field, parent=parent, preferred_help=preferred_help)
+        logger.debug(f"wrapped field at {field_wrapper.dest} has a default value of {field_wrapper.default}")
+        return field_wrapper
     elif utils.is_choice_type(field.type):
         return ChoiceWrapper(
             cast(Type[ChoiceType], field.type), field.name, parent=parent, _field=field, preferred_help=preferred_help
         )
 
     elif utils.is_tuple_or_list_of_dataclasses(field.type):
         logger.debug(f"wrapped field at {field.name} is a list of dataclasses, treating a ordinary field for argparse")
```

### Comparing `draccus-0.7.1/draccus/wrappers/docstring.py` & `draccus-0.7.2/draccus/wrappers/docstring.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/wrappers/field_metavar.py` & `draccus-0.7.2/draccus/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/wrappers/field_wrapper.py` & `draccus-0.7.2/draccus/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/wrappers/suppressing_argparse.py` & `draccus-0.7.2/draccus/wrappers/suppressing_argparse.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus/wrappers/wrapper.py` & `draccus-0.7.2/draccus/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/draccus.egg-info/PKG-INFO` & `draccus-0.7.2/draccus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.7.1
+Version: 0.7.2
 Summary: A slightly opinionated framework for simple dataclass-based configurations based on Pyrallis.
 Author-email: David Hall <dlwh@cs.stanford.edu>, Siddharth Karamcheti <skaramcheti@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2019 Fabrice Normandin
         Copyright (c) 2021 Elad Richardson
         Copyright (c) 2023 David Hall
@@ -38,19 +38,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mergedeep
-Requires-Dist: pyyaml
-Requires-Dist: pyyaml-include
-Requires-Dist: toml
-Requires-Dist: typing-inspect
+Requires-Dist: mergedeep~=1.3
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: pyyaml-include~=1.4
+Requires-Dist: toml~=0.10
+Requires-Dist: typing-inspect~=0.9.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
```

### Comparing `draccus-0.7.1/draccus.egg-info/SOURCES.txt` & `draccus-0.7.2/draccus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/examples/choice_class_demo.py` & `draccus-0.7.2/examples/choice_class_demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/examples/demo.py` & `draccus-0.7.2/examples/demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/pyproject.toml` & `draccus-0.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "draccus"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   {name = "David Hall", email = "dlwh@cs.stanford.edu"},
   {name = "Siddharth Karamcheti", email = "skaramcheti@cs.stanford.edu"},
 ]
 description = "A slightly opinionated framework for simple dataclass-based configurations based on Pyrallis."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -20,19 +20,19 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "mergedeep",
-    "pyyaml",
-    "pyyaml-include",
-    "toml",
-    "typing-inspect",
+    "mergedeep~=1.3",
+    "pyyaml~=6.0",
+    "pyyaml-include~=1.4",
+    "toml~=0.10",
+    "typing-inspect~=0.9.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "mypy",
     "pre-commit",
```

### Comparing `draccus-0.7.1/tests/conftest.py` & `draccus-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_argparse_choice_types.py` & `draccus-0.7.2/tests/test_argparse_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_argparse_choice_types_plugin.py` & `draccus-0.7.2/tests/test_argparse_choice_types_plugin.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_base.py` & `draccus-0.7.2/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Type
 
 import draccus
 from draccus import ParsingError
+from draccus.utils import DecodingError
 
 from .testutils import TestSetup, parametrize, raises
 
 
 def test_basic_required_argument(simple_attribute, silent):
     some_type, passed_value, expected_value = simple_attribute
 
@@ -23,15 +24,15 @@
 def test_not_passing_required_argument_raises_error(simple_attribute):
     some_type, passed_value, expected_value = simple_attribute
 
     @dataclass
     class SomeDataclass(TestSetup):
         some_attribute: some_type  # type: ignore
 
-    with raises(ParsingError):
+    with raises(DecodingError):
         _ = SomeDataclass.setup("")
 
 
 def test_basic_optional_argument(simple_attribute, silent):
     some_type, _, expected_value = simple_attribute
 
     @dataclass
@@ -174,7 +175,23 @@
 
     @dataclass
     class OtherFoo(Foo):
         a_class: Type[Base] = field(default=Extended, init=False)
 
     foo = OtherFoo.setup("")
     assert foo.a == Extended()
+
+
+@dataclass
+class SomeClass:
+    val: str
+
+
+def test_argparse_with_custom_parsing():
+    @dataclass
+    class Config(TestSetup):
+        s: SomeClass = SomeClass("bob")
+
+    draccus.encode.register(SomeClass, lambda x: f"custom_{x.val}")
+    draccus.decode.register(SomeClass, lambda x: SomeClass(x[7:]))
+
+    Config.setup("--s custom_bob")
```

### Comparing `draccus-0.7.1/tests/test_bools.py` & `draccus-0.7.2/tests/test_bools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 
 import pytest
 
 from draccus import ParsingError
+from draccus.utils import DecodingError
 
 from .testutils import TestSetup
 
 
 @dataclass
 class Base(TestSetup):
     """Some extension of base-class `Base`"""
@@ -24,12 +25,14 @@
     false_strings = ["False", "false"]
     for s in false_strings:
         ext = Base.setup(f"--a 5 --f {s}")
         assert ext.f is False
 
 
 def test_bool_doesnt_parse_non_bools():
-    with pytest.raises(ParsingError):
+    with pytest.raises(DecodingError) as e:
         Base.setup("--a 5 --f 5")
 
-    with pytest.raises(ParsingError):
+    assert e.value.key_path == ("f",)
+
+    with pytest.raises(DecodingError):
         Base.setup("--a 5 --f foo")
```

### Comparing `draccus-0.7.1/tests/test_choice_types.py` & `draccus-0.7.2/tests/test_choice_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 
 import pytest
 
 import draccus
 from draccus import ParsingError
 from draccus.choice_types import ChoiceRegistry
+from draccus.utils import DecodingError
 
 
 @dataclasses.dataclass
 class Person(ChoiceRegistry):
     name: str  # Person's name
 
 
@@ -29,24 +30,24 @@
 def test_choice_registry_decode():
     assert draccus.decode(Person, {"type": "adult", "name": "bob", "age": 10}) == Adult("bob", 10)
     assert draccus.decode(Person, {"type": "child", "name": "bob", "favorite_toy": "truck"}) == Child("bob", "truck")
 
     with pytest.raises(ParsingError):
         draccus.decode(Person, {"type": "baby", "name": "bob"})
 
-    with pytest.raises(ParsingError):
+    with pytest.raises(DecodingError):
         draccus.decode(Person, {"type": "adult", "name": "bob", "age": 10, "favorite_toy": "truck"})
 
-    with pytest.raises(ParsingError):
+    with pytest.raises(DecodingError):
         draccus.decode(Person, {"type": "adult", "name": 3})
 
 
 def test_registry_decode_subtype_without_type():
     draccus.decode(Child, {"name": "bob", "favorite_toy": "truck"})
 
-    with pytest.raises(ParsingError):
+    with pytest.raises(DecodingError):
         draccus.decode(Child, {"type": "adult", "name": "bob", "age": 10})
 
 
 def test_choice_registry_encode():
     assert draccus.encode(Adult("bob", 10)) == {"type": "adult", "name": "bob", "age": 10}
     assert draccus.encode(Child("bob", "truck")) == {"type": "child", "name": "bob", "favorite_toy": "truck"}
```

### Comparing `draccus-0.7.1/tests/test_decoding.py` & `draccus-0.7.2/tests/test_decoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 from dataclasses import dataclass, field
 from enum import Enum, auto
 
 import yaml
 
-from draccus.utils import PyrallisException
+import draccus
+from draccus.utils import DraccusException
 
 from .testutils import *
 
 
 class Color(Enum):
-    blue: str = auto()
-    red: str = auto()
+    blue = auto()
+    red = auto()
 
 
 def test_encode_something(simple_attribute):
     some_type, _, expected_value = simple_attribute
 
     @dataclass
     class SomeClass:
@@ -118,23 +119,19 @@
 
 
 def test_reserved_config_word():
     @dataclass
     class MainClass:
         config_path: str = ""
 
-    with raises(PyrallisException):
+    with raises(DraccusException):
         draccus.parse(MainClass)
 
 
 def test_super_nesting():
     @dataclass
     class Complicated:
         x: List[List[List[Dict[int, Tuple[int, float, str, List[float]]]]]] = field(default_factory=list)
 
     c = Complicated()
     c.x = [[[{0: (2, 1.23, "bob", [1.2, 1.3])}]]]
     assert draccus.decode(Complicated, draccus.encode(c)) == c
-
-
-#
-#
```

### Comparing `draccus-0.7.1/tests/test_default_args.py` & `draccus-0.7.2/tests/test_default_args.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from dataclasses import dataclass
 
+from draccus.utils import DecodingError
+
 from .testutils import *
 
 
 def test_no_default_argument(simple_attribute):
     some_type, passed_value, expected_value = simple_attribute
 
     @dataclass
     class SomeClass:
         a: some_type
 
     cfg = draccus.parse(config_class=SomeClass, args=shlex.split(f"--a {passed_value}"))
     assert cfg == SomeClass(a=expected_value)
 
-    with raises(ParsingError):
+    with raises(DecodingError):
         draccus.parse(config_class=SomeClass, args="")
 
 
 def test_default_dataclass_argument(simple_attribute, silent):
     some_type, passed_value, expected_value = simple_attribute
 
     @dataclass
```

### Comparing `draccus-0.7.1/tests/test_docstrings.py` & `draccus-0.7.2/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_enums.py` & `draccus-0.7.2/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_inheritance.py` & `draccus-0.7.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_lists.py` & `draccus-0.7.2/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_optional.py` & `draccus-0.7.2/tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_preferred_help.py` & `draccus-0.7.2/tests/test_preferred_help.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_tuples.py` & `draccus-0.7.2/tests/test_tuples.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from dataclasses import dataclass
 from typing import Tuple
 
 import pytest
 
 from draccus import ParsingError
+from draccus.utils import DecodingError
 from tests.testutils import TestSetup
 
 
 def test_tuple_with_n_items_takes_only_n_values():
     @dataclass
     class Container(TestSetup):
         ints: Tuple[int, int] = (1, 5)
 
     c = Container.setup("")
     assert c.ints == (1, 5)
     c = Container.setup("--ints [4,8]")
     assert c.ints == (4, 8)
-    with pytest.raises(ParsingError):
+    with pytest.raises(DecodingError) as e:
         c = Container.setup("--ints [4,5,6,7,8]")
 
+    assert "Expected 2 items, got 5" in str(e.value)
+    assert e.value.key_path == ("ints",)
+
 
 def test_tuple_elipsis_takes_any_number_of_args():
     @dataclass
     class Container(TestSetup):
         ints: Tuple[int, ...] = (1, 2, 3)
 
     c = Container.setup("")
```

### Comparing `draccus-0.7.1/tests/test_utils.py` & `draccus-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/test_yaml_inclusion.py` & `draccus-0.7.2/tests/test_yaml_inclusion.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.1/tests/testutils.py` & `draccus-0.7.2/tests/testutils.py`

 * *Files identical despite different names*

