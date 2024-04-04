# Comparing `tmp/commons_lib-1.1.1.tar.gz` & `tmp/commons_lib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commons_lib-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "commons_lib-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `commons_lib-1.1.1.tar` & `commons_lib-1.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1889 2024-02-14 08:30:07.100686 commons_lib-1.1.1/.gitignore
--rw-r--r--   0        0        0      166 2024-02-14 08:14:46.191466 commons_lib-1.1.1/README.md
--rw-r--r--   0        0        0       42 2024-02-14 08:14:46.191612 commons_lib-1.1.1/commons_lib/README.md
--rw-r--r--   0        0        0       21 2024-03-24 11:38:05.051644 commons_lib-1.1.1/commons_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.191797 commons_lib-1.1.1/commons_lib/models/__init__.py
--rw-r--r--   0        0        0     1086 2024-03-30 10:42:56.269827 commons_lib-1.1.1/commons_lib/models/entities/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.831991 commons_lib-1.1.1/commons_lib/models/entities/accounts/__init__.py
--rw-r--r--   0        0        0      587 2024-03-27 15:07:04.860134 commons_lib-1.1.1/commons_lib/models/entities/accounts/account_category_entity.py
--rw-r--r--   0        0        0      888 2024-03-27 12:25:52.776380 commons_lib-1.1.1/commons_lib/models/entities/accounts/accountـentity.py
--rw-r--r--   0        0        0     1545 2024-03-27 12:25:52.776652 commons_lib-1.1.1/commons_lib/models/entities/appreciatation.py
--rw-r--r--   0        0        0     1489 2024-03-27 12:25:52.776752 commons_lib-1.1.1/commons_lib/models/entities/appreciatation_entity.py
--rw-r--r--   0        0        0      886 2024-03-27 12:26:07.182779 commons_lib-1.1.1/commons_lib/models/entities/base_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.835239 commons_lib-1.1.1/commons_lib/models/entities/gift/__init__.py
--rw-r--r--   0        0        0      738 2024-03-27 12:26:10.061669 commons_lib-1.1.1/commons_lib/models/entities/gift/redeem_entity.py
--rw-r--r--   0        0        0      734 2024-03-27 12:26:11.213548 commons_lib-1.1.1/commons_lib/models/entities/gift/vended_winning_entity.py
--rw-r--r--   0        0        0      541 2024-03-30 10:45:58.246339 commons_lib-1.1.1/commons_lib/models/entities/gift/winning_category_entity.py
--rw-r--r--   0        0        0     1090 2024-03-30 10:49:28.750810 commons_lib-1.1.1/commons_lib/models/entities/gift/winning_entity.py
--rw-r--r--   0        0        0      357 2024-03-27 12:26:11.858360 commons_lib-1.1.1/commons_lib/models/entities/gift/winning_vendors.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.838587 commons_lib-1.1.1/commons_lib/models/entities/organization/__init__.py
--rw-r--r--   0        0        0      799 2024-03-28 11:23:13.314366 commons_lib-1.1.1/commons_lib/models/entities/organization/company_entity.py
--rw-r--r--   0        0        0      289 2024-03-27 12:25:52.778091 commons_lib-1.1.1/commons_lib/models/entities/organization/sub_org_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.841515 commons_lib-1.1.1/commons_lib/models/entities/permissions/__init__.py
--rw-r--r--   0        0        0      410 2024-03-27 12:25:52.778412 commons_lib-1.1.1/commons_lib/models/entities/permissions/permission_entity.py
--rw-r--r--   0        0        0      267 2024-03-27 12:25:52.778656 commons_lib-1.1.1/commons_lib/models/entities/permissions/role_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.844104 commons_lib-1.1.1/commons_lib/models/entities/position/__init__.py
--rw-r--r--   0        0        0      573 2024-03-27 12:25:52.778904 commons_lib-1.1.1/commons_lib/models/entities/position/position_category_entity.py
--rw-r--r--   0        0        0     1375 2024-03-27 12:25:52.779013 commons_lib-1.1.1/commons_lib/models/entities/position/position_entity.py
--rw-r--r--   0        0        0      984 2024-03-27 12:25:52.779117 commons_lib-1.1.1/commons_lib/models/entities/position/positionentity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.845299 commons_lib-1.1.1/commons_lib/models/entities/transfers/__init__.py
--rw-r--r--   0        0        0      284 2024-03-27 12:25:45.642872 commons_lib-1.1.1/commons_lib/models/entities/transfers/transaction_category_entity.py
--rw-r--r--   0        0        0      907 2024-03-27 12:26:10.732404 commons_lib-1.1.1/commons_lib/models/entities/transfers/transation_entity.py
--rw-r--r--   0        0        0      259 2024-03-27 12:25:45.643291 commons_lib-1.1.1/commons_lib/models/entities/transfers/transfer_category_entity.py
--rw-r--r--   0        0        0      751 2024-03-27 12:26:10.884842 commons_lib-1.1.1/commons_lib/models/entities/transfers/transfer_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.846343 commons_lib-1.1.1/commons_lib/models/entities/user/__init__.py
--rw-r--r--   0        0        0      262 2024-03-27 12:25:52.779737 commons_lib-1.1.1/commons_lib/models/entities/user/employee_entiry.py
--rw-r--r--   0        0        0      258 2024-03-27 12:25:52.779862 commons_lib-1.1.1/commons_lib/models/entities/user/employee_entity.py
--rw-r--r--   0        0        0     1692 2024-03-27 12:26:09.243772 commons_lib-1.1.1/commons_lib/models/entities/user/employment_entity.py
--rw-r--r--   0        0        0      945 2024-03-27 12:26:11.047431 commons_lib-1.1.1/commons_lib/models/entities/user/user_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.848188 commons_lib-1.1.1/commons_lib/models/entities/values/__init__.py
--rw-r--r--   0        0        0      954 2024-03-27 17:14:18.715525 commons_lib-1.1.1/commons_lib/models/entities/values/org_behavior_entity.py
--rw-r--r--   0        0        0      618 2024-03-27 17:14:18.704419 commons_lib-1.1.1/commons_lib/models/entities/values/org_value_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.194923 commons_lib-1.1.1/commons_lib/models/enums/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195024 commons_lib-1.1.1/commons_lib/models/records/__init__.py
--rw-r--r--   0        0        0      844 2024-02-14 08:14:46.195134 commons_lib-1.1.1/commons_lib/models/records/base_record.py
--rw-r--r--   0        0        0      283 2024-02-14 08:14:46.195227 commons_lib-1.1.1/commons_lib/models/records/records.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195319 commons_lib-1.1.1/commons_lib/utils/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-14 08:14:46.195430 commons_lib-1.1.1/commons_lib/utils/singleton.py
--rw-r--r--   0        0        0     1243 2024-02-14 08:14:46.195529 commons_lib-1.1.1/commons_lib/utils/ttl_cache.py
--rw-r--r--   0        0        0      634 2024-02-14 08:14:46.195689 commons_lib-1.1.1/docs/Makefile
--rw-r--r--   0        0        0     2329 2024-02-14 08:14:46.195793 commons_lib-1.1.1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-02-14 08:14:46.195888 commons_lib-1.1.1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-02-14 08:14:46.195976 commons_lib-1.1.1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-02-14 08:14:46.196071 commons_lib-1.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-02-14 08:14:46.196170 commons_lib-1.1.1/docs/make.bat
--rw-r--r--   0        0        0       57 2024-02-14 08:14:46.196268 commons_lib-1.1.1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-02-14 08:14:46.196365 commons_lib-1.1.1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-02-14 08:14:46.196548 commons_lib-1.1.1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-02-14 08:14:46.196639 commons_lib-1.1.1/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-02-14 08:14:46.196736 commons_lib-1.1.1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      427 2024-02-14 08:14:46.196827 commons_lib-1.1.1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-02-14 08:14:46.196899 commons_lib-1.1.1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-02-14 08:14:46.196978 commons_lib-1.1.1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-02-14 08:14:46.197063 commons_lib-1.1.1/docs/workflows.md
--rw-r--r--   0        0        0     6070 2024-02-14 08:14:46.197192 commons_lib-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      989 2024-02-14 08:14:46.197324 commons_lib-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1217 2024-02-14 08:14:46.197423 commons_lib-1.1.1/tests/test_methods.py
--rw-r--r--   0        0        0      328 2024-02-14 08:14:46.197514 commons_lib-1.1.1/tests/test_ttl_cache.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 commons_lib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1889 2024-02-14 08:30:07.100686 commons_lib-1.1.2/.gitignore
+-rw-r--r--   0        0        0      166 2024-02-14 08:14:46.191466 commons_lib-1.1.2/README.md
+-rw-r--r--   0        0        0       42 2024-02-14 08:14:46.191612 commons_lib-1.1.2/commons_lib/README.md
+-rw-r--r--   0        0        0       21 2024-04-04 07:20:01.982572 commons_lib-1.1.2/commons_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.191797 commons_lib-1.1.2/commons_lib/models/__init__.py
+-rw-r--r--   0        0        0     1086 2024-03-30 10:42:56.269827 commons_lib-1.1.2/commons_lib/models/entities/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.831991 commons_lib-1.1.2/commons_lib/models/entities/accounts/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-04 07:18:47.788258 commons_lib-1.1.2/commons_lib/models/entities/accounts/account_category_entity.py
+-rw-r--r--   0        0        0      888 2024-04-04 07:18:47.786404 commons_lib-1.1.2/commons_lib/models/entities/accounts/accountـentity.py
+-rw-r--r--   0        0        0     1545 2024-04-04 07:18:47.769117 commons_lib-1.1.2/commons_lib/models/entities/appreciatation.py
+-rw-r--r--   0        0        0     1489 2024-04-04 07:18:47.754825 commons_lib-1.1.2/commons_lib/models/entities/appreciatation_entity.py
+-rw-r--r--   0        0        0      886 2024-03-27 12:26:07.182779 commons_lib-1.1.2/commons_lib/models/entities/base_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.835239 commons_lib-1.1.2/commons_lib/models/entities/gift/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-04 07:18:47.767377 commons_lib-1.1.2/commons_lib/models/entities/gift/redeem_entity.py
+-rw-r--r--   0        0        0      734 2024-04-04 07:18:47.791017 commons_lib-1.1.2/commons_lib/models/entities/gift/vended_winning_entity.py
+-rw-r--r--   0        0        0      541 2024-04-04 07:18:47.779188 commons_lib-1.1.2/commons_lib/models/entities/gift/winning_category_entity.py
+-rw-r--r--   0        0        0     1090 2024-04-04 07:18:47.784181 commons_lib-1.1.2/commons_lib/models/entities/gift/winning_entity.py
+-rw-r--r--   0        0        0      357 2024-04-04 07:18:47.758854 commons_lib-1.1.2/commons_lib/models/entities/gift/winning_vendors.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.838587 commons_lib-1.1.2/commons_lib/models/entities/organization/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-04 07:18:47.782939 commons_lib-1.1.2/commons_lib/models/entities/organization/company_entity.py
+-rw-r--r--   0        0        0      289 2024-04-04 07:18:47.792138 commons_lib-1.1.2/commons_lib/models/entities/organization/sub_org_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.841515 commons_lib-1.1.2/commons_lib/models/entities/permissions/__init__.py
+-rw-r--r--   0        0        0      410 2024-04-04 07:18:47.798616 commons_lib-1.1.2/commons_lib/models/entities/permissions/permission_entity.py
+-rw-r--r--   0        0        0      267 2024-04-04 07:18:47.795119 commons_lib-1.1.2/commons_lib/models/entities/permissions/role_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.844104 commons_lib-1.1.2/commons_lib/models/entities/position/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-04 07:18:47.797505 commons_lib-1.1.2/commons_lib/models/entities/position/position_category_entity.py
+-rw-r--r--   0        0        0     1375 2024-04-04 07:18:47.777854 commons_lib-1.1.2/commons_lib/models/entities/position/position_entity.py
+-rw-r--r--   0        0        0      984 2024-04-04 07:18:47.765683 commons_lib-1.1.2/commons_lib/models/entities/position/positionentity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.845299 commons_lib-1.1.2/commons_lib/models/entities/transfers/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-04 07:18:47.761765 commons_lib-1.1.2/commons_lib/models/entities/transfers/transaction_category_entity.py
+-rw-r--r--   0        0        0      907 2024-04-04 07:18:47.763846 commons_lib-1.1.2/commons_lib/models/entities/transfers/transation_entity.py
+-rw-r--r--   0        0        0      259 2024-04-04 07:18:47.771690 commons_lib-1.1.2/commons_lib/models/entities/transfers/transfer_category_entity.py
+-rw-r--r--   0        0        0      751 2024-04-04 07:18:47.772862 commons_lib-1.1.2/commons_lib/models/entities/transfers/transfer_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.846343 commons_lib-1.1.2/commons_lib/models/entities/user/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-04 07:18:47.776564 commons_lib-1.1.2/commons_lib/models/entities/user/employee_entiry.py
+-rw-r--r--   0        0        0      258 2024-04-04 07:18:47.785209 commons_lib-1.1.2/commons_lib/models/entities/user/employee_entity.py
+-rw-r--r--   0        0        0     1692 2024-04-04 07:18:47.774047 commons_lib-1.1.2/commons_lib/models/entities/user/employment_entity.py
+-rw-r--r--   0        0        0      945 2024-04-04 07:18:47.781604 commons_lib-1.1.2/commons_lib/models/entities/user/user_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.848188 commons_lib-1.1.2/commons_lib/models/entities/values/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-04 07:18:47.775381 commons_lib-1.1.2/commons_lib/models/entities/values/org_behavior_entity.py
+-rw-r--r--   0        0        0      618 2024-04-04 07:18:47.770427 commons_lib-1.1.2/commons_lib/models/entities/values/org_value_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.194923 commons_lib-1.1.2/commons_lib/models/enums/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195024 commons_lib-1.1.2/commons_lib/models/records/__init__.py
+-rw-r--r--   0        0        0      844 2024-02-14 08:14:46.195134 commons_lib-1.1.2/commons_lib/models/records/base_record.py
+-rw-r--r--   0        0        0      283 2024-02-14 08:14:46.195227 commons_lib-1.1.2/commons_lib/models/records/records.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195319 commons_lib-1.1.2/commons_lib/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-14 08:14:46.195430 commons_lib-1.1.2/commons_lib/utils/singleton.py
+-rw-r--r--   0        0        0     1243 2024-02-14 08:14:46.195529 commons_lib-1.1.2/commons_lib/utils/ttl_cache.py
+-rw-r--r--   0        0        0      634 2024-02-14 08:14:46.195689 commons_lib-1.1.2/docs/Makefile
+-rw-r--r--   0        0        0     2329 2024-02-14 08:14:46.195793 commons_lib-1.1.2/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-02-14 08:14:46.195888 commons_lib-1.1.2/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-02-14 08:14:46.195976 commons_lib-1.1.2/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-02-14 08:14:46.196071 commons_lib-1.1.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-02-14 08:14:46.196170 commons_lib-1.1.2/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-02-14 08:14:46.196268 commons_lib-1.1.2/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-02-14 08:14:46.196365 commons_lib-1.1.2/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-02-14 08:14:46.196548 commons_lib-1.1.2/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-02-14 08:14:46.196639 commons_lib-1.1.2/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-02-14 08:14:46.196736 commons_lib-1.1.2/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      427 2024-02-14 08:14:46.196827 commons_lib-1.1.2/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-02-14 08:14:46.196899 commons_lib-1.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-02-14 08:14:46.196978 commons_lib-1.1.2/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-02-14 08:14:46.197063 commons_lib-1.1.2/docs/workflows.md
+-rw-r--r--   0        0        0     6070 2024-02-14 08:14:46.197192 commons_lib-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      989 2024-02-14 08:14:46.197324 commons_lib-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1217 2024-02-14 08:14:46.197423 commons_lib-1.1.2/tests/test_methods.py
+-rw-r--r--   0        0        0      328 2024-02-14 08:14:46.197514 commons_lib-1.1.2/tests/test_ttl_cache.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 commons_lib-1.1.2/PKG-INFO
```

### Comparing `commons_lib-1.1.1/.gitignore` & `commons_lib-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/__init__.py` & `commons_lib-1.1.2/commons_lib/models/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/accounts/account_category_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/accounts/account_category_entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy import VARCHAR, Column
 from sqlalchemy.orm import relationship
 from sqlalchemy import BIGINT, ForeignKey
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class AccountCategoryEntity(BaseEntity):
 
     __tablename__ = "accounts_type"
 
     title: str = Column(VARCHAR(256), nullable=False)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/accounts/accountـentity.py` & `commons_lib-1.1.2/commons_lib/models/entities/accounts/accountـentity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import date
 from sqlalchemy.dialects.postgresql import UUID
 
 from sqlalchemy import Column, BIGINT, ForeignKey, VARCHAR, DateTime
 from sqlalchemy.orm import relationship, Mapped
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class AccountEntity(BaseEntity):
 
     __tablename__ = "accounts"
     employee = relationship('EmploymentEntity', back_populates="accounts",)
     employee_uuid = Column(UUID(as_uuid=True), ForeignKey("employment.pk_uuid"),)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/appreciatation.py` & `commons_lib-1.1.2/commons_lib/models/entities/appreciatation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, Integer, String, BIGINT, BOOLEAN, ForeignKey, Table
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity, Base
+from commons_lib.models.entities.base_entity import BaseEntity, Base
 
 
 class AppreciationEntity(BaseEntity):
     __tablename__ = "appreciations"
 
     amount: Mapped[int] = Column(Integer, nullable=False)
     organization_id: Mapped[int] = mapped_column(BIGINT, nullable=False)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/appreciatation_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/appreciatation_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, Integer, String, BIGINT, BOOLEAN, ForeignKey, Table
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity, Base
+from commons_lib.models.entities.base_entity import BaseEntity, Base
 
 
 class AppreciationEntity(BaseEntity):
     __tablename__ = "appreciations"
 
     amount: Mapped[int] = Column(Integer, nullable=False)
     message: str = Column(String, nullable=False)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/base_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/base_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/gift/vended_winning_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/gift/vended_winning_entity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlmodel import VARCHAR, Integer
 from sqlalchemy import Column, BIGINT, ForeignKey
 from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy.dialects.postgresql import UUID
 import uuid
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class VendedWinningEntity(BaseEntity):
     __tablename__ = "vended_winnings"
 
     pk_uuid = Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4)
     title = Column(VARCHAR(255), nullable=False)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/gift/winning_category_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/gift/winning_category_entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy import Column, ForeignKey,VARCHAR
 from sqlalchemy.orm import Mapped, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
 
