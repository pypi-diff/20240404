# Comparing `tmp/commons_lib-1.1.0.tar.gz` & `tmp/commons_lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commons_lib-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "commons_lib-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `commons_lib-1.1.0.tar` & `commons_lib-1.1.1.tar`

### file list

```diff
@@ -1,63 +1,68 @@
--rw-r--r--   0        0        0     1889 2024-02-14 08:30:07.100686 commons_lib-1.1.0/.gitignore
--rw-r--r--   0        0        0      166 2024-02-14 08:14:46.191466 commons_lib-1.1.0/README.md
--rw-r--r--   0        0        0       42 2024-02-14 08:14:46.191612 commons_lib-1.1.0/commons_lib/README.md
--rw-r--r--   0        0        0       21 2024-02-18 12:59:40.109094 commons_lib-1.1.0/commons_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.191797 commons_lib-1.1.0/commons_lib/models/__init__.py
--rw-r--r--   0        0        0     1022 2024-02-18 11:09:40.528145 commons_lib-1.1.0/commons_lib/models/entities/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.831991 commons_lib-1.1.0/commons_lib/models/entities/accounts/__init__.py
--rw-r--r--   0        0        0      416 2024-02-18 12:57:41.603213 commons_lib-1.1.0/commons_lib/models/entities/accounts/account_category_entity.py
--rw-r--r--   0        0        0      839 2024-02-18 12:57:41.609742 commons_lib-1.1.0/commons_lib/models/entities/accounts/accountـentity.py
--rw-r--r--   0        0        0     1545 2024-02-14 09:26:54.173812 commons_lib-1.1.0/commons_lib/models/entities/appreciatation.py
--rw-r--r--   0        0        0     1489 2024-02-18 12:57:41.615925 commons_lib-1.1.0/commons_lib/models/entities/appreciatation_entity.py
--rw-r--r--   0        0        0      824 2024-02-18 12:17:31.143492 commons_lib-1.1.0/commons_lib/models/entities/base_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.835239 commons_lib-1.1.0/commons_lib/models/entities/gift/__init__.py
--rw-r--r--   0        0        0      454 2024-02-18 12:57:41.617348 commons_lib-1.1.0/commons_lib/models/entities/gift/redeem_entity.py
--rw-r--r--   0        0        0      570 2024-02-18 12:57:41.614691 commons_lib-1.1.0/commons_lib/models/entities/gift/winning_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.838587 commons_lib-1.1.0/commons_lib/models/entities/organization/__init__.py
--rw-r--r--   0        0        0      329 2024-02-18 12:57:41.608323 commons_lib-1.1.0/commons_lib/models/entities/organization/company_entity.py
--rw-r--r--   0        0        0      289 2024-02-18 12:57:11.460485 commons_lib-1.1.0/commons_lib/models/entities/organization/sub_org_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.841515 commons_lib-1.1.0/commons_lib/models/entities/permissions/__init__.py
--rw-r--r--   0        0        0      410 2024-02-18 12:57:41.610901 commons_lib-1.1.0/commons_lib/models/entities/permissions/permission_entity.py
--rw-r--r--   0        0        0      267 2024-02-18 12:57:11.773959 commons_lib-1.1.0/commons_lib/models/entities/permissions/role_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.844104 commons_lib-1.1.0/commons_lib/models/entities/position/__init__.py
--rw-r--r--   0        0        0      573 2024-02-18 12:57:41.601100 commons_lib-1.1.0/commons_lib/models/entities/position/position_category_entity.py
--rw-r--r--   0        0        0     1375 2024-02-18 12:57:41.620792 commons_lib-1.1.0/commons_lib/models/entities/position/position_entity.py
--rw-r--r--   0        0        0      984 2024-02-14 09:26:54.200236 commons_lib-1.1.0/commons_lib/models/entities/position/positionentity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.845299 commons_lib-1.1.0/commons_lib/models/entities/transfers/__init__.py
--rw-r--r--   0        0        0      907 2024-02-18 12:57:41.606718 commons_lib-1.1.0/commons_lib/models/entities/transfers/transation_entity.py
--rw-r--r--   0        0        0      751 2024-02-18 12:57:41.596548 commons_lib-1.1.0/commons_lib/models/entities/transfers/transfer_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.846343 commons_lib-1.1.0/commons_lib/models/entities/user/__init__.py
--rw-r--r--   0        0        0      262 2024-02-14 09:26:54.183429 commons_lib-1.1.0/commons_lib/models/entities/user/employee_entiry.py
--rw-r--r--   0        0        0      258 2024-02-18 12:57:41.618517 commons_lib-1.1.0/commons_lib/models/entities/user/employee_entity.py
--rw-r--r--   0        0        0     1671 2024-02-18 12:57:41.619674 commons_lib-1.1.0/commons_lib/models/entities/user/employment_entity.py
--rw-r--r--   0        0        0      945 2024-02-18 12:57:41.621878 commons_lib-1.1.0/commons_lib/models/entities/user/user_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.848188 commons_lib-1.1.0/commons_lib/models/entities/values/__init__.py
--rw-r--r--   0        0        0      954 2024-02-18 12:57:41.613397 commons_lib-1.1.0/commons_lib/models/entities/values/org_behavior_entity.py
--rw-r--r--   0        0        0      549 2024-02-18 12:57:41.612151 commons_lib-1.1.0/commons_lib/models/entities/values/org_value_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.194923 commons_lib-1.1.0/commons_lib/models/enums/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195024 commons_lib-1.1.0/commons_lib/models/records/__init__.py
--rw-r--r--   0        0        0      844 2024-02-14 08:14:46.195134 commons_lib-1.1.0/commons_lib/models/records/base_record.py
--rw-r--r--   0        0        0      283 2024-02-14 08:14:46.195227 commons_lib-1.1.0/commons_lib/models/records/records.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195319 commons_lib-1.1.0/commons_lib/utils/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-14 08:14:46.195430 commons_lib-1.1.0/commons_lib/utils/singleton.py
--rw-r--r--   0        0        0     1243 2024-02-14 08:14:46.195529 commons_lib-1.1.0/commons_lib/utils/ttl_cache.py
--rw-r--r--   0        0        0      634 2024-02-14 08:14:46.195689 commons_lib-1.1.0/docs/Makefile
--rw-r--r--   0        0        0     2329 2024-02-14 08:14:46.195793 commons_lib-1.1.0/docs/conf.py
--rw-r--r--   0        0        0      360 2024-02-14 08:14:46.195888 commons_lib-1.1.0/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-02-14 08:14:46.195976 commons_lib-1.1.0/docs/developer.md
--rw-r--r--   0        0        0      468 2024-02-14 08:14:46.196071 commons_lib-1.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2024-02-14 08:14:46.196170 commons_lib-1.1.0/docs/make.bat
--rw-r--r--   0        0        0       57 2024-02-14 08:14:46.196268 commons_lib-1.1.0/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-02-14 08:14:46.196365 commons_lib-1.1.0/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-02-14 08:14:46.196548 commons_lib-1.1.0/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-02-14 08:14:46.196639 commons_lib-1.1.0/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-02-14 08:14:46.196736 commons_lib-1.1.0/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      427 2024-02-14 08:14:46.196827 commons_lib-1.1.0/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-02-14 08:14:46.196899 commons_lib-1.1.0/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-02-14 08:14:46.196978 commons_lib-1.1.0/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-02-14 08:14:46.197063 commons_lib-1.1.0/docs/workflows.md
--rw-r--r--   0        0        0     6070 2024-02-14 08:14:46.197192 commons_lib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      989 2024-02-14 08:14:46.197324 commons_lib-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1217 2024-02-14 08:14:46.197423 commons_lib-1.1.0/tests/test_methods.py
--rw-r--r--   0        0        0      328 2024-02-14 08:14:46.197514 commons_lib-1.1.0/tests/test_ttl_cache.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 commons_lib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1889 2024-02-14 08:30:07.100686 commons_lib-1.1.1/.gitignore
+-rw-r--r--   0        0        0      166 2024-02-14 08:14:46.191466 commons_lib-1.1.1/README.md
+-rw-r--r--   0        0        0       42 2024-02-14 08:14:46.191612 commons_lib-1.1.1/commons_lib/README.md
+-rw-r--r--   0        0        0       21 2024-03-24 11:38:05.051644 commons_lib-1.1.1/commons_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.191797 commons_lib-1.1.1/commons_lib/models/__init__.py
+-rw-r--r--   0        0        0     1086 2024-03-30 10:42:56.269827 commons_lib-1.1.1/commons_lib/models/entities/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.831991 commons_lib-1.1.1/commons_lib/models/entities/accounts/__init__.py
+-rw-r--r--   0        0        0      587 2024-03-27 15:07:04.860134 commons_lib-1.1.1/commons_lib/models/entities/accounts/account_category_entity.py
+-rw-r--r--   0        0        0      888 2024-03-27 12:25:52.776380 commons_lib-1.1.1/commons_lib/models/entities/accounts/accountـentity.py
+-rw-r--r--   0        0        0     1545 2024-03-27 12:25:52.776652 commons_lib-1.1.1/commons_lib/models/entities/appreciatation.py
+-rw-r--r--   0        0        0     1489 2024-03-27 12:25:52.776752 commons_lib-1.1.1/commons_lib/models/entities/appreciatation_entity.py
+-rw-r--r--   0        0        0      886 2024-03-27 12:26:07.182779 commons_lib-1.1.1/commons_lib/models/entities/base_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.835239 commons_lib-1.1.1/commons_lib/models/entities/gift/__init__.py
+-rw-r--r--   0        0        0      738 2024-03-27 12:26:10.061669 commons_lib-1.1.1/commons_lib/models/entities/gift/redeem_entity.py
+-rw-r--r--   0        0        0      734 2024-03-27 12:26:11.213548 commons_lib-1.1.1/commons_lib/models/entities/gift/vended_winning_entity.py
+-rw-r--r--   0        0        0      541 2024-03-30 10:45:58.246339 commons_lib-1.1.1/commons_lib/models/entities/gift/winning_category_entity.py
+-rw-r--r--   0        0        0     1090 2024-03-30 10:49:28.750810 commons_lib-1.1.1/commons_lib/models/entities/gift/winning_entity.py
+-rw-r--r--   0        0        0      357 2024-03-27 12:26:11.858360 commons_lib-1.1.1/commons_lib/models/entities/gift/winning_vendors.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.838587 commons_lib-1.1.1/commons_lib/models/entities/organization/__init__.py
+-rw-r--r--   0        0        0      799 2024-03-28 11:23:13.314366 commons_lib-1.1.1/commons_lib/models/entities/organization/company_entity.py
+-rw-r--r--   0        0        0      289 2024-03-27 12:25:52.778091 commons_lib-1.1.1/commons_lib/models/entities/organization/sub_org_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.841515 commons_lib-1.1.1/commons_lib/models/entities/permissions/__init__.py
+-rw-r--r--   0        0        0      410 2024-03-27 12:25:52.778412 commons_lib-1.1.1/commons_lib/models/entities/permissions/permission_entity.py
+-rw-r--r--   0        0        0      267 2024-03-27 12:25:52.778656 commons_lib-1.1.1/commons_lib/models/entities/permissions/role_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.844104 commons_lib-1.1.1/commons_lib/models/entities/position/__init__.py
+-rw-r--r--   0        0        0      573 2024-03-27 12:25:52.778904 commons_lib-1.1.1/commons_lib/models/entities/position/position_category_entity.py
+-rw-r--r--   0        0        0     1375 2024-03-27 12:25:52.779013 commons_lib-1.1.1/commons_lib/models/entities/position/position_entity.py
+-rw-r--r--   0        0        0      984 2024-03-27 12:25:52.779117 commons_lib-1.1.1/commons_lib/models/entities/position/positionentity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.845299 commons_lib-1.1.1/commons_lib/models/entities/transfers/__init__.py
+-rw-r--r--   0        0        0      284 2024-03-27 12:25:45.642872 commons_lib-1.1.1/commons_lib/models/entities/transfers/transaction_category_entity.py
+-rw-r--r--   0        0        0      907 2024-03-27 12:26:10.732404 commons_lib-1.1.1/commons_lib/models/entities/transfers/transation_entity.py
+-rw-r--r--   0        0        0      259 2024-03-27 12:25:45.643291 commons_lib-1.1.1/commons_lib/models/entities/transfers/transfer_category_entity.py
+-rw-r--r--   0        0        0      751 2024-03-27 12:26:10.884842 commons_lib-1.1.1/commons_lib/models/entities/transfers/transfer_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.846343 commons_lib-1.1.1/commons_lib/models/entities/user/__init__.py
+-rw-r--r--   0        0        0      262 2024-03-27 12:25:52.779737 commons_lib-1.1.1/commons_lib/models/entities/user/employee_entiry.py
+-rw-r--r--   0        0        0      258 2024-03-27 12:25:52.779862 commons_lib-1.1.1/commons_lib/models/entities/user/employee_entity.py
+-rw-r--r--   0        0        0     1692 2024-03-27 12:26:09.243772 commons_lib-1.1.1/commons_lib/models/entities/user/employment_entity.py
+-rw-r--r--   0        0        0      945 2024-03-27 12:26:11.047431 commons_lib-1.1.1/commons_lib/models/entities/user/user_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.848188 commons_lib-1.1.1/commons_lib/models/entities/values/__init__.py
+-rw-r--r--   0        0        0      954 2024-03-27 17:14:18.715525 commons_lib-1.1.1/commons_lib/models/entities/values/org_behavior_entity.py
+-rw-r--r--   0        0        0      618 2024-03-27 17:14:18.704419 commons_lib-1.1.1/commons_lib/models/entities/values/org_value_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.194923 commons_lib-1.1.1/commons_lib/models/enums/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195024 commons_lib-1.1.1/commons_lib/models/records/__init__.py
+-rw-r--r--   0        0        0      844 2024-02-14 08:14:46.195134 commons_lib-1.1.1/commons_lib/models/records/base_record.py
+-rw-r--r--   0        0        0      283 2024-02-14 08:14:46.195227 commons_lib-1.1.1/commons_lib/models/records/records.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195319 commons_lib-1.1.1/commons_lib/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-14 08:14:46.195430 commons_lib-1.1.1/commons_lib/utils/singleton.py
+-rw-r--r--   0        0        0     1243 2024-02-14 08:14:46.195529 commons_lib-1.1.1/commons_lib/utils/ttl_cache.py
+-rw-r--r--   0        0        0      634 2024-02-14 08:14:46.195689 commons_lib-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0     2329 2024-02-14 08:14:46.195793 commons_lib-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-02-14 08:14:46.195888 commons_lib-1.1.1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-02-14 08:14:46.195976 commons_lib-1.1.1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-02-14 08:14:46.196071 commons_lib-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-02-14 08:14:46.196170 commons_lib-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-02-14 08:14:46.196268 commons_lib-1.1.1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-02-14 08:14:46.196365 commons_lib-1.1.1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-02-14 08:14:46.196548 commons_lib-1.1.1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-02-14 08:14:46.196639 commons_lib-1.1.1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-02-14 08:14:46.196736 commons_lib-1.1.1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      427 2024-02-14 08:14:46.196827 commons_lib-1.1.1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-02-14 08:14:46.196899 commons_lib-1.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-02-14 08:14:46.196978 commons_lib-1.1.1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-02-14 08:14:46.197063 commons_lib-1.1.1/docs/workflows.md
+-rw-r--r--   0        0        0     6070 2024-02-14 08:14:46.197192 commons_lib-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      989 2024-02-14 08:14:46.197324 commons_lib-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1217 2024-02-14 08:14:46.197423 commons_lib-1.1.1/tests/test_methods.py
+-rw-r--r--   0        0        0      328 2024-02-14 08:14:46.197514 commons_lib-1.1.1/tests/test_ttl_cache.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 commons_lib-1.1.1/PKG-INFO
```

