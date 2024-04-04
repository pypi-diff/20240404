# Comparing `tmp/amsdal_server-0.1.5.tar.gz` & `tmp/amsdal_server-0.1.6.tar.gz`

## Comparing `amsdal_server-0.1.5.tar` & `amsdal_server-0.1.6.tar`

### file list

```diff
@@ -1,101 +1,103 @@
--rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/.editorconfig
--rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/py.typed
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/errors.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/class_create.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/class_delete.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/class_detail.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/class_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/mixins/__init__.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/mixins/column_info_mixin.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/mixins/model_class_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/serializers/__init__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/serializers/class_info.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/serializers/register_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/services/__init__.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/classes/services/classes_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/__init__.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/authentication.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/depends.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/error_handlers/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/error_handlers/class_not_found.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/error_handlers/invalid_auth.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/__init__.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/logger.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/response_event.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/mixins/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/mixins/permissions_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/permissions/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/permissions/enums.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/permissions/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/base_serializer.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/column_format.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/column_response.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/fields_restriction.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/filter.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/objects_response.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/option.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/enums.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/controllers/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/controllers/liveness.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/controllers/readiness.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/serializers/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/serializers/healthcheck_result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/services/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/services/healthcheck.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/services/checkers/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/services/checkers/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/router.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/__init__.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_create.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_delete.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_detail.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_list.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_update.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/mixins/__init__.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/mixins/object_data_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/__init__.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/object_api.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/object_list_api.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/object_versions_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/router.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/controllers/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/controllers/transaction_execute.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/controllers/transaction_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/mixins/__init__.py
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/serializers/__init__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/serializers/transaction_item.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/serializers/transaction_property.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/services/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/services/transaction_api.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/apps/transactions/services/transaction_execution_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/configs/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/configs/constants.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/configs/main.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/src/amsdal_server/docs/api.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/.gitignore
--rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0    27844 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/README.md
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    57046 2020-02-02 00:00:00.000000 amsdal_server-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/.editorconfig
+-rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/py.typed
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/errors.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/class_create.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/class_delete.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/class_detail.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/class_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/mixins/__init__.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/mixins/column_info_mixin.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/mixins/model_class_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/serializers/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/serializers/class_info.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/serializers/register_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/services/__init__.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/classes/services/classes_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/__init__.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/authentication.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/depends.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/error_handlers/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/error_handlers/class_not_found.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/error_handlers/invalid_auth.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/__init__.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/logger.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/response_event.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/mixins/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/mixins/permissions_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/permissions/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/permissions/enums.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/permissions/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/base_serializer.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/column_format.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/column_response.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/fields_restriction.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/filter.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/objects_response.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/option.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/enums.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/controllers/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/controllers/liveness.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/controllers/readiness.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/serializers/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/serializers/healthcheck_result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/services/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/services/healthcheck.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/services/checkers/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/services/checkers/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/router.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/__init__.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/file_download.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_create.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_delete.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_detail.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_list.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_update.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/mixins/__init__.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/mixins/object_data_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/file_object.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/object_api.py
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/object_list_api.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/object_versions_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/router.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/controllers/__init__.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/controllers/transaction_execute.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/controllers/transaction_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/mixins/__init__.py
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/serializers/__init__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/serializers/transaction_item.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/serializers/transaction_property.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/services/__init__.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/services/transaction_api.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/apps/transactions/services/transaction_execution_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/configs/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/configs/constants.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/configs/main.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/src/amsdal_server/docs/api.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/.gitignore
+-rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0    27844 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/README.md
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    57048 2020-02-02 00:00:00.000000 amsdal_server-0.1.6/PKG-INFO
```

### Comparing `amsdal_server-0.1.5/.editorconfig` & `amsdal_server-0.1.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md` & `amsdal_server-0.1.6/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/server.py` & `amsdal_server-0.1.6/src/amsdal_server/server.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/router.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/router.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/errors.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/errors.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/class_create.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/class_create.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/controllers/class_list.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/controllers/class_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/mixins/column_info_mixin.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/mixins/column_info_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/mixins/model_class_info.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/mixins/model_class_info.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/serializers/register_class.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/serializers/register_class.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/classes/services/classes_api.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/classes/services/classes_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/authentication.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/authentication.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/depends.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/depends.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/errors.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/errors.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/logger.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/logger.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/response_event.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/response_event.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/middlewares/utils.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/middlewares/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/mixins/permissions_mixin.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/mixins/permissions_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/column_response.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/column_response.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/common/serializers/filter.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/common/serializers/filter.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/controllers/liveness.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/controllers/liveness.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/healthcheck/services/healthcheck.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/healthcheck/services/healthcheck.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/utils.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_create.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,11 +14,12 @@
     class_name: str,
     *,
     load_references: bool = False,
     data: dict[str, Any] = Body(...),
 ) -> dict[str, Any]:
     return ObjectApi.create_object(
         request.user,
+        base_url=str(request.base_url),
         class_name=class_name,
         data=data,
         load_references=load_references,
     )
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_detail.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_detail.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 async def object_detail(
     address: str,
     request: Request,
     version_id: str = '',
     *,
     all_versions: bool = False,
     include_metadata: bool = True,
+    file_optimized: bool = False,
 ) -> ObjectsResponse:
     return ObjectVersionsApi.get_object_versions(
         request.user,
-        urllib.parse.unquote(address),
+        base_url=str(request.base_url),
+        address=urllib.parse.unquote(address),
         version_id=version_id,
         all_versions=all_versions,
         include_metadata=include_metadata,
+        file_optimized=file_optimized,
     )
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/controllers/object_list.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/controllers/object_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,23 @@
     request: Request,
     class_name: str,
     *,
     include_metadata: bool = True,
     include_subclasses: bool = True,
     load_references: bool = False,
     all_versions: bool = False,
