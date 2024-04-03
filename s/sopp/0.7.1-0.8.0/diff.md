# Comparing `tmp/sopp-0.7.1.tar.gz` & `tmp/sopp-0.8.0.tar.gz`

## Comparing `sopp-0.7.1.tar` & `sopp-0.8.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/generate_tardys3.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/sopp.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/tardys4_generator.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/utilities.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/window_finder.py
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/builder/configuration_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/config_file_loader/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/config_file_loader/config_file_loader_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/config_file_loader/support/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/config_file_loader/support/config_file_loader_base.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/config_file_loader/support/config_file_loader_json.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/config_file_loader/support/utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/configuration.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/configuration_file.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/coordinates.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/facility.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/observation_target.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/overhead_window.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/position.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/position_time.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/reservation.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/runtime_settings.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/time_window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/frequency_range/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/frequency_range/frequency_range.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/frequency_range/support/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/satellite/__init__.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/satellite/international_designator.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/satellite/mean_motion.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/satellite/satellite.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/custom_dataclasses/satellite/tle_information.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/__init__.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/__init__.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/__init__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/support/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/event_finder/support/overhead_window_from_events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/path_finder/__init__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/path_finder/observation_path_finder.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/path_finder/observation_path_finder_rhodesmill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/retriever.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/retriever_json_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/satellite_retriever/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/satellite_retriever/satellite_retriever.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/satellite_retriever/satellite_retriever_json_file.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/retrievers/satellite_retriever/skyfield_satellite_retriever.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/satellites_filter/__init__.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/satellites_filter/filterer.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/satellites_filter/filters.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/satellites_loader/satellites_loader.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/satellites_loader/satellites_loader_from_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/tle_fetcher/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/tle_fetcher/tle_fetcher_base.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/tle_fetcher/tle_fetcher_celestrak.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 sopp-0.7.1/sopp/tle_fetcher/tle_fetcher_spacetrack.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sopp-0.7.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 sopp-0.7.1/COPYING
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sopp-0.7.1/hatch.toml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 sopp-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    16572 2020-02-02 00:00:00.000000 sopp-0.7.1/quickstart.md
--rw-r--r--   0        0        0    17469 2020-02-02 00:00:00.000000 sopp-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/generate_tardys3.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/sopp.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tardys4_generator.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/utilities.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/window_finder.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/builder/configuration_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/config_file_loader_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/config_file_loader_base.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/config_file_loader_json.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/utilities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/configuration.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/configuration_file.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/coordinates.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/facility.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/observation_target.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/overhead_window.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/position.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/position_time.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/reservation.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/runtime_settings.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/time_window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/frequency_range.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/support/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/__init__.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/international_designator.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/mean_motion.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/satellite.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/tle_information.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/__init__.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/support/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/support/overhead_window_from_events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/path_finder/__init__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/path_finder/observation_path_finder.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/path_finder/observation_path_finder_rhodesmill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/retriever.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/retriever_json_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/satellite_retriever.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/satellite_retriever_json_file.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/skyfield_satellite_retriever.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_filter/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_filter/filterer.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_filter/filters.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_loader/satellites_loader.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_loader/satellites_loader_from_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_base.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_celestrak.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_spacetrack.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sopp-0.8.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 sopp-0.8.0/COPYING
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 sopp-0.8.0/hatch.toml
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 sopp-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 sopp-0.8.0/quickstart.md
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 sopp-0.8.0/PKG-INFO
```

### Comparing `sopp-0.7.1/sopp/generate_tardys3.py` & `sopp-0.8.0/sopp/generate_tardys3.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/sopp.py` & `sopp-0.8.0/sopp/sopp.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/tardys4_generator.py` & `sopp-0.8.0/sopp/tardys4_generator.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/utilities.py` & `sopp-0.8.0/sopp/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import os
 from contextlib import contextmanager
-from datetime import datetime
+from datetime import datetime, timezone
 from io import TextIOWrapper
 from pathlib import Path
 from typing import ContextManager, List, Optional, Union
 from uuid import uuid4
 
-import pytz
 from dateutil import parser
 
 
 def read_json_file(filepath: Path) -> dict:
     with open(filepath, 'r') as f:
         return json.load(f)
 