### Comparing `commons_lib-1.1.0/.gitignore` & `commons_lib-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/__init__.py` & `commons_lib-1.1.1/commons_lib/models/entities/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .base_entity import Base, BaseEntity
 from .accounts.account_category_entity import AccountCategoryEntity
 from .accounts.accountـentity import AccountEntity
 from .gift.winning_entity import WinningEntity
+from .gift.winning_category_entity import WinningCategoryEntity
 from .gift.redeem_entity import RedeemEntity
 from .organization.company_entity import CompanyEntity
 from .organization.sub_org_entity import SubOrganizationEntity
 from .permissions.permission_entity import PermissionEntity
 from .permissions.role_entity import RoleEntity
 from .transfers.transfer_entity import TransferEntity
 from .transfers.transation_entity import TransactionEntity
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/accounts/accountـentity.py` & `commons_lib-1.1.1/commons_lib/models/entities/accounts/accountـentity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import date
 from sqlalchemy.dialects.postgresql import UUID
 
 from sqlalchemy import Column, BIGINT, ForeignKey, VARCHAR, DateTime
 from sqlalchemy.orm import relationship, Mapped
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class AccountEntity(BaseEntity):
 
     __tablename__ = "accounts"
     employee = relationship('EmploymentEntity', back_populates="accounts",)
     employee_uuid = Column(UUID(as_uuid=True), ForeignKey("employment.pk_uuid"),)
     appreciation_balance: int = Column(BIGINT, nullable=True)
     personal_balance: int = Column(BIGINT, nullable=True)
