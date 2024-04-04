# Comparing `tmp/threedi-schema-0.219.2.dev1.tar.gz` & `tmp/threedi-schema-0.220.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.219.2.dev1.tar", last modified: Mon Feb 26 14:41:28 2024, max compression
+gzip compressed data, was "threedi-schema-0.220.tar", last modified: Thu Feb 29 10:10:56 2024, max compression
```

## Comparing `threedi-schema-0.219.2.dev1.tar` & `threedi-schema-0.220.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.452255 threedi-schema-0.219.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-02-26 14:41:28.448255 threedi-schema-0.219.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 14:41:28.452255 threedi-schema-0.219.2.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.440255 threedi-schema-0.219.2.dev1/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.440255 threedi-schema-0.219.2.dev1/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.444255 threedi-schema-0.219.2.dev1/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.444255 threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.444255 threedi-schema-0.219.2.dev1/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.448255 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.448255 threedi-schema-0.219.2.dev1/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.448255 threedi-schema-0.219.2.dev1/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/test_beta_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-26 14:41:20.000000 threedi-schema-0.219.2.dev1/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:41:28.448255 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-02-26 14:41:28.000000 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-26 14:41:28.000000 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:41:28.000000 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-26 14:41:28.000000 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-26 14:41:28.000000 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-26 14:41:28.000000 threedi-schema-0.219.2.dev1/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-02-29 10:10:48.000000 threedi-schema-0.220/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-29 10:10:48.000000 threedi-schema-0.220/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-29 10:10:48.000000 threedi-schema-0.220/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-29 10:10:56.535987 threedi-schema-0.220/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-29 10:10:48.000000 threedi-schema-0.220/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-29 10:10:48.000000 threedi-schema-0.220/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 10:10:56.535987 threedi-schema-0.220/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.523987 threedi-schema-0.220/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.531987 threedi-schema-0.220/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_beta_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.219.2.dev1/CHANGES.rst` & `threedi-schema-0.220/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Changelog of threedi-schema
 ===================================================
 
-0.220 (unreleased)
---------------------
+0.220 (2024-02-29)
+------------------
 - Add support for geopackage
 - Remove `the_geom_linestring` from `v2_connection_nodes` because geopackage does not support multiple geometry objects in one table
 
 
 0.219.1 (2024-01-30)
 --------------------
```

### Comparing `threedi-schema-0.219.2.dev1/LICENSE` & `threedi-schema-0.220/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/PKG-INFO` & `threedi-schema-0.220/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.219.2.dev1
+Version: 0.220
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -85,16 +85,16 @@
 Install with::
 
   $ pip install threedi-schema
 
 Changelog of threedi-schema
 ===================================================
 
-0.220 (unreleased)
---------------------
+0.220 (2024-02-29)
+------------------
 - Add support for geopackage
 - Remove `the_geom_linestring` from `v2_connection_nodes` because geopackage does not support multiple geometry objects in one table
 
 
 0.219.1 (2024-01-30)
 --------------------
```

### Comparing `threedi-schema-0.219.2.dev1/README.rst` & `threedi-schema-0.220/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/pyproject.toml` & `threedi-schema-0.220/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/application/schema.py` & `threedi-schema-0.220/threedi_schema/application/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import subprocess
 import warnings
+from pathlib import Path
 
 # This import is needed for alembic to recognize the geopackage dialect
 import geoalchemy2.alembic_helpers  # noqa: F401
 from alembic import command as alembic_command
 from alembic.config import Config
 from alembic.environment import EnvironmentContext
 from alembic.migration import MigrationContext
@@ -264,46 +265,51 @@
                 session.execute(text("DROP TABLE IF EXISTS spatialite_history;"))
                 session.execute(text("DROP TABLE IF EXISTS views_geometry_columns;"))
             cmd = [
                 "ogr2ogr",
                 "-skipfailures",
                 "-f",
                 "gpkg",
-                str(self.db.path.with_suffix(".gpkg")),
+                str(Path(self.db.path).with_suffix(".gpkg")),
                 str(work_db.path),
                 "-oo",
                 "LIST_ALL_TABLES=YES",
             ]
             try:
                 p = subprocess.Popen(
                     cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, bufsize=-1
                 )
             except Exception as e:
                 raise UpgradeFailedError(f"ogr2ogr failed conversion:\n{e}")