@@ -21,20 +20,20 @@
     filepath = Path(filepath or f'{uuid4().hex}.tmp')
     with open(filepath, 'w') as f:
         yield f
     filepath.unlink(missing_ok=True)
 
 
 def convert_datetime_to_utc(localtime: datetime) -> datetime:
-    if localtime.tzinfo == pytz.UTC:
+    if localtime.tzinfo == timezone.utc:
         return localtime
     elif localtime.tzinfo is None:
-        return localtime.replace(tzinfo=pytz.UTC)
+        return localtime.replace(tzinfo=timezone.utc)
     else:
-        return localtime.astimezone(pytz.UTC)
+        return localtime.astimezone(timezone.utc)
 
 
 def read_datetime_string_as_utc(string_value: str) -> datetime:
     try:
         time = parser.parse(string_value)
         return convert_datetime_to_utc(time)
     except ValueError:
```

### Comparing `sopp-0.7.1/sopp/window_finder.py` & `sopp-0.8.0/sopp/window_finder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/builder/configuration_builder.py` & `sopp-0.8.0/sopp/builder/configuration_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         return self
 
     def add_filter(self, filter_fn: Callable[[Satellite, Any], bool]):
         self._filterer.add_filter(filter_fn)
         return self
 
     def _filter_satellites(self):
-        self.satellites = self._filterer.apply_filters(self.satellites, self)
+        self.satellites = self._filterer.apply_filters(self.satellites)
 
     def _build_reservation(self):
         self.reservation = Reservation(
             facility=self.facility,
             time=self.time_window,
             frequency=self.frequency_range
         )
```

### Comparing `sopp-0.7.1/sopp/config_file_loader/config_file_loader_factory.py` & `sopp-0.8.0/sopp/config_file_loader/config_file_loader_factory.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/config_file_loader/support/config_file_loader_json.py` & `sopp-0.8.0/sopp/config_file_loader/support/config_file_loader_json.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/configuration.py` & `sopp-0.8.0/sopp/custom_dataclasses/configuration.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/configuration_file.py` & `sopp-0.8.0/sopp/custom_dataclasses/configuration_file.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/facility.py` & `sopp-0.8.0/sopp/custom_dataclasses/facility.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/overhead_window.py` & `sopp-0.8.0/sopp/custom_dataclasses/overhead_window.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/position.py` & `sopp-0.8.0/sopp/custom_dataclasses/position.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/reservation.py` & `sopp-0.8.0/sopp/custom_dataclasses/reservation.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/runtime_settings.py` & `sopp-0.8.0/sopp/custom_dataclasses/runtime_settings.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/time_window.py` & `sopp-0.8.0/sopp/custom_dataclasses/time_window.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/frequency_range/frequency_range.py` & `sopp-0.8.0/sopp/custom_dataclasses/frequency_range/frequency_range.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py` & `sopp-0.8.0/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/satellite/international_designator.py` & `sopp-0.8.0/sopp/custom_dataclasses/satellite/international_designator.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/satellite/satellite.py` & `sopp-0.8.0/sopp/custom_dataclasses/satellite/satellite.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/custom_dataclasses/satellite/tle_information.py` & `sopp-0.8.0/sopp/custom_dataclasses/satellite/tle_information.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/event_finder.py` & `sopp-0.8.0/sopp/event_finder/event_finder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py` & `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py` & `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py` & `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py` & `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py` & `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/event_finder/support/overhead_window_from_events.py` & `sopp-0.8.0/sopp/event_finder/support/overhead_window_from_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List
-import pytz
 from sopp.custom_dataclasses.overhead_window import OverheadWindow
 from sopp.custom_dataclasses.reservation import Reservation
 from sopp.custom_dataclasses.satellite.satellite import Satellite
 from sopp.custom_dataclasses.time_window import TimeWindow
 
 
 class EventTypesRhodesmill(Enum):