+    balance: int = Column(BIGINT, nullable=True)
     account_type = relationship('AccountCategoryEntity', back_populates="accounts",)
     account_type_uuid = Column(UUID(as_uuid=True), ForeignKey("accounts_type.pk_uuid"),)
     expire_date: Mapped[date] = Column(DateTime, nullable=True)
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/appreciatation.py` & `commons_lib-1.1.1/commons_lib/models/entities/appreciatation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, Integer, String, BIGINT, BOOLEAN, ForeignKey, Table
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity, Base
+from server_main.models.entities.base_entity import BaseEntity, Base
 
 
 class AppreciationEntity(BaseEntity):
     __tablename__ = "appreciations"
 
     amount: Mapped[int] = Column(Integer, nullable=False)
     organization_id: Mapped[int] = mapped_column(BIGINT, nullable=False)
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/appreciatation_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/appreciatation_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, Integer, String, BIGINT, BOOLEAN, ForeignKey, Table
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity, Base
+from server_main.models.entities.base_entity import BaseEntity, Base
 
 
 class AppreciationEntity(BaseEntity):
     __tablename__ = "appreciations"
 
     amount: Mapped[int] = Column(Integer, nullable=False)
     message: str = Column(String, nullable=False)
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/base_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/base_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,12 +14,15 @@
 
     pk_uuid = Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4)
     created_at = Column(DateTime, nullable=False, default=datetime.utcnow)
     created_by = Column(BigInteger, nullable=True)
     updated_at = Column(DateTime, nullable=True, default=datetime.utcnow)
     updated_by = Column(BigInteger, nullable=True)
     is_deleted = Column(Boolean, nullable=True, default=False)
