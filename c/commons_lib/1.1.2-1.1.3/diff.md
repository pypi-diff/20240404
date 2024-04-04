# Comparing `tmp/commons_lib-1.1.2.tar.gz` & `tmp/commons_lib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commons_lib-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "commons_lib-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `commons_lib-1.1.2.tar` & `commons_lib-1.1.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1889 2024-02-14 08:30:07.100686 commons_lib-1.1.2/.gitignore
--rw-r--r--   0        0        0      166 2024-02-14 08:14:46.191466 commons_lib-1.1.2/README.md
--rw-r--r--   0        0        0       42 2024-02-14 08:14:46.191612 commons_lib-1.1.2/commons_lib/README.md
--rw-r--r--   0        0        0       21 2024-04-04 07:20:01.982572 commons_lib-1.1.2/commons_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.191797 commons_lib-1.1.2/commons_lib/models/__init__.py
--rw-r--r--   0        0        0     1086 2024-03-30 10:42:56.269827 commons_lib-1.1.2/commons_lib/models/entities/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.831991 commons_lib-1.1.2/commons_lib/models/entities/accounts/__init__.py
--rw-r--r--   0        0        0      587 2024-04-04 07:18:47.788258 commons_lib-1.1.2/commons_lib/models/entities/accounts/account_category_entity.py
--rw-r--r--   0        0        0      888 2024-04-04 07:18:47.786404 commons_lib-1.1.2/commons_lib/models/entities/accounts/accountـentity.py
--rw-r--r--   0        0        0     1545 2024-04-04 07:18:47.769117 commons_lib-1.1.2/commons_lib/models/entities/appreciatation.py
--rw-r--r--   0        0        0     1489 2024-04-04 07:18:47.754825 commons_lib-1.1.2/commons_lib/models/entities/appreciatation_entity.py
--rw-r--r--   0        0        0      886 2024-03-27 12:26:07.182779 commons_lib-1.1.2/commons_lib/models/entities/base_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.835239 commons_lib-1.1.2/commons_lib/models/entities/gift/__init__.py
--rw-r--r--   0        0        0      738 2024-04-04 07:18:47.767377 commons_lib-1.1.2/commons_lib/models/entities/gift/redeem_entity.py
--rw-r--r--   0        0        0      734 2024-04-04 07:18:47.791017 commons_lib-1.1.2/commons_lib/models/entities/gift/vended_winning_entity.py
--rw-r--r--   0        0        0      541 2024-04-04 07:18:47.779188 commons_lib-1.1.2/commons_lib/models/entities/gift/winning_category_entity.py
--rw-r--r--   0        0        0     1090 2024-04-04 07:18:47.784181 commons_lib-1.1.2/commons_lib/models/entities/gift/winning_entity.py
--rw-r--r--   0        0        0      357 2024-04-04 07:18:47.758854 commons_lib-1.1.2/commons_lib/models/entities/gift/winning_vendors.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.838587 commons_lib-1.1.2/commons_lib/models/entities/organization/__init__.py
--rw-r--r--   0        0        0      799 2024-04-04 07:18:47.782939 commons_lib-1.1.2/commons_lib/models/entities/organization/company_entity.py
--rw-r--r--   0        0        0      289 2024-04-04 07:18:47.792138 commons_lib-1.1.2/commons_lib/models/entities/organization/sub_org_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.841515 commons_lib-1.1.2/commons_lib/models/entities/permissions/__init__.py
--rw-r--r--   0        0        0      410 2024-04-04 07:18:47.798616 commons_lib-1.1.2/commons_lib/models/entities/permissions/permission_entity.py
--rw-r--r--   0        0        0      267 2024-04-04 07:18:47.795119 commons_lib-1.1.2/commons_lib/models/entities/permissions/role_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.844104 commons_lib-1.1.2/commons_lib/models/entities/position/__init__.py
--rw-r--r--   0        0        0      573 2024-04-04 07:18:47.797505 commons_lib-1.1.2/commons_lib/models/entities/position/position_category_entity.py
--rw-r--r--   0        0        0     1375 2024-04-04 07:18:47.777854 commons_lib-1.1.2/commons_lib/models/entities/position/position_entity.py
--rw-r--r--   0        0        0      984 2024-04-04 07:18:47.765683 commons_lib-1.1.2/commons_lib/models/entities/position/positionentity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.845299 commons_lib-1.1.2/commons_lib/models/entities/transfers/__init__.py
--rw-r--r--   0        0        0      284 2024-04-04 07:18:47.761765 commons_lib-1.1.2/commons_lib/models/entities/transfers/transaction_category_entity.py
--rw-r--r--   0        0        0      907 2024-04-04 07:18:47.763846 commons_lib-1.1.2/commons_lib/models/entities/transfers/transation_entity.py
--rw-r--r--   0        0        0      259 2024-04-04 07:18:47.771690 commons_lib-1.1.2/commons_lib/models/entities/transfers/transfer_category_entity.py
--rw-r--r--   0        0        0      751 2024-04-04 07:18:47.772862 commons_lib-1.1.2/commons_lib/models/entities/transfers/transfer_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.846343 commons_lib-1.1.2/commons_lib/models/entities/user/__init__.py
--rw-r--r--   0        0        0      262 2024-04-04 07:18:47.776564 commons_lib-1.1.2/commons_lib/models/entities/user/employee_entiry.py
--rw-r--r--   0        0        0      258 2024-04-04 07:18:47.785209 commons_lib-1.1.2/commons_lib/models/entities/user/employee_entity.py
--rw-r--r--   0        0        0     1692 2024-04-04 07:18:47.774047 commons_lib-1.1.2/commons_lib/models/entities/user/employment_entity.py
--rw-r--r--   0        0        0      945 2024-04-04 07:18:47.781604 commons_lib-1.1.2/commons_lib/models/entities/user/user_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 09:43:53.848188 commons_lib-1.1.2/commons_lib/models/entities/values/__init__.py
--rw-r--r--   0        0        0      954 2024-04-04 07:18:47.775381 commons_lib-1.1.2/commons_lib/models/entities/values/org_behavior_entity.py
--rw-r--r--   0        0        0      618 2024-04-04 07:18:47.770427 commons_lib-1.1.2/commons_lib/models/entities/values/org_value_entity.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.194923 commons_lib-1.1.2/commons_lib/models/enums/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195024 commons_lib-1.1.2/commons_lib/models/records/__init__.py
--rw-r--r--   0        0        0      844 2024-02-14 08:14:46.195134 commons_lib-1.1.2/commons_lib/models/records/base_record.py
--rw-r--r--   0        0        0      283 2024-02-14 08:14:46.195227 commons_lib-1.1.2/commons_lib/models/records/records.py
--rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195319 commons_lib-1.1.2/commons_lib/utils/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-14 08:14:46.195430 commons_lib-1.1.2/commons_lib/utils/singleton.py
--rw-r--r--   0        0        0     1243 2024-02-14 08:14:46.195529 commons_lib-1.1.2/commons_lib/utils/ttl_cache.py
--rw-r--r--   0        0        0      634 2024-02-14 08:14:46.195689 commons_lib-1.1.2/docs/Makefile
--rw-r--r--   0        0        0     2329 2024-02-14 08:14:46.195793 commons_lib-1.1.2/docs/conf.py
--rw-r--r--   0        0        0      360 2024-02-14 08:14:46.195888 commons_lib-1.1.2/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-02-14 08:14:46.195976 commons_lib-1.1.2/docs/developer.md
--rw-r--r--   0        0        0      468 2024-02-14 08:14:46.196071 commons_lib-1.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2024-02-14 08:14:46.196170 commons_lib-1.1.2/docs/make.bat
--rw-r--r--   0        0        0       57 2024-02-14 08:14:46.196268 commons_lib-1.1.2/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-02-14 08:14:46.196365 commons_lib-1.1.2/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-02-14 08:14:46.196548 commons_lib-1.1.2/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-02-14 08:14:46.196639 commons_lib-1.1.2/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-02-14 08:14:46.196736 commons_lib-1.1.2/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      427 2024-02-14 08:14:46.196827 commons_lib-1.1.2/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-02-14 08:14:46.196899 commons_lib-1.1.2/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-02-14 08:14:46.196978 commons_lib-1.1.2/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-02-14 08:14:46.197063 commons_lib-1.1.2/docs/workflows.md
--rw-r--r--   0        0        0     6070 2024-02-14 08:14:46.197192 commons_lib-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      989 2024-02-14 08:14:46.197324 commons_lib-1.1.2/tests/conftest.py
--rw-r--r--   0        0        0     1217 2024-02-14 08:14:46.197423 commons_lib-1.1.2/tests/test_methods.py
--rw-r--r--   0        0        0      328 2024-02-14 08:14:46.197514 commons_lib-1.1.2/tests/test_ttl_cache.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 commons_lib-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1889 2024-02-14 08:30:07.100686 commons_lib-1.1.3/.gitignore
+-rw-r--r--   0        0        0      166 2024-02-14 08:14:46.191466 commons_lib-1.1.3/README.md
+-rw-r--r--   0        0        0       42 2024-02-14 08:14:46.191612 commons_lib-1.1.3/commons_lib/README.md
+-rw-r--r--   0        0        0       21 2024-04-04 08:07:24.470065 commons_lib-1.1.3/commons_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.191797 commons_lib-1.1.3/commons_lib/models/__init__.py
+-rw-r--r--   0        0        0     1086 2024-03-30 10:42:56.269827 commons_lib-1.1.3/commons_lib/models/entities/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.831991 commons_lib-1.1.3/commons_lib/models/entities/accounts/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-04 07:18:47.788258 commons_lib-1.1.3/commons_lib/models/entities/accounts/account_category_entity.py
+-rw-r--r--   0        0        0      888 2024-04-04 07:18:47.786404 commons_lib-1.1.3/commons_lib/models/entities/accounts/accountـentity.py
+-rw-r--r--   0        0        0     1545 2024-04-04 07:18:47.769117 commons_lib-1.1.3/commons_lib/models/entities/appreciatation.py
+-rw-r--r--   0        0        0     1489 2024-04-04 07:18:47.754825 commons_lib-1.1.3/commons_lib/models/entities/appreciatation_entity.py
+-rw-r--r--   0        0        0      886 2024-03-27 12:26:07.182779 commons_lib-1.1.3/commons_lib/models/entities/base_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.835239 commons_lib-1.1.3/commons_lib/models/entities/gift/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-04 07:18:47.767377 commons_lib-1.1.3/commons_lib/models/entities/gift/redeem_entity.py
+-rw-r--r--   0        0        0      736 2024-04-04 08:07:24.486147 commons_lib-1.1.3/commons_lib/models/entities/gift/vended_winning_entity.py
+-rw-r--r--   0        0        0      541 2024-04-04 07:18:47.779188 commons_lib-1.1.3/commons_lib/models/entities/gift/winning_category_entity.py
+-rw-r--r--   0        0        0     1092 2024-04-04 08:07:24.488295 commons_lib-1.1.3/commons_lib/models/entities/gift/winning_entity.py
+-rw-r--r--   0        0        0      357 2024-04-04 07:18:47.758854 commons_lib-1.1.3/commons_lib/models/entities/gift/winning_vendors.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.838587 commons_lib-1.1.3/commons_lib/models/entities/organization/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-04 07:18:47.782939 commons_lib-1.1.3/commons_lib/models/entities/organization/company_entity.py
+-rw-r--r--   0        0        0      289 2024-04-04 07:18:47.792138 commons_lib-1.1.3/commons_lib/models/entities/organization/sub_org_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.841515 commons_lib-1.1.3/commons_lib/models/entities/permissions/__init__.py
+-rw-r--r--   0        0        0      410 2024-04-04 07:18:47.798616 commons_lib-1.1.3/commons_lib/models/entities/permissions/permission_entity.py
+-rw-r--r--   0        0        0      267 2024-04-04 07:18:47.795119 commons_lib-1.1.3/commons_lib/models/entities/permissions/role_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.844104 commons_lib-1.1.3/commons_lib/models/entities/position/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-04 07:18:47.797505 commons_lib-1.1.3/commons_lib/models/entities/position/position_category_entity.py
+-rw-r--r--   0        0        0     1375 2024-04-04 07:18:47.777854 commons_lib-1.1.3/commons_lib/models/entities/position/position_entity.py
+-rw-r--r--   0        0        0      984 2024-04-04 07:18:47.765683 commons_lib-1.1.3/commons_lib/models/entities/position/positionentity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.845299 commons_lib-1.1.3/commons_lib/models/entities/transfers/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-04 07:18:47.761765 commons_lib-1.1.3/commons_lib/models/entities/transfers/transaction_category_entity.py
+-rw-r--r--   0        0        0      909 2024-04-04 08:07:24.483630 commons_lib-1.1.3/commons_lib/models/entities/transfers/transation_entity.py
+-rw-r--r--   0        0        0      259 2024-04-04 07:18:47.771690 commons_lib-1.1.3/commons_lib/models/entities/transfers/transfer_category_entity.py
+-rw-r--r--   0        0        0      751 2024-04-04 07:18:47.772862 commons_lib-1.1.3/commons_lib/models/entities/transfers/transfer_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.846343 commons_lib-1.1.3/commons_lib/models/entities/user/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-04 07:18:47.776564 commons_lib-1.1.3/commons_lib/models/entities/user/employee_entiry.py
+-rw-r--r--   0        0        0      258 2024-04-04 07:18:47.785209 commons_lib-1.1.3/commons_lib/models/entities/user/employee_entity.py
+-rw-r--r--   0        0        0     1692 2024-04-04 07:18:47.774047 commons_lib-1.1.3/commons_lib/models/entities/user/employment_entity.py
+-rw-r--r--   0        0        0      947 2024-04-04 08:07:24.478230 commons_lib-1.1.3/commons_lib/models/entities/user/user_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:43:53.848188 commons_lib-1.1.3/commons_lib/models/entities/values/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-04 07:18:47.775381 commons_lib-1.1.3/commons_lib/models/entities/values/org_behavior_entity.py
+-rw-r--r--   0        0        0      618 2024-04-04 07:18:47.770427 commons_lib-1.1.3/commons_lib/models/entities/values/org_value_entity.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.194923 commons_lib-1.1.3/commons_lib/models/enums/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195024 commons_lib-1.1.3/commons_lib/models/records/__init__.py
+-rw-r--r--   0        0        0      844 2024-02-14 08:14:46.195134 commons_lib-1.1.3/commons_lib/models/records/base_record.py
+-rw-r--r--   0        0        0      283 2024-02-14 08:14:46.195227 commons_lib-1.1.3/commons_lib/models/records/records.py
+-rw-r--r--   0        0        0        0 2024-02-14 08:14:46.195319 commons_lib-1.1.3/commons_lib/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-14 08:14:46.195430 commons_lib-1.1.3/commons_lib/utils/singleton.py
+-rw-r--r--   0        0        0     1243 2024-02-14 08:14:46.195529 commons_lib-1.1.3/commons_lib/utils/ttl_cache.py
+-rw-r--r--   0        0        0      634 2024-02-14 08:14:46.195689 commons_lib-1.1.3/docs/Makefile
+-rw-r--r--   0        0        0     2329 2024-02-14 08:14:46.195793 commons_lib-1.1.3/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-02-14 08:14:46.195888 commons_lib-1.1.3/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-02-14 08:14:46.195976 commons_lib-1.1.3/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-02-14 08:14:46.196071 commons_lib-1.1.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-02-14 08:14:46.196170 commons_lib-1.1.3/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-02-14 08:14:46.196268 commons_lib-1.1.3/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-02-14 08:14:46.196365 commons_lib-1.1.3/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-02-14 08:14:46.196548 commons_lib-1.1.3/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-02-14 08:14:46.196639 commons_lib-1.1.3/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-02-14 08:14:46.196736 commons_lib-1.1.3/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      427 2024-02-14 08:14:46.196827 commons_lib-1.1.3/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-02-14 08:14:46.196899 commons_lib-1.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-02-14 08:14:46.196978 commons_lib-1.1.3/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-02-14 08:14:46.197063 commons_lib-1.1.3/docs/workflows.md
+-rw-r--r--   0        0        0     6070 2024-02-14 08:14:46.197192 commons_lib-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      989 2024-02-14 08:14:46.197324 commons_lib-1.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     1217 2024-02-14 08:14:46.197423 commons_lib-1.1.3/tests/test_methods.py
+-rw-r--r--   0        0        0      328 2024-02-14 08:14:46.197514 commons_lib-1.1.3/tests/test_ttl_cache.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 commons_lib-1.1.3/PKG-INFO
```

### Comparing `commons_lib-1.1.2/.gitignore` & `commons_lib-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/__init__.py` & `commons_lib-1.1.3/commons_lib/models/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/accounts/account_category_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/accounts/account_category_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/accounts/accountـentity.py` & `commons_lib-1.1.3/commons_lib/models/entities/accounts/accountـentity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/appreciatation.py` & `commons_lib-1.1.3/commons_lib/models/entities/appreciatation.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/appreciatation_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/appreciatation_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/base_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/base_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/gift/redeem_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/gift/redeem_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/gift/vended_winning_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/gift/vended_winning_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlmodel import VARCHAR, Integer
+from sqlalchemy import VARCHAR, Integer
 from sqlalchemy import Column, BIGINT, ForeignKey
 from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy.dialects.postgresql import UUID
 import uuid
 
 from commons_lib.models.entities.base_entity import BaseEntity