-from server_main.models.entities import BaseEntity
+from commons_lib.models.entities import BaseEntity
 
 
 class WinningCategoryEntity(BaseEntity):
     __tablename__ = "winning_category"
 
     title = Column(VARCHAR(255), nullable=False)
     description = Column(VARCHAR(1000), nullable=True)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/gift/winning_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/gift/winning_entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlmodel import VARCHAR, Integer
 from sqlalchemy import Column, ForeignKey
 from sqlalchemy.orm import Mapped, relationship
 from sqlalchemy.dialects.postgresql import UUID
 import uuid
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class WinningEntity(BaseEntity):
     __tablename__ = "winnings"
 
     title = Column(VARCHAR(255), nullable=False)
     image = Column(VARCHAR(512), nullable=True)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/organization/company_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/organization/company_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, VARCHAR, BIGINT, ForeignKey
 from sqlalchemy.dialects.postgresql import UUID
 
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class CompanyEntity(BaseEntity):
     __tablename__ = "company"
 
     name: str = Column(VARCHAR(256), nullable=False)
     description: str = Column(VARCHAR(1000), nullable=True)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/position/position_category_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/position/position_category_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from sqlalchemy import String, Column
 from sqlalchemy.orm import relationship, Mapped
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class PositionCategoryEntity(BaseEntity):
     __tablename__ = "positiontypes"
 
     title = Column(String(255), nullable=False)
     description = Column(String(1000))
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/position/position_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/position/position_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, ForeignKey, BIGINT, VARCHAR
 from sqlalchemy.orm import Mapped, relationship, mapped_column
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class PositionEntity(BaseEntity):
     __tablename__ = "positions"
 
     position_type_uuid = Column(UUID(as_uuid=True), ForeignKey("positiontypes.pk_uuid"))  # Foreign key constraint added
     position_type = relationship('PositionCategoryEntity', back_populates='positions')
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/position/positionentity.py` & `commons_lib-1.1.2/commons_lib/models/entities/position/positionentity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, ForeignKey, BIGINT, VARCHAR
 from sqlalchemy.orm import Mapped, relationship, mapped_column
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class PositionEntity(BaseEntity):
     __tablename__ = "positions"
 
     position_type_id = Column(UUID(as_uuid=True), ForeignKey("company.pk_uuid"))
     positionType = relationship('PositionCategoryEntity', back_populates='positions')
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/transfers/transation_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/transfers/transation_entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlmodel import BIGINT
 from sqlalchemy import Column
 from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy import ForeignKey
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class TransactionEntity(BaseEntity):
     
     __tablename__ = "transactions"
 
     employee_uuid = Column(UUID(as_uuid=True), ForeignKey("employment.pk_uuid"))
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/transfers/transfer_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/transfers/transfer_entity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 from sqlalchemy import ForeignKey, Column, DateTime
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.orm import Mapped
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class TransferEntity(BaseEntity):
     __tablename__ = "transfers"
 
     from_appreciation_account_uuid: UUID = Column(UUID(as_uuid=True), ForeignKey("account.pk_uuid"),)
     to_appreciation_account_uuid: UUID = Column(UUID(as_uuid=True), ForeignKey("account.pk_uuid"),)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/user/employment_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/user/employment_entity.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy.orm import relationship
 from sqlalchemy import ForeignKey, Boolean, Column, VARCHAR,  BIGINT
 from sqlalchemy.dialects.postgresql import UUID
 
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class EmploymentEntity(BaseEntity):
     __tablename__ = "employment"
 
     employee_uuid = Column(UUID(as_uuid=True), ForeignKey('employees.pk_uuid'))
     employee = relationship('EmployeeEntity', back_populates='employments')
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/user/user_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/user/user_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy import DateTime, String, Boolean
 from sqlalchemy.orm import Mapped, mapped_column
 from sqlmodel import VARCHAR
 from datetime import datetime
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class UserEntity(BaseEntity):
     __abstract__ = True
 
     first_name: Mapped[str] = mapped_column(type_=String(255), nullable=False)
     last_name: Mapped[str] = mapped_column(VARCHAR(255), nullable=False)
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/values/org_behavior_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/values/org_behavior_entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, VARCHAR, Table, ForeignKey
 from sqlalchemy.orm import Mapped, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity, Base
