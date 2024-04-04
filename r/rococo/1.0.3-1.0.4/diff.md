# Comparing `tmp/rococo-1.0.3.tar.gz` & `tmp/rococo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rococo-1.0.3.tar", last modified: Fri Mar 29 01:52:52 2024, max compression
+gzip compressed data, was "rococo-1.0.4.tar", last modified: Thu Apr  4 21:36:06 2024, max compression
```

## Comparing `rococo-1.0.3.tar` & `rococo-1.0.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.164679 rococo-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-29 01:52:48.000000 rococo-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-03-29 01:52:52.164679 rococo-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-03-29 01:52:48.000000 rococo-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.156679 rococo-1.0.3/rococo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.156679 rococo-1.0.3/rococo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.156679 rococo-1.0.3/rococo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/data/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/data/surrealdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.160679 rococo-1.0.3/rococo/emailing/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/mailjet.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/emailing/ses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.160679 rococo-1.0.3/rococo/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/messaging/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/messaging/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.160679 rococo-1.0.3/rococo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/recovery_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.160679 rococo-1.0.3/rococo/models/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/surrealdb/surreal_versioned_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/models/versioned_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.164679 rococo-1.0.3/rococo/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/base_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.164679 rococo-1.0.3/rococo/repositories/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/mysql/mysql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/mysql/organization_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.164679 rococo-1.0.3/rococo/repositories/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/surrealdb/organization_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/surrealdb/person_organization_role_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-03-29 01:52:48.000000 rococo-1.0.3/rococo/repositories/surrealdb/surreal_db_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.164679 rococo-1.0.3/rococo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-03-29 01:52:52.000000 rococo-1.0.3/rococo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-29 01:52:52.000000 rococo-1.0.3/rococo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 01:52:52.000000 rococo-1.0.3/rococo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-29 01:52:52.000000 rococo-1.0.3/rococo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 01:52:52.000000 rococo-1.0.3/rococo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 01:52:52.164679 rococo-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-29 01:52:48.000000 rococo-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:52.164679 rococo-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:52:48.000000 rococo-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-03-29 01:52:48.000000 rococo-1.0.3/tests/base_repository_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-29 01:52:48.000000 rococo-1.0.3/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-29 01:52:48.000000 rococo-1.0.3/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-29 01:52:48.000000 rococo-1.0.3/tests/surreal_db_repository_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.146496 rococo-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 21:36:02.000000 rococo-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-04 21:36:06.146496 rococo-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-04 21:36:02.000000 rococo-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.138496 rococo-1.0.4/rococo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.138496 rococo-1.0.4/rococo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.138496 rococo-1.0.4/rococo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/data/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/data/surrealdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.138496 rococo-1.0.4/rococo/emailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/mailjet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/emailing/ses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.142496 rococo-1.0.4/rococo/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/messaging/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/messaging/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.142496 rococo-1.0.4/rococo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/recovery_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.142496 rococo-1.0.4/rococo/models/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/surrealdb/surreal_versioned_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/models/versioned_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.142496 rococo-1.0.4/rococo/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/base_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.142496 rococo-1.0.4/rococo/repositories/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/mysql/mysql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/mysql/organization_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.146496 rococo-1.0.4/rococo/repositories/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/surrealdb/organization_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/surrealdb/person_organization_role_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-04 21:36:02.000000 rococo-1.0.4/rococo/repositories/surrealdb/surreal_db_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.146496 rococo-1.0.4/rococo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-04 21:36:06.000000 rococo-1.0.4/rococo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-04 21:36:06.000000 rococo-1.0.4/rococo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:36:06.000000 rococo-1.0.4/rococo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 21:36:06.000000 rococo-1.0.4/rococo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 21:36:06.000000 rococo-1.0.4/rococo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:36:06.146496 rococo-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 21:36:02.000000 rococo-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:06.146496 rococo-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:36:02.000000 rococo-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-04 21:36:02.000000 rococo-1.0.4/tests/base_repository_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-04 21:36:02.000000 rococo-1.0.4/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 21:36:02.000000 rococo-1.0.4/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-04 21:36:02.000000 rococo-1.0.4/tests/surreal_db_repository_test.py
```

### Comparing `rococo-1.0.3/LICENSE` & `rococo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/PKG-INFO` & `rococo-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.3/README.md` & `rococo-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/config/config.py` & `rococo-1.0.4/rococo/config/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/data/base.py` & `rococo-1.0.4/rococo/data/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/data/mysql.py` & `rococo-1.0.4/rococo/data/mysql.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/data/surrealdb.py` & `rococo-1.0.4/rococo/data/surrealdb.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/emailing/config.py` & `rococo-1.0.4/rococo/emailing/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/emailing/factory.py` & `rococo-1.0.4/rococo/emailing/factory.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/emailing/mailjet.py` & `rococo-1.0.4/rococo/emailing/mailjet.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/messaging/base.py` & `rococo-1.0.4/rococo/messaging/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/messaging/rabbitmq.py` & `rococo-1.0.4/rococo/messaging/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/messaging/sqs.py` & `rococo-1.0.4/rococo/messaging/sqs.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         Args:
             queue_name (str): The name of the queue to send the message to.
             message (dict): The message to send.
         """
         if queue_name in self._queue_map:
             queue = self._queue_map[queue_name]
         else:
-            queue = self._sqs.get_queue_by_name(QueueName=queue_name)
+            queue = self._sqs.create_queue(QueueName=queue_name)
 
         queue.send_message(QueueUrl=queue_name, MessageBody=json.dumps(message))
 
     def consume_messages(self, queue_name: str, callback_function: callable = None):
         """Consumes messages from the specified SQS queue.
 
         Args:
@@ -68,15 +68,15 @@
                         'Id': str(uuid.uuid4()),
                         'ReceiptHandle': handle
                     },
                 ]
             )
 
         logger.info("Connecting to SQS queue: %s...", queue_name)
-        queue = self._sqs.get_queue_by_name(QueueName=queue_name)
+        queue = self._sqs.create_queue(QueueName=queue_name)
 
         while True:
             logger.info("Fetching messages from SQS queue: %s...", queue_name)
             responses = queue.receive_messages(
                 AttributeNames=['All'],
                 MaxNumberOfMessages=1,
                 WaitTimeSeconds=20
```

### Comparing `rococo-1.0.3/rococo/models/login_method.py` & `rococo-1.0.4/rococo/models/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/organization.py` & `rococo-1.0.4/rococo/models/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/person_organization_role.py` & `rococo-1.0.4/rococo/models/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/surrealdb/login_method.py` & `rococo-1.0.4/rococo/models/surrealdb/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/surrealdb/organization.py` & `rococo-1.0.4/rococo/models/surrealdb/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/surrealdb/person_organization_role.py` & `rococo-1.0.4/rococo/models/surrealdb/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/surrealdb/surreal_versioned_model.py` & `rococo-1.0.4/rococo/models/surrealdb/surreal_versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/models/versioned_model.py` & `rococo-1.0.4/rococo/models/versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/repositories/base_repository.py` & `rococo-1.0.4/rococo/repositories/base_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/repositories/mysql/mysql_repository.py` & `rococo-1.0.4/rococo/repositories/mysql/mysql_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/repositories/mysql/organization_repository.py` & `rococo-1.0.4/rococo/repositories/mysql/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/repositories/surrealdb/organization_repository.py` & `rococo-1.0.4/rococo/repositories/surrealdb/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/repositories/surrealdb/person_organization_role_repository.py` & `rococo-1.0.4/rococo/repositories/surrealdb/person_organization_role_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo/repositories/surrealdb/surreal_db_repository.py` & `rococo-1.0.4/rococo/repositories/surrealdb/surreal_db_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/rococo.egg-info/PKG-INFO` & `rococo-1.0.4/rococo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.3/rococo.egg-info/SOURCES.txt` & `rococo-1.0.4/rococo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/setup.py` & `rococo-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='rococo',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     url='https://github.com/EcorRouge/rococo',
     license='MIT',
     author='Jay Grieves',
     author_email='jaygrieves@gmail.com',
     description='A Python library to help build things the way we want them built',
     long_description=open('README.md').read(),
```

### Comparing `rococo-1.0.3/tests/base_repository_test.py` & `rococo-1.0.4/tests/base_repository_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/tests/config_test.py` & `rococo-1.0.4/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/tests/model_test.py` & `rococo-1.0.4/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.3/tests/surreal_db_repository_test.py` & `rococo-1.0.4/tests/surreal_db_repository_test.py`

 * *Files identical despite different names*