-            _, err = p.communicate()
+            _, out = p.communicate()
         # Error handling
-        err_list = err.decode("ascii").split("\n")
+        # convert bytes to utf and split lines
+        out_list = out.decode("utf-8").split("\n")
         # collect only errors and remove 'ERROR #:'
         errors = [
-            ": ".join(item.split(": ")[1:])
-            for item in err_list
+            [idx, ": ".join(item.split(": ")[1:])]
+            for idx, item in enumerate(out_list)
             if item.lower().startswith("error")
         ]
         # While creating the geopackage with ogr2ogr an error occurs
         # because ogr2ogr tries to create a table `sqlite_sequence`, which
         # is reserved for internal use. The resulting database seems fine,
         # so this specific error is ignored
         # convert error output to list
         expected_error = 'sqlite3_exec(CREATE TABLE "sqlite_sequence" ( "rowid" INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL, "name" TEXT, "seq" TEXT)) failed: object name reserved for internal use: sqlite_sequence'
-        if (len(errors) != 1) or errors[0] != expected_error:
-            raise UpgradeFailedError(
-                f"ogr2ogr didn't finish as expected:\n{err.decode('ascii')}"
+        unexpected_error_indices = [
+            idx for idx, error in errors if error.lower() != expected_error.lower()
+        ]
+        if len(unexpected_error_indices) > 0:
+            error_str = "\n".join(
+                [out_list[idx].decode("utf-8") for idx in unexpected_error_indices]
             )
+            raise UpgradeFailedError(f"ogr2ogr didn't finish as expected:\n{error_str}")
         # Correct path of current database
-        self.db.path = self.db.path.with_suffix(".gpkg")
+        self.db.path = Path(self.db.path).with_suffix(".gpkg")
         # Reset engine so new path is used on the next call of get_engine()
         self.db._engine = None
         # Recreate views_geometry_columns so set_views works as expected
         with self.db.get_session() as session:
             session.execute(
                 text(
                     "CREATE TABLE views_geometry_columns(view_name TEXT, view_geometry TEXT, view_rowid TEXT, f_table_name VARCHAR(256), f_geometry_column VARCHAR(256))"
```

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/application/threedi_database.py` & `threedi-schema-0.220/threedi_schema/application/threedi_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,16 @@
     cursor.execute("PRAGMA cell_size_check=ON")
     cursor.execute("PRAGMA mmap_size=0")
     cursor.close()
 
 
 class ThreediDatabase:
     def __init__(self, path, echo=False):
-        self._path = path
+        self.path = path
         self.echo = echo
-
         self._engine = None
         self._base_metadata = None
 
     @property
     def schema(self):
         return ModelSchema(self)
 
@@ -55,52 +54,36 @@
     def engine(self):
         return self.get_engine()
 
     @property
     def base_path(self):
         return Path(self.path).absolute().parent
 
-    @property
-    def path(self):
-        return Path(self._path)
-
-    @path.setter
-    def path(self, value):
-        if isinstance(value, Path):
-            self._path = str(value)
-        else:
-            self._path = value
-
     def get_engine(self, get_seperate_engine=False):
+        # Ensure that path is a Path so checks below don't break
+        path = Path(self.path)
         if self._engine is None or get_seperate_engine:
-            if self._path == "":
+            if path == Path(""):
                 # Special case in-memory SQLite:
                 # https://docs.sqlalchemy.org/en/20/dialects/sqlite.html#threading-pooling-behavior
                 poolclass = None
             else:
                 poolclass = NullPool
-            if str(self.path).endswith(".gpkg"):
-                engine = create_engine(
-                    "gpkg:///{0}".format(self._path),
-                    echo=self.echo,
-                    poolclass=poolclass,
-                )
-                listen(engine, "connect", load_spatialite_gpkg)
+            if path.suffix.lower() == ".gpkg":
+                engine_path = f"gpkg:///{path}"
+                engine_fn = load_spatialite_gpkg
             else:
-                engine = create_engine(
-                    "sqlite:///{0}".format(self._path),
-                    echo=self.echo,
-                    poolclass=poolclass,
-                )
-                listen(engine, "connect", load_spatialite)
+                engine_path = "sqlite:///" if path == Path("") else f"sqlite:///{path}"
+                engine_fn = load_spatialite
+            engine = create_engine(engine_path, echo=self.echo, poolclass=poolclass)
+            listen(engine, "connect", engine_fn)
             if get_seperate_engine:
                 return engine
             else:
                 self._engine = engine
-
         return self._engine
 
     def get_session(self, **kwargs):
         """Get a SQLAlchemy session for optimal control.
 
         It is probably necessary to call ``session.commit``, ``session.rollback``
         and/or ``session.close``.
```

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/beta_features.py` & `threedi-schema-0.220/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/domain/constants.py` & `threedi-schema-0.220/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/domain/custom_types.py` & `threedi-schema-0.220/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/domain/indexes.py` & `threedi-schema-0.220/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/domain/models.py` & `threedi-schema-0.220/threedi_schema/domain/models.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/domain/views.py` & `threedi-schema-0.220/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.220/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.220/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/infrastructure/views.py` & `threedi-schema-0.220/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/env.py` & `threedi-schema-0.220/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py` & `threedi-schema-0.220/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/scripts.py` & `threedi-schema-0.220/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/tests/conftest.py` & `threedi-schema-0.220/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/tests/test_beta_features.py` & `threedi-schema-0.220/threedi_schema/tests/test_beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/tests/test_gpkg.py` & `threedi-schema-0.220/threedi_schema/tests/test_gpkg.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,23 @@
         # get version
         version = re.findall(r"\b(\d+\.\d+\.\d+)\b", result.stdout)[0]
         # trim patch version and convert to float
         float_version = float(version[0 : version.rfind(".")])
         if float_version >= 3.4:
             expect_success = True
     if expect_success:
-        oldest_sqlite.schema.upgrade(convert_to_geopackage=True)
+        oldest_sqlite.schema.convert_to_geopackage()
         # Ensure that after the conversion the geopackage is used
         assert oldest_sqlite.path.suffix == ".gpkg"
         assert oldest_sqlite.get_engine().dialect.name == "geopackage"
         assert oldest_sqlite.schema.validate_schema()
     else:
+        # Upgrade is not performed in convert_to_geopackage when ogr2ogr doesn't run
+        # because no operation should be performed in that case.
+        # However, this wil result in an invalid schema, so here we will run upgrade manually.
+        # Because convert_to_geopackage() is only used via upgrade; this is not an issue.
         with pytest.warns():
-            oldest_sqlite.schema.upgrade(convert_to_geopackage=True)
+            oldest_sqlite.schema.convert_to_geopackage()
+            oldest_sqlite.schema.upgrade()
             assert oldest_sqlite.path.suffix == ".sqlite"
             assert oldest_sqlite.get_engine().dialect.name == "sqlite"
             assert oldest_sqlite.schema.validate_schema()
```

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.220/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/tests/test_schema.py` & `threedi-schema-0.220/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.220/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.220/threedi_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.219.2.dev1
+Version: 0.220
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -85,16 +85,16 @@
 Install with::
 
   $ pip install threedi-schema
 
 Changelog of threedi-schema
 ===================================================
 
-0.220 (unreleased)
---------------------
+0.220 (2024-02-29)
+------------------
 - Add support for geopackage
 - Remove `the_geom_linestring` from `v2_connection_nodes` because geopackage does not support multiple geometry objects in one table
 
 
 0.219.1 (2024-01-30)
 --------------------
```

### Comparing `threedi-schema-0.219.2.dev1/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.220/threedi_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

