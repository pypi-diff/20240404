# Comparing `tmp/climate_finance-1.0.0.tar.gz` & `tmp/climate_finance-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_finance-1.0.0.tar", max compression
+gzip compressed data, was "climate_finance-1.0.1.tar", max compression
```

## Comparing `climate_finance-1.0.0.tar` & `climate_finance-1.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1069 2024-04-02 16:35:59.590178 climate_finance-1.0.0/LICENSE
--rw-r--r--   0        0        0     1557 2024-04-02 16:35:59.590178 climate_finance-1.0.0/README.md
--rw-r--r--   0        0        0       11 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/.raw_data/README.md
--rw-r--r--   0        0        0       26 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/.raw_data/data_updates.json
--rw-r--r--   0        0        0       66 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/.raw_data/imputed_missing.csv
--rw-r--r--   0        0        0    16080 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/README.md
--rw-r--r--   0        0        0      499 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/__init__.py
--rw-r--r--   0        0        0     7222 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/analysis_tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/cleaning_tools.py
--rw-r--r--   0        0        0     9505 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/schema.py
--rw-r--r--   0        0        0     1128 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/config.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/__init__.py
--rw-r--r--   0        0        0    25778 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/data.py
--rw-r--r--   0        0        0     3817 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/deflators.py
--rw-r--r--   0        0        0     4466 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/dtypes.py
--rw-r--r--   0        0        0     3081 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/enums.py
--rw-r--r--   0        0        0     3366 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/loaders.py
--rw-r--r--   0        0        0    12444 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/tools.py
--rw-r--r--   0        0        0     2582 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/validation.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/bilateral/__init__.py
--rw-r--r--   0        0        0    10180 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/bilateral/bilateral_methodologies.py
--rw-r--r--   0        0        0     4589 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/bilateral/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/__init__.py
--rw-r--r--   0        0        0    19795 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/crs_tools.py
--rw-r--r--   0        0        0    10482 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/multilateral_spending_data.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/__init__.py
--rw-r--r--   0        0        0     6969 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py
--rw-r--r--   0        0        0     2606 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/__init__.py
--rw-r--r--   0        0        0     5781 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py
--rw-r--r--   0        0        0     1037 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/imputations.py
--rw-r--r--   0        0        0      308 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/shares.py
--rw-r--r--   0        0        0     9869 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/__init__.py
--rw-r--r--   0        0        0     8157 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/crdf.py
--rw-r--r--   0        0        0    13352 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/crdf_crs.py
--rw-r--r--   0        0        0     5679 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/crs.py
--rw-r--r--   0        0        0     6329 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/__init__.py
--rw-r--r--   0        0        0    19065 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv
--rw-r--r--   0        0        0     7484 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/names.py
--rw-r--r--   0        0        0    23354 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_agency_names.feather
--rw-r--r--   0        0        0     5570 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_names.feather
--rw-r--r--   0        0        0     5370 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/recipient_names.feather
--rw-r--r--   0        0        0     1436 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/settings.py
--rw-r--r--   0        0        0    14959 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/__init__.py
--rw-r--r--   0        0        0     4144 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/provider_perspective.py
--rw-r--r--   0        0        0     4144 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/recipient_perspective.py
--rw-r--r--   0        0        0     3579 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crs/__init__.py
--rw-r--r--   0        0        0    13300 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crs/add_crs_data.py
--rw-r--r--   0        0        0     9598 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crs/get_data.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/multisystem/__init__.py
--rw-r--r--   0        0        0     4492 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/multisystem/crs_channel_mapping.csv
--rw-r--r--   0        0        0     2709 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/multisystem/get_data.py
--rw-r--r--   0        0        0    22597 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/README.md
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/__init__.py
--rw-r--r--   0        0        0     7981 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/tools.py
--rw-r--r--   0        0        0     3705 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json
--rw-r--r--   0        0        0     3439 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/validation.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/__init__.py
--rw-r--r--   0        0        0    17281 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/download_data.py
--rw-r--r--   0        0        0     9534 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/get_data.py
--rw-r--r--   0        0        0     3413 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/pre_process.py
--rw-r--r--   0        0        0     6309 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/get_unfccc_data.py
--rw-r--r--   0        0        0        0 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/__init__.py
--rw-r--r--   0        0        0     2966 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/get_data.py
--rw-r--r--   0        0        0    11767 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/pre_process.py
--rw-r--r--   0        0        0     1164 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/read_files.py
--rw-r--r--   0        0        0      664 2024-04-02 16:35:59.598178 climate_finance-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 climate_finance-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 09:35:24.926246 climate_finance-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3001 2024-04-04 09:35:24.926246 climate_finance-1.0.1/README.md
+-rw-r--r--   0        0        0       11 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/.raw_data/README.md
+-rw-r--r--   0        0        0       26 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/.raw_data/data_updates.json
+-rw-r--r--   0        0        0       66 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/.raw_data/imputed_missing.csv
+-rw-r--r--   0        0        0    16080 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/README.md
+-rw-r--r--   0        0        0      499 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/__init__.py
+-rw-r--r--   0        0        0     7222 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/analysis_tools.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/cleaning_tools.py
+-rw-r--r--   0        0        0     9505 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/schema.py
+-rw-r--r--   0        0        0     1120 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/config.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/__init__.py
+-rw-r--r--   0        0        0    25777 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/data.py
+-rw-r--r--   0        0        0     3817 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/deflators.py
+-rw-r--r--   0        0        0     4466 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/dtypes.py
+-rw-r--r--   0        0        0     3081 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/enums.py
+-rw-r--r--   0        0        0     3366 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/core/loaders.py
+-rw-r--r--   0        0        0    12444 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/core/tools.py
+-rw-r--r--   0        0        0     2582 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/core/validation.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/bilateral/__init__.py
+-rw-r--r--   0        0        0    10180 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/bilateral/bilateral_methodologies.py
+-rw-r--r--   0        0        0     4589 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/bilateral/tools.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/__init__.py
+-rw-r--r--   0        0        0    19795 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/crs_tools.py
+-rw-r--r--   0        0        0    10482 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/multilateral_spending_data.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py
+-rw-r--r--   0        0        0     2620 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/__init__.py
+-rw-r--r--   0        0        0     5781 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py
+-rw-r--r--   0        0        0     1037 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/imputations.py
+-rw-r--r--   0        0        0      308 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/shares.py
+-rw-r--r--   0        0        0     9869 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/tools.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/__init__.py
+-rw-r--r--   0        0        0     8157 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/crdf.py
+-rw-r--r--   0        0        0    13352 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/crdf_crs.py
+-rw-r--r--   0        0        0     5679 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/crs.py
+-rw-r--r--   0        0        0     6329 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/tools.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0    19065 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     7484 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/names.py
+-rw-r--r--   0        0        0    23354 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_agency_names.feather
+-rw-r--r--   0        0        0     5570 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_names.feather
+-rw-r--r--   0        0        0     5370 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/recipient_names.feather
+-rw-r--r--   0        0        0     1436 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/settings.py
+-rw-r--r--   0        0        0    14959 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/tools.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/__init__.py
+-rw-r--r--   0        0        0     4144 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/provider_perspective.py
+-rw-r--r--   0        0        0     4144 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/recipient_perspective.py
+-rw-r--r--   0        0        0     3579 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/tools.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crs/__init__.py
+-rw-r--r--   0        0        0    13296 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crs/add_crs_data.py
+-rw-r--r--   0        0        0     9598 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crs/get_data.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/multisystem/__init__.py
+-rw-r--r--   0        0        0     4492 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/oecd/multisystem/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     2709 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/oecd/multisystem/get_data.py
+-rw-r--r--   0        0        0    22597 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0     7981 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/tools.py
+-rw-r--r--   0        0        0     3705 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json
+-rw-r--r--   0        0        0     3439 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/validation.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/__init__.py
+-rw-r--r--   0        0        0    17282 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/download_data.py
+-rw-r--r--   0        0        0     9534 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/get_data.py
+-rw-r--r--   0        0        0     3413 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/pre_process.py
+-rw-r--r--   0        0        0     6309 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/get_unfccc_data.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/__init__.py
+-rw-r--r--   0        0        0     2966 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/get_data.py
+-rw-r--r--   0        0        0    11767 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/pre_process.py
+-rw-r--r--   0        0        0     1165 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/read_files.py
+-rw-r--r--   0        0        0      660 2024-04-04 09:35:24.934246 climate_finance-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 climate_finance-1.0.1/PKG-INFO
```

### Comparing `climate_finance-1.0.0/LICENSE` & `climate_finance-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/README.md` & `climate_finance-1.0.1/climate_finance/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/common/analysis_tools.py` & `climate_finance-1.0.1/climate_finance/common/analysis_tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/common/schema.py` & `climate_finance-1.0.1/climate_finance/common/schema.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/config.py` & `climate_finance-1.0.1/climate_finance/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 
 # Set levels for the logger, shell and file
 logger.setLevel(logging.DEBUG)
 shell_handler.setLevel(logging.DEBUG)
 
 # Format the outputs
 fmt_file = "%(levelname)s (%(asctime)s): %(message)s"