+    is_active: Mapped[bool] = Column(Boolean, default=True)
+
+
 
 
     @staticmethod
     def get_id_field_name()->str:
         return "pk_uuid"
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/gift/winning_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/values/org_value_entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from sqlmodel import VARCHAR, Integer
-from sqlalchemy import Column, BIGINT, ForeignKey
-from sqlalchemy.orm import Mapped, mapped_column
+from sqlalchemy import Column, VARCHAR, BIGINT, ForeignKey
+from sqlalchemy.orm import Mapped, relationship, mapped_column
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
-class WinningEntity(BaseEntity):
-    __tablename__ = "winnings"
+class OrgValueEntity(BaseEntity):
+    __tablename__ = "organizationvalues"
 
     title: Mapped[str] = Column(VARCHAR(255), nullable=False)
     description: Mapped[str] = Column(VARCHAR(1000))
-    price: Mapped[int] = Column(Integer, nullable=False)
+
+    behaviors = relationship("OrgBehaviorEntity", secondary="orgvaluebehavior", back_populates="values")
     organization_uuid = Column(UUID(as_uuid=True), ForeignKey("company.pk_uuid"))
+
+
+
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/position/position_category_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/position/position_category_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from sqlalchemy import String, Column
 from sqlalchemy.orm import relationship, Mapped
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class PositionCategoryEntity(BaseEntity):
     __tablename__ = "positiontypes"
 
     title = Column(String(255), nullable=False)
     description = Column(String(1000))
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/position/position_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/position/position_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, ForeignKey, BIGINT, VARCHAR
 from sqlalchemy.orm import Mapped, relationship, mapped_column
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class PositionEntity(BaseEntity):
     __tablename__ = "positions"
 
     position_type_uuid = Column(UUID(as_uuid=True), ForeignKey("positiontypes.pk_uuid"))  # Foreign key constraint added
     position_type = relationship('PositionCategoryEntity', back_populates='positions')
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/position/positionentity.py` & `commons_lib-1.1.1/commons_lib/models/entities/position/positionentity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, ForeignKey, BIGINT, VARCHAR
 from sqlalchemy.orm import Mapped, relationship, mapped_column
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class PositionEntity(BaseEntity):
     __tablename__ = "positions"
 
     position_type_id = Column(UUID(as_uuid=True), ForeignKey("company.pk_uuid"))
     positionType = relationship('PositionCategoryEntity', back_populates='positions')
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/transfers/transation_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/transfers/transation_entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlmodel import BIGINT
 from sqlalchemy import Column
 from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy import ForeignKey
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class TransactionEntity(BaseEntity):
     
     __tablename__ = "transactions"
 
     employee_uuid = Column(UUID(as_uuid=True), ForeignKey("employment.pk_uuid"))
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/transfers/transfer_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/transfers/transfer_entity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 from sqlalchemy import ForeignKey, Column, DateTime
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.orm import Mapped
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class TransferEntity(BaseEntity):
     __tablename__ = "transfers"
 
     from_appreciation_account_uuid: UUID = Column(UUID(as_uuid=True), ForeignKey("account.pk_uuid"),)
     to_appreciation_account_uuid: UUID = Column(UUID(as_uuid=True), ForeignKey("account.pk_uuid"),)
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/user/employment_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/user/employment_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from sqlalchemy.orm import relationship
-from sqlalchemy import ForeignKey
-from sqlalchemy import Column, BIGINT
-from sqlalchemy import VARCHAR
+from sqlalchemy import ForeignKey, Boolean, Column, VARCHAR,  BIGINT
 from sqlalchemy.dialects.postgresql import UUID
 
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class EmploymentEntity(BaseEntity):
     __tablename__ = "employment"
 
     employee_uuid = Column(UUID(as_uuid=True), ForeignKey('employees.pk_uuid'))
     employee = relationship('EmployeeEntity', back_populates='employments')