+    file_optimized: bool = False,
     fields_restrictions: dict[str, FieldsRestriction] = Depends(get_fields_restrictions),
     filters: list[Filter] = Depends(get_filters),
 ) -> dict[str, Any]:
     return ObjectListApi.fetch_objects(
         request.user,
-        class_name,
+        base_url=str(request.base_url),
+        class_name=class_name,
         filters=filters,
         fields_restrictions=fields_restrictions,
         include_metadata=include_metadata,
         include_subclasses=include_subclasses,
         load_references=load_references,
         all_versions=all_versions,
+        file_optimized=file_optimized,
     ).model_dump()
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/mixins/object_data_mixin.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/mixins/object_data_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 
 
 class ObjectDataMixin:
     @classmethod
     def build_object_data(
         cls,
         item: Model,
+        base_url: str,
         *,
         include_metadata: bool = False,
         fields_restrictions: dict[str, FieldsRestriction] | None = None,
         load_references: bool = False,
+        is_file_object: bool = False,
     ) -> dict[str, Any]:
         if load_references:
             _item_data = item.model_dump()
         else:
             _item_data = item.model_dump_refs()
 
         _item_data = cls._encode_bytes(_item_data)
@@ -39,14 +41,19 @@
                 if new_metadata:
                     _item_data['_metadata'] = new_metadata
 
             _item_data['_metadata']['lakehouse_address'] = urllib.parse.quote(item.get_metadata().address.to_string())
         else:
             _item_data.pop('_metadata', None)
 