-fmt_shell = (
-    "%(levelname)s [%(funcName)s] %(message)s"
-)
+fmt_shell = "%(levelname)s [%(funcName)s] %(message)s"
 
 # Create formatters
 shell_formatter = logging.Formatter(fmt_shell)
 file_formatter = logging.Formatter(fmt_file)
 
 # Add formatters to handlers
 shell_handler.setFormatter(shell_formatter)
```

### Comparing `climate_finance-1.0.0/climate_finance/core/data.py` & `climate_finance-1.0.1/climate_finance/core/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,15 +626,15 @@
         # Concatenate the dataframes
         loaded_data = pd.concat(loaded_dataframes, ignore_index=True)
 
         if self._ignore_prices_and_currency:
             return loaded_data
 
         # Convert to the right currency and prices, if needed
-        if self.prices != "current" and self.currency != "USD":
+        if self.prices != "current" or self.currency != "USD":
             loaded_data = DEFLATOR(
                 data=loaded_data,
                 target_currency=self.currency,
                 prices=self.prices,
                 base_year=self.base_year,
             )
         else:
```

### Comparing `climate_finance-1.0.0/climate_finance/core/deflators.py` & `climate_finance-1.0.1/climate_finance/core/deflators.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/core/dtypes.py` & `climate_finance-1.0.1/climate_finance/core/dtypes.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/core/enums.py` & `climate_finance-1.0.1/climate_finance/core/enums.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/core/loaders.py` & `climate_finance-1.0.1/climate_finance/core/loaders.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/core/tools.py` & `climate_finance-1.0.1/climate_finance/core/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/core/validation.py` & `climate_finance-1.0.1/climate_finance/core/validation.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/bilateral/bilateral_methodologies.py` & `climate_finance-1.0.1/climate_finance/methodologies/bilateral/bilateral_methodologies.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/bilateral/tools.py` & `climate_finance-1.0.1/climate_finance/methodologies/bilateral/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/crs_tools.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/crs_tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/multilateral_spending_data.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/multilateral_spending_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
     # Ensure key columns are integers
     data[[ClimateSchema.YEAR, ClimateSchema.PROVIDER_CODE]] = data[
         [ClimateSchema.YEAR, ClimateSchema.PROVIDER_CODE]
     ].astype("Int32")
 
     # Make Cross-cutting negative
