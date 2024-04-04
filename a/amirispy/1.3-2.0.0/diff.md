# Comparing `tmp/amirispy-1.3.tar.gz` & `tmp/amirispy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amirispy-1.3.tar", last modified: Tue Jun 13 17:17:58 2023, max compression
+gzip compressed data, was "amirispy-2.0.0.tar", max compression
```

## Comparing `amirispy-1.3.tar` & `amirispy-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.118888 amirispy-1.3/
--rw-rw-rw-   0        0        0       42 2022-10-28 14:04:41.000000 amirispy-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7801 2023-06-13 17:17:58.118888 amirispy-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7212 2023-04-21 13:23:31.000000 amirispy-1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 17:17:58.118888 amirispy-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1557 2023-06-13 17:14:48.000000 amirispy-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.049877 amirispy-1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.056883 amirispy-1.3/src/amirispy/
--rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.3/src/amirispy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.070881 amirispy-1.3/src/amirispy/scripts/
--rw-rw-rw-   0        0        0      182 2022-11-04 09:40:34.000000 amirispy-1.3/src/amirispy/scripts/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/scripts/amiris.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.071879 amirispy-1.3/src/amirispy/scripts/resources/
--rw-rw-rw-   0        0        0      331 2022-10-28 13:24:56.000000 amirispy-1.3/src/amirispy/scripts/resources/fameSetup.yaml
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.085877 amirispy-1.3/src/amirispy/scripts/subcommands/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:38:53.000000 amirispy-1.3/src/amirispy/scripts/subcommands/__init__.py
--rw-rw-rw-   0        0        0     4659 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/scripts/subcommands/batch.py
--rw-rw-rw-   0        0        0     1711 2022-11-04 09:43:46.000000 amirispy-1.3/src/amirispy/scripts/subcommands/compare.py
--rw-rw-rw-   0        0        0     6149 2023-06-13 17:14:48.000000 amirispy-1.3/src/amirispy/scripts/subcommands/install.py
--rw-rw-rw-   0        0        0     1395 2023-06-13 17:07:39.000000 amirispy-1.3/src/amirispy/scripts/subcommands/run.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.117887 amirispy-1.3/src/amirispy/source/
--rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.3/src/amirispy/source/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-13 17:14:48.000000 amirispy-1.3/src/amirispy/source/cli.py
--rw-rw-rw-   0        0        0     4080 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/source/fameio_calls.py
--rw-rw-rw-   0        0        0     5671 2022-11-04 09:43:46.000000 amirispy-1.3/src/amirispy/source/file_comparison.py
--rw-rw-rw-   0        0        0     2103 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/source/files.py
--rw-rw-rw-   0        0        0     2641 2023-02-07 15:32:49.000000 amirispy-1.3/src/amirispy/source/logs.py
--rw-rw-rw-   0        0        0      828 2023-02-07 15:47:53.000000 amirispy-1.3/src/amirispy/source/util.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.065876 amirispy-1.3/src/amirispy.egg-info/
--rw-rw-rw-   0        0        0     7801 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      852 2023-06-13 17:17:58.000000 amirispy-1.3/src/amirispy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 13:24:36.000000 amirispy-1.3/src/amirispy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/top_level.txt
+-rw-r--r--   0        0        0     3153 2024-04-04 11:55:47.392180 amirispy-2.0.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2024-01-08 09:00:55.404045 amirispy-2.0.0/LICENSES/
+-rw-r--r--   0        0        0    10389 2024-01-08 09:00:55.405047 amirispy-2.0.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    13229 2023-04-21 13:23:31.581857 amirispy-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7167 2022-11-04 09:40:34.074112 amirispy-2.0.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1664 2024-04-04 11:55:47.392693 amirispy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8263 2024-04-04 11:55:47.392456 amirispy-2.0.0/README.md
+-rw-r--r--   0        0        0      111 2022-11-04 09:40:34.076185 amirispy-2.0.0/src/amirispy/__init__.py
+-rw-r--r--   0        0        0      182 2022-11-04 09:40:34.076185 amirispy-2.0.0/src/amirispy/scripts/__init__.py
+-rw-r--r--   0        0        0     2065 2024-01-08 09:26:21.087000 amirispy-2.0.0/src/amirispy/scripts/amiris.py
+-rw-r--r--   0        0        0      331 2024-04-04 09:45:19.492597 amirispy-2.0.0/src/amirispy/scripts/resources/fameSetup.yaml
+-rw-r--r--   0        0        0        0 2022-11-04 09:38:53.186209 amirispy-2.0.0/src/amirispy/scripts/subcommands/__init__.py
+-rw-r--r--   0        0        0     4667 2024-04-04 11:55:47.393018 amirispy-2.0.0/src/amirispy/scripts/subcommands/batch.py
+-rw-r--r--   0        0        0     1711 2022-11-04 09:43:46.536502 amirispy-2.0.0/src/amirispy/scripts/subcommands/compare.py
+-rw-r--r--   0        0        0     6149 2024-04-04 11:55:47.393139 amirispy-2.0.0/src/amirispy/scripts/subcommands/install.py
+-rw-r--r--   0        0        0     1390 2024-04-04 10:27:55.347558 amirispy-2.0.0/src/amirispy/scripts/subcommands/run.py
+-rw-r--r--   0        0        0      111 2022-11-04 09:40:34.078105 amirispy-2.0.0/src/amirispy/source/__init__.py
+-rw-r--r--   0        0        0     6883 2024-04-04 11:55:47.393139 amirispy-2.0.0/src/amirispy/source/cli.py
+-rw-r--r--   0        0        0     5510 2024-04-04 11:55:47.393139 amirispy-2.0.0/src/amirispy/source/fameio_calls.py
+-rw-r--r--   0        0        0     5671 2022-11-04 09:43:46.537508 amirispy-2.0.0/src/amirispy/source/file_comparison.py
+-rw-r--r--   0        0        0     2442 2024-04-04 10:27:55.348582 amirispy-2.0.0/src/amirispy/source/files.py
+-rw-r--r--   0        0        0     2641 2023-02-07 15:32:49.998683 amirispy-2.0.0/src/amirispy/source/logs.py
+-rw-r--r--   0        0        0      828 2023-02-07 15:47:53.342532 amirispy-2.0.0/src/amirispy/source/util.py
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 amirispy-2.0.0/PKG-INFO
```

### Comparing `amirispy-1.3/PKG-INFO` & `amirispy-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: amirispy
-Version: 1.3
-Summary: Python tools for the electricity market model AMIRIS
-Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
-Author: Christoph Schimeczek, Felix Nitsch
-Author-email: amiris@dlr.de
-License: Apache License 2.0
-Keywords: AMIRIS,agent-based modelling
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-<!-- SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
+<!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 
 [![PyPI version](https://badge.fury.io/py/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![PyPI license](https://img.shields.io/pypi/l/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![pipeline status](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/badges/main/pipeline.svg)](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/commits/main)
 
@@ -27,58 +10,67 @@
 # AMIRIS-Py
 Python tools for the electricity market model [AMIRIS](https://dlr-ve.gitlab.io/esy/amiris/home/).
 
 ## Installation
 
     pip install amirispy
 
-
-You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
+You may also use `pipx`. For detailed information please refer to the
+official `pipx` [documentation](https://github.com/pypa/pipx).
 
     pipx install amirispy
 
 
 ### Further Requirements
 
 In order to execute all commands provided by `amirispy`, you also require a Java Development Kit (JDK).
-JDK must be installed and accessible via your console in which you run `amirispy`. 
-
-To test, run `java --version` which should show your JDK version (required: 8 or above).
-If `java` command is not found or relates to a Java Runtime Environment (JRE), please download and install JDK (e.g. from [Adoptium](https://adoptium.net/de/temurin/releases/?version=11))
+JDK must be installed and accessible via your console in which you run `amirispy`.
 
+To test, run `java --version` which should show your JDK version (required: 11 or above).
+If `java` command is not found or relates to a Java Runtime Environment (JRE), please download and install JDK (e.g.
+from [Adoptium](https://adoptium.net/de/temurin/releases/?version=17))
 
 ## Usage
 Currently, there are three distinct commands available:
 
-- `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris) and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
-- `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and converting results
+- `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris)
+  and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
+- `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and
+  converting results
 - `amiris batch`: perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction
 - `amiris comparison`: compare the results of two different AMIRIS runs to check them for their equivalence
 
+You may also use the arguments as a list of strings in your script directly, e.g.
+
+```python
+from amirispy.scripts import amiris_cli
+
+amiris_cli(["install", "-m", "model"])
+```
 
 ### `amiris install`
 Downloads and installs the latest open access AMIRIS instance and accompanying examples.
 
-| Option               | Action                                                                                                                                                       |
-|----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `-u` or `--url`      | URL to download AMIRIS from (default: latest AMIRIS artifact from [https://gitlab.com/dlr-ve/esy/amiris/amiris](https://gitlab.com/dlr-ve/esy/amiris/amiris) |
-| `-t` or `--target`   | Folder to install `amiris-core_<version>-jar-with-dependencies.jar` to (default: `./`)                                                                       |
-| `-f` or `--force`    | Force install which may overwrites existing AMIRIS installation of same version and existing examples (default: False)                                       |
-| `-m` or `--mode`     | Option to install model and examples `all` (default), only `model`, or only `examples`                                                                       |
+| Option             | Action                                                                                                                                                       |
+|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-u` or `--url`    | URL to download AMIRIS from (default: latest AMIRIS artifact from [https://gitlab.com/dlr-ve/esy/amiris/amiris](https://gitlab.com/dlr-ve/esy/amiris/amiris) |
+| `-t` or `--target` | Folder to install `amiris-core_<version>-jar-with-dependencies.jar` to (default: `./`)                                                                       |
+| `-f` or `--force`  | Force install which may overwrites existing AMIRIS installation of same version and existing examples (default: False)                                       |
+| `-m` or `--mode`   | Option to install model and examples `all` (default), only `model`, or only `examples`                                                                       |
 
 
 ### `amiris run`
 Compile scenario, execute AMIRIS, and extract results.
 
-| Option               | Action                                                    |
-|----------------------|-----------------------------------------------------------|
-| `-j` or `--jar`      | Path to `amiris-core_<version>-jar-with-dependencies.jar` |
-| `-s` or `--scenario` | Path to a scenario yaml-file                              |
-| `-o` or `--output`   | Directory to write output to                              |
-
+| Option                      | Action                                                                                                                                                            |
+|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-j` or `--jar`             | Path to `amiris-core_<version>-jar-with-dependencies.jar`                                                                                                         |
+| `-s` or `--scenario`        | Path to a scenario yaml-file                                                                                                                                      |
+| `-o` or `--output`          | Directory to write output to, defaults to "./results"                                                                                                             |
+| `-oo` or `--output-options` | Optional arguments to override default output [conversion arguments of fameio](https://gitlab.com/fame-framework/fame-io/-/blob/main/README.md#read-fame-results) |
 
 ### `amiris batch`
 Perform multiple runs - each with scenario compilation, AMIRIS execution, and results extraction
 
 | Option                | Action                                                                        |
 |-----------------------|-------------------------------------------------------------------------------|
 | `-j` or `--jar`       | Path to `amiris-core_<version>-jar-with-dependencies.jar`                     |
@@ -101,33 +93,40 @@
 ### Help
 You reach the help menu at any point using `-h` or `--help` which gives you a list of all available options, e.g.:
 
 `amiris --help`
 
 
 ### Logging
-You may define a logging level or optional log file as **first** arguments in your workflow using any of the following arguments:
+You may define a logging level or optional log file as **first** arguments in your workflow using any of the following
+arguments:
 
-| Option               | Action                                                                                                            |
-|----------------------|-------------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.  |
-| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.        |
+| Option               | Action                                                                                                           |
+|----------------------|------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`. |
+| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.       |
 
 Example: `amiris --log debug --logfile my/log/file.txt install`
 
 ## Cite AMIRIS-Py
 If you use AMIRIS-Py for academic work, please cite:
 
-Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
+Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes
+Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated
+energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
 
 ## Contributing
 Please see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Available Support
-This is a purely scientific project by (at the moment) one research group. 
+This is a purely scientific project by (at the moment) one research group.
 Thus, there is no paid technical support available.
 
-If you experience any trouble with AMIRIS, you may contact the developers at the [openMod-Forum](https://forum.openmod.org/tag/amiris) or via [amiris@dlr.de](mailto:amiris@dlr.de).
-Please report bugs and make feature requests by filing issues following the provided templates (see also [CONTRIBUTING](CONTRIBUTING.md)).
-For substantial enhancements, we recommend that you contact us via [amiris@dlr.de](mailto:amiris@dlr.de) for working together on the code in common projects or towards common publications and thus further develop AMIRIS.
-
+If you experience any trouble with AMIRIS, you may contact the developers at
+the [openMod-Forum](https://forum.openmod.org/tag/amiris) or via [amiris@dlr.de](mailto:amiris@dlr.de).
+Please report bugs and make feature requests by filing issues following the provided templates (see
+also [CONTRIBUTING](CONTRIBUTING.md)).
+For substantial enhancements, we recommend that you contact us via [amiris@dlr.de](mailto:amiris@dlr.de) for working
+together on the code in common projects or towards common publications and thus further develop AMIRIS.
 
+## Acknowledgement
+Work on AMIRIS-Py was financed by the Helmholtz Association's Energy System Design research programme.
```

### Comparing `amirispy-1.3/src/amirispy/scripts/amiris.py` & `amirispy-2.0.0/src/amirispy/scripts/amiris.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import logging as log
+from typing import Optional, List
 
 from amirispy.scripts.subcommands.compare import compare_results
 from amirispy.scripts.subcommands.run import run_amiris
 from amirispy.scripts.subcommands.batch import batch_run_amiris
 from amirispy.scripts.subcommands.install import install_amiris
 from amirispy.source.cli import (
     arg_handling_run,
@@ -18,18 +18,18 @@
     RunOptions,
     BatchOptions,
     GeneralOptions,
 )
 from amirispy.source.logs import set_up_logger, log_and_print
 
 
-def amiris_cli() -> None:
+def amiris_cli(args: Optional[List[str]] = None) -> None:
     """Calls sub-commands with appropriate arguments as returned by the command line parser"""
 
-    command, options = arg_handling_run()
+    command, options = arg_handling_run(args)
     set_up_logger(options[GeneralOptions.LOG], options[GeneralOptions.LOGFILE])
     if command is Command.INSTALL:
         log_and_print("Starting install script")
         install_amiris(
             options[InstallOptions.URL],
             options[InstallOptions.TARGET],
             options[InstallOptions.FORCE],
```

### Comparing `amirispy-1.3/src/amirispy/scripts/subcommands/batch.py` & `amirispy-2.0.0/src/amirispy/scripts/subcommands/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,13 +105,13 @@
         file_to_test: Path to a file
 
     Returns:
         True if the given path points to valid FAME input YAML file, otherwise False
     """
     try:
         scenario = Scenario.from_dict(load_yaml(file_to_test))
-        SchemaValidator.ensure_is_valid_scenario(scenario)
+        SchemaValidator.validate_scenario_and_timeseries(scenario)
         return True
     except (ScenarioException, SchemaException, FileNotFoundError, ValidationException) as e:
         log.warning(_ERR_NO_VALID_FAME_SCENARIO.format(file_to_test))
         log.info(f"Error: {e}")
     return False
```

### Comparing `amirispy-1.3/src/amirispy/scripts/subcommands/compare.py` & `amirispy-2.0.0/src/amirispy/scripts/subcommands/compare.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.3/src/amirispy/scripts/subcommands/install.py` & `amirispy-2.0.0/src/amirispy/scripts/subcommands/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import shutil
 import zipfile
 from enum import Enum, auto
 from pathlib import Path
 from urllib.error import HTTPError
 
-import pkg_resources
+import importlib.resources
 import wget
 
 from amirispy.source.files import ensure_folder_exists, check_if_write_access
 from amirispy.source.logs import log_and_print, log_and_raise_critical
 from amirispy.source.util import check_java_installation
 
 MSG_SKIPPED_DOWNLOAD = "Skipped download of {} due to option '-m/--mode {}'"
@@ -102,16 +102,16 @@
                         f"'{file.name}' already exists in '{target_folder}'. Use `-f/--force` to override anyway."
                     )
         shutil.rmtree(Path(target_folder, "target"))
 
     else:
         log.info("Downloaded file is not a zip file: Could not unzip")
     log.info(f"Copying standard configuration files to '{target_folder}'")
-    resource_path = Path(pkg_resources.resource_filename("amirispy.scripts", "resources"))  # noqa
-    shutil.copy(src=Path(resource_path, "fameSetup.yaml"), dst=Path(target_folder, "fameSetup.yaml"))
+    resource_path = Path(importlib.resources.files("amirispy.scripts"))  # noqa
+    shutil.copy(src=Path(resource_path, "resources", "fameSetup.yaml"), dst=Path(target_folder, "fameSetup.yaml"))
     log_and_print(f"AMIRIS installation to '{target_folder}' completed.")
 
 
 def progress_bar(current, total, _) -> str:
     """Progress bar that adds a newline in the end"""
     progress_message = "Download status: "
     if total < 0:
```

### Comparing `amirispy-1.3/src/amirispy/scripts/subcommands/run.py` & `amirispy-2.0.0/src/amirispy/scripts/subcommands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 _ERR_NOT_A_FILE = "Specified path '{}' is no file."
 
 
 def run_amiris(options: dict) -> None:
     """
     Compile scenario to protobuf using fameio.scripts.make_config,
-    execute AMIRIS,
-    and extract results using fameio.scripts.convert_results
+    execute AMIRIS, and extract results using fameio.scripts.convert_results
 
     Args:
         options: dictionary of command line instructions
 
     Returns:
         None
     """
```

### Comparing `amirispy-1.3/src/amirispy/source/cli.py` & `amirispy-2.0.0/src/amirispy/source/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 from enum import Enum, auto
 from pathlib import Path
-from typing import Tuple, Any, Dict
+from typing import Any, Dict, Tuple, Optional, List
 
 from amirispy.scripts.subcommands.install import InstallMode
 from amirispy.source.logs import LogLevels
 
 AMIRIS_PARSER = "Command-line interface to the electricity market model AMIRIS"
 AMIRIS_LOG_FILE_HELP = "Provide logging file (default: None)"
 AMIRIS_LOG_LEVEL_HELP = f"Choose logging level (default: {LogLevels.ERROR.name})"
@@ -19,17 +19,19 @@
 INSTALL_TARGET_HELP = "Folder to install 'amiris-core_<version>-jar-with-dependencies.jar' to (default: './')"
 INSTALL_FORCE_HELP = "Force install to overwrite existing AMIRIS installation and/or examples (default: False)"
 INSTALL_MODE_HELP = "Choose to install model and examples `all` (default), only `model`, or only `examples`"
 RUN_HELP = "Compile scenario, execute AMIRIS, and extract results"
 RUN_JAR_HELP = "Path to 'amiris-core_<version>-jar-with-dependencies.jar'"
 RUN_SCENARIO_HELP = "Path to a scenario yaml-file"
 RUN_OUTPUT_HELP = "Directory to write output to"
-BATCH_HELP = (
-    "Batch mode to perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction"
+RUN_OUTPUT_OPTION_HELP = (
+    "optional pass through of FAME-Io's output conversion options, see "
+    "https://gitlab.com/fame-framework/fame-io/-/blob/main/README.md#read-fame-results"
 )
+BATCH_HELP = "Batch mode to perform multiple runs each with scenario compilation, execution, and results extraction"
 BATCH_SCENARIO_HELP = "Path to single or list of: scenario yaml-files or their enclosing directories"
 BATCH_RECURSIVE_HELP = "Option to recursively search in provided Path for scenario (default: False)"
 DEFAULT_PATTERN = "*.y*ml"
 BATCH_PATTERN_HELP = f"Optional name pattern that scenario files searched for must match (default: '{DEFAULT_PATTERN}')"
 COMPARE_HELP = "Compare if results of two AMIRIS runs and equivalent"
 COMPARE_EXPECTED_HELP = "Path to folder with expected results"
 COMPARE_TEST_HELP = "Path to folder with results to test"
@@ -72,14 +74,15 @@
 
 class RunOptions(Enum):
     """Options for command `run`"""
 
     JAR = auto()
     SCENARIO = auto()
     OUTPUT = auto()
+    OUTPUT_OPTIONS = auto()
 
 
 class BatchOptions(Enum):
     """Options for command `batch`"""
 
     JAR = auto()
     SCENARIOS = auto()
@@ -92,23 +95,26 @@
     Command.COMPARE: CompareOptions,
     Command.RUN: RunOptions,
     Command.INSTALL: InstallOptions,
     Command.BATCH: BatchOptions,
 }
 
 
-def arg_handling_run() -> Tuple[Command, Dict[Enum, Any]]:
-    """Handles command line arguments for `amiris` and returns `command` and its options `args`"""
+def arg_handling_run(input_args: Optional[List[str]] = None) -> Tuple[Command, Dict[Enum, Any]]:
+    """
+    Handles command line arguments for `amiris` and returns `command` and its options `args`
+    Allows to set args from a string through input_args
+    """
 
     parent_parser = argparse.ArgumentParser(prog="amiris", description=AMIRIS_PARSER)
     parent_parser.add_argument("-lf", "--logfile", type=Path, required=False, help=AMIRIS_LOG_FILE_HELP)
     parent_parser.add_argument(
         "-l",
         "--log",
-        default=LogLevels.ERROR.name,
+        default=LogLevels.WARN.name,
         choices=[level.name.lower() for level in LogLevels],
         help=AMIRIS_LOG_LEVEL_HELP,
     )
     subparsers = parent_parser.add_subparsers(dest="command", required=True, help=AMIRIS_COMMAND_HELP)
 
     install_parser = subparsers.add_parser("install", help=INSTALL_HELP)
     install_parser.add_argument("--url", "-u", default=URL_LATEST_AMIRIS, help=INSTALL_URL_MODEL_HELP)
@@ -121,29 +127,30 @@
         choices=[mode.name.lower() for mode in InstallMode],
         default=InstallMode.ALL.name,
         help=INSTALL_MODE_HELP,
     )
     run_parser = subparsers.add_parser("run", help=RUN_HELP)
     run_parser.add_argument("--jar", "-j", type=Path, required=True, help=RUN_JAR_HELP)
     run_parser.add_argument("--scenario", "-s", type=Path, required=True, help=RUN_SCENARIO_HELP)
-    run_parser.add_argument("--output", "-o", type=Path, default=Path("./"), help=RUN_OUTPUT_HELP)
+    run_parser.add_argument("--output", "-o", type=Path, default=Path("./result"), help=RUN_OUTPUT_HELP)
+    run_parser.add_argument("--output-options", "-oo", type=str, default="", help=RUN_OUTPUT_OPTION_HELP)
 
     batch_parser = subparsers.add_parser("batch", help=BATCH_HELP)
     batch_parser.add_argument("--jar", "-j", type=Path, required=True, help=RUN_JAR_HELP)
     batch_parser.add_argument("--scenarios", "-s", nargs="+", type=Path, required=True, help=BATCH_SCENARIO_HELP)
     batch_parser.add_argument("--output", "-o", type=Path, default=Path("./"), help=RUN_OUTPUT_HELP)
     batch_parser.add_argument("--recursive", "-r", default=False, action="store_true", help=BATCH_RECURSIVE_HELP)
     batch_parser.add_argument("--pattern", "-p", type=str, default=DEFAULT_PATTERN, help=BATCH_PATTERN_HELP)
 
     compare_parser = subparsers.add_parser("compare", help=COMPARE_HELP)
     compare_parser.add_argument("--expected", "-e", type=Path, required=True, help=COMPARE_EXPECTED_HELP)
     compare_parser.add_argument("--test", "-t", type=Path, required=True, help=COMPARE_TEST_HELP)
     compare_parser.add_argument("--ignore", "-i", required=False, help=COMPARE_IGNORE_HELP)
 
-    args = vars(parent_parser.parse_args())
+    args = vars(parent_parser.parse_args(input_args))
 
     command = Command[args.pop("command").upper()]
 
     return command, enumify(command, args)
 
 
 def enumify(command: Command, args: dict) -> Dict[Enum, Any]:
```

### Comparing `amirispy-1.3/src/amirispy/source/file_comparison.py` & `amirispy-2.0.0/src/amirispy/source/file_comparison.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.3/src/amirispy/source/files.py` & `amirispy-2.0.0/src/amirispy/source/files.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+import logging
 import os
 from pathlib import Path
 from typing import List
 
 from amirispy.source.logs import log_error_and_raise
 
 _CSV_FILE_ENDING = ".csv"
 
 _ERR_NOT_A_FOLDER = "Given Path '{}' is not a directory."
 _ERR_MISSING_FOLDER = "Specified directory '{}' is missing."
 _ERR_NO_ACCESS = "No writing permission to directory '{}'."
 
+_WARN_NOT_EMPTY = "Folder '{}' is not empty - overriding files."
+
 
 def get_all_csv_files_in_folder_except(folder: Path, exceptions: List[str] = None) -> List[Path]:
     """
     Find all csv files in a folder that can optionally ignore a files with a given file name
 
     Args:
         folder: to search for csv files - file ending is **not** case sensitive
@@ -55,7 +58,18 @@
         path.mkdir(parents=True)
 
 
 def check_if_write_access(path: Path) -> None:
     """Raises Error if no writing access to `path`"""
     if not os.access(path, os.W_OK):
         log_error_and_raise(OSError(_ERR_NO_ACCESS.format(path)))
+
+
+def warn_if_not_empty(folder: Path) -> None:
+    """
+    Logs a warning if given folder is not empty
+
+    Args:
+        folder: to check for files
+    """
+    if list(folder.glob("*")):
+        logging.warning(_WARN_NOT_EMPTY.format(folder))
```

### Comparing `amirispy-1.3/src/amirispy/source/logs.py` & `amirispy-2.0.0/src/amirispy/source/logs.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.3/src/amirispy/source/util.py` & `amirispy-2.0.0/src/amirispy/source/util.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.3/src/amirispy.egg-info/PKG-INFO` & `amirispy-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,160 @@
-Metadata-Version: 2.1
-Name: amirispy
-Version: 1.3
-Summary: Python tools for the electricity market model AMIRIS
-Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
-Author: Christoph Schimeczek, Felix Nitsch
-Author-email: amiris@dlr.de
-License: Apache License 2.0
-Keywords: AMIRIS,agent-based modelling
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-<!-- SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
-
-SPDX-License-Identifier: Apache-2.0 -->
-
-[![PyPI version](https://badge.fury.io/py/amirispy.svg)](https://badge.fury.io/py/amirispy)
-[![PyPI license](https://img.shields.io/pypi/l/amirispy.svg)](https://badge.fury.io/py/amirispy)
-[![pipeline status](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/badges/main/pipeline.svg)](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/commits/main)
-
-
-# AMIRIS-Py
-Python tools for the electricity market model [AMIRIS](https://dlr-ve.gitlab.io/esy/amiris/home/).
-
-## Installation
-
-    pip install amirispy
-
-
-You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
-
-    pipx install amirispy
-
-
-### Further Requirements
-
-In order to execute all commands provided by `amirispy`, you also require a Java Development Kit (JDK).
-JDK must be installed and accessible via your console in which you run `amirispy`. 
-
-To test, run `java --version` which should show your JDK version (required: 8 or above).
-If `java` command is not found or relates to a Java Runtime Environment (JRE), please download and install JDK (e.g. from [Adoptium](https://adoptium.net/de/temurin/releases/?version=11))
-
-
-## Usage
-Currently, there are three distinct commands available:
-
-- `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris) and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
-- `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and converting results
-- `amiris batch`: perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction
-- `amiris comparison`: compare the results of two different AMIRIS runs to check them for their equivalence
-
-
-### `amiris install`
-Downloads and installs the latest open access AMIRIS instance and accompanying examples.
-
-| Option               | Action                                                                                                                                                       |
-|----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `-u` or `--url`      | URL to download AMIRIS from (default: latest AMIRIS artifact from [https://gitlab.com/dlr-ve/esy/amiris/amiris](https://gitlab.com/dlr-ve/esy/amiris/amiris) |
-| `-t` or `--target`   | Folder to install `amiris-core_<version>-jar-with-dependencies.jar` to (default: `./`)                                                                       |
-| `-f` or `--force`    | Force install which may overwrites existing AMIRIS installation of same version and existing examples (default: False)                                       |
-| `-m` or `--mode`     | Option to install model and examples `all` (default), only `model`, or only `examples`                                                                       |
-
-
-### `amiris run`
-Compile scenario, execute AMIRIS, and extract results.
-
-| Option               | Action                                                    |
-|----------------------|-----------------------------------------------------------|
-| `-j` or `--jar`      | Path to `amiris-core_<version>-jar-with-dependencies.jar` |
-| `-s` or `--scenario` | Path to a scenario yaml-file                              |
-| `-o` or `--output`   | Directory to write output to                              |
-
-
-### `amiris batch`
-Perform multiple runs - each with scenario compilation, AMIRIS execution, and results extraction
-
-| Option                | Action                                                                        |
-|-----------------------|-------------------------------------------------------------------------------|
-| `-j` or `--jar`       | Path to `amiris-core_<version>-jar-with-dependencies.jar`                     |
-| `-s` or `--scenarios` | Path to single or list of: scenario yaml-files or their enclosing directories |
-| `-o` or `--output`    | Directory to write output to                                                  |
-| `-r` or `--recursive` | Option to recursively search in provided Path for scenario (default: False)   |
-| `-p` or `--pattern`   | Optional name pattern that scenario files searched for must match             |
-
-
-### `amiris compare`
-Compare if results of two AMIRIS runs and equivalent.
-
-| Option               | Action                                                            |
-|----------------------|-------------------------------------------------------------------|
-| `-e` or `--expected` | Path to folder with expected result .csv files                    |
-| `-t` or `--test`     | Path to folder with results files (.csv) to test  for equivalence |
-| `-i` or `--ignore`   | Optional list of file names not to be compared                    |
-
-
-### Help
-You reach the help menu at any point using `-h` or `--help` which gives you a list of all available options, e.g.:
-
-`amiris --help`
-
-
-### Logging
-You may define a logging level or optional log file as **first** arguments in your workflow using any of the following arguments:
-
-| Option               | Action                                                                                                            |
-|----------------------|-------------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.  |
-| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.        |
-
-Example: `amiris --log debug --logfile my/log/file.txt install`
-
-## Cite AMIRIS-Py
-If you use AMIRIS-Py for academic work, please cite:
-
-Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
-
-## Contributing
-Please see [CONTRIBUTING](CONTRIBUTING.md).
-
-## Available Support
-This is a purely scientific project by (at the moment) one research group. 
-Thus, there is no paid technical support available.
-
-If you experience any trouble with AMIRIS, you may contact the developers at the [openMod-Forum](https://forum.openmod.org/tag/amiris) or via [amiris@dlr.de](mailto:amiris@dlr.de).
-Please report bugs and make feature requests by filing issues following the provided templates (see also [CONTRIBUTING](CONTRIBUTING.md)).
-For substantial enhancements, we recommend that you contact us via [amiris@dlr.de](mailto:amiris@dlr.de) for working together on the code in common projects or towards common publications and thus further develop AMIRIS.
-
-
+Metadata-Version: 2.1
+Name: amirispy
+Version: 2.0.0
+Summary: Python tools for the electricity market model AMIRIS
+Home-page: https://dlr-ve.gitlab.io/esy/amiris/home/
+License: Apache-2.0
+Keywords: AMIRIS,agent-based modelling,electricity market
+Author: Christoph Schimeczek
+Author-email: amiris@dlr.de
+Maintainer: Christoph Schimeczek
+Maintainer-email: amiris@dlr.de
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: fameio (>=2.0.0,<3.0.0)
+Requires-Dist: wget (>=3.2,<4.0)
+Project-URL: Repository, https://gitlab.com/dlr-ve/esy/amiris/amiris-py/
+Description-Content-Type: text/markdown
+
+<!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
+
+SPDX-License-Identifier: Apache-2.0 -->
+
+[![PyPI version](https://badge.fury.io/py/amirispy.svg)](https://badge.fury.io/py/amirispy)
+[![PyPI license](https://img.shields.io/pypi/l/amirispy.svg)](https://badge.fury.io/py/amirispy)
+[![pipeline status](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/badges/main/pipeline.svg)](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/commits/main)
+
+
+# AMIRIS-Py
+Python tools for the electricity market model [AMIRIS](https://dlr-ve.gitlab.io/esy/amiris/home/).
+
+## Installation
+
+    pip install amirispy
+
+You may also use `pipx`. For detailed information please refer to the
+official `pipx` [documentation](https://github.com/pypa/pipx).
+
+    pipx install amirispy
+
+
+### Further Requirements
+
+In order to execute all commands provided by `amirispy`, you also require a Java Development Kit (JDK).
+JDK must be installed and accessible via your console in which you run `amirispy`.
+
+To test, run `java --version` which should show your JDK version (required: 11 or above).
+If `java` command is not found or relates to a Java Runtime Environment (JRE), please download and install JDK (e.g.
+from [Adoptium](https://adoptium.net/de/temurin/releases/?version=17))
+
+## Usage
+Currently, there are three distinct commands available:
+
+- `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris)
+  and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
+- `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and
+  converting results
+- `amiris batch`: perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction
+- `amiris comparison`: compare the results of two different AMIRIS runs to check them for their equivalence
+
+You may also use the arguments as a list of strings in your script directly, e.g.
+
+```python
+from amirispy.scripts import amiris_cli
+
+amiris_cli(["install", "-m", "model"])
+```
+
+### `amiris install`
+Downloads and installs the latest open access AMIRIS instance and accompanying examples.
+
+| Option             | Action                                                                                                                                                       |
+|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-u` or `--url`    | URL to download AMIRIS from (default: latest AMIRIS artifact from [https://gitlab.com/dlr-ve/esy/amiris/amiris](https://gitlab.com/dlr-ve/esy/amiris/amiris) |
+| `-t` or `--target` | Folder to install `amiris-core_<version>-jar-with-dependencies.jar` to (default: `./`)                                                                       |
+| `-f` or `--force`  | Force install which may overwrites existing AMIRIS installation of same version and existing examples (default: False)                                       |
+| `-m` or `--mode`   | Option to install model and examples `all` (default), only `model`, or only `examples`                                                                       |
+
+
+### `amiris run`
+Compile scenario, execute AMIRIS, and extract results.
+
+| Option                      | Action                                                                                                                                                            |
+|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-j` or `--jar`             | Path to `amiris-core_<version>-jar-with-dependencies.jar`                                                                                                         |
+| `-s` or `--scenario`        | Path to a scenario yaml-file                                                                                                                                      |
+| `-o` or `--output`          | Directory to write output to, defaults to "./results"                                                                                                             |
+| `-oo` or `--output-options` | Optional arguments to override default output [conversion arguments of fameio](https://gitlab.com/fame-framework/fame-io/-/blob/main/README.md#read-fame-results) |
+
+### `amiris batch`
+Perform multiple runs - each with scenario compilation, AMIRIS execution, and results extraction
+
+| Option                | Action                                                                        |
+|-----------------------|-------------------------------------------------------------------------------|
+| `-j` or `--jar`       | Path to `amiris-core_<version>-jar-with-dependencies.jar`                     |
+| `-s` or `--scenarios` | Path to single or list of: scenario yaml-files or their enclosing directories |
+| `-o` or `--output`    | Directory to write output to                                                  |
+| `-r` or `--recursive` | Option to recursively search in provided Path for scenario (default: False)   |
+| `-p` or `--pattern`   | Optional name pattern that scenario files searched for must match             |
+
+
+### `amiris compare`
+Compare if results of two AMIRIS runs and equivalent.
+
+| Option               | Action                                                            |
+|----------------------|-------------------------------------------------------------------|
+| `-e` or `--expected` | Path to folder with expected result .csv files                    |
+| `-t` or `--test`     | Path to folder with results files (.csv) to test  for equivalence |
+| `-i` or `--ignore`   | Optional list of file names not to be compared                    |
+
+
+### Help
+You reach the help menu at any point using `-h` or `--help` which gives you a list of all available options, e.g.:
+
+`amiris --help`
+
+
+### Logging
+You may define a logging level or optional log file as **first** arguments in your workflow using any of the following
+arguments:
+
+| Option               | Action                                                                                                           |
+|----------------------|------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`. |
+| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.       |
+
+Example: `amiris --log debug --logfile my/log/file.txt install`
+
+## Cite AMIRIS-Py
+If you use AMIRIS-Py for academic work, please cite:
+
+Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes
+Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated
+energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
+
+## Contributing
+Please see [CONTRIBUTING](CONTRIBUTING.md).
+
+## Available Support
+This is a purely scientific project by (at the moment) one research group.
+Thus, there is no paid technical support available.
+
+If you experience any trouble with AMIRIS, you may contact the developers at
+the [openMod-Forum](https://forum.openmod.org/tag/amiris) or via [amiris@dlr.de](mailto:amiris@dlr.de).
+Please report bugs and make feature requests by filing issues following the provided templates (see
+also [CONTRIBUTING](CONTRIBUTING.md)).
+For substantial enhancements, we recommend that you contact us via [amiris@dlr.de](mailto:amiris@dlr.de) for working
+together on the code in common projects or towards common publications and thus further develop AMIRIS.
+
+## Acknowledgement
+Work on AMIRIS-Py was financed by the Helmholtz Association's Energy System Design research programme.
```

