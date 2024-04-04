# Comparing `tmp/nrel_pypsse-1.1.1.tar.gz` & `tmp/nrel_pypsse-1.1.2.tar.gz`

## Comparing `nrel_pypsse-1.1.1.tar` & `nrel_pypsse-1.1.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/__init__.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/channel_map.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/common.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/compile.bat
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/conec.flx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/conet.flx
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/contingencies.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/custom_logger.py
--rw-r--r--   0        0        0     9747 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/enumerations.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/exceptions.py
--rw-r--r--   0        0        0    20618 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/helics_interface.py
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/mdao_interface.py
--rw-r--r--   0        0        0    14322 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/models.py
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/project.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/result_container.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/simulation_controller.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/simulator.py
--rw-r--r--   0        0        0    18413 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/PSSE.v2.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/common.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/config.yaml
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/app/__init__.py
--rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/app/psse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/web/__init__.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/api/web/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/__init__.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/create_profiles.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/create_project.py
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/explore.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/pypsse.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/run.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/cli/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/branch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/bus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/fixed_shunt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/machine.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/switched_shunt.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/components/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/data_writers/__init__.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/data_writers/csv.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/data_writers/data_writer.py
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/data_writers/hdf5.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/data_writers/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/defaults/__init__.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/defaults/export_settings.toml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/defaults/simulation_settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/__init__.py
--rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/abstract_mode.py
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/constants.py
--rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/dynamic.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/pcm.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/snap.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/modes/static.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/parsers/__init__.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/parsers/gic_parser.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/parsers/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/profile_manager/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/profile_manager/common.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/profile_manager/profile.py
--rw-r--r--   0        0        0    10687 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/profile_manager/profile_store.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/utils/__init__.py
--rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/utils/dynamic_utils.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/utils/dc2ac/__init__.py
--rw-r--r--   0        0        0    33318 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/utils/dc2ac/dc_ac_algorithm.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pypsse/utils/dc2ac/helper_functions.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/README.md
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/__init__.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/channel_map.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/common.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/compile.bat
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/conec.flx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/conet.flx
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/contingencies.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/custom_logger.py
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/enumerations.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/exceptions.py
+-rw-r--r--   0        0        0    20618 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/helics_interface.py
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/mdao_interface.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/models.py
+-rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/project.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/result_container.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/simulation_controller.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/simulator.py
+-rw-r--r--   0        0        0    18413 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/PSSE.v2.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/common.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/config.yaml
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/app/__init__.py
+-rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/app/psse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/web/__init__.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/web/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/__init__.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/create_profiles.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/create_project.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/explore.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/pypsse.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/run.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/branch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/bus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/fixed_shunt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/machine.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/switched_shunt.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/__init__.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/csv.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/data_writer.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/hdf5.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/defaults/__init__.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/defaults/export_settings.toml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/defaults/simulation_settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/__init__.py
+-rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/abstract_mode.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/constants.py
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/dynamic.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/pcm.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/snap.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/static.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/parsers/__init__.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/parsers/gic_parser.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/parsers/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/common.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/profile.py
+-rw-r--r--   0        0        0    10687 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/profile_store.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/__init__.py
+-rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dynamic_utils.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dc2ac/__init__.py
+-rw-r--r--   0        0        0    33318 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dc2ac/dc_ac_algorithm.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dc2ac/helper_functions.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/README.md
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/PKG-INFO
```

### Comparing `nrel_pypsse-1.1.1/pypsse/channel_map.py` & `nrel_pypsse-1.1.2/pypsse/channel_map.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/common.py` & `nrel_pypsse-1.1.2/pypsse/common.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/compile.bat` & `nrel_pypsse-1.1.2/pypsse/compile.bat`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/contingencies.py` & `nrel_pypsse-1.1.2/pypsse/contingencies.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/custom_logger.py` & `nrel_pypsse-1.1.2/pypsse/custom_logger.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/enumerations.py` & `nrel_pypsse-1.1.2/pypsse/enumerations.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,22 +62,22 @@
     "Support model properties"
     PU = "PU"
     FREQ = "FREQ"
     ANGLE = "ANGLE"
     ANGLED = "ANGLED"
 
 
-class LoggingLevels(IntEnum):
+class LoggingLevels(str, Enum):
     "logging level setting options"
-    NOTSET = 0
-    DEBUG = 10
-    INFO = 20
-    WARN = 30
-    ERROR = 40
-    CRITICAL = 50
+    NOTSET = "INFO"
+    DEBUG = "DEBUG"
+    INFO = "INFO"
+    WARNING = "WARNING"
+    ERROR = "ERROR"
+    CRITICAL = "CRITICAL"
 
 
 class SubscriptionFileRequiredColumns(str, Enum):
     "Subscription file requirements"
     bus_subsystem_id = "bus_subsystem_id"
     element_type = "element_type"
     element_id = "element_id"
```