-    data.loc[lambda d: d[ClimateSchema.INDICATOR] == "Cross-cutting", ClimateSchema.VALUE] *= -1
+    data.loc[
+        lambda d: d[ClimateSchema.INDICATOR] == "Cross-cutting", ClimateSchema.VALUE
+    ] *= -1
 
     # Summarise the data at the right level
     data_by_indicator = summarise_by_party_idx(data=data, idx=idx, by_indicator=True)
 
     # Summarise data by yearly totals
     data_yearly = summarise_by_party_idx(data=data, idx=idx, by_indicator=False).assign(
         **{ClimateSchema.INDICATOR: ClimateSchema.CLIMATE_UNSPECIFIED}
```

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/imputations.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/imputations.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/multilateral/tools.py` & `climate_finance-1.0.1/climate_finance/methodologies/multilateral/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/spending/crdf.py` & `climate_finance-1.0.1/climate_finance/methodologies/spending/crdf.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/spending/crdf_crs.py` & `climate_finance-1.0.1/climate_finance/methodologies/spending/crdf_crs.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/spending/crs.py` & `climate_finance-1.0.1/climate_finance/methodologies/spending/crs.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/methodologies/spending/tools.py` & `climate_finance-1.0.1/climate_finance/methodologies/spending/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/names.py` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/names.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_agency_names.feather` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_agency_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_names.feather` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/recipient_names.feather` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/recipient_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/settings.py` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/settings.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/tools.py` & `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/crdf/provider_perspective.py` & `climate_finance-1.0.1/climate_finance/oecd/crdf/provider_perspective.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/crdf/recipient_perspective.py` & `climate_finance-1.0.1/climate_finance/oecd/crdf/recipient_perspective.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/crdf/tools.py` & `climate_finance-1.0.1/climate_finance/oecd/crdf/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/crs/add_crs_data.py` & `climate_finance-1.0.1/climate_finance/oecd/crs/add_crs_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         .fillna(projects_df[ClimateSchema.PROJECT_TITLE])
     )
     return projects_df
 
 
 def clean_idx_to_str(data: pd.DataFrame, idx: list[str]) -> pd.DataFrame:
     """Convert idx to string for consistent merge"""