@@ -26,7 +24,9 @@
     transactions = relationship('TransactionEntity', back_populates='employee')
     organization_uuid = Column(UUID(as_uuid=True), ForeignKey("company.pk_uuid"))
 
     sent_appreciations = relationship("AppreciationEntity", back_populates="from_employment",
                                       foreign_keys="AppreciationEntity.from_employment_uuid")
     received_appreciations = relationship("AppreciationEntity", back_populates="to_employment",
                                           foreign_keys="AppreciationEntity.to_employment_uuid")
+    is_manager: bool = Column(Boolean, default=False)
+
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/user/user_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/user/user_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy import DateTime, String, Boolean
 from sqlalchemy.orm import Mapped, mapped_column
 from sqlmodel import VARCHAR
 from datetime import datetime
 
-from commons_lib.models.entities.base_entity import BaseEntity
+from server_main.models.entities.base_entity import BaseEntity
 
 
 class UserEntity(BaseEntity):
     __abstract__ = True
 
     first_name: Mapped[str] = mapped_column(type_=String(255), nullable=False)
     last_name: Mapped[str] = mapped_column(VARCHAR(255), nullable=False)
```

### Comparing `commons_lib-1.1.0/commons_lib/models/entities/values/org_behavior_entity.py` & `commons_lib-1.1.1/commons_lib/models/entities/values/org_behavior_entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import Column, VARCHAR, Table, ForeignKey
 from sqlalchemy.orm import Mapped, relationship
 from sqlalchemy.dialects.postgresql import UUID
 