### Comparing `nrel_pypsse-1.1.1/pypsse/helics_interface.py` & `nrel_pypsse-1.1.2/pypsse/helics_interface.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/mdao_interface.py` & `nrel_pypsse-1.1.2/pypsse/mdao_interface.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/models.py` & `nrel_pypsse-1.1.2/pypsse/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Dict, List, Literal, Optional, Union
+from typing import Dict, List, Literal, Optional, Union, Any
 
 import pandas as pd
 from pydantic import UUID4, BaseModel, Field, model_validator
 from pydantic.networks import IPvAnyAddress
 from typing_extensions import Annotated
 
 from pypsse.common import CASESTUDY_FOLDER, EXPORTS_FOLDER, LOGS_FOLDER
@@ -385,15 +385,15 @@
 
 class ExportFileOptions(ExportAssetTypes):
     "Export settings for a PyPSSE project"
 
     export_results_using_channels: bool = False
     filename_prefix :str = ""
     defined_subsystems_only: bool = True
-    file_format: ExportModes = "h5"
+    file_format: ExportModes = ExportModes.H5
     channels: Optional[List[str]] = None
     channel_setup: Optional[List[channel_types]] = None
 
 
 class ProjectDefination(BaseModel):
     "PyPSSE project defination"
     overwrite: bool = False
@@ -419,15 +419,15 @@
 class MdaoProblem(BaseModel):
     outputs: MdaoOutput
     inputs: List[MdaoInput]
 
 
 class ApiPsseReply(BaseModel):
     status: str
-    message: Union[Dict, str]
+    message: Optional[Any] = None
     uuid: Union[UUID4, None] = None
 
 
 class ApiPsseException(BaseModel):
     message: str
     uuid: Union[UUID4, None] = None
