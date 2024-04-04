# Comparing `tmp/hrin_msb-0.2.94.tar.gz` & `tmp/hrin_msb-0.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrin_msb-0.2.94.tar", max compression
+gzip compressed data, was "hrin_msb-0.2.95.tar", max compression
```

## Comparing `hrin_msb-0.2.94.tar` & `hrin_msb-0.2.95.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1486 2023-12-01 10:15:20.273536 hrin_msb-0.2.94/hrin_msb.py
--rw-r--r--   0        0        0     1092 2023-12-01 10:11:17.921598 hrin_msb-0.2.94/LICENSE
--rw-r--r--   0        0        0        0 2023-12-01 10:15:20.273536 hrin_msb-0.2.94/msb/__init__.py
--rw-r--r--   0        0        0      173 2023-12-01 10:15:20.283701 hrin_msb-0.2.94/msb/apis/__init__.py
--rw-r--r--   0        0        0     2810 2023-12-01 10:15:20.283701 hrin_msb-0.2.94/msb/apis/api_view.py
--rw-r--r--   0        0        0     5324 2023-12-01 10:15:20.283701 hrin_msb-0.2.94/msb/apis/api_viewset.py
--rw-r--r--   0        0        0      945 2023-12-01 10:15:20.283701 hrin_msb-0.2.94/msb/apis/constants.py
--rw-r--r--   0        0        0      995 2023-12-01 10:15:20.291748 hrin_msb-0.2.94/msb/apis/errors.py
--rw-r--r--   0        0        0      576 2023-12-01 10:15:20.293791 hrin_msb-0.2.94/msb/apis/exceptions.py
--rw-r--r--   0        0        0     3834 2023-12-01 10:15:20.293791 hrin_msb-0.2.94/msb/apis/funcs.py
--rw-r--r--   0        0        0      234 2023-12-01 10:15:20.293791 hrin_msb-0.2.94/msb/auth/__init__.py
--rw-r--r--   0        0        0      769 2023-12-01 10:15:20.293791 hrin_msb-0.2.94/msb/auth/authenticators.py
--rw-r--r--   0        0        0     3491 2023-12-01 10:15:20.301895 hrin_msb-0.2.94/msb/auth/constants.py
--rw-r--r--   0        0        0     1317 2023-12-01 10:15:20.301895 hrin_msb-0.2.94/msb/auth/decorators.py
--rw-r--r--   0        0        0     2801 2023-12-01 10:15:20.301895 hrin_msb-0.2.94/msb/auth/defaults.py
--rw-r--r--   0        0        0      989 2023-12-01 10:15:20.301895 hrin_msb-0.2.94/msb/auth/exceptions.py
--rw-r--r--   0        0        0     4682 2023-12-01 10:15:20.301895 hrin_msb-0.2.94/msb/auth/permissions.py
--rw-r--r--   0        0        0     1188 2023-12-01 10:15:20.311939 hrin_msb-0.2.94/msb/auth/results.py
--rw-r--r--   0        0        0     2928 2023-12-01 10:15:20.313988 hrin_msb-0.2.94/msb/auth/serializers.py
--rw-r--r--   0        0        0     3523 2023-12-01 10:15:20.313988 hrin_msb-0.2.94/msb/auth/session.py
--rw-r--r--   0        0        0     1791 2023-12-01 10:15:20.313988 hrin_msb-0.2.94/msb/auth/token.py
--rw-r--r--   0        0        0     2996 2023-12-01 10:15:20.322135 hrin_msb-0.2.94/msb/auth/users.py
--rw-r--r--   0        0        0     2414 2023-12-01 10:15:20.322135 hrin_msb-0.2.94/msb/auth/validators.py
--rw-r--r--   0        0        0       28 2023-12-01 10:15:20.322135 hrin_msb-0.2.94/msb/cipher/__init__.py
--rw-r--r--   0        0        0       34 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/cipher/asymmetric_cipher.py
--rw-r--r--   0        0        0     2241 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/cipher/cipher.py
--rw-r--r--   0        0        0        0 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/cipher/constants.py
--rw-r--r--   0        0        0      160 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/cipher/exceptions.py
--rw-r--r--   0        0        0      714 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/cipher/symmetric_cipher.py
--rw-r--r--   0        0        0      295 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/dataclasses/__init__.py
--rw-r--r--   0        0        0     1760 2023-12-01 10:15:20.332148 hrin_msb-0.2.94/msb/dataclasses/_email.py
--rw-r--r--   0        0        0      928 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/dataclasses/_singleton.py
--rw-r--r--   0        0        0      759 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/dataclasses/_wrappers.py
--rw-r--r--   0        0        0     1840 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/dataclasses/notification.py
--rw-r--r--   0        0        0     4546 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/dataclasses/search_parameter.py
--rw-r--r--   0        0        0      354 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/datetime/__init__.py
--rw-r--r--   0        0        0      370 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/datetime/constants.py
--rw-r--r--   0        0        0     2419 2023-12-01 10:15:20.347794 hrin_msb-0.2.94/msb/datetime/wrappers.py
--rw-r--r--   0        0        0      107 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/__init__.py
--rw-r--r--   0        0        0     1231 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/config_model.py
--rw-r--r--   0        0        0      672 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/constants.py
--rw-r--r--   0        0        0     2558 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/logging_models.py
--rw-r--r--   0        0        0      767 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/metafields.py
--rw-r--r--   0        0        0     1294 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/model_fields.py
--rw-r--r--   0        0        0      506 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/models.py
--rw-r--r--   0        0        0     5219 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/msb_model.py
--rw-r--r--   0        0        0     1096 2023-12-01 10:15:20.363417 hrin_msb-0.2.94/msb/db/msb_model_manager.py
--rw-r--r--   0        0        0     3747 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/db/routers.py
--rw-r--r--   0        0        0      198 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/devtools/__init__.py
--rw-r--r--   0        0        0      752 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/devtools/constants.py
--rw-r--r--   0        0        0     1928 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/devtools/dataclasses.py
--rw-r--r--   0        0        0     3426 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/devtools/django.py
--rw-r--r--   0        0        0     2256 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/devtools/funcs.py
--rw-r--r--   0        0        0     4392 2023-12-01 10:15:20.379040 hrin_msb-0.2.94/msb/devtools/tasks.py
--rw-r--r--   0        0        0      162 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/__init__.py
--rw-r--r--   0        0        0     3006 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/config.py
--rw-r--r--   0        0        0     6422 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/constants.py
--rw-r--r--   0        0        0     1444 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/core.py
--rw-r--r--   0        0        0      382 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/exceptions.py
--rw-r--r--   0        0        0     5541 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/loging.py
--rw-r--r--   0        0        0     8624 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/env/settings.py
--rw-r--r--   0        0        0      117 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/exceptions/__init__.py
--rw-r--r--   0        0        0     1271 2023-12-01 10:15:20.394667 hrin_msb-0.2.94/msb/exceptions/_exception.py
--rw-r--r--   0        0        0      442 2023-12-01 10:15:20.410291 hrin_msb-0.2.94/msb/exceptions/handlers.py
--rw-r--r--   0        0        0      132 2023-12-01 10:15:20.410291 hrin_msb-0.2.94/msb/files/__init__.py
--rw-r--r--   0        0        0      951 2023-12-01 10:15:20.410291 hrin_msb-0.2.94/msb/files/core.py
--rw-r--r--   0        0        0     1038 2023-12-15 05:16:26.702070 hrin_msb-0.2.94/msb/files/csv.py
--rw-r--r--   0        0        0      181 2023-12-01 10:15:20.410291 hrin_msb-0.2.94/msb/files/dataclasses.py
--rw-r--r--   0        0        0     1407 2023-12-15 05:17:09.529420 hrin_msb-0.2.94/msb/files/docx.py
--rw-r--r--   0        0        0      604 2023-12-01 10:15:20.410291 hrin_msb-0.2.94/msb/files/exceptions.py
--rw-r--r--   0        0        0      329 2023-12-01 10:15:20.410291 hrin_msb-0.2.94/msb/files/factory.py
--rw-r--r--   0        0        0      198 2023-12-01 10:15:20.425914 hrin_msb-0.2.94/msb/files/messages.py
--rw-r--r--   0        0        0     1074 2023-12-15 05:17:09.516269 hrin_msb-0.2.94/msb/files/pdf.py
--rw-r--r--   0        0        0      515 2023-12-01 10:15:20.425914 hrin_msb-0.2.94/msb/http/__init__.py
--rw-r--r--   0        0        0     6420 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/client.py
--rw-r--r--   0        0        0      692 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/constants.py
--rw-r--r--   0        0        0     6835 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/dataclasses.py
--rw-r--r--   0        0        0      988 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/exceptions.py
--rw-r--r--   0        0        0     1491 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/request.py
--rw-r--r--   0        0        0     3390 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/response.py
--rw-r--r--   0        0        0     1008 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/utils.py
--rw-r--r--   0        0        0     4809 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/http/wrappers.py
--rw-r--r--   0        0        0      169 2023-12-01 10:15:20.432429 hrin_msb-0.2.94/msb/logging/__init__.py
--rw-r--r--   0        0        0     5281 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/logging/config.py
--rw-r--r--   0        0        0     1440 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/logging/constants.py
--rw-r--r--   0        0        0      593 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/logging/handlers.py
--rw-r--r--   0        0        0      229 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/services/__init__.py
--rw-r--r--   0        0        0     5338 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/services/api_service.py
--rw-r--r--   0        0        0     1784 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/services/exceptions.py
--rw-r--r--   0        0        0      183 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/services/isr_service.py
--rw-r--r--   0        0        0      702 2023-12-01 10:15:20.448072 hrin_msb-0.2.94/msb/services/msb_service.py
--rw-r--r--   0        0        0     1658 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/services/notification_service.py
--rw-r--r--   0        0        0     1996 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/services/queue_service.py
--rw-r--r--   0        0        0       25 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/testing/__init__.py
--rw-r--r--   0        0        0     4639 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/testing/api_test.py
--rw-r--r--   0        0        0      450 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/testing/constants.py
--rw-r--r--   0        0        0     1983 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/testing/core.py
--rw-r--r--   0        0        0     3665 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/testing/testdata.py
--rw-r--r--   0        0        0      476 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/testing/unit_test.py
--rw-r--r--   0        0        0        0 2023-12-01 10:15:20.463695 hrin_msb-0.2.94/msb/utils/__init__.py
--rw-r--r--   0        0        0      714 2023-12-01 10:15:20.479325 hrin_msb-0.2.94/msb/validation/__init__.py
--rw-r--r--   0        0        0     2198 2023-12-01 10:15:20.479325 hrin_msb-0.2.94/msb/validation/decorators.py
--rw-r--r--   0        0        0     1065 2023-12-01 10:15:20.479325 hrin_msb-0.2.94/msb/validation/exceptions.py
--rw-r--r--   0        0        0     1059 2023-12-01 10:15:20.479325 hrin_msb-0.2.94/msb/validation/rules.py
--rw-r--r--   0        0        0     6480 2023-12-01 10:15:20.479325 hrin_msb-0.2.94/msb/validation/schema.py
--rw-r--r--   0        0        0     2931 2023-12-01 10:15:20.479325 hrin_msb-0.2.94/msb/validation/utils.py
--rw-r--r--   0        0        0      933 2023-12-15 05:18:22.199856 hrin_msb-0.2.94/pyproject.toml
--rw-r--r--   0        0        0     8681 2023-12-01 10:15:20.253241 hrin_msb-0.2.94/README.md
--rw-r--r--   0        0        0     9559 1970-01-01 00:00:00.000000 hrin_msb-0.2.94/PKG-INFO
+-rw-r--r--   0        0        0     1510 2024-04-03 03:12:46.690806 hrin_msb-0.2.95/hrin_msb.py
+-rw-r--r--   0        0        0     1092 2023-12-01 10:11:17.921598 hrin_msb-0.2.95/LICENSE
+-rw-r--r--   0        0        0        0 2023-12-01 10:15:20.273536 hrin_msb-0.2.95/msb/__init__.py
+-rw-r--r--   0        0        0      173 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/__init__.py
+-rw-r--r--   0        0        0     2810 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/api_view.py
+-rw-r--r--   0        0        0     5324 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/api_viewset.py
+-rw-r--r--   0        0        0      945 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/constants.py
+-rw-r--r--   0        0        0      995 2023-12-01 10:15:20.291748 hrin_msb-0.2.95/msb/apis/errors.py
+-rw-r--r--   0        0        0      576 2023-12-01 10:15:20.293791 hrin_msb-0.2.95/msb/apis/exceptions.py
+-rw-r--r--   0        0        0     3834 2023-12-01 10:15:20.293791 hrin_msb-0.2.95/msb/apis/funcs.py
+-rw-r--r--   0        0        0      262 2024-04-03 03:10:28.578136 hrin_msb-0.2.95/msb/auth/__init__.py
+-rw-r--r--   0        0        0      769 2023-12-01 10:15:20.293791 hrin_msb-0.2.95/msb/auth/authenticators.py
+-rw-r--r--   0        0        0     3491 2023-12-01 10:15:20.301895 hrin_msb-0.2.95/msb/auth/constants.py
+-rw-r--r--   0        0        0     1838 2024-04-03 03:08:51.994576 hrin_msb-0.2.95/msb/auth/decorators.py
+-rw-r--r--   0        0        0     2801 2023-12-01 10:15:20.301895 hrin_msb-0.2.95/msb/auth/defaults.py
+-rw-r--r--   0        0        0      989 2023-12-01 10:15:20.301895 hrin_msb-0.2.95/msb/auth/exceptions.py
+-rw-r--r--   0        0        0     4682 2024-04-03 03:06:34.009238 hrin_msb-0.2.95/msb/auth/permissions.py
+-rw-r--r--   0        0        0     1188 2023-12-01 10:15:20.311939 hrin_msb-0.2.95/msb/auth/results.py
+-rw-r--r--   0        0        0     2928 2023-12-01 10:15:20.313988 hrin_msb-0.2.95/msb/auth/serializers.py
+-rw-r--r--   0        0        0     3523 2023-12-01 10:15:20.313988 hrin_msb-0.2.95/msb/auth/session.py
+-rw-r--r--   0        0        0     1791 2023-12-01 10:15:20.313988 hrin_msb-0.2.95/msb/auth/token.py
+-rw-r--r--   0        0        0     2996 2023-12-01 10:15:20.322135 hrin_msb-0.2.95/msb/auth/users.py
+-rw-r--r--   0        0        0     2414 2023-12-01 10:15:20.322135 hrin_msb-0.2.95/msb/auth/validators.py
+-rw-r--r--   0        0        0       28 2023-12-01 10:15:20.322135 hrin_msb-0.2.95/msb/cipher/__init__.py
+-rw-r--r--   0        0        0       34 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/asymmetric_cipher.py
+-rw-r--r--   0        0        0     2241 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/cipher.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/constants.py
+-rw-r--r--   0        0        0      160 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/exceptions.py
+-rw-r--r--   0        0        0      714 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/symmetric_cipher.py
+-rw-r--r--   0        0        0      295 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/dataclasses/__init__.py
+-rw-r--r--   0        0        0     1760 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/dataclasses/_email.py
+-rw-r--r--   0        0        0      928 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/_singleton.py
+-rw-r--r--   0        0        0      759 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/_wrappers.py
+-rw-r--r--   0        0        0     1840 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/notification.py
+-rw-r--r--   0        0        0     4546 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/search_parameter.py
+-rw-r--r--   0        0        0      354 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/datetime/__init__.py
+-rw-r--r--   0        0        0      370 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/datetime/constants.py
+-rw-r--r--   0        0        0     2419 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/datetime/wrappers.py
+-rw-r--r--   0        0        0      107 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/__init__.py
+-rw-r--r--   0        0        0     1231 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/config_model.py
+-rw-r--r--   0        0        0      672 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/constants.py
+-rw-r--r--   0        0        0     2558 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/logging_models.py
+-rw-r--r--   0        0        0      767 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/metafields.py
+-rw-r--r--   0        0        0     1294 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/model_fields.py
+-rw-r--r--   0        0        0      506 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/models.py
+-rw-r--r--   0        0        0     5219 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/msb_model.py
+-rw-r--r--   0        0        0     1096 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/msb_model_manager.py
+-rw-r--r--   0        0        0     3747 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/db/routers.py
+-rw-r--r--   0        0        0      198 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/__init__.py
+-rw-r--r--   0        0        0      752 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/constants.py
+-rw-r--r--   0        0        0     1928 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/dataclasses.py
+-rw-r--r--   0        0        0     3426 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/django.py
+-rw-r--r--   0        0        0     2256 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/funcs.py
+-rw-r--r--   0        0        0     4392 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/tasks.py
+-rw-r--r--   0        0        0      162 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/__init__.py
+-rw-r--r--   0        0        0     3006 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/config.py
+-rw-r--r--   0        0        0     6422 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/constants.py
+-rw-r--r--   0        0        0     1444 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/core.py
+-rw-r--r--   0        0        0      382 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/exceptions.py
+-rw-r--r--   0        0        0     5541 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/loging.py
+-rw-r--r--   0        0        0     8624 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/settings.py
+-rw-r--r--   0        0        0      117 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/exceptions/__init__.py
+-rw-r--r--   0        0        0     1271 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/exceptions/_exception.py
+-rw-r--r--   0        0        0      442 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/exceptions/handlers.py
+-rw-r--r--   0        0        0      132 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/__init__.py
+-rw-r--r--   0        0        0      951 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/core.py
+-rw-r--r--   0        0        0     1038 2023-12-15 05:16:26.702070 hrin_msb-0.2.95/msb/files/csv.py
+-rw-r--r--   0        0        0      181 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/dataclasses.py
+-rw-r--r--   0        0        0     1407 2023-12-15 05:17:09.529420 hrin_msb-0.2.95/msb/files/docx.py
+-rw-r--r--   0        0        0      604 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/exceptions.py
+-rw-r--r--   0        0        0      329 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/factory.py
+-rw-r--r--   0        0        0      198 2023-12-01 10:15:20.425914 hrin_msb-0.2.95/msb/files/messages.py
+-rw-r--r--   0        0        0     1074 2023-12-15 05:17:09.516269 hrin_msb-0.2.95/msb/files/pdf.py
+-rw-r--r--   0        0        0      515 2023-12-01 10:15:20.425914 hrin_msb-0.2.95/msb/http/__init__.py
+-rw-r--r--   0        0        0     6420 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/client.py
+-rw-r--r--   0        0        0      692 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/constants.py
+-rw-r--r--   0        0        0     6835 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/dataclasses.py
+-rw-r--r--   0        0        0      988 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/exceptions.py
+-rw-r--r--   0        0        0     1491 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/request.py
+-rw-r--r--   0        0        0     3390 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/response.py
+-rw-r--r--   0        0        0     1008 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/utils.py
+-rw-r--r--   0        0        0     4809 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/wrappers.py
+-rw-r--r--   0        0        0      169 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/logging/__init__.py
+-rw-r--r--   0        0        0     5281 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/logging/config.py
+-rw-r--r--   0        0        0     1440 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/logging/constants.py
+-rw-r--r--   0        0        0      593 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/logging/handlers.py
+-rw-r--r--   0        0        0      229 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/__init__.py
+-rw-r--r--   0        0        0     5338 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/api_service.py
+-rw-r--r--   0        0        0     1784 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/exceptions.py
+-rw-r--r--   0        0        0      183 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/isr_service.py
+-rw-r--r--   0        0        0      702 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/msb_service.py
+-rw-r--r--   0        0        0     1658 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/services/notification_service.py
+-rw-r--r--   0        0        0     1996 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/services/queue_service.py
+-rw-r--r--   0        0        0       25 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/__init__.py
+-rw-r--r--   0        0        0     4639 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/api_test.py
+-rw-r--r--   0        0        0      450 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/constants.py
+-rw-r--r--   0        0        0     1983 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/core.py
+-rw-r--r--   0        0        0     3665 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/testdata.py
+-rw-r--r--   0        0        0      476 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/unit_test.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/utils/__init__.py
+-rw-r--r--   0        0        0      714 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/__init__.py
+-rw-r--r--   0        0        0     2198 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/decorators.py
+-rw-r--r--   0        0        0     1065 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/exceptions.py
+-rw-r--r--   0        0        0     1059 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/rules.py
+-rw-r--r--   0        0        0     6480 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/schema.py
+-rw-r--r--   0        0        0     2931 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/utils.py
+-rw-r--r--   0        0        0      933 2024-04-03 03:23:04.155125 hrin_msb-0.2.95/pyproject.toml
+-rw-r--r--   0        0        0     8779 2024-04-03 03:23:04.147120 hrin_msb-0.2.95/README.md
+-rw-r--r--   0        0        0     9653 1970-01-01 00:00:00.000000 hrin_msb-0.2.95/PKG-INFO
```

### Comparing `hrin_msb-0.2.94/hrin_msb.py` & `hrin_msb-0.2.95/hrin_msb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from msb.apis import (ApiView, api_details, ApiViewset, )
-from msb.auth import (Permissions, api_permissions, TokenUser, SessionData)
+from msb.auth import (Permissions, api_permissions, TokenUser, SessionData, verify_ip)
 from msb.cipher import (Cipher)
 from msb.dataclasses import (SearchParameter, SearchParameterRequest, Singleton)
 from msb.db.models import (MsbModel, MsbModelMetaFields, MsbModelManager, model_fields)
 from msb.exceptions import (ApiException, AppException, CrudApiException)
 from msb.http import (RequestHeaders, RestResponse, RequestInfo, ApiResponse)
 from msb.services import (ApiService, MsbService, ApiServiceExceptions, CrudApiException)
 from msb.validation import (api_inputs, DefaultRules, ValidationSchema, InputField, Validate, validation_schema_wrapper)
 
 __all__ = [
 
 	# core msb_apis/service imports
 	"ApiView", "ApiViewset", "api_details", "ApiService", "MsbService",
 
 	# core msb_auth imports
-	"TokenUser", "SessionData", "api_permissions", "Permissions",
+	"TokenUser", "SessionData", "api_permissions", "Permissions", "verify_ip",
 
 	# core msb_http imports
 	"ApiResponse", "RequestInfo", "RequestHeaders", "RestResponse",
 
 	# core msb_exceptions imports
 	"ApiException", "CrudApiException", "AppException", "ApiServiceExceptions",
```

### Comparing `hrin_msb-0.2.94/LICENSE` & `hrin_msb-0.2.95/LICENSE`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/apis/api_view.py` & `hrin_msb-0.2.95/msb/apis/api_view.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/apis/api_viewset.py` & `hrin_msb-0.2.95/msb/apis/api_viewset.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/apis/constants.py` & `hrin_msb-0.2.95/msb/apis/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/apis/errors.py` & `hrin_msb-0.2.95/msb/apis/errors.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/apis/exceptions.py` & `hrin_msb-0.2.95/msb/apis/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/apis/funcs.py` & `hrin_msb-0.2.95/msb/apis/funcs.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/authenticators.py` & `hrin_msb-0.2.95/msb/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/constants.py` & `hrin_msb-0.2.95/msb/auth/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/decorators.py` & `hrin_msb-0.2.95/msb/auth/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from functools import wraps
 
 from .exceptions import MsbAuthExceptions
 
 
-def api_permissions(*permission_classes, _all: bool = False,**kwargs):
+def api_permissions(*permission_classes, _all: bool = False, **kwargs):
 	def decorator_function(_decorated_function):
 		@wraps(_decorated_function)
 		def wrapper_function(cls, request, *args, **kwargs):
-			override_validation = kwargs.get('override',True)
-			api_permission_is_validated = getattr(cls,'_api_permission_is_validated',False)
+			override_validation = kwargs.get('override', True)
+			api_permission_is_validated = getattr(cls, '_api_permission_is_validated', False)
 
 			if override_validation and not api_permission_is_validated:
 				evaluator = all if _all else any
 				if not evaluator([permission().has_permission(request, cls) for permission in permission_classes]):
 					raise MsbAuthExceptions.UnauthorizedAccess
 				cls._api_permission_is_validated = True
 			return _decorated_function(cls, *args, **dict(request=request, **kwargs))
@@ -33,7 +33,24 @@
 			return _decorated_function(cls, *args, **_kwargs)
 
 		return wrapper_function
 
 	return decorator_function
 
 
+def verify_ip(*allowed_ips):
+	def decorator_function(func):
+		@wraps(func)
+		def wrapper_function(cls, request, *args, **kwargs):
+			"""
+			This function takes the IPs allowed.
+			It validates all the IP in the request header and if it is not in the allowed IPs,
+			it will raise an exception.
+			"""
+			if request._auth.get('ip') not in allowed_ips:
+				raise MsbAuthExceptions.UnauthorizedAccess
+
+			return func(cls, request, *args, **kwargs)
+
+		return wrapper_function
+
+	return decorator_function
```

### Comparing `hrin_msb-0.2.94/msb/auth/defaults.py` & `hrin_msb-0.2.95/msb/auth/defaults.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/exceptions.py` & `hrin_msb-0.2.95/msb/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/permissions.py` & `hrin_msb-0.2.95/msb/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/results.py` & `hrin_msb-0.2.95/msb/auth/results.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/serializers.py` & `hrin_msb-0.2.95/msb/auth/serializers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/session.py` & `hrin_msb-0.2.95/msb/auth/session.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/token.py` & `hrin_msb-0.2.95/msb/auth/token.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/users.py` & `hrin_msb-0.2.95/msb/auth/users.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/auth/validators.py` & `hrin_msb-0.2.95/msb/auth/validators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/cipher/cipher.py` & `hrin_msb-0.2.95/msb/cipher/cipher.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/cipher/symmetric_cipher.py` & `hrin_msb-0.2.95/msb/cipher/symmetric_cipher.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/dataclasses/_email.py` & `hrin_msb-0.2.95/msb/dataclasses/_email.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/dataclasses/_singleton.py` & `hrin_msb-0.2.95/msb/dataclasses/_singleton.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/dataclasses/_wrappers.py` & `hrin_msb-0.2.95/msb/dataclasses/_wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/dataclasses/notification.py` & `hrin_msb-0.2.95/msb/dataclasses/notification.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/dataclasses/search_parameter.py` & `hrin_msb-0.2.95/msb/dataclasses/search_parameter.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/datetime/wrappers.py` & `hrin_msb-0.2.95/msb/datetime/wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/config_model.py` & `hrin_msb-0.2.95/msb/db/config_model.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/constants.py` & `hrin_msb-0.2.95/msb/db/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/logging_models.py` & `hrin_msb-0.2.95/msb/db/logging_models.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/metafields.py` & `hrin_msb-0.2.95/msb/db/metafields.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/model_fields.py` & `hrin_msb-0.2.95/msb/db/model_fields.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/msb_model.py` & `hrin_msb-0.2.95/msb/db/msb_model.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/msb_model_manager.py` & `hrin_msb-0.2.95/msb/db/msb_model_manager.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/db/routers.py` & `hrin_msb-0.2.95/msb/db/routers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/devtools/constants.py` & `hrin_msb-0.2.95/msb/devtools/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/devtools/dataclasses.py` & `hrin_msb-0.2.95/msb/devtools/dataclasses.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/devtools/django.py` & `hrin_msb-0.2.95/msb/devtools/django.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/devtools/funcs.py` & `hrin_msb-0.2.95/msb/devtools/funcs.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/devtools/tasks.py` & `hrin_msb-0.2.95/msb/devtools/tasks.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/env/config.py` & `hrin_msb-0.2.95/msb/env/config.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/env/constants.py` & `hrin_msb-0.2.95/msb/env/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/env/core.py` & `hrin_msb-0.2.95/msb/env/core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/env/loging.py` & `hrin_msb-0.2.95/msb/env/loging.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/env/settings.py` & `hrin_msb-0.2.95/msb/env/settings.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/exceptions/_exception.py` & `hrin_msb-0.2.95/msb/exceptions/_exception.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/files/core.py` & `hrin_msb-0.2.95/msb/files/core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/files/csv.py` & `hrin_msb-0.2.95/msb/files/csv.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/files/docx.py` & `hrin_msb-0.2.95/msb/files/docx.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/files/exceptions.py` & `hrin_msb-0.2.95/msb/files/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/files/pdf.py` & `hrin_msb-0.2.95/msb/files/pdf.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/__init__.py` & `hrin_msb-0.2.95/msb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/client.py` & `hrin_msb-0.2.95/msb/http/client.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/constants.py` & `hrin_msb-0.2.95/msb/http/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/dataclasses.py` & `hrin_msb-0.2.95/msb/http/dataclasses.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/exceptions.py` & `hrin_msb-0.2.95/msb/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/request.py` & `hrin_msb-0.2.95/msb/http/request.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/response.py` & `hrin_msb-0.2.95/msb/http/response.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/utils.py` & `hrin_msb-0.2.95/msb/http/utils.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/http/wrappers.py` & `hrin_msb-0.2.95/msb/http/wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/logging/config.py` & `hrin_msb-0.2.95/msb/logging/config.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/logging/constants.py` & `hrin_msb-0.2.95/msb/logging/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/logging/handlers.py` & `hrin_msb-0.2.95/msb/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/services/api_service.py` & `hrin_msb-0.2.95/msb/services/api_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/services/exceptions.py` & `hrin_msb-0.2.95/msb/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/services/msb_service.py` & `hrin_msb-0.2.95/msb/services/msb_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/services/notification_service.py` & `hrin_msb-0.2.95/msb/services/notification_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/services/queue_service.py` & `hrin_msb-0.2.95/msb/services/queue_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/testing/api_test.py` & `hrin_msb-0.2.95/msb/testing/api_test.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/testing/core.py` & `hrin_msb-0.2.95/msb/testing/core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/testing/testdata.py` & `hrin_msb-0.2.95/msb/testing/testdata.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/validation/__init__.py` & `hrin_msb-0.2.95/msb/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/validation/decorators.py` & `hrin_msb-0.2.95/msb/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/validation/exceptions.py` & `hrin_msb-0.2.95/msb/validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/validation/rules.py` & `hrin_msb-0.2.95/msb/validation/rules.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/validation/schema.py` & `hrin_msb-0.2.95/msb/validation/schema.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/msb/validation/utils.py` & `hrin_msb-0.2.95/msb/validation/utils.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.94/pyproject.toml` & `hrin_msb-0.2.95/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hrin-msb"
-version = "0.2.94"
+version = "0.2.95"
 description = ""
 authors = [
     "Prakash Mishra <prakash.mishra@intimetec.com>",
     "Mohit Verma<mohit.verma@intimetec.com>",
     "Prajwal S <prajwal.s@intimetec.com>",
     "Sathwik Somayaji S <sathwik.s.s@intimetec.com>",
 ]
```

### Comparing `hrin_msb-0.2.94/README.md` & `hrin_msb-0.2.95/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -246,7 +246,11 @@
 2. Fixed : list/retrieve api bug
 
 ### -- Version 0.2.2xx
 
 1. Fixed : UserRole.__init__() got an unexpected keyword argument 'access_type'
 2. Added: recover method in model
 3. Refactor : moved all constants to `msb_constants`
+
+### -- Version 0.2.95
+
+1. Added: Added decorator `verify_ip` to restrict the CRON Jobs tasks
```

### Comparing `hrin_msb-0.2.94/PKG-INFO` & `hrin_msb-0.2.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrin-msb
-Version: 0.2.94
+Version: 0.2.95
 Summary: 
 Author: Prakash Mishra
 Author-email: prakash.mishra@intimetec.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -276,7 +276,11 @@
 
 ### -- Version 0.2.2xx
 
 1. Fixed : UserRole.__init__() got an unexpected keyword argument 'access_type'
 2. Added: recover method in model
 3. Refactor : moved all constants to `msb_constants`
 
+### -- Version 0.2.95
+
+1. Added: Added decorator `verify_ip` to restrict the CRON Jobs tasks
+
```

