# Comparing `tmp/foundrytools-cli-1.1.8.tar.gz` & `tmp/foundrytools-cli-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundrytools-cli-1.1.8.tar", last modified: Fri Mar  1 07:28:59 2024, max compression
+gzip compressed data, was "foundrytools-cli-1.1.9.tar", last modified: Mon Mar  4 07:41:59 2024, max compression
```

## Comparing `foundrytools-cli-1.1.8.tar` & `foundrytools-cli-1.1.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.237424 foundrytools-cli-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-01 07:28:59.237424 foundrytools-cli-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.225424 foundrytools-cli-1.1.8/foundryToolsCLI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.229424 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13682 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_cff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    32961 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_hhea.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_os2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_otf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_print.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_ttf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.229424 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/
--rw-r--r--   0 runner    (1001) docker     (127)    39836 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/Font.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/VFont.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.229424 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    21284 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/UI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27904 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/fonts_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/styles_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    16844 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.229424 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/otf_to_ttf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/sfnt_to_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/ttf_to_otf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/variable_to_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/web_to_sfnt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.229424 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/printer/
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/printer/UI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.233424 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/CFF_.py
--rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/OS_2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/head.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/hhea.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.233424 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/bits_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/click_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/otf_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/ps_recalc_stems.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/ps_recalc_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/skia_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/ttf_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/foundryToolsCLI/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:28:59.237424 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 07:28:59.000000 foundrytools-cli-1.1.8/foundrytools_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 07:28:59.237424 foundrytools-cli-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-01 07:28:54.000000 foundrytools-cli-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.770468 foundrytools-cli-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-04 07:41:59.770468 foundrytools-cli-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.762467 foundrytools-cli-1.1.9/foundryToolsCLI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.762467 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13682 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_cff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32961 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_hhea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_os2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_otf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.766467 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    39836 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/Font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/VFont.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.766467 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    21284 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/UI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27904 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/fonts_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/styles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16844 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.766467 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/otf_to_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/sfnt_to_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/ttf_to_otf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/variable_to_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/web_to_sfnt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.766467 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/printer/
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/printer/UI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.770468 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/CFF_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/OS_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/hhea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/post.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.770468 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/bits_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/click_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/otf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/ps_recalc_stems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/ps_recalc_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/skia_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/ttf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/foundryToolsCLI/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 07:41:59.770468 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 07:41:59.000000 foundrytools-cli-1.1.9/foundrytools_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 07:41:59.770468 foundrytools-cli-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-04 07:41:49.000000 foundrytools-cli-1.1.9/setup.py
```

### Comparing `foundrytools-cli-1.1.8/LICENSE` & `foundrytools-cli-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/PKG-INFO` & `foundrytools-cli-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundrytools-cli
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of command line tools to inspect, manipulate and convert font files
 Home-page: https://github.com/ftCLI/FoundryTools-CLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `foundrytools-cli-1.1.8/README.md` & `foundrytools-cli-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_assistant.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_assistant.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_cff.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_cff.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_converter.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_converter.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_fix.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_fix.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_hhea.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_hhea.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_metrics.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_metrics.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_name.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_name.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_os2.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_os2.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_otf.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_otf.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_post.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_post.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_print.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_print.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_ttf.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_ttf.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/CLI/ftcli_utils.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/CLI/ftcli_utils.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/Font.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/Font.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/VFont.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/VFont.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/UI.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/UI.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/fonts_data.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/fonts_data.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/assistant/styles_mapping.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/assistant/styles_mapping.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/constants.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/constants.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/options.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/options.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/otf_to_ttf.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/otf_to_ttf.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/sfnt_to_web.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/sfnt_to_web.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/ttf_to_otf.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/ttf_to_otf.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 
                 # We need to save the file here, otherwise the script won't correctly compile
                 # cff.topDictIndex values
                 # TODO: this is a workaround. Try to find a solution
                 cff_font.save(output_file)
                 cff_font = Font(output_file, recalcTimestamp=False)
                 cff_font.otf_fix_contours(min_area=25, verbose=False)
+                cff_font.recalc_avg_char_width()
+                cff_font.recalc_max_context()
 
                 if self.options.subroutinize:
                     cff_font.otf_subroutinize()
 
                 other_blues, blue_values = cff_font.otf_recalc_zones()
                 cff_font.set_zones(other_blues=other_blues, blue_values=blue_values)
                 std_h_w, std_v_w = cff_font.otf_recalc_stems()
```

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/variable_to_static.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/variable_to_static.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/converters/web_to_sfnt.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/converters/web_to_sfnt.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/printer/UI.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/printer/UI.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/CFF_.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/CFF_.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/OS_2.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/OS_2.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/head.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/head.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/hhea.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/hhea.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/name.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/name.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/tables/post.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/tables/post.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/bits_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/bits_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/cli_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/click_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/click_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/logger.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/otf_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/otf_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/ps_recalc_stems.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/ps_recalc_stems.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/ps_recalc_zones.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/ps_recalc_zones.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/skia_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/skia_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/text_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/text_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/timer.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/timer.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/Lib/utils/ttf_tools.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/Lib/utils/ttf_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundryToolsCLI/__main__.py` & `foundrytools-cli-1.1.9/foundryToolsCLI/__main__.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/foundrytools_cli.egg-info/PKG-INFO` & `foundrytools-cli-1.1.9/foundrytools_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundrytools-cli
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of command line tools to inspect, manipulate and convert font files
 Home-page: https://github.com/ftCLI/FoundryTools-CLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `foundrytools-cli-1.1.8/foundrytools_cli.egg-info/SOURCES.txt` & `foundrytools-cli-1.1.9/foundrytools_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.1.8/setup.py` & `foundrytools-cli-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     with io.open("requirements.txt", encoding="utf-8") as requirements:
         return [line.replace("==", ">=") for line in requirements.readlines()]
 
 
 setuptools.setup(
     name="foundrytools-cli",
-    version="1.1.8",
+    version="1.1.9",
     description="A set of command line tools to inspect, manipulate and convert font files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ftCLI",
     author_email="ftcli@proton.me",
     url="https://github.com/ftCLI/FoundryTools-CLI",
     packages=setuptools.find_packages(),
```