+from commons_lib.models.entities.base_entity import BaseEntity, Base
 
 
 class OrgBehaviorEntity(BaseEntity):
         __tablename__ = "organizationbehaviors"
 
         title: Mapped[str] = Column(VARCHAR(255))
         description: Mapped[str] = Column(VARCHAR(1000))
```

### Comparing `commons_lib-1.1.1/commons_lib/models/entities/values/org_value_entity.py` & `commons_lib-1.1.2/commons_lib/models/entities/values/org_value_entity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, VARCHAR, BIGINT, ForeignKey
 from sqlalchemy.orm import Mapped, relationship, mapped_column
 from sqlalchemy.dialects.postgresql import UUID
 
-from server_main.models.entities.base_entity import BaseEntity
+from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class OrgValueEntity(BaseEntity):
     __tablename__ = "organizationvalues"
 
     title: Mapped[str] = Column(VARCHAR(255), nullable=False)
     description: Mapped[str] = Column(VARCHAR(1000))
```

### Comparing `commons_lib-1.1.1/commons_lib/models/records/base_record.py` & `commons_lib-1.1.2/commons_lib/models/records/base_record.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/commons_lib/utils/singleton.py` & `commons_lib-1.1.2/commons_lib/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/commons_lib/utils/ttl_cache.py` & `commons_lib-1.1.2/commons_lib/utils/ttl_cache.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/docs/Makefile` & `commons_lib-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/docs/conf.py` & `commons_lib-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/docs/make.bat` & `commons_lib-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/docs/pylint.md` & `commons_lib-1.1.2/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/pyproject.toml` & `commons_lib-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/tests/conftest.py` & `commons_lib-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/tests/test_methods.py` & `commons_lib-1.1.2/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.1/PKG-INFO` & `commons_lib-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commons_lib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Arad PassioNikoo
 Author-email: Mehdi Einali <einali@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