+        if is_file_object:
+            _object_id = item.get_metadata().address.object_id
+            _object_version = item.get_metadata().address.object_version
+            _item_data['data'] = f'{base_url}api/objects/file-download/{_object_id}/?version_id={_object_version}'
+
         return _item_data
 
     @classmethod
     def _encode_bytes(cls, data: Any) -> Any:
         if isinstance(data, dict):
             return {key: cls._encode_bytes(value) for key, value in data.items()}
         elif isinstance(data, list):
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/object_api.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/object_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 class ObjectApi(PermissionsMixin, ObjectDataMixin):
     @classmethod
     def create_object(
         cls,
         user: BaseUser,
+        base_url: str,
         class_name: str,
         data: dict[str, Any],
         *,
         load_references: bool = False,
     ) -> dict[str, Any]:
         model_class = cls._get_model_class_and_check_permissions(
             user,
@@ -44,14 +45,15 @@
             raise ValueError(msg) from e
 
         except AmsdalUniquenessError as e:
             raise ValueError(str(e)) from e
 
         return cls.build_object_data(
             object_item,
+            base_url=base_url,
             load_references=load_references,
             include_metadata=True,
         )
 
     @classmethod
     def validate_object(
         cls,
@@ -61,14 +63,15 @@
         model_class = cls._get_model_class(class_name=class_name)
         model_class(**data)
 
     @classmethod
     def update_object(
         cls,
         user: BaseUser,
+        base_url: str,
         address: str,
         data: dict[str, Any],
         *,
         load_references: bool = False,
     ) -> dict[str, Any]:
         _address = Address.from_string(address)
         model_class = cls._get_model_class_and_check_permissions(
@@ -93,20 +96,21 @@
         )
 
         try:
             updated_item.save()
         except AmsdalUniquenessError as e:
             raise ValueError(str(e)) from e
 
-        return cls.build_object_data(updated_item, load_references=load_references)
+        return cls.build_object_data(updated_item, base_url=base_url, load_references=load_references)
 
     @classmethod
     def partial_update_object(
         cls,
         user: BaseUser,
+        base_url: str,
         address: str,
         data: dict[str, Any],
         *,
         load_references: bool = False,
     ) -> dict[str, Any]:
         _address = Address.from_string(address)
         model_class = cls._get_model_class_and_check_permissions(
@@ -129,15 +133,15 @@
                 setattr(object_item, _field, _value)
 
         try:
             object_item.save()
         except AmsdalUniquenessError as e:
             raise ValueError(str(e)) from e
 
-        return cls.build_object_data(object_item, load_references=load_references)
+        return cls.build_object_data(object_item, base_url=base_url, load_references=load_references)
 
     @classmethod
     def delete_object(
         cls,
         user: BaseUser,
         address: str,
     ) -> None:
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/object_list_api.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/object_list_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any
 
+from amsdal_models.classes.constants import FILE_CLASS_NAME
 from amsdal_models.classes.model import Model
 from amsdal_models.querysets.executor import LAKEHOUSE_DB_ALIAS
 from amsdal_utils.models.base import ModelBase
 from amsdal_utils.models.enums import Versions
 from amsdal_utils.models.utils.get_subclasses import get_subclasses
 from amsdal_utils.query.utils import Q
 from starlette.authentication import BaseUser
@@ -19,22 +20,24 @@
 
 
 class ObjectListApi(PermissionsMixin, ModelClassMixin, ColumnInfoMixin, ObjectDataMixin):
     @classmethod
     def fetch_objects(
         cls,
         user: BaseUser,
+        base_url: str,
         class_name: str,
         *,
         filters: list[Filter] | None = None,
         include_metadata: bool = False,
         include_subclasses: bool = False,
         fields_restrictions: dict[str, FieldsRestriction] | None = None,
         load_references: bool = False,
         all_versions: bool = False,
+        file_optimized: bool = False,
     ) -> ObjectsResponse:
         model_class = cls.get_model_class_by_name(class_name)
         permissions_info = cls.get_permissions_info(model_class, user)
         class_item: Model = cls.get_class_objects_qs().get(_address__object_id=class_name).execute()
         class_meta_item: Model = cls.get_class_object_metas_qs().get(_address__object_id=class_item.object_id).execute()
 
         class_properties: list[ColumnInfo] = cls.get_class_properties_by_class_and_meta(
@@ -63,35 +66,39 @@
                 for available_column in available_columns
             )
         ]
 
         return ObjectsResponse(
             columns=class_properties,
             rows=cls._fetch_objects(
+                base_url,
                 model_class,
                 filters=_filters,
                 fields_restrictions=fields_restrictions,
                 include_metadata=include_metadata,
                 include_subclasses=include_subclasses,
                 load_references=load_references,
                 all_versions=all_versions,
+                file_optimized=file_optimized,
             ),
         )
 
     @classmethod
     def _fetch_objects(
         cls,
+        base_url: str,
         model_class: type[Model],
         filters: list[Filter],
         *,
         include_subclasses: bool = False,
         include_metadata: bool = False,
         fields_restrictions: dict[str, FieldsRestriction] | None = None,
         load_references: bool = False,
         all_versions: bool = False,
+        file_optimized: bool = False,
     ) -> list[dict[str, Any]]:
         result: list[dict[str, Any]] = []
         classes: list[type[ModelBase]] = [model_class]
 
         if include_subclasses:
             for subclass in get_subclasses(model_class):
                 classes.append(subclass)
@@ -111,24 +118,31 @@
 
             if fields_restrictions:
                 fields_restriction = fields_restrictions.get(_model_class.__name__, None)
 
                 if fields_restriction:
                     qs = qs.only(fields_restriction.fields)
 
+            is_optimized_file = model_class.__name__ == FILE_CLASS_NAME and file_optimized
+
+            if is_optimized_file:
+                qs = qs.only(['filename', 'size'])
+
             if filters:
                 qs = qs.filter(
                     Q(**{f'{_filter.key}__{_filter.filter_type.name}': _filter.target for _filter in filters}),
                 )
 
             items: list[Model] = qs.order_by('-_metadata__updated_at').execute()
 
             for item in items:
                 result.append(
                     cls.build_object_data(
                         item,
+                        base_url=base_url,
                         include_metadata=include_metadata,
                         fields_restrictions=fields_restrictions,
                         load_references=load_references,
+                        is_file_object=is_optimized_file,
                     )
                 )
         return result
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/objects/services/object_versions_api.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/objects/services/object_versions_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from amsdal.schemas.manager import SchemaManager
+from amsdal_models.classes.constants import FILE_CLASS_NAME
 from amsdal_models.classes.errors import AmsdalClassError
 from amsdal_models.classes.manager import ClassManager
 from amsdal_models.classes.model import Model
 from amsdal_models.querysets.executor import LAKEHOUSE_DB_ALIAS
 from amsdal_models.schemas.data_models.schema import ObjectSchema
 from amsdal_utils.models.data_models.address import Address
 from starlette.authentication import BaseUser
@@ -16,19 +17,21 @@
 
 
 class ObjectVersionsApi(PermissionsMixin, ColumnInfoMixin, ObjectDataMixin):
     @classmethod
     def get_object_versions(
         cls,
         user: BaseUser,
+        base_url: str,
         address: str,
         version_id: str = '',
         *,
         all_versions: bool = False,
         include_metadata: bool = True,
+        file_optimized: bool = False,
     ) -> ObjectsResponse:
         _address = Address.from_string(address)
         schema_manager = SchemaManager()
         schema: ObjectSchema | None = schema_manager.get_schema_by_name(
             _address.class_name,
         )
 
@@ -59,18 +62,25 @@
                 _address__class_version=_address.class_version,
                 _address__object_version=_address.object_version,
             )
 
             if all_versions:
                 qs = qs.using(LAKEHOUSE_DB_ALIAS)
 
+            is_optimized_file = model_class.__name__ == FILE_CLASS_NAME and file_optimized
+
+            if is_optimized_file:
+                qs = qs.only(['filename', 'size'])
+
             items: list[Model] = qs.order_by('-_metadata__updated_at').execute()
 
             for item in items:
                 result.rows.append(
                     cls.build_object_data(
                         item,
+                        base_url=base_url,
                         include_metadata=include_metadata,
+                        is_file_object=is_optimized_file,
                     ),
                 )
 
         return result
```

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/transactions/utils.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/transactions/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/transactions/controllers/transaction_list.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/transactions/controllers/transaction_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/transactions/services/transaction_api.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/transactions/services/transaction_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/apps/transactions/services/transaction_execution_api.py` & `amsdal_server-0.1.6/src/amsdal_server/apps/transactions/services/transaction_execution_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/configs/constants.py` & `amsdal_server-0.1.6/src/amsdal_server/configs/constants.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/configs/main.py` & `amsdal_server-0.1.6/src/amsdal_server/configs/main.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/src/amsdal_server/docs/api.md` & `amsdal_server-0.1.6/src/amsdal_server/docs/api.md`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/LICENSE.txt` & `amsdal_server-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/README.md` & `amsdal_server-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.5/pyproject.toml` & `amsdal_server-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 dependencies = [
     "pydantic~=2.3",
     "pydantic-settings~=2.0",
     "fastapi~=0.100",
     "orjson~=3.9",
     "uvicorn~=0.23",
-    "amsdal==0.*",
+    "amsdal==0.1.*",
     "asgi-correlation-id~=4.3",
 ]
 
 [project.urls]
 Documentation = "https://pypi.org/project/amsdal_server/#readme"
 Issues = "https://pypi.org/project/amsdal_server/"
 Source = "https://pypi.org/project/amsdal_server/"
@@ -62,14 +62,15 @@
     "pytest==8.1.1",
     "pytest-mock==3.12.0",
     "pytest-subtests==0.12.1",
     "black>=24.3.0",
     "mypy>=1.9.0",
     "ruff>=0.3.3",
     "httpx==0.27.*",
+    "types-openpyxl==3.*",
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
     "- coverage combine",
@@ -102,14 +103,15 @@
     "pytest==8.1.1",
     "pytest-mock==3.12.0",
     "pytest-subtests==0.12.1",
     "black>=24.3.0",
     "mypy>=1.9.0",
     "ruff>=0.3.3",
     "httpx==0.27.*",
+    "types-openpyxl==3.*",
 ]
 pre-install-commands = [
   "pip install -e ../amsdal_utils/",
   "pip install -e ../amsdal_data/",
   "pip install -e ../amsdal_models/",
   "pip install -e ../amsdal_framework/",
 ]
```

### Comparing `amsdal_server-0.1.5/PKG-INFO` & `amsdal_server-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: amsdal_server
-Version: 0.1.5
+Version: 0.1.6
 Summary: Rest API server for AMSDAL framework
 Project-URL: Documentation, https://pypi.org/project/amsdal_server/#readme
 Project-URL: Issues, https://pypi.org/project/amsdal_server/
 Project-URL: Source, https://pypi.org/project/amsdal_server/
 Author-email: "A. Michael Salem" <ams@amsdal.com>
 License: AMSDAL End User License Agreement
         
@@ -117,15 +117,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: amsdal==0.*
+Requires-Dist: amsdal==0.1.*
 Requires-Dist: asgi-correlation-id~=4.3
 Requires-Dist: fastapi~=0.100
 Requires-Dist: orjson~=3.9
 Requires-Dist: pydantic-settings~=2.0
 Requires-Dist: pydantic~=2.3
 Requires-Dist: uvicorn~=0.23
 Description-Content-Type: text/markdown
```

