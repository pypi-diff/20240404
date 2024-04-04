# Comparing `tmp/fdk_rdf_parser-2.6.0.tar.gz` & `tmp/fdk_rdf_parser-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_rdf_parser-2.6.0.tar", max compression
+gzip compressed data, was "fdk_rdf_parser-2.7.0.tar", max compression
```

## Comparing `fdk_rdf_parser-2.6.0.tar` & `fdk_rdf_parser-2.7.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/LICENSE
--rw-r--r--   0        0        0     1206 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/pyproject.toml
--rw-r--r--   0        0        0      473 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/__init__.py
--rw-r--r--   0        0        0     1587 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/__init__.py
--rw-r--r--   0        0        0      270 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/address.py
--rw-r--r--   0        0        0      342 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/agent.py
--rw-r--r--   0        0        0      766 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/business_event.py
--rw-r--r--   0        0        0      336 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/catalog.py
--rw-r--r--   0        0        0      610 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/channel.py
--rw-r--r--   0        0        0     2711 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/concept.py
--rw-r--r--   0        0        0      189 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/conforms_to.py
--rw-r--r--   0        0        0      750 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/contactpoint.py
--rw-r--r--   0        0        0      436 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/cost.py
--rw-r--r--   0        0        0     2449 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/cpsvno_service.py
--rw-r--r--   0        0        0      356 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/data_distribution_service.py
--rw-r--r--   0        0        0     1668 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dataservice.py
--rw-r--r--   0        0        0     8657 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dataset.py
--rw-r--r--   0        0        0     1143 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dcat_resource.py
--rw-r--r--   0        0        0      274 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dct_standard.py
--rw-r--r--   0        0        0      924 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/distribution.py
--rw-r--r--   0        0        0      777 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/event.py
--rw-r--r--   0        0        0      758 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/evidence.py
--rw-r--r--   0        0        0      355 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/exceptions.py
--rw-r--r--   0        0        0      349 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/format.py
--rw-r--r--   0        0        0      198 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/harvest_meta_data.py
--rw-r--r--   0        0        0     3478 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/info_model.py
--rw-r--r--   0        0        0      331 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/legal_resource.py
--rw-r--r--   0        0        0      758 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/life_event.py
--rw-r--r--   0        0        0      402 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/media_type.py
--rw-r--r--   0        0        0     1910 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/model_element.py
--rw-r--r--   0        0        0     1147 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/model_property.py
--rw-r--r--   0        0        0      430 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/organization.py
--rw-r--r--   0        0        0      466 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/output.py
--rw-r--r--   0        0        0      376 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/participation.py
--rw-r--r--   0        0        0     1888 2024-03-13 13:11:23.316486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/public_service.py
--rw-r--r--   0        0        0      326 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/publisher.py
--rw-r--r--   0        0        0      206 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/qualified_attribution.py
--rw-r--r--   0        0        0      202 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/quality_annotation.py
--rw-r--r--   0        0        0      227 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/reference_data_code.py
--rw-r--r--   0        0        0      277 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/references.py
--rw-r--r--   0        0        0      412 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/requirement.py
--rw-r--r--   0        0        0      424 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/rule.py
--rw-r--r--   0        0        0      317 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/skos_concept.py
--rw-r--r--   0        0        0      271 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/subject.py
--rw-r--r--   0        0        0      191 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/temporal.py
--rw-r--r--   0        0        0      610 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/theme.py
--rw-r--r--   0        0        0      506 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/types.py
--rw-r--r--   0        0        0     8796 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/fdk_rdf_parser.py
--rw-r--r--   0        0        0     1349 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/__init__.py
--rw-r--r--   0        0        0     1070 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/address.py
--rw-r--r--   0        0        0     2175 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/agent.py
--rw-r--r--   0        0        0     1153 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/catalog.py
--rw-r--r--   0        0        0     1739 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/channel.py
--rw-r--r--   0        0        0    11906 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/concept.py
--rw-r--r--   0        0        0      992 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/conforms_to.py
--rw-r--r--   0        0        0     3172 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/contactpoint.py
--rw-r--r--   0        0        0     1336 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/cost.py
--rw-r--r--   0        0        0     6030 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
--rw-r--r--   0        0        0     1555 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
--rw-r--r--   0        0        0     1671 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dataservice.py
--rw-r--r--   0        0        0     9262 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dataset.py
--rw-r--r--   0        0        0     2928 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dcat_resource.py
--rw-r--r--   0        0        0      979 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dct_standard.py
--rw-r--r--   0        0        0     2051 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/distribution.py
--rw-r--r--   0        0        0     3093 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/event.py
--rw-r--r--   0        0        0     2018 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/evidence.py
--rw-r--r--   0        0        0     1116 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/format.py
--rw-r--r--   0        0        0      444 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
--rw-r--r--   0        0        0     6492 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/info_model.py
--rw-r--r--   0        0        0     1047 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/legal_resource.py
--rw-r--r--   0        0        0     3338 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/media_type.py
--rw-r--r--   0        0        0     4432 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/model_element.py
--rw-r--r--   0        0        0     3439 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/model_property.py
--rw-r--r--   0        0        0     2623 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/organization.py
--rw-r--r--   0        0        0     1247 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/output.py
--rw-r--r--   0        0        0      816 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/participation.py
--rw-r--r--   0        0        0     2155 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/publisher.py
--rw-r--r--   0        0        0      911 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
--rw-r--r--   0        0        0     1451 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/quality_annotation.py
--rw-r--r--   0        0        0     5858 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/reference_data_code.py
--rw-r--r--   0        0        0     1610 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/references.py
--rw-r--r--   0        0        0     1170 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/requirement.py
--rw-r--r--   0        0        0     1251 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/rule.py
--rw-r--r--   0        0        0     1605 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/skos_concept.py
--rw-r--r--   0        0        0     1049 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/spatial.py
--rw-r--r--   0        0        0      965 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/subject.py
--rw-r--r--   0        0        0     2540 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/temporal.py
--rw-r--r--   0        0        0     2891 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/theme.py
--rw-r--r--   0        0        0      802 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/rdf_utils/__init__.py
--rw-r--r--   0        0        0     3624 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/rdf_utils/ns.py
--rw-r--r--   0        0        0     4797 2024-03-13 13:11:23.320486 fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/rdf_utils/utils.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/LICENSE
+-rw-r--r--   0        0        0     1246 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0      473 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/__init__.py
+-rw-r--r--   0        0        0     1587 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/address.py
+-rw-r--r--   0        0        0      342 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/agent.py
+-rw-r--r--   0        0        0      766 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/business_event.py
+-rw-r--r--   0        0        0      336 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/catalog.py
+-rw-r--r--   0        0        0      610 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/channel.py
+-rw-r--r--   0        0        0     2711 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/concept.py
+-rw-r--r--   0        0        0      189 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/conforms_to.py
+-rw-r--r--   0        0        0      750 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/contactpoint.py
+-rw-r--r--   0        0        0      436 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/cost.py
+-rw-r--r--   0        0        0     2449 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/cpsvno_service.py
+-rw-r--r--   0        0        0      356 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/data_distribution_service.py
+-rw-r--r--   0        0        0     1668 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataservice.py
+-rw-r--r--   0        0        0     8657 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataset.py
+-rw-r--r--   0        0        0     1143 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dcat_resource.py
+-rw-r--r--   0        0        0      274 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dct_standard.py
+-rw-r--r--   0        0        0      924 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/distribution.py
+-rw-r--r--   0        0        0      777 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/event.py
+-rw-r--r--   0        0        0      758 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/evidence.py
+-rw-r--r--   0        0        0      355 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/exceptions.py
+-rw-r--r--   0        0        0      349 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/format.py
+-rw-r--r--   0        0        0      183 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/harvest_meta_data.py
+-rw-r--r--   0        0        0     3478 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/info_model.py
+-rw-r--r--   0        0        0      331 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/legal_resource.py
+-rw-r--r--   0        0        0      758 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/life_event.py
+-rw-r--r--   0        0        0      402 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/media_type.py
+-rw-r--r--   0        0        0     1910 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_element.py
+-rw-r--r--   0        0        0     1147 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_property.py
+-rw-r--r--   0        0        0      430 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/organization.py
+-rw-r--r--   0        0        0      466 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/output.py
+-rw-r--r--   0        0        0      376 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/participation.py
+-rw-r--r--   0        0        0     1888 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/public_service.py
+-rw-r--r--   0        0        0      326 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/publisher.py
+-rw-r--r--   0        0        0      206 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/qualified_attribution.py
+-rw-r--r--   0        0        0      202 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/quality_annotation.py
+-rw-r--r--   0        0        0      227 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/reference_data_code.py
+-rw-r--r--   0        0        0      277 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/references.py
+-rw-r--r--   0        0        0      412 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/requirement.py
+-rw-r--r--   0        0        0      424 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/rule.py
+-rw-r--r--   0        0        0      317 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/skos_concept.py
+-rw-r--r--   0        0        0      271 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/subject.py
+-rw-r--r--   0        0        0      191 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/temporal.py
+-rw-r--r--   0        0        0      610 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/theme.py
+-rw-r--r--   0        0        0      506 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/types.py
+-rw-r--r--   0        0        0     8796 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/fdk_rdf_parser.py
+-rw-r--r--   0        0        0     1349 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/address.py
+-rw-r--r--   0        0        0     2175 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/agent.py
+-rw-r--r--   0        0        0     1153 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/catalog.py
+-rw-r--r--   0        0        0     1739 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/channel.py
+-rw-r--r--   0        0        0    11906 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/concept.py
+-rw-r--r--   0        0        0      992 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/conforms_to.py
+-rw-r--r--   0        0        0     3172 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/contactpoint.py
+-rw-r--r--   0        0        0     1336 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cost.py
+-rw-r--r--   0        0        0     6030 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
+-rw-r--r--   0        0        0     1555 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
+-rw-r--r--   0        0        0     1671 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataservice.py
+-rw-r--r--   0        0        0     9262 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataset.py
+-rw-r--r--   0        0        0     2928 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dcat_resource.py
+-rw-r--r--   0        0        0      979 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dct_standard.py
+-rw-r--r--   0        0        0     2051 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/distribution.py
+-rw-r--r--   0        0        0     3093 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/event.py
+-rw-r--r--   0        0        0     2018 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/evidence.py
+-rw-r--r--   0        0        0     1116 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/format.py
+-rw-r--r--   0        0        0      431 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
+-rw-r--r--   0        0        0     6492 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/info_model.py
+-rw-r--r--   0        0        0     1047 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/legal_resource.py
+-rw-r--r--   0        0        0     3338 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/media_type.py
+-rw-r--r--   0        0        0     4432 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_element.py
+-rw-r--r--   0        0        0     3439 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_property.py
+-rw-r--r--   0        0        0     2623 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/organization.py
+-rw-r--r--   0        0        0     1247 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/output.py
+-rw-r--r--   0        0        0      816 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/participation.py
+-rw-r--r--   0        0        0     2155 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/publisher.py
+-rw-r--r--   0        0        0      911 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
+-rw-r--r--   0        0        0     1451 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/quality_annotation.py
+-rw-r--r--   0        0        0     5858 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/reference_data_code.py
+-rw-r--r--   0        0        0     1610 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/references.py
+-rw-r--r--   0        0        0     1170 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/requirement.py
+-rw-r--r--   0        0        0     1251 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/rule.py
+-rw-r--r--   0        0        0     1605 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/skos_concept.py
+-rw-r--r--   0        0        0     1049 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/spatial.py
+-rw-r--r--   0        0        0      965 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/subject.py
+-rw-r--r--   0        0        0     2540 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/temporal.py
+-rw-r--r--   0        0        0     2891 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/theme.py
+-rw-r--r--   0        0        0      787 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/__init__.py
+-rw-r--r--   0        0        0     3624 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/ns.py
+-rw-r--r--   0        0        0     4335 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/utils.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.0/PKG-INFO
```

### Comparing `fdk_rdf_parser-2.6.0/LICENSE` & `fdk_rdf_parser-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/pyproject.toml` & `fdk_rdf_parser-2.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "fdk-rdf-parser"
-version = "2.6.0"
+version = "2.7.0"
 description = ""
 authors = ["NilsOveTen <nils.ove.tendenes@digdir.no>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 rdflib = "^7.0.0"
 isodate = "^0.6.1"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.0.0"
 coverage = {extras = ["toml"], version = "^7.4.1"}
 pytest-cov = "^4.1.0"
-black = "^24.1.1"
+black = "^24.3.0"
 flake8 = "^7.0.0"
 flake8-bandit = "^4.1.1"
 flake8-black = "^0.3.6"
 flake8-bugbear = "^24.1.17"
 flake8-import-order = "^0.18.2"
 pep8-naming = "^0.13.3"
 safety = "^3.0.1"
 pytest-mock = "^3.12.0"
 codecov = "^2.1.13"
 flake8-annotations = "^3.0.1"
 mypy = "^1.8.0"
+nox = "^2024.3.2"
+nox-poetry = "^1.0.3"
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.run]
 branch = true
 source = ["fdk_rdf_parser"]