```

### Comparing `sopp-0.7.1/sopp/path_finder/observation_path_finder.py` & `sopp-0.8.0/sopp/path_finder/observation_path_finder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/path_finder/observation_path_finder_rhodesmill.py` & `sopp-0.8.0/sopp/path_finder/observation_path_finder_rhodesmill.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/satellites_filter/filterer.py` & `sopp-0.8.0/sopp/satellites_filter/filterer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,9 +34,9 @@
         self._filters: List[T] = []
 
     def add_filter(self, filter_lambda: Callable[[T], bool]):
         if filter_lambda:
             self._filters.append(filter_lambda)
         return self
 
-    def apply_filters(self, elements: List[T], context: Optional[Any] = None):
-        return [element for element in elements if all(f(element, context) for f in self._filters)]
+    def apply_filters(self, elements: List[T]):
+        return [element for element in elements if all(f(element) for f in self._filters)]
```

### Comparing `sopp-0.7.1/sopp/satellites_filter/filters.py` & `sopp-0.8.0/sopp/satellites_filter/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable, Optional, Any
+import re
 
 from sopp.custom_dataclasses.frequency_range.frequency_range import FrequencyRange
 from sopp.custom_dataclasses.satellite.satellite import Satellite
 
 
-def filter_frequency(observation_frequency: Optional[FrequencyRange] = None) -> Callable[[Satellite, Any], bool]:
+def filter_frequency(observation_frequency: FrequencyRange) -> Callable[[Satellite], bool]:
     """
     filter_frequency returns True if a satellite's downlink transmission frequency
     overlaps with the desired observation frequency. If there is no information
     on the satellite frequency, it will return True to err on the side of caution
     for potential interference.
 
     Parameters:
@@ -30,76 +31,93 @@
                 )
             )
         else:
             return True
 
     return filter_function
 
+def filter_name_regex(regex: str) -> Callable[[Satellite], bool]:
+    """
+    filter_name_contains returns a lambda function that checks if a given regex
+    is present in the name of a Satellite.
+
+    Parameters:
+    - regex: The regex to check for in the satellite names.
+
+    Returns:
+    - A lambda function that takes a Satellite object and returns True if the name
+      matches the specified regex, False otherwise.
+    """
+    def filter_function(satellite: Satellite) -> bool:
+        return not regex or bool(re.search(regex, satellite.name))
+
+    return filter_function
+
 def filter_name_contains(substring: str) -> Callable[[Satellite], bool]:
     """
     filter_name_contains returns a lambda function that checks if a given substring
     is present in the name of a Satellite.
 
     Parameters:
     - substring: The substring to check for in the satellite names.
 
     Returns:
     - A lambda function that takes a Satellite object and returns True if the name
       contains the specified substring, False otherwise.
     """
-    def filter_function(satellite: Satellite, ctx: Optional[Any] = None) -> bool:
+    def filter_function(satellite: Satellite) -> bool:
         return not substring or substring in satellite.name
 
     return filter_function
 
-def filter_name_does_not_contain(substring: str) -> Callable[[Satellite, Any], bool]:
+def filter_name_does_not_contain(substring: str) -> Callable[[Satellite], bool]:
     """
     filter_name_does_not_contain returns a lambda function that checks if a given substring
     is not present in the name of a Satellite.
 
     Parameters:
     - substring: The substring to check for absence in the satellite names.
 
     Returns:
     - A lambda function that takes a Satellite object and returns True if the name
       does not contain the specified substring, False otherwise.
     """
-    def filter_function(satellite: Satellite, ctx: Optional[Any] = None) -> bool:
+    def filter_function(satellite: Satellite) -> bool:
         return not substring or not filter_name_contains(substring)(satellite)
 
     return filter_function
 
-def filter_name_is(substring: str) -> Callable[[Satellite, Any], bool]:
+def filter_name_is(substring: str) -> Callable[[Satellite], bool]:
     """
     filter_name_is returns a lambda function that checks if a given substring
     matches exactly the name of a Satellite.
 
     Parameters:
     - substring: The substring to match exactly in the satellite names.
 
     Returns:
     - A lambda function that takes a Satellite object and returns True if the name
       matches the specified substring exactly, False otherwise.
     """
-    def filter_function(satellite: Satellite, ctx: Optional[Any] = None) -> bool:
+    def filter_function(satellite: Satellite) -> bool:
         return not substring or substring == satellite.name
 
     return filter_function
 
-def filter_orbit_is(orbit_type: str) -> Callable[[Satellite, Any], bool]:
+def filter_orbit_is(orbit_type: str) -> Callable[[Satellite], bool]:
     """
     filter_orbit_type returns a lambda function to filter satellites based on their orbital type.
 
     Parameters:
     - orbit_type (str): The type of orbit ('leo', 'meo', or 'geo').
 
     Returns:
     - A lambda function that takes a Satellite object and returns True if it is in the specified orbit type, False otherwise.
     """
-    def filter_function(satellite: Satellite, ctx: Optional[Any] = None) -> bool:
+    def filter_function(satellite: Satellite) -> bool:
         if orbit_type == 'leo':
             return satellite.orbits_per_day >= 5.0
         elif orbit_type == 'meo':
             return satellite.orbits_per_day >= 1.5 and satellite.orbits_per_day < 5.0
         elif orbit_type == 'geo':
             return satellite.orbits_per_day >= 0.85 and satellite.orbits_per_day < 1.5
         elif not orbit_type:
```

### Comparing `sopp-0.7.1/sopp/satellites_loader/satellites_loader_from_files.py` & `sopp-0.8.0/sopp/satellites_loader/satellites_loader_from_files.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/tle_fetcher/tle_fetcher_base.py` & `sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_base.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/sopp/tle_fetcher/tle_fetcher_spacetrack.py` & `sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_spacetrack.py`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/COPYING` & `sopp-0.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopp-0.7.1/pyproject.toml` & `sopp-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [project]
 name = "sopp"
 dynamic = ["version"]
 dependencies = [
-    "pytz~=2022.7",
     "sgp4~=2.21",
     "skyfield~=1.47",
     "requests~=2.31.0",
     "python-dateutil~=2.8.2",
     "python-dotenv~=0.21.0",
 ]
 requires-python = ">=3.8"
```

### Comparing `sopp-0.7.1/quickstart.md` & `sopp-0.8.0/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 ```
 
 #### `add_filter()`
 
 Alternatively to constructing a `Filterer` object you can simply call `add_filter()`
 
 ```python
-configuration.add_filter(filter_frequency())
+configuration.add_filter(filter_frequency(FrequencyRange(10, 10)))
 ```
 
 #### `set_runtime_settings()`
 
 The `set_runtime_settings()` method:
 - Specifies the time resolution for calculating satellite positions in seconds via the `time_continuity_resolution` parameter.
 - Specifies the `concurrency_level` parameter determines the number of parallel jobs during satellite position calculation, optimizing runtime speeds. This value should be not exceed the number of cores on the machine.
@@ -276,25 +276,37 @@
 ```
 The `Satellite` class, containins details about the satellite and a list of PositionTime objects. The `PositionTime` dataclass specifies the satellite's position in altitude, azimuth and distance in km at a discrete point in time. All times are in UTC.
 
 ### Filtering Satellites
 
 The list of satellites can be filtered by using a `Filterer` object, adding filters to it and then passing the `Filterer` object to a `ConfigurationBuilder`. The user can define any filtering logic wanted, however a few built in filters are provided. If the filtering condition evaluates to `True` the Satellite will be included in the final list.
 If `None` is passed to any of the filters, no filtering for that specific filter will be applied.
-Alternatively to passing a `Filterer` object to the `ConfigurationBuilder` via `set_satellites_filter`, filters can simply be added with `add_filter(filter_frequency())`.
+Alternatively to passing a `Filterer` object to the `ConfigurationBuilder` via `set_satellites_filter`, filters can simply be added with `add_filter(filter_name_contains('STARLINK'))`.
 
 The provided filters accessible from `sopp.satellites_filter.filters` include:
 
 #### `filter_frequency()`:
 
+Parameters:
+    - observation_frequency (FrequencyRange): The observation frequency range.
+
 returns `True` if a satellite's downlink transmission frequency
 overlaps with the desired observation frequency. If there is no information
 on the satellite frequency, it will return True to err on the side of caution
-for potential interference. Accepts a `FrequencyRange` object, if none is provided it will
-default to the `Reservation` frequency, if available.
+for potential interference. Requires a `FrequencyRange` object.
+
+#### `filter_name_regex()`:
+
+Parameters:
+    - regex (str): The regex to match for in the satellite names.
+
+returns `True` if a given regex matches in the name of a Satellite.
+
+Example: filter_name_regex('YAM|ZARYA') will return a list of satellites that
+contain YAM or ZARYA within their name.
 
 #### `filter_name_contains()`:
 
 Parameters:
     - substring (str): The substring to check for in the satellite names.
 
 returns `True` if a given substring is present in the name of a Satellite.
```

### Comparing `sopp-0.7.1/PKG-INFO` & `sopp-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sopp
-Version: 0.7.1
+Version: 0.8.0
 Summary: SOPP is an open-source tool for calculating satellite interference to radio astronomy observations.
 Project-URL: Repository, https://github.com/NSF-Swift/satellite-overhead
 Project-URL: Bug Tracker, https://github.com/NSF-Swift/satellite-overhead/issues
 License-Expression: AGPL-3.0-or-later
 License-File: COPYING
 Keywords: astronomy,satellites
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Requires-Dist: python-dateutil~=2.8.2
 Requires-Dist: python-dotenv~=0.21.0
-Requires-Dist: pytz~=2022.7
 Requires-Dist: requests~=2.31.0
 Requires-Dist: sgp4~=2.21
 Requires-Dist: skyfield~=1.47
 Description-Content-Type: text/markdown
 
 # S.O.P.P. - Satellite Orbit Prediction Processor
 
@@ -194,15 +193,15 @@
 ```
 
 #### `add_filter()`
 
 Alternatively to constructing a `Filterer` object you can simply call `add_filter()`
 
 ```python
-configuration.add_filter(filter_frequency())
+configuration.add_filter(filter_frequency(FrequencyRange(10, 10)))
 ```
 
 #### `set_runtime_settings()`
 
 The `set_runtime_settings()` method:
 - Specifies the time resolution for calculating satellite positions in seconds via the `time_continuity_resolution` parameter.
 - Specifies the `concurrency_level` parameter determines the number of parallel jobs during satellite position calculation, optimizing runtime speeds. This value should be not exceed the number of cores on the machine.
@@ -298,25 +297,37 @@
 ```
 The `Satellite` class, containins details about the satellite and a list of PositionTime objects. The `PositionTime` dataclass specifies the satellite's position in altitude, azimuth and distance in km at a discrete point in time. All times are in UTC.
 
 ### Filtering Satellites
 
 The list of satellites can be filtered by using a `Filterer` object, adding filters to it and then passing the `Filterer` object to a `ConfigurationBuilder`. The user can define any filtering logic wanted, however a few built in filters are provided. If the filtering condition evaluates to `True` the Satellite will be included in the final list.
 If `None` is passed to any of the filters, no filtering for that specific filter will be applied.
-Alternatively to passing a `Filterer` object to the `ConfigurationBuilder` via `set_satellites_filter`, filters can simply be added with `add_filter(filter_frequency())`.
+Alternatively to passing a `Filterer` object to the `ConfigurationBuilder` via `set_satellites_filter`, filters can simply be added with `add_filter(filter_name_contains('STARLINK'))`.
 
 The provided filters accessible from `sopp.satellites_filter.filters` include:
 
 #### `filter_frequency()`:
 
+Parameters:
+    - observation_frequency (FrequencyRange): The observation frequency range.
+
 returns `True` if a satellite's downlink transmission frequency
 overlaps with the desired observation frequency. If there is no information
 on the satellite frequency, it will return True to err on the side of caution
-for potential interference. Accepts a `FrequencyRange` object, if none is provided it will
-default to the `Reservation` frequency, if available.
+for potential interference. Requires a `FrequencyRange` object.
+
+#### `filter_name_regex()`:
+
+Parameters:
+    - regex (str): The regex to match for in the satellite names.
+
+returns `True` if a given regex matches in the name of a Satellite.
+
+Example: filter_name_regex('YAM|ZARYA') will return a list of satellites that
+contain YAM or ZARYA within their name.
 
 #### `filter_name_contains()`:
 
 Parameters:
     - substring (str): The substring to check for in the satellite names.
 
 returns `True` if a given substring is present in the name of a Satellite.
```

