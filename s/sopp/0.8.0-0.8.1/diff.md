# Comparing `tmp/sopp-0.8.0.tar.gz` & `tmp/sopp-0.8.1.tar.gz`

## Comparing `sopp-0.8.0.tar` & `sopp-0.8.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/generate_tardys3.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/sopp.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tardys4_generator.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/utilities.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/window_finder.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/builder/configuration_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/config_file_loader_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/config_file_loader_base.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/config_file_loader_json.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/config_file_loader/support/utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/configuration.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/configuration_file.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/coordinates.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/facility.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/observation_target.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/overhead_window.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/position.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/position_time.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/reservation.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/runtime_settings.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/time_window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/frequency_range.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/support/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/__init__.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/international_designator.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/mean_motion.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/satellite.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/custom_dataclasses/satellite/tle_information.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/__init__.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/__init__.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/__init__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/support/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/event_finder/support/overhead_window_from_events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/path_finder/__init__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/path_finder/observation_path_finder.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/path_finder/observation_path_finder_rhodesmill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/retriever.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/retriever_json_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/satellite_retriever.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/satellite_retriever_json_file.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/retrievers/satellite_retriever/skyfield_satellite_retriever.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_filter/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_filter/filterer.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_filter/filters.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_loader/satellites_loader.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/satellites_loader/satellites_loader_from_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_base.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_celestrak.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_spacetrack.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sopp-0.8.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 sopp-0.8.0/COPYING
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 sopp-0.8.0/hatch.toml
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 sopp-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 sopp-0.8.0/quickstart.md
--rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 sopp-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/generate_tardys3.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/sopp.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/tardys4_generator.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/utilities.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/window_finder.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/builder/configuration_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/config_file_loader/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/config_file_loader/config_file_loader_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/config_file_loader/support/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/config_file_loader/support/config_file_loader_base.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/config_file_loader/support/config_file_loader_json.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/config_file_loader/support/utilities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/configuration.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/configuration_file.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/coordinates.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/facility.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/observation_target.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/overhead_window.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/position.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/position_time.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/reservation.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/runtime_settings.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/time_window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/frequency_range/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/frequency_range/frequency_range.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/frequency_range/support/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/satellite/__init__.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/satellite/international_designator.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/satellite/mean_motion.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/satellite/satellite.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/custom_dataclasses/satellite/tle_information.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/__init__.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/support/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/event_finder/support/overhead_window_from_events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/path_finder/__init__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/path_finder/observation_path_finder.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/path_finder/observation_path_finder_rhodesmill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/retriever.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/retriever_json_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/satellite_retriever/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/satellite_retriever/satellite_retriever.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/satellite_retriever/satellite_retriever_json_file.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/retrievers/satellite_retriever/skyfield_satellite_retriever.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/satellites_filter/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/satellites_filter/filterer.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/satellites_filter/filters.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/satellites_loader/satellites_loader.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/satellites_loader/satellites_loader_from_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/tle_fetcher/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/tle_fetcher/tle_fetcher_base.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/tle_fetcher/tle_fetcher_celestrak.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 sopp-0.8.1/sopp/tle_fetcher/tle_fetcher_spacetrack.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sopp-0.8.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 sopp-0.8.1/COPYING
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 sopp-0.8.1/hatch.toml
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 sopp-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 sopp-0.8.1/quickstart.md
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 sopp-0.8.1/PKG-INFO
```

### Comparing `sopp-0.8.0/sopp/generate_tardys3.py` & `sopp-0.8.1/sopp/generate_tardys3.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/tardys4_generator.py` & `sopp-0.8.1/sopp/tardys4_generator.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/utilities.py` & `sopp-0.8.1/sopp/utilities.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/window_finder.py` & `sopp-0.8.1/sopp/window_finder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/builder/configuration_builder.py` & `sopp-0.8.1/sopp/builder/configuration_builder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/config_file_loader/config_file_loader_factory.py` & `sopp-0.8.1/sopp/config_file_loader/config_file_loader_factory.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/config_file_loader/support/config_file_loader_json.py` & `sopp-0.8.1/sopp/config_file_loader/support/config_file_loader_json.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/configuration.py` & `sopp-0.8.1/sopp/custom_dataclasses/configuration.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/configuration_file.py` & `sopp-0.8.1/sopp/custom_dataclasses/configuration_file.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/facility.py` & `sopp-0.8.1/sopp/custom_dataclasses/facility.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/overhead_window.py` & `sopp-0.8.1/sopp/custom_dataclasses/overhead_window.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/position.py` & `sopp-0.8.1/sopp/custom_dataclasses/position.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/reservation.py` & `sopp-0.8.1/sopp/custom_dataclasses/reservation.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/runtime_settings.py` & `sopp-0.8.1/sopp/custom_dataclasses/runtime_settings.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/time_window.py` & `sopp-0.8.1/sopp/custom_dataclasses/time_window.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/frequency_range/frequency_range.py` & `sopp-0.8.1/sopp/custom_dataclasses/frequency_range/frequency_range.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py` & `sopp-0.8.1/sopp/custom_dataclasses/frequency_range/support/get_frequency_data_from_csv.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/satellite/international_designator.py` & `sopp-0.8.1/sopp/custom_dataclasses/satellite/international_designator.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/satellite/satellite.py` & `sopp-0.8.1/sopp/custom_dataclasses/satellite/satellite.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/custom_dataclasses/satellite/tle_information.py` & `sopp-0.8.1/sopp/custom_dataclasses/satellite/tle_information.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/event_finder.py` & `sopp-0.8.1/sopp/event_finder/event_finder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py` & `sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/event_finder_rhodesmill.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py` & `sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/evenly_spaced_time_intervals_calculator.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py` & `sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellites_interference_filter.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py` & `sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py` & `sopp-0.8.1/sopp/event_finder/event_finder_rhodesmill/support/satellite_positions_with_respect_to_facility_retriever/satellite_positions_with_respect_to_facility_retriever_rhodesmill.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/event_finder/support/overhead_window_from_events.py` & `sopp-0.8.1/sopp/event_finder/support/overhead_window_from_events.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/path_finder/observation_path_finder.py` & `sopp-0.8.1/sopp/path_finder/observation_path_finder.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/path_finder/observation_path_finder_rhodesmill.py` & `sopp-0.8.1/sopp/path_finder/observation_path_finder_rhodesmill.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/satellites_filter/filterer.py` & `sopp-0.8.1/sopp/satellites_filter/filterer.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/satellites_filter/filters.py` & `sopp-0.8.1/sopp/satellites_filter/filters.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/satellites_loader/satellites_loader_from_files.py` & `sopp-0.8.1/sopp/satellites_loader/satellites_loader_from_files.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_base.py` & `sopp-0.8.1/sopp/tle_fetcher/tle_fetcher_base.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/sopp/tle_fetcher/tle_fetcher_spacetrack.py` & `sopp-0.8.1/sopp/tle_fetcher/tle_fetcher_spacetrack.py`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/COPYING` & `sopp-0.8.1/COPYING`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/pyproject.toml` & `sopp-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/quickstart.md` & `sopp-0.8.1/quickstart.md`

 * *Files identical despite different names*

### Comparing `sopp-0.8.0/PKG-INFO` & `sopp-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sopp
-Version: 0.8.0
+Version: 0.8.1
 Summary: SOPP is an open-source tool for calculating satellite interference to radio astronomy observations.
 Project-URL: Repository, https://github.com/NSF-Swift/satellite-overhead
 Project-URL: Bug Tracker, https://github.com/NSF-Swift/satellite-overhead/issues
 License-Expression: AGPL-3.0-or-later
 License-File: COPYING
 Keywords: astronomy,satellites
 Classifier: Development Status :: 3 - Alpha
```