```

### Comparing `nrel_pypsse-1.1.1/pypsse/project.py` & `nrel_pypsse-1.1.2/pypsse/project.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/result_container.py` & `nrel_pypsse-1.1.2/pypsse/result_container.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/simulation_controller.py` & `nrel_pypsse-1.1.2/pypsse/simulation_controller.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/simulator.py` & `nrel_pypsse-1.1.2/pypsse/simulator.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/api/PSSE.v2.json` & `nrel_pypsse-1.1.2/pypsse/api/PSSE.v2.json`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/api/server.py` & `nrel_pypsse-1.1.2/pypsse/api/server.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/api/app/psse.py` & `nrel_pypsse-1.1.2/pypsse/api/app/psse.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/api/web/handler.py` & `nrel_pypsse-1.1.2/pypsse/api/web/handler.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/cli/create_profiles.py` & `nrel_pypsse-1.1.2/pypsse/cli/create_profiles.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/cli/create_project.py` & `nrel_pypsse-1.1.2/pypsse/cli/create_project.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/cli/explore.py` & `nrel_pypsse-1.1.2/pypsse/cli/explore.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 
 from loguru import logger
 import pandas as pd
 import click
+import toml
 
 from pypsse.common import EXPORTS_SETTINGS_FILENAME, SIMULATION_SETTINGS_FILENAME
 from pypsse.models import ExportFileOptions, SimulationSettings
 from pypsse.simulator import Simulator
 
 @click.argument(
     "project-path",
@@ -89,51 +90,71 @@
     
     export_file_path = Path(export_file_path)
     
     file_path = Path(project_path) / simulations_file
     msg = "Simulation file not found. Use -s to choose a valid settings file"
     "if its name differs from the default file name."
     assert file_path.exists(), msg
-    x = Simulator.from_setting_files(file_path)
+    
+    simulation_settings = toml.load(file_path)
+    simulation_settings = SimulationSettings(**simulation_settings)
+    simulation_settings.helics.cosimulation_mode = False
+    x = Simulator(simulation_settings)
     buses = set(x.raw_data.buses)
     quantities =  {
-        'Loads': ['MVA', 'FmA', 'FmB', 'FmC', 'FmD', 'Fel', 'PFel'], 
+        'Loads': ['MVA', "IL", "YL", 'FmA', 'FmB', 'FmC', 'FmD', 'Fel', 'PFel'], 
         'Induction_generators': ['MVA'], 
         'Machines': ['MVA', 'PERCENT'], 
         }
     results = x.sim.read_subsystems(quantities,  buses)
+
+    # print(results.keys())
+    print(results["LOAD_P"])
+    # quit()
+
     had_comp_models = False
     if "Loads_FmA" in results:
         had_comp_models = True
-        
+    
     load_dict = {}
     bus_load_real = {}
     bus_load_imag = {}
     is_comp_load = {}
     for bus, ld_id in x.raw_data.loads:
         if bus not in load_dict:
             load_dict[bus] = []
             bus_load_real[bus] = 0
             bus_load_imag[bus] = 0
-            is_comp_load = []
         
+        load_bus_id = f'{bus}_{ld_id}'
         if had_comp_models:
             is_comp = True if f'{bus}_{ld_id}' in results["Loads_FmA"] else False
         else:
             is_comp = False
-        is_comp_load.append(is_comp)    
+            
+        is_comp_load[bus] = is_comp
         load_dict[bus].append(ld_id)
         key = f"{ld_id} _{bus}" if len(ld_id) == 1 else f"{ld_id}_{bus}" 
-        bus_load_real[bus] += results["Loads_MVA"][key].real
-        bus_load_imag[bus] += results["Loads_MVA"][key].imag
+        key2 =  f"{bus}_{ld_id}".replace(" ", "") 
+        load_p  = max(
+            results["Loads_MVA"][key].real + results["Loads_IL"][key].real + results["Loads_YL"][key].real, 
+            results["LOAD_P"][key2] *100 if key2 in results["LOAD_P"] else 0
+            )
+        load_q  = max(
+            results["Loads_MVA"][key].imag + results["Loads_IL"][key].imag + results["Loads_YL"][key].imag, 
+            results["LOAD_Q"][key2] *100 if key2 in results["LOAD_Q"] else 0
+            )
+        
+        bus_load_real[bus] += load_p
+        bus_load_imag[bus] += load_q
         
     generator_dict = {}
     bus_gen = {}
     for bus, gen_id in x.raw_data.generators:
-        if bus not in load_dict:
+        if bus not in generator_dict:
             generator_dict[bus] = []
             bus_gen[bus] = 0
         key = f"{gen_id} _{bus}" if len(gen_id) == 1 else f"{gen_id}_{bus}" 
         generator_dict[bus].append(gen_id)
         bus_gen[bus] += results["Machines_MVA"][key]
 
     results = {
@@ -152,35 +173,42 @@
         results["total P load [MW]"].append(bus_load_real[bus] if bus in bus_load_real else 0)
         results["total Q load [MVar]"].append(bus_load_imag[bus] if bus in bus_load_imag else 0)
         results["has generation"].append(True if bus in generator_dict else False)
         results["total generation [MVA]"].append(bus_gen[bus] if bus in bus_gen else 0)
     
     
     results = pd.DataFrame(results)
-    if filter:
-        if load_filter and load:
+    
+    results["total P load [MW]"] = results["total P load [MW]"] 
+    results["total Q load [MVar]"] = results["total Q load [MVar]"]
+    
+    if load_filter:
+        if load:
             results=results[results["has load"] == True]
-        elif load_filter and not load:
+        elif not load:
             results=results[results["has load"] == False]
         
-        if gen_filter and generation:
-            results=results[results["has generation"] == True]
-        elif gen_filter and not generation:
-            results=results[results["has generation"] == False]    
-        
-        if load_filter and comp_load:
+        if comp_load:
             results=results[results["is load comp"] == True]
-        elif load_filter and not comp_load:
+        elif not comp_load:
             results=results[results["is load comp"] == False]
         
-        load_lower, load_upper = [float(x) for x in load_bounds.split("/")] 
-        gen_lower, gen_upper = [float(x) for x in gen_bounds.split("/")] 
-        if apply_bounds:
-            results=results[(results["total P load [MW]"] >= load_lower) & (results["total P load [MW]"] <= load_upper)]
-            results=results[(results["total generation [MVA]"] >= gen_lower) & (results["total generation [MVA]"] <= gen_upper)]
-            
+    if gen_filter:
+        if generation:
+            results=results[results["has generation"] == True]
+        elif not generation:
+            results=results[results["has generation"] == False]    
+    
+    load_lower, load_upper = [float(x) for x in load_bounds.split("/")] 
+    gen_lower, gen_upper = [float(x) for x in gen_bounds.split("/")] 
+    if apply_bounds:
+        results=results[(results["total P load [MW]"] >= load_lower) & (results["total P load [MW]"] <= load_upper)]
+        results=results[(results["total generation [MVA]"] >= gen_lower) & (results["total generation [MVA]"] <= gen_upper)]
+
+    print(results)    
     results.to_csv(export_file_path)
+    logger.info(f"Results exported to {export_file_path.absolute()}")
```