-from commons_lib.models.entities.base_entity import BaseEntity, Base
+from server_main.models.entities.base_entity import BaseEntity, Base
 
 
 class OrgBehaviorEntity(BaseEntity):
         __tablename__ = "organizationbehaviors"
 
         title: Mapped[str] = Column(VARCHAR(255))
         description: Mapped[str] = Column(VARCHAR(1000))
@@ -14,10 +14,10 @@
         values = relationship("OrgValueEntity", secondary="orgvaluebehavior", back_populates="behaviors")
         appreciations = relationship("AppreciationEntity", secondary="appreciationbehavior", back_populates="behaviors")
 
 
 org_value_behavior = Table(
     "orgvaluebehavior",
     Base.metadata,
-    Column("org_value_pk_uuid", UUID(as_uuid=True), ForeignKey("organizationValues.pk_uuid"), primary_key=True),
+    Column("org_value_pk_uuid", UUID(as_uuid=True), ForeignKey("organizationvalues.pk_uuid"), primary_key=True),
     Column("org_behavior_pk_uuid", UUID(as_uuid=True), ForeignKey("organizationbehaviors.pk_uuid"), primary_key=True),
 )
```

### Comparing `commons_lib-1.1.0/commons_lib/models/records/base_record.py` & `commons_lib-1.1.1/commons_lib/models/records/base_record.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/commons_lib/utils/singleton.py` & `commons_lib-1.1.1/commons_lib/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/commons_lib/utils/ttl_cache.py` & `commons_lib-1.1.1/commons_lib/utils/ttl_cache.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/docs/Makefile` & `commons_lib-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/docs/conf.py` & `commons_lib-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/docs/make.bat` & `commons_lib-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/docs/pylint.md` & `commons_lib-1.1.1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/pyproject.toml` & `commons_lib-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/tests/conftest.py` & `commons_lib-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/tests/test_methods.py` & `commons_lib-1.1.1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.0/PKG-INFO` & `commons_lib-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commons_lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Arad PassioNikoo
 Author-email: Mehdi Einali <einali@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