```

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/gift/winning_category_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/gift/winning_category_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/gift/winning_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/gift/winning_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlmodel import VARCHAR, Integer
+from sqlalchemy import VARCHAR, Integer
 from sqlalchemy import Column, ForeignKey
 from sqlalchemy.orm import Mapped, relationship
 from sqlalchemy.dialects.postgresql import UUID
 import uuid
 
 from commons_lib.models.entities.base_entity import BaseEntity
```

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/organization/company_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/organization/company_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/position/position_category_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/position/position_category_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/position/position_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/position/position_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/position/positionentity.py` & `commons_lib-1.1.3/commons_lib/models/entities/position/positionentity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/transfers/transation_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/transfers/transation_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlmodel import BIGINT
+from sqlalchemy import BIGINT
 from sqlalchemy import Column
 from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy import ForeignKey
 from sqlalchemy.dialects.postgresql import UUID
 
 from commons_lib.models.entities.base_entity import BaseEntity
```

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/transfers/transfer_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/transfers/transfer_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/user/employment_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/user/employment_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/user/user_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/user/user_entity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy import DateTime, String, Boolean
 from sqlalchemy.orm import Mapped, mapped_column
-from sqlmodel import VARCHAR
+from sqlalchemy import VARCHAR
 from datetime import datetime
 
 from commons_lib.models.entities.base_entity import BaseEntity
 
 
 class UserEntity(BaseEntity):
     __abstract__ = True
```

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/values/org_behavior_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/values/org_behavior_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/entities/values/org_value_entity.py` & `commons_lib-1.1.3/commons_lib/models/entities/values/org_value_entity.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/models/records/base_record.py` & `commons_lib-1.1.3/commons_lib/models/records/base_record.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/utils/singleton.py` & `commons_lib-1.1.3/commons_lib/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/commons_lib/utils/ttl_cache.py` & `commons_lib-1.1.3/commons_lib/utils/ttl_cache.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/docs/Makefile` & `commons_lib-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/docs/conf.py` & `commons_lib-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/docs/make.bat` & `commons_lib-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/docs/pylint.md` & `commons_lib-1.1.3/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/pyproject.toml` & `commons_lib-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/tests/conftest.py` & `commons_lib-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/tests/test_methods.py` & `commons_lib-1.1.3/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `commons_lib-1.1.2/PKG-INFO` & `commons_lib-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commons_lib
-Version: 1.1.2
+Version: 1.1.3
 Summary: Arad PassioNikoo
 Author-email: Mehdi Einali <einali@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