-    
+
     data = data.copy()
 
     for col in idx:
         data[col] = (
             data[col]
             .astype("string[pyarrow]")
             .replace("nan", np.nan, regex=False)
```

### Comparing `climate_finance-1.0.0/climate_finance/oecd/crs/get_data.py` & `climate_finance-1.0.1/climate_finance/oecd/crs/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/multisystem/crs_channel_mapping.csv` & `climate_finance-1.0.1/climate_finance/oecd/multisystem/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/oecd/multisystem/get_data.py` & `climate_finance-1.0.1/climate_finance/oecd/multisystem/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/README.md` & `climate_finance-1.0.1/climate_finance/unfccc/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/tools.py` & `climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json` & `climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/validation.py` & `climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/validation.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/download/download_data.py` & `climate_finance-1.0.1/climate_finance/unfccc/download/download_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This script downloads data from the UNFCCC data interface."""
+
 import fnmatch
 import os
 import pathlib
 from time import sleep
 
 import pandas as pd
 from selenium import webdriver
```

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/download/get_data.py` & `climate_finance-1.0.1/climate_finance/unfccc/download/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
 
 def get_unfccc_summary(
     start_year: int,
     end_year: int,
     br: list[int] = None,
     party: str | list[str] = None,
-    directory: pathlib.Path
-    | str = ClimateDataPath.raw_data / "unfccc_data_interface_files",
+    directory: pathlib.Path | str = ClimateDataPath.raw_data
+    / "unfccc_data_interface_files",
     force_download: bool = False,
 ) -> pd.DataFrame:
     """
     Function to get the UNFCCC summary data.
 
     Args:
         start_year: the start year of the data
@@ -168,16 +168,16 @@
 
 
 def get_unfccc_multilateral(
     start_year: int,
     end_year: int,
     br: list[int] = None,
     party: str | list[str] = None,
-    directory: pathlib.Path
-    | str = ClimateDataPath.raw_data / "unfccc_data_interface_files",
+    directory: pathlib.Path | str = ClimateDataPath.raw_data
+    / "unfccc_data_interface_files",
     force_download: bool = False,
 ) -> pd.DataFrame:
     """
     Function to get the UNFCCC multilateral data.
 
     Args:
         start_year: the start year of the data
@@ -237,16 +237,16 @@
 
 
 def get_unfccc_bilateral(
     start_year: int,
     end_year: int,
     br: list[int] = None,
     party: str | list[str] = None,
-    directory: pathlib.Path
-    | str = ClimateDataPath.raw_data / "unfccc_data_interface_files",
+    directory: pathlib.Path | str = ClimateDataPath.raw_data
+    / "unfccc_data_interface_files",
     force_download: bool = False,
 ) -> pd.DataFrame:
     """
     Function to get the UNFCCC bilateral data.
     Args:
 
         start_year: the start year of the data
```

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/download/pre_process.py` & `climate_finance-1.0.1/climate_finance/unfccc/download/pre_process.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/get_unfccc_data.py` & `climate_finance-1.0.1/climate_finance/unfccc/get_unfccc_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/manual/get_data.py` & `climate_finance-1.0.1/climate_finance/unfccc/manual/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/manual/pre_process.py` & `climate_finance-1.0.1/climate_finance/unfccc/manual/pre_process.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.0/climate_finance/unfccc/manual/read_files.py` & `climate_finance-1.0.1/climate_finance/unfccc/manual/read_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This script deals with reading in the raw data from the UNFCCC biennial reports."""
+
 import glob
 import pathlib
 
 import pandas as pd
 
 
 def _load_br_files(
```

### Comparing `climate_finance-1.0.0/pyproject.toml` & `climate_finance-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "climate-finance"
-version = "1.0.0"
+version = "1.0.1"
 description = "Climate Finance data"
 authors = ["Jorge Rivera, The ONE Campaign"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "climate_finance"}]
 
 [tool.poetry.dependencies]
@@ -18,14 +18,14 @@
 thefuzz = {extras = ["speedup"], version = "^0.22"}
 oda-data = "^1.1"
 webdriver-manager = "^4.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8"
-bump2version = "^1.0.1"
+bump2version = "^1.0"
 black = "^24"
-pytest-cov = "^4.1.0"
+pytest-cov = "^4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