```

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/__init__.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/business_event.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/business_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/channel.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/concept.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/contactpoint.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/cpsvno_service.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dataservice.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dataset.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/dcat_resource.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/distribution.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/event.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/evidence.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/info_model.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/life_event.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/life_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/model_element.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/model_property.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/public_service.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/public_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/classes/theme.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/fdk_rdf_parser.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/fdk_rdf_parser.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/__init__.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/address.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/address.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/agent.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/agent.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/catalog.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/catalog.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/channel.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/concept.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/conforms_to.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/conforms_to.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/contactpoint.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/cost.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cost.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/cpsvno_service.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/data_distribution_service.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/data_distribution_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dataservice.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dataset.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dcat_resource.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/dct_standard.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dct_standard.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/distribution.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/event.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/evidence.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/format.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/format.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/info_model.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/legal_resource.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/legal_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/media_type.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/media_type.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/model_element.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/model_property.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/organization.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/organization.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/output.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/output.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/participation.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/participation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/publisher.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/publisher.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/qualified_attribution.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/qualified_attribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/quality_annotation.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/reference_data_code.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/reference_data_code.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/references.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/references.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/requirement.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/requirement.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/rule.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/rule.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/skos_concept.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/skos_concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/spatial.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/spatial.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/subject.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/subject.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/temporal.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/temporal.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/parse_functions/theme.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/rdf_utils/__init__.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     skosxl_uri,
     uneskos_uri,
     vcard_uri,
     xkos_uri,
     xkos_uri_v_2,
 )
 from .utils import (
-    date_list,
     date_value,
     duration_string_value,
     is_type,
     linguistic_system_keywords,
     object_number_value,
     object_value,
     resource_list,
```

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/rdf_utils/ns.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/ns.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.6.0/src/fdk_rdf_parser/rdf_utils/utils.py` & `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,26 +130,14 @@
             return date_isoformat(date_object)
         else:
             return None
     else:
         return None
 
 
-def date_list(graph: Graph, subject: URIRef, predicate: URIRef) -> Optional[List[str]]:
-    values = []
-    for obj in graph.objects(subject, predicate):
-        date_object = obj.toPython()
-        if isinstance(date_object, datetime):
-            values.append(datetime_isoformat(date_object))
-        elif isinstance(date_object, date):
-            values.append(date_isoformat(date_object))
-    values.sort()
-    return values if len(values) > 0 else None
-
-
 def string_to_float(str_value: str) -> Optional[float]:
     dot_split = str_value.split(".")
     comma_split = str_value.split(",")
     if len(dot_split) == 2 and "," not in dot_split[1]:
         to_convert = str_value.replace(",", "")
     elif len(comma_split) == 2 and "." not in comma_split[1]:
         to_convert = str_value.replace(".", "").replace(",", ".")
```

### Comparing `fdk_rdf_parser-2.6.0/PKG-INFO` & `fdk_rdf_parser-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk-rdf-parser
-Version: 2.6.0
+Version: 2.7.0
 Summary: 
 Author: NilsOveTen
 Author-email: nils.ove.tendenes@digdir.no
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