### Comparing `nrel_pypsse-1.1.1/pypsse/cli/pypsse.py` & `nrel_pypsse-1.1.2/pypsse/cli/pypsse.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/data_writers/csv.py` & `nrel_pypsse-1.1.2/pypsse/data_writers/csv.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/data_writers/data_writer.py` & `nrel_pypsse-1.1.2/pypsse/data_writers/data_writer.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/data_writers/hdf5.py` & `nrel_pypsse-1.1.2/pypsse/data_writers/hdf5.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/data_writers/json.py` & `nrel_pypsse-1.1.2/pypsse/data_writers/json.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/defaults/export_settings.toml` & `nrel_pypsse-1.1.2/pypsse/defaults/export_settings.toml`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/defaults/simulation_settings.toml` & `nrel_pypsse-1.1.2/pypsse/defaults/simulation_settings.toml`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/modes/abstract_mode.py` & `nrel_pypsse-1.1.2/pypsse/modes/abstract_mode.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/modes/constants.py` & `nrel_pypsse-1.1.2/pypsse/modes/constants.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/modes/dynamic.py` & `nrel_pypsse-1.1.2/pypsse/modes/dynamic.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/modes/pcm.py` & `nrel_pypsse-1.1.2/pypsse/modes/pcm.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/modes/snap.py` & `nrel_pypsse-1.1.2/pypsse/modes/snap.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/modes/static.py` & `nrel_pypsse-1.1.2/pypsse/modes/static.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/parsers/gic_parser.py` & `nrel_pypsse-1.1.2/pypsse/parsers/gic_parser.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/parsers/reader.py` & `nrel_pypsse-1.1.2/pypsse/parsers/reader.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/profile_manager/common.py` & `nrel_pypsse-1.1.2/pypsse/profile_manager/common.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/profile_manager/profile.py` & `nrel_pypsse-1.1.2/pypsse/profile_manager/profile.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/profile_manager/profile_store.py` & `nrel_pypsse-1.1.2/pypsse/profile_manager/profile_store.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/utils/dynamic_utils.py` & `nrel_pypsse-1.1.2/pypsse/utils/dynamic_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/utils/utils.py` & `nrel_pypsse-1.1.2/pypsse/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/utils/dc2ac/dc_ac_algorithm.py` & `nrel_pypsse-1.1.2/pypsse/utils/dc2ac/dc_ac_algorithm.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pypsse/utils/dc2ac/helper_functions.py` & `nrel_pypsse-1.1.2/pypsse/utils/dc2ac/helper_functions.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/.gitignore` & `nrel_pypsse-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/LICENSE` & `nrel_pypsse-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/README.md` & `nrel_pypsse-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.1/pyproject.toml` & `nrel_pypsse-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     "pydantic~=2.4",
     "PyYAML",
     "requests",
     "terminaltables",
     "toml",
     "xlrd",
     "loguru",
-    # "powersystem-data-models"
 ]
 
 [project.scripts]
 pypsse = "pypsse.cli.pypsse:cli"
 
 [project.urls]
 Homepage = "http://www.github.com/nrel/pypsse"
```

### Comparing `nrel_pypsse-1.1.1/PKG-INFO` & `nrel_pypsse-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-pypsse
-Version: 1.1.1
+Version: 1.1.2
 Summary: A high-level python interface for PSS/E
 Project-URL: Homepage, http://www.github.com/nrel/pypsse
 Author-email: Aadil Latif <Aadil.Latif@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

