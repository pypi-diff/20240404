# Comparing `tmp/django-mfa2-2.8.0.tar.gz` & `tmp/django-mfa2-2.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mfa2-2.8.0.tar", last modified: Mon Dec 19 11:56:08 2022, max compression
+gzip compressed data, was "dist/django-mfa2-2.9.0b1.tar", last modified: Thu Apr  4 13:44:54 2024, max compression
```

## Comparing `django-mfa2-2.8.0.tar` & `django-mfa2-2.9.0b1.tar`

### file list

```diff
@@ -1,89 +1,93 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       64 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/MANIFEST.in
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    13271 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    10134 2022-12-19 11:55:48.000000 django-mfa2-2.8.0/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/django_mfa2.egg-info/
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)    13271 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/django_mfa2.egg-info/PKG-INFO
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)     2078 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/django_mfa2.egg-info/SOURCES.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        1 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/django_mfa2.egg-info/dependency_links.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        1 2019-01-18 07:28:18.000000 django-mfa2-2.8.0/django_mfa2.egg-info/not-zip-safe
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)       97 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/django_mfa2.egg-info/requires.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        4 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/django_mfa2.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/ApproveLogin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      730 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/Common.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3309 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/Email.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     8043 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5337 2022-12-19 11:23:22.000000 django-mfa2-2.8.0/mfa/TrustedDevice.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5149 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/U2F.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       20 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      124 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1345 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      534 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/middleware.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      624 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      407 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0002_user_keys_key_type.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      405 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0003_auto_20181114_2159.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      402 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0004_user_keys_enabled.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1038 2022-12-19 11:50:07.000000 django-mfa2-2.8.0/mfa/migrations/0005_auto_20181115_2014.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      956 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0006_trusted_devices.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      502 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0007_auto_20181230_1549.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      428 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0008_user_keys_last_used.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      740 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0009_user_keys_owned_by_enterprise.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      412 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0010_auto_20201110_0557.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      421 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/migrations/0011_auto_20210530_0622.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1617 2022-12-19 11:27:08.000000 django-mfa2-2.8.0/mfa/models.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4956 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/recovery.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/static/mfa/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/static/mfa/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/static/mfa/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/static/mfa/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/static/mfa/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    12175 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/static/mfa/js/cbor.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    17579 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/static/mfa/js/qrious.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    21007 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/static/mfa/js/u2f-api.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    19071 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/static/mfa/js/ua-parser.min.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/ApproveLogin/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      123 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/ApproveLogin/Add.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/Email/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1714 2022-06-22 05:55:49.000000 django-mfa2-2.8.0/mfa/templates/Email/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      235 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/Email/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      108 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/Email/mfa_email_token_template.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2554 2022-06-22 05:55:49.000000 django-mfa2-2.8.0/mfa/templates/Email/recheck.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/FIDO2/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3164 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/FIDO2/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      121 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/FIDO2/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4726 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/FIDO2/recheck.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5593 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/MFA.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/RECOVERY/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4795 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/RECOVERY/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      240 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/RECOVERY/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3184 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/RECOVERY/recheck.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/TOTP/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5300 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/TOTP/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      236 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/TOTP/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2581 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/TOTP/recheck.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/TrustedDevices/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3961 2022-06-22 05:55:49.000000 django-mfa2-2.8.0/mfa/templates/TrustedDevices/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      735 2022-06-22 05:55:49.000000 django-mfa2-2.8.0/mfa/templates/TrustedDevices/Done.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      278 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/TrustedDevices/email.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4315 2022-12-19 11:23:22.000000 django-mfa2-2.8.0/mfa/templates/TrustedDevices/start.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      306 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/TrustedDevices/user-agent.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/mfa/templates/U2F/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2690 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/U2F/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      135 2021-11-16 07:57:44.000000 django-mfa2-2.8.0/mfa/templates/U2F/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3575 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/U2F/recheck.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2021-11-16 08:31:00.000000 django-mfa2-2.8.0/mfa/templates/mfa_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1034 2022-06-22 05:55:49.000000 django-mfa2-2.8.0/mfa/templates/mfa_check.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2022-06-22 05:55:49.000000 django-mfa2-2.8.0/mfa/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1419 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/templates/select_mfa_method.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       60 2021-11-16 08:30:56.000000 django-mfa2-2.8.0/mfa/tests.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3934 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/totp.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2715 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4098 2022-11-01 06:09:57.000000 django-mfa2-2.8.0/mfa/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       67 2022-12-19 11:56:08.000000 django-mfa2-2.8.0/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1952 2022-12-19 11:38:50.000000 django-mfa2-2.8.0/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1075 2019-01-18 07:17:11.000000 django-mfa2-2.9.0b1/LICENSE
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       64 2019-01-18 12:15:28.000000 django-mfa2-2.9.0b1/MANIFEST.in
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    11768 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    10355 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    11768 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     2210 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2019-01-18 07:28:18.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       97 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/requires.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        4 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/ApproveLogin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      804 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/Common.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3790 2024-04-04 13:37:24.000000 django-mfa2-2.9.0b1/mfa/Email.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     9019 2024-04-04 13:31:55.000000 django-mfa2-2.9.0b1/mfa/FIDO2.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5851 2024-04-04 13:39:27.000000 django-mfa2-2.9.0b1/mfa/TrustedDevice.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5455 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/U2F.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       22 2024-04-04 13:15:05.000000 django-mfa2-2.9.0b1/mfa/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      127 2024-04-04 13:15:05.000000 django-mfa2-2.9.0b1/mfa/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1521 2024-04-04 13:32:57.000000 django-mfa2-2.9.0b1/mfa/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      680 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/middleware.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      796 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      406 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0002_user_keys_key_type.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      404 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0003_auto_20181114_2159.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      401 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0004_user_keys_enabled.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1081 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0005_auto_20181115_2014.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1133 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0006_trusted_devices.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      501 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0007_auto_20181230_1549.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      427 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0008_user_keys_last_used.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      756 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0009_user_keys_owned_by_enterprise.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      411 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0010_auto_20201110_0557.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      420 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0011_auto_20210530_0622.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      440 2022-09-02 07:52:00.000000 django-mfa2-2.9.0b1/mfa/migrations/0012_alter_user_keys_id.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1717 2024-04-04 13:37:46.000000 django-mfa2-2.9.0b1/mfa/models.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5266 2024-04-04 13:38:22.000000 django-mfa2-2.9.0b1/mfa/recovery.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/mfa/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/mfa/css/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1590 2018-05-09 11:30:28.000000 django-mfa2-2.9.0b1/mfa/static/mfa/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     4129 2018-05-09 11:30:28.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4106 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js.map
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    12175 2023-12-31 18:37:19.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/cbor.js
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    17579 2019-01-02 14:37:10.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)   114187 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js.map
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    21007 2019-01-16 17:28:14.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/u2f-api.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    19071 2021-02-26 10:25:56.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/ua-parser.min.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/ApproveLogin/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      123 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/templates/ApproveLogin/Add.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/Email/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1714 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/Email/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      235 2019-01-21 15:33:45.000000 django-mfa2-2.9.0b1/mfa/templates/Email/Auth.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      108 2019-01-21 15:33:45.000000 django-mfa2-2.9.0b1/mfa/templates/Email/mfa_email_token_template.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2554 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/Email/recheck.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3164 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      121 2019-06-20 17:36:18.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4726 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/recheck.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5593 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/MFA.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4795 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/Add.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      240 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3184 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/recheck.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5300 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      236 2019-01-18 12:39:43.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2581 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/recheck.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3961 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Add.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      735 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Done.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      278 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/email.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4315 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/start.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      306 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/user-agent.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2690 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      135 2019-01-18 12:40:01.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3575 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/recheck.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/mfa_base.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1034 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/mfa_check.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/modal.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1419 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/select_mfa_method.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       60 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/tests.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4338 2024-04-04 13:34:39.000000 django-mfa2-2.9.0b1/mfa/totp.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2740 2024-04-04 13:41:35.000000 django-mfa2-2.9.0b1/mfa/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4076 2024-04-04 13:36:18.000000 django-mfa2-2.9.0b1/mfa/views.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       67 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1954 2024-04-04 13:43:31.000000 django-mfa2-2.9.0b1/setup.py
```

### Comparing `django-mfa2-2.8.0/PKG-INFO` & `django-mfa2-2.9.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,232 +1,17 @@
 Metadata-Version: 2.1
 Name: django-mfa2
-Version: 2.8.0
+Version: 2.9.0b1
 Summary: Allows user to add 2FA to their accounts
 Home-page: https://github.com/mkalioby/django-mfa2/
+Download-URL: https://github.com/mkalioby/django-mfa2/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Download-URL: https://github.com/mkalioby/django-mfa2/
-Description: # django-mfa2
-        A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
-        
-        [![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
-        ### Pip Stats
-        [![PyPI version](https://badge.fury.io/py/django-mfa2.svg)](https://badge.fury.io/py/django-mfa2)
-        [![Downloads Count](https://static.pepy.tech/personalized-badge/django-mfa2?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/django-mfa2)
-        
-        ### Conda Stats
-        [![Conda Recipe](https://img.shields.io/badge/recipe-django--mfa2-green.svg)](https://anaconda.org/conda-forge/django-mfa2) 
-        [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
-        
-        Web Authencation API (WebAuthn) is state-of-the art techology that is expected to replace passwords.
-        
-        ![Andriod Fingerprint](https://cdn-images-1.medium.com/max/800/1*1FWkRE8D7NTA2Kn1DrPjPA.png)
-        
-        For FIDO2, the following are supported
-         * **security keys** (Firefox 60+, Chrome 67+, Edge 18+, Safari 13 on Mac OS, Chrome on Andriod, Safari on iOS 13.3+),
-         * **Windows Hello** (Firefox 67+, Chrome 72+ , Edge),
-         * **Apple's Touch ID/Face ID** (Chrome 70+ on Mac OS X, Safari on macOS Big Sur, Safari on iOS 14.0+ ),
-         * **android-safetynet** (Chrome 70+, Firefox 68+)
-         * **NFC devices using PCSC** (Not Tested, but as supported in fido2)
-         * **Soft Tokens** 
-            * ~~[krypt.co](https://krypt.co/): Login by a notification on your phone.~~
-        
-        **Update**: Dec 2022, krypt.co has been killed by Google for Passkeys.
-        
-        In English :), It allows you to verify the user by security keys on PC, Laptops or Mobiles, Windows Hello (Fingerprint, PIN) on Windows 10 Build 1903+ (May 2019 Update) Touch/Face ID on Macbooks (Chrome, Safari), Touch/Face ID on iPhone and iPad and Fingerprint/Face/Iris/PIN on Android Phones.
-        
-        Trusted device is a mode for the user to add a device that doesn't support security keys like Android without fingerprints or NFC.
-        
-        **Note**: `U2F and FIDO2 can only be served under secure context (https)`
-        
-        Package tested with Django 1.8, Django 2.2 on Python 2.7 and Python 3.5+ but it was not checked with any version in between but open for issues.
-        
-        If you just need WebAuthn and Passkeys, you can use **[django-passkeys](https://github.com/mkalioby/django-passkeys)**, which is a slim-down of this app and much easier to integrate.
-        
-        Depends on
-        
-        * pyotp
-        * python-u2flib-server
-        * ua-parser
-        * user-agents
-        * python-jose
-        * fido2==1.0.0
-        
-        # Installation
-        1. using pip 
-            * For Django >= 4.0
-               
-                `pip install django-mfa2`
-            * For Django < 4.0
-                   
-              `pip install django-mfa2 jsonfield`
-        2. Using Conda forge 
-           
-           `conda config --add channels conda-forge`
-           
-           `conda install django-mfa2`
-           
-           For more info, see the conda-forge repo (https://github.com/conda-forge/django-mfa2-feedstock)
-           
-           Thanks for [swainn](https://github.com/swainn) for adding package to conda-forge
-        
-        # Usage
-        1. in your settings.py add the application to your installed apps
-           ```python
-           INSTALLED_APPS=(
-           '......',
-           'mfa',
-           '......')
-           ```
-        2. Collect Static Files
-        `python manage.py collectstatic`
-        3. Add the following settings to your file
-        
-           ```python
-           from django.conf.global_settings import PASSWORD_HASHERS as DEFAULT_PASSWORD_HASHERS #Preferably at the same place where you import your other modules
-           MFA_UNALLOWED_METHODS=()   # Methods that shouldn't be allowed for the user e.g ('TOTP','U2F',)
-           MFA_LOGIN_CALLBACK=""      # A function that should be called by username to login the user in session
-           MFA_RECHECK=True           # Allow random rechecking of the user
-           MFA_REDIRECT_AFTER_REGISTRATION="mfa_home"   # Allows Changing the page after successful registeration
-           MFA_SUCCESS_REGISTRATION_MSG = "Go to Security Home" # The text of the link
-           MFA_RECHECK_MIN=10         # Minimum interval in seconds
-           MFA_RECHECK_MAX=30         # Maximum in seconds
-           MFA_QUICKLOGIN=True        # Allow quick login for returning users by provide only their 2FA
-           MFA_ALWAYS_GO_TO_LAST_METHOD = False # Always redirect the user to the last method used to save a click (Added in 2.6.0).
-           MFA_RENAME_METHODS={} #Rename the methods in a more user-friendly way e.g {"RECOVERY":"Backup Codes"} (Added in 2.6.0)
-           MFA_HIDE_DISABLE=('FIDO2',)     # Can the user disable his key (Added in 1.2.0).
-           MFA_OWNED_BY_ENTERPRISE = FALSE  # Who owns security keys   
-           PASSWORD_HASHERS = DEFAULT_PASSWORD_HASHERS # Comment if PASSWORD_HASHER already set in your settings.py
-           PASSWORD_HASHERS += ['mfa.recovery.Hash'] 
-           RECOVERY_ITERATION = 350000 #Number of iteration for recovery code, higher is more secure, but uses more resources for generation and check...
-        
-           TOKEN_ISSUER_NAME="PROJECT_NAME"      #TOTP Issuer name
-        
-           U2F_APPID="https://localhost"    #URL For U2F
-           FIDO_SERVER_ID=u"localehost"      # Server rp id for FIDO2, it is the full domain of your project
-           FIDO_SERVER_NAME=u"PROJECT_NAME"
-           ```
-           **Method Names**
-           * U2F
-           * FIDO2
-           * TOTP
-           * Trusted_Devices
-           * Email
-           * RECOVERY
-           
-           **Notes**:
-            * Starting version 1.1, ~~FIDO_LOGIN_URL~~ isn't required for FIDO2 anymore.
-            * Starting version 1.7.0, Key owners can be specified.
-            * Starting version 2.2.0
-                * Added: `MFA_SUCCESS_REGISTRATION_MSG` & `MFA_REDIRECT_AFTER_REGISTRATION`
-            Start version 2.6.0
-                * Added: `MFA_ALWAYS_GO_TO_LAST_METHOD`, `MFA_RENAME_METHODS`, `MFA_ENFORCE_RECOVERY_METHOD` & `RECOVERY_ITERATION`
-        4. Break your login function
-        
-           Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support mfa, this has to change
-           
-              * authenticate the user
-              * if username and password are correct , check if the user has mfa or not
-                  * if user has mfa then redirect to mfa page
-                  * if user doesn't have mfa then call your function to create the user session
-        
-           ```python
-            def login(request): # this function handles the login form POST
-               user = auth.authenticate(username=username, password=password)  
-               if user is not None: # if the user object exist
-                    from mfa.helpers import has_mfa
-                    res =  has_mfa(username = username,request=request) # has_mfa returns false or HttpResponseRedirect
-                    if res:
-                        return res
-                    return log_user_in(request,username=user.username) 
-                    #log_user_in is a function that handles creatung user session, it should be in the setting file as MFA_CALLBACK
-             ```
-        5. Add mfa to urls.py
-           ```python 
-           import mfa
-           import mfa.TrustedDevice
-           urls_patterns= [
-           '...',
-           url(r'^mfa/', include('mfa.urls')),
-           url(r'devices/add$', mfa.TrustedDevice.add,name="mfa_add_new_trusted_device"), # This short link to add new trusted device
-           '....',
-            ]
-            ```
-        6. Provide `mfa_auth_base.html` in your templates with block called 'head' and 'content', The template will be included during the user login, the template shall be close to the login template.
-            If you will use Email Token method, then you have to provide template named `mfa_email_token_template.html` that will content the format of the email with parameter named `user` and `otp`.
-        7. To match the look and feel of your project, MFA includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
-           **Note:** Starting v2.3.0, a new template `mfa_base.html` is introduced, this template is used by `MFA.html` so you can control the styling better and current `mfa_base.html` extends `base.html`
-        8. Somewhere in your app, add a link to 'mfa_home'
-        ```<li><a href="{% url 'mfa_home' %}">Security</a> </li>```
-        
-        
-        For Example, See 'example' app and look at EXAMPLE.md to see how to set it up.
-        
-        # Going Passwordless
-        
-        To be able to go passwordless for returning users, create a cookie  named 'base_username' containing username as shown in snippet below
-        ```python
-            response = render(request, 'Dashboard.html', context))
-            if request.session.get("mfa",{}).get("verified",False)  and getattr(settings,"MFA_QUICKLOGIN",False):
-                if request.session["mfa"]["method"]!="Trusted Device":
-                    response.set_cookie("base_username", request.user.username, path="/",max_age = 15*24*60*60)
-            return response
-        ```
-        
-        Second, update the GET part of your login view
-        ```python
-            if "mfa" in settings.INSTALLED_APPS and getattr(settings,"MFA_QUICKLOGIN",False) and request.COOKIES.get('base_username'):
-                username=request.COOKIES.get('base_username')
-                from mfa.helpers import has_mfa
-                res =  has_mfa(username = username,request=request,)
-                if res: return res
-                ## continue and return the form.
-        ```
-        # Checking MFA on Client Side
-        
-        Sometimes you like to verify that the user is still there so simple you can ask django-mfa2 to check that for you
-        
-        ```html
-            {% include 'mfa_check.html' %}
-        ```
-        ````js
-        function success_func() {
-          //logic if mfa check succeeds
-        }
-        function fail_func() {
-          //logic if mfa check fails
-        }
-        function some_func() {
-            recheck_mfa(success_func,fail_func,MUST_BE_MFA)
-            //MUST_BE_MFA true or false, if the user must has with MFA
-          }
-        
-        ````
-        
-        # Contributors
-        * [mahmoodnasr](https://github.com/mahmoodnasr)
-        * [d3cline](https://github.com/d3cline)
-        * [swainn](https://github.com/swainn)
-        * [unramk](https://github.com/unramk)
-        * [willingham](https://github.com/willingham)
-        * [AndreasDickow](https://github.com/AndreasDickow)
-        * [mnelson4](https://github.com/mnelson4)
-        * [ezrajrice](https://github.com/ezrajrice)
-        * [Spitfireap](https://github.com/Spitfireap)
-        * [peterthomassen](https://github.com/peterthomassen)
-        
-        
-         # Security contact information
-        To report a security vulnerability, please use the [Tidelift security contact](https://tidelift.com/security). Tidelift will coordinate the fix and disclosure.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -243,7 +28,225 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-mfa2
+A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
+
+[![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
+
+[![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Type Checker By Pyre](https://img.shields.io/badge/type%20checker-pyre-orange)](https://pyre-check.org/)
+### Pip Stats
+[![PyPI version](https://badge.fury.io/py/django-mfa2.svg)](https://badge.fury.io/py/django-mfa2)
+[![Downloads Count](https://static.pepy.tech/personalized-badge/django-mfa2?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/django-mfa2)
+
+### Conda Stats
+[![Conda Recipe](https://img.shields.io/badge/recipe-django--mfa2-green.svg)](https://anaconda.org/conda-forge/django-mfa2) 
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
+
+Web Authencation API (WebAuthn) is state-of-the art techology that is expected to replace passwords.
+
+![Andriod Fingerprint](https://cdn-images-1.medium.com/max/800/1*1FWkRE8D7NTA2Kn1DrPjPA.png)
+
+For FIDO2, the following are supported
+ * **security keys** (Firefox 60+, Chrome 67+, Edge 18+, Safari 13 on Mac OS, Chrome on Andriod, Safari on iOS 13.3+),
+ * **Windows Hello** (Firefox 67+, Chrome 72+ , Edge),
+ * **Apple's Touch ID/Face ID** (Chrome 70+ on Mac OS X, Safari on macOS Big Sur, Safari on iOS 14.0+ ),
+ * **android-safetynet** (Chrome 70+, Firefox 68+)
+ * **NFC devices using PCSC** (Not Tested, but as supported in fido2)
+ * **Soft Tokens** 
+    * ~~[krypt.co](https://krypt.co/): Login by a notification on your phone.~~
+
+**Update**: Dec 2022, krypt.co has been killed by Google for Passkeys.
+
+In English :), It allows you to verify the user by security keys on PC, Laptops or Mobiles, Windows Hello (Fingerprint, PIN) on Windows 10 Build 1903+ (May 2019 Update) Touch/Face ID on Macbooks (Chrome, Safari), Touch/Face ID on iPhone and iPad and Fingerprint/Face/Iris/PIN on Android Phones.
+
+Trusted device is a mode for the user to add a device that doesn't support security keys like Android without fingerprints or NFC.
+
+**Note**: `U2F and FIDO2 can only be served under secure context (https)`
+
+Package tested with Django 1.8, Django 2.2 on Python 2.7 and Python 3.5+ but it was not checked with any version in between but open for issues.
+
+If you just need WebAuthn and Passkeys, you can use **[django-passkeys](https://github.com/mkalioby/django-passkeys)**, which is a slim-down of this app and much easier to integrate.
+
+Depends on
+
+* pyotp
+* python-u2flib-server
+* ua-parser
+* user-agents
+* python-jose
+* fido2==1.0.0
+
+# Installation
+1. using pip 
+    * For Django >= 4.0
+       
+        `pip install django-mfa2`
+    * For Django < 4.0
+           
+      `pip install django-mfa2 jsonfield`
+2. Using Conda forge 
+   
+   `conda config --add channels conda-forge`
+   
+   `conda install django-mfa2`
+   
+   For more info, see the conda-forge repo (https://github.com/conda-forge/django-mfa2-feedstock)
+   
+   Thanks for [swainn](https://github.com/swainn) for adding package to conda-forge
+
+# Usage
+1. in your settings.py add the application to your installed apps
+   ```python
+   INSTALLED_APPS=(
+   '......',
+   'mfa',
+   '......')
+   ```
+2. Collect Static Files
+`python manage.py collectstatic`
+3. Add the following settings to your file
+
+   ```python
+   from django.conf.global_settings import PASSWORD_HASHERS as DEFAULT_PASSWORD_HASHERS #Preferably at the same place where you import your other modules
+   MFA_UNALLOWED_METHODS=()   # Methods that shouldn't be allowed for the user e.g ('TOTP','U2F',)
+   MFA_LOGIN_CALLBACK=""      # A function that should be called by username to login the user in session
+   MFA_RECHECK=True           # Allow random rechecking of the user
+   MFA_REDIRECT_AFTER_REGISTRATION="mfa_home"   # Allows Changing the page after successful registeration
+   MFA_SUCCESS_REGISTRATION_MSG = "Go to Security Home" # The text of the link
+   MFA_RECHECK_MIN=10         # Minimum interval in seconds
+   MFA_RECHECK_MAX=30         # Maximum in seconds
+   MFA_QUICKLOGIN=True        # Allow quick login for returning users by provide only their 2FA
+   MFA_ALWAYS_GO_TO_LAST_METHOD = False # Always redirect the user to the last method used to save a click (Added in 2.6.0).
+   MFA_RENAME_METHODS={} #Rename the methods in a more user-friendly way e.g {"RECOVERY":"Backup Codes"} (Added in 2.6.0)
+   MFA_HIDE_DISABLE=('FIDO2',)     # Can the user disable his key (Added in 1.2.0).
+   MFA_OWNED_BY_ENTERPRISE = FALSE  # Who owns security keys   
+   PASSWORD_HASHERS = DEFAULT_PASSWORD_HASHERS # Comment if PASSWORD_HASHER already set in your settings.py
+   PASSWORD_HASHERS += ['mfa.recovery.Hash'] 
+   RECOVERY_ITERATION = 350000 #Number of iteration for recovery code, higher is more secure, but uses more resources for generation and check...
+
+   TOKEN_ISSUER_NAME="PROJECT_NAME"      #TOTP Issuer name
+
+   U2F_APPID="https://localhost"    #URL For U2F
+   FIDO_SERVER_ID=u"localehost"      # Server rp id for FIDO2, it is the full domain of your project
+   FIDO_SERVER_NAME=u"PROJECT_NAME"
+   ```
+   **Method Names**
+   * U2F
+   * FIDO2
+   * TOTP
+   * Trusted_Devices
+   * Email
+   * RECOVERY
+   
+   **Notes**:
+    * Starting version 1.1, ~~FIDO_LOGIN_URL~~ isn't required for FIDO2 anymore.
+    * Starting version 1.7.0, Key owners can be specified.
+    * Starting version 2.2.0
+        * Added: `MFA_SUCCESS_REGISTRATION_MSG` & `MFA_REDIRECT_AFTER_REGISTRATION`
+    Start version 2.6.0
+        * Added: `MFA_ALWAYS_GO_TO_LAST_METHOD`, `MFA_RENAME_METHODS`, `MFA_ENFORCE_RECOVERY_METHOD` & `RECOVERY_ITERATION`
+4. Break your login function
+
+   Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support mfa, this has to change
+   
+      * authenticate the user
+      * if username and password are correct , check if the user has mfa or not
+          * if user has mfa then redirect to mfa page
+          * if user doesn't have mfa then call your function to create the user session
+
+   ```python
+    def login(request): # this function handles the login form POST
+       user = auth.authenticate(username=username, password=password)  
+       if user is not None: # if the user object exist
+            from mfa.helpers import has_mfa
+            res =  has_mfa(username = username,request=request) # has_mfa returns false or HttpResponseRedirect
+            if res:
+                return res
+            return log_user_in(request,username=user.username) 
+            #log_user_in is a function that handles creatung user session, it should be in the setting file as MFA_CALLBACK
+     ```
+5. Add mfa to urls.py
+   ```python 
+   import mfa
+   import mfa.TrustedDevice
+   urls_patterns= [
+   '...',
+   url(r'^mfa/', include('mfa.urls')),
+   url(r'devices/add$', mfa.TrustedDevice.add,name="mfa_add_new_trusted_device"), # This short link to add new trusted device
+   '....',
+    ]
+    ```
+6. Provide `mfa_auth_base.html` in your templates with block called 'head' and 'content', The template will be included during the user login, the template shall be close to the login template.
+    If you will use Email Token method, then you have to provide template named `mfa_email_token_template.html` that will content the format of the email with parameter named `user` and `otp`.
+7. To match the look and feel of your project, MFA includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
+   **Note:** Starting v2.3.0, a new template `mfa_base.html` is introduced, this template is used by `MFA.html` so you can control the styling better and current `mfa_base.html` extends `base.html`
+8. Somewhere in your app, add a link to 'mfa_home'
+```<li><a href="{% url 'mfa_home' %}">Security</a> </li>```
+
+
+For Example, See 'example' app and look at EXAMPLE.md to see how to set it up.
+
+# Going Passwordless
+
+To be able to go passwordless for returning users, create a cookie  named 'base_username' containing username as shown in snippet below
+```python
+    response = render(request, 'Dashboard.html', context))
+    if request.session.get("mfa",{}).get("verified",False)  and getattr(settings,"MFA_QUICKLOGIN",False):
+        if request.session["mfa"]["method"]!="Trusted Device":
+            response.set_cookie("base_username", request.user.username, path="/",max_age = 15*24*60*60)
+    return response
+```
+
+Second, update the GET part of your login view
+```python
+    if "mfa" in settings.INSTALLED_APPS and getattr(settings,"MFA_QUICKLOGIN",False) and request.COOKIES.get('base_username'):
+        username=request.COOKIES.get('base_username')
+        from mfa.helpers import has_mfa
+        res =  has_mfa(username = username,request=request,)
+        if res: return res
+        ## continue and return the form.
+```
+# Checking MFA on Client Side
+
+Sometimes you like to verify that the user is still there so simple you can ask django-mfa2 to check that for you
+
+```html
+    {% include 'mfa_check.html' %}
+```
+````js
+function success_func() {
+  //logic if mfa check succeeds
+}
+function fail_func() {
+  //logic if mfa check fails
+}
+function some_func() {
+    recheck_mfa(success_func,fail_func,MUST_BE_MFA)
+    //MUST_BE_MFA true or false, if the user must has with MFA
+  }
+
+````
+
+# Contributors
+* [mahmoodnasr](https://github.com/mahmoodnasr)
+* [d3cline](https://github.com/d3cline)
+* [swainn](https://github.com/swainn)
+* [unramk](https://github.com/unramk)
+* [willingham](https://github.com/willingham)
+* [AndreasDickow](https://github.com/AndreasDickow)
+* [mnelson4](https://github.com/mnelson4)
+* [ezrajrice](https://github.com/ezrajrice)
+* [Spitfireap](https://github.com/Spitfireap)
+* [peterthomassen](https://github.com/peterthomassen)
+
+
+ # Security contact information
+To report a security vulnerability, please use the [Tidelift security contact](https://tidelift.com/security). Tidelift will coordinate the fix and disclosure.
```

### Comparing `django-mfa2-2.8.0/README.md` & `django-mfa2-2.9.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # django-mfa2
 A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
 
 [![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
+
+[![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Type Checker By Pyre](https://img.shields.io/badge/type%20checker-pyre-orange)](https://pyre-check.org/)
 ### Pip Stats
 [![PyPI version](https://badge.fury.io/py/django-mfa2.svg)](https://badge.fury.io/py/django-mfa2)
 [![Downloads Count](https://static.pepy.tech/personalized-badge/django-mfa2?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/django-mfa2)
 
 ### Conda Stats
 [![Conda Recipe](https://img.shields.io/badge/recipe-django--mfa2-green.svg)](https://anaconda.org/conda-forge/django-mfa2) 
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2)
```

### Comparing `django-mfa2-2.8.0/django_mfa2.egg-info/PKG-INFO` & `django-mfa2-2.9.0b1/django_mfa2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,232 +1,17 @@
 Metadata-Version: 2.1
 Name: django-mfa2
-Version: 2.8.0
+Version: 2.9.0b1
 Summary: Allows user to add 2FA to their accounts
 Home-page: https://github.com/mkalioby/django-mfa2/
+Download-URL: https://github.com/mkalioby/django-mfa2/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Download-URL: https://github.com/mkalioby/django-mfa2/
-Description: # django-mfa2
-        A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
-        
-        [![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
-        ### Pip Stats
-        [![PyPI version](https://badge.fury.io/py/django-mfa2.svg)](https://badge.fury.io/py/django-mfa2)
-        [![Downloads Count](https://static.pepy.tech/personalized-badge/django-mfa2?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/django-mfa2)
-        
-        ### Conda Stats
-        [![Conda Recipe](https://img.shields.io/badge/recipe-django--mfa2-green.svg)](https://anaconda.org/conda-forge/django-mfa2) 
-        [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
-        
-        Web Authencation API (WebAuthn) is state-of-the art techology that is expected to replace passwords.
-        
-        ![Andriod Fingerprint](https://cdn-images-1.medium.com/max/800/1*1FWkRE8D7NTA2Kn1DrPjPA.png)
-        
-        For FIDO2, the following are supported
-         * **security keys** (Firefox 60+, Chrome 67+, Edge 18+, Safari 13 on Mac OS, Chrome on Andriod, Safari on iOS 13.3+),
-         * **Windows Hello** (Firefox 67+, Chrome 72+ , Edge),
-         * **Apple's Touch ID/Face ID** (Chrome 70+ on Mac OS X, Safari on macOS Big Sur, Safari on iOS 14.0+ ),
-         * **android-safetynet** (Chrome 70+, Firefox 68+)
-         * **NFC devices using PCSC** (Not Tested, but as supported in fido2)
-         * **Soft Tokens** 
-            * ~~[krypt.co](https://krypt.co/): Login by a notification on your phone.~~
-        
-        **Update**: Dec 2022, krypt.co has been killed by Google for Passkeys.
-        
-        In English :), It allows you to verify the user by security keys on PC, Laptops or Mobiles, Windows Hello (Fingerprint, PIN) on Windows 10 Build 1903+ (May 2019 Update) Touch/Face ID on Macbooks (Chrome, Safari), Touch/Face ID on iPhone and iPad and Fingerprint/Face/Iris/PIN on Android Phones.
-        
-        Trusted device is a mode for the user to add a device that doesn't support security keys like Android without fingerprints or NFC.
-        
-        **Note**: `U2F and FIDO2 can only be served under secure context (https)`
-        
-        Package tested with Django 1.8, Django 2.2 on Python 2.7 and Python 3.5+ but it was not checked with any version in between but open for issues.
-        
-        If you just need WebAuthn and Passkeys, you can use **[django-passkeys](https://github.com/mkalioby/django-passkeys)**, which is a slim-down of this app and much easier to integrate.
-        
-        Depends on
-        
-        * pyotp
-        * python-u2flib-server
-        * ua-parser
-        * user-agents
-        * python-jose
-        * fido2==1.0.0
-        
-        # Installation
-        1. using pip 
-            * For Django >= 4.0
-               
-                `pip install django-mfa2`
-            * For Django < 4.0
-                   
-              `pip install django-mfa2 jsonfield`
-        2. Using Conda forge 
-           
-           `conda config --add channels conda-forge`
-           
-           `conda install django-mfa2`
-           
-           For more info, see the conda-forge repo (https://github.com/conda-forge/django-mfa2-feedstock)
-           
-           Thanks for [swainn](https://github.com/swainn) for adding package to conda-forge
-        
-        # Usage
-        1. in your settings.py add the application to your installed apps
-           ```python
-           INSTALLED_APPS=(
-           '......',
-           'mfa',
-           '......')
-           ```
-        2. Collect Static Files
-        `python manage.py collectstatic`
-        3. Add the following settings to your file
-        
-           ```python
-           from django.conf.global_settings import PASSWORD_HASHERS as DEFAULT_PASSWORD_HASHERS #Preferably at the same place where you import your other modules
-           MFA_UNALLOWED_METHODS=()   # Methods that shouldn't be allowed for the user e.g ('TOTP','U2F',)
-           MFA_LOGIN_CALLBACK=""      # A function that should be called by username to login the user in session
-           MFA_RECHECK=True           # Allow random rechecking of the user
-           MFA_REDIRECT_AFTER_REGISTRATION="mfa_home"   # Allows Changing the page after successful registeration
-           MFA_SUCCESS_REGISTRATION_MSG = "Go to Security Home" # The text of the link
-           MFA_RECHECK_MIN=10         # Minimum interval in seconds
-           MFA_RECHECK_MAX=30         # Maximum in seconds
-           MFA_QUICKLOGIN=True        # Allow quick login for returning users by provide only their 2FA
-           MFA_ALWAYS_GO_TO_LAST_METHOD = False # Always redirect the user to the last method used to save a click (Added in 2.6.0).
-           MFA_RENAME_METHODS={} #Rename the methods in a more user-friendly way e.g {"RECOVERY":"Backup Codes"} (Added in 2.6.0)
-           MFA_HIDE_DISABLE=('FIDO2',)     # Can the user disable his key (Added in 1.2.0).
-           MFA_OWNED_BY_ENTERPRISE = FALSE  # Who owns security keys   
-           PASSWORD_HASHERS = DEFAULT_PASSWORD_HASHERS # Comment if PASSWORD_HASHER already set in your settings.py
-           PASSWORD_HASHERS += ['mfa.recovery.Hash'] 
-           RECOVERY_ITERATION = 350000 #Number of iteration for recovery code, higher is more secure, but uses more resources for generation and check...
-        
-           TOKEN_ISSUER_NAME="PROJECT_NAME"      #TOTP Issuer name
-        
-           U2F_APPID="https://localhost"    #URL For U2F
-           FIDO_SERVER_ID=u"localehost"      # Server rp id for FIDO2, it is the full domain of your project
-           FIDO_SERVER_NAME=u"PROJECT_NAME"
-           ```
-           **Method Names**
-           * U2F
-           * FIDO2
-           * TOTP
-           * Trusted_Devices
-           * Email
-           * RECOVERY
-           
-           **Notes**:
-            * Starting version 1.1, ~~FIDO_LOGIN_URL~~ isn't required for FIDO2 anymore.
-            * Starting version 1.7.0, Key owners can be specified.
-            * Starting version 2.2.0
-                * Added: `MFA_SUCCESS_REGISTRATION_MSG` & `MFA_REDIRECT_AFTER_REGISTRATION`
-            Start version 2.6.0
-                * Added: `MFA_ALWAYS_GO_TO_LAST_METHOD`, `MFA_RENAME_METHODS`, `MFA_ENFORCE_RECOVERY_METHOD` & `RECOVERY_ITERATION`
-        4. Break your login function
-        
-           Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support mfa, this has to change
-           
-              * authenticate the user
-              * if username and password are correct , check if the user has mfa or not
-                  * if user has mfa then redirect to mfa page
-                  * if user doesn't have mfa then call your function to create the user session
-        
-           ```python
-            def login(request): # this function handles the login form POST
-               user = auth.authenticate(username=username, password=password)  
-               if user is not None: # if the user object exist
-                    from mfa.helpers import has_mfa
-                    res =  has_mfa(username = username,request=request) # has_mfa returns false or HttpResponseRedirect
-                    if res:
-                        return res
-                    return log_user_in(request,username=user.username) 
-                    #log_user_in is a function that handles creatung user session, it should be in the setting file as MFA_CALLBACK
-             ```
-        5. Add mfa to urls.py
-           ```python 
-           import mfa
-           import mfa.TrustedDevice
-           urls_patterns= [
-           '...',
-           url(r'^mfa/', include('mfa.urls')),
-           url(r'devices/add$', mfa.TrustedDevice.add,name="mfa_add_new_trusted_device"), # This short link to add new trusted device
-           '....',
-            ]
-            ```
-        6. Provide `mfa_auth_base.html` in your templates with block called 'head' and 'content', The template will be included during the user login, the template shall be close to the login template.
-            If you will use Email Token method, then you have to provide template named `mfa_email_token_template.html` that will content the format of the email with parameter named `user` and `otp`.
-        7. To match the look and feel of your project, MFA includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
-           **Note:** Starting v2.3.0, a new template `mfa_base.html` is introduced, this template is used by `MFA.html` so you can control the styling better and current `mfa_base.html` extends `base.html`
-        8. Somewhere in your app, add a link to 'mfa_home'
-        ```<li><a href="{% url 'mfa_home' %}">Security</a> </li>```
-        
-        
-        For Example, See 'example' app and look at EXAMPLE.md to see how to set it up.
-        
-        # Going Passwordless
-        
-        To be able to go passwordless for returning users, create a cookie  named 'base_username' containing username as shown in snippet below
-        ```python
-            response = render(request, 'Dashboard.html', context))
-            if request.session.get("mfa",{}).get("verified",False)  and getattr(settings,"MFA_QUICKLOGIN",False):
-                if request.session["mfa"]["method"]!="Trusted Device":
-                    response.set_cookie("base_username", request.user.username, path="/",max_age = 15*24*60*60)
-            return response
-        ```
-        
-        Second, update the GET part of your login view
-        ```python
-            if "mfa" in settings.INSTALLED_APPS and getattr(settings,"MFA_QUICKLOGIN",False) and request.COOKIES.get('base_username'):
-                username=request.COOKIES.get('base_username')
-                from mfa.helpers import has_mfa
-                res =  has_mfa(username = username,request=request,)
-                if res: return res
-                ## continue and return the form.
-        ```
-        # Checking MFA on Client Side
-        
-        Sometimes you like to verify that the user is still there so simple you can ask django-mfa2 to check that for you
-        
-        ```html
-            {% include 'mfa_check.html' %}
-        ```
-        ````js
-        function success_func() {
-          //logic if mfa check succeeds
-        }
-        function fail_func() {
-          //logic if mfa check fails
-        }
-        function some_func() {
-            recheck_mfa(success_func,fail_func,MUST_BE_MFA)
-            //MUST_BE_MFA true or false, if the user must has with MFA
-          }
-        
-        ````
-        
-        # Contributors
-        * [mahmoodnasr](https://github.com/mahmoodnasr)
-        * [d3cline](https://github.com/d3cline)
-        * [swainn](https://github.com/swainn)
-        * [unramk](https://github.com/unramk)
-        * [willingham](https://github.com/willingham)
-        * [AndreasDickow](https://github.com/AndreasDickow)
-        * [mnelson4](https://github.com/mnelson4)
-        * [ezrajrice](https://github.com/ezrajrice)
-        * [Spitfireap](https://github.com/Spitfireap)
-        * [peterthomassen](https://github.com/peterthomassen)
-        
-        
-         # Security contact information
-        To report a security vulnerability, please use the [Tidelift security contact](https://tidelift.com/security). Tidelift will coordinate the fix and disclosure.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -243,7 +28,225 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-mfa2
+A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
+
+[![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
+
+[![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Type Checker By Pyre](https://img.shields.io/badge/type%20checker-pyre-orange)](https://pyre-check.org/)
+### Pip Stats
+[![PyPI version](https://badge.fury.io/py/django-mfa2.svg)](https://badge.fury.io/py/django-mfa2)
+[![Downloads Count](https://static.pepy.tech/personalized-badge/django-mfa2?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/django-mfa2)
+
+### Conda Stats
+[![Conda Recipe](https://img.shields.io/badge/recipe-django--mfa2-green.svg)](https://anaconda.org/conda-forge/django-mfa2) 
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/django-mfa2.svg)](https://anaconda.org/conda-forge/django-mfa2) 
+
+Web Authencation API (WebAuthn) is state-of-the art techology that is expected to replace passwords.
+
+![Andriod Fingerprint](https://cdn-images-1.medium.com/max/800/1*1FWkRE8D7NTA2Kn1DrPjPA.png)
+
+For FIDO2, the following are supported
+ * **security keys** (Firefox 60+, Chrome 67+, Edge 18+, Safari 13 on Mac OS, Chrome on Andriod, Safari on iOS 13.3+),
+ * **Windows Hello** (Firefox 67+, Chrome 72+ , Edge),
+ * **Apple's Touch ID/Face ID** (Chrome 70+ on Mac OS X, Safari on macOS Big Sur, Safari on iOS 14.0+ ),
+ * **android-safetynet** (Chrome 70+, Firefox 68+)
+ * **NFC devices using PCSC** (Not Tested, but as supported in fido2)
+ * **Soft Tokens** 
+    * ~~[krypt.co](https://krypt.co/): Login by a notification on your phone.~~
+
+**Update**: Dec 2022, krypt.co has been killed by Google for Passkeys.
+
+In English :), It allows you to verify the user by security keys on PC, Laptops or Mobiles, Windows Hello (Fingerprint, PIN) on Windows 10 Build 1903+ (May 2019 Update) Touch/Face ID on Macbooks (Chrome, Safari), Touch/Face ID on iPhone and iPad and Fingerprint/Face/Iris/PIN on Android Phones.
+
+Trusted device is a mode for the user to add a device that doesn't support security keys like Android without fingerprints or NFC.
+
+**Note**: `U2F and FIDO2 can only be served under secure context (https)`
+
+Package tested with Django 1.8, Django 2.2 on Python 2.7 and Python 3.5+ but it was not checked with any version in between but open for issues.
+
+If you just need WebAuthn and Passkeys, you can use **[django-passkeys](https://github.com/mkalioby/django-passkeys)**, which is a slim-down of this app and much easier to integrate.
+
+Depends on
+
+* pyotp
+* python-u2flib-server
+* ua-parser
+* user-agents
+* python-jose
+* fido2==1.0.0
+
+# Installation
+1. using pip 
+    * For Django >= 4.0
+       
+        `pip install django-mfa2`
+    * For Django < 4.0
+           
+      `pip install django-mfa2 jsonfield`
+2. Using Conda forge 
+   
+   `conda config --add channels conda-forge`
+   
+   `conda install django-mfa2`
+   
+   For more info, see the conda-forge repo (https://github.com/conda-forge/django-mfa2-feedstock)
+   
+   Thanks for [swainn](https://github.com/swainn) for adding package to conda-forge
+
+# Usage
+1. in your settings.py add the application to your installed apps
+   ```python
+   INSTALLED_APPS=(
+   '......',
+   'mfa',
+   '......')
+   ```
+2. Collect Static Files
+`python manage.py collectstatic`
+3. Add the following settings to your file
+
+   ```python
+   from django.conf.global_settings import PASSWORD_HASHERS as DEFAULT_PASSWORD_HASHERS #Preferably at the same place where you import your other modules
+   MFA_UNALLOWED_METHODS=()   # Methods that shouldn't be allowed for the user e.g ('TOTP','U2F',)
+   MFA_LOGIN_CALLBACK=""      # A function that should be called by username to login the user in session
+   MFA_RECHECK=True           # Allow random rechecking of the user
+   MFA_REDIRECT_AFTER_REGISTRATION="mfa_home"   # Allows Changing the page after successful registeration
+   MFA_SUCCESS_REGISTRATION_MSG = "Go to Security Home" # The text of the link
+   MFA_RECHECK_MIN=10         # Minimum interval in seconds
+   MFA_RECHECK_MAX=30         # Maximum in seconds
+   MFA_QUICKLOGIN=True        # Allow quick login for returning users by provide only their 2FA
+   MFA_ALWAYS_GO_TO_LAST_METHOD = False # Always redirect the user to the last method used to save a click (Added in 2.6.0).
+   MFA_RENAME_METHODS={} #Rename the methods in a more user-friendly way e.g {"RECOVERY":"Backup Codes"} (Added in 2.6.0)
+   MFA_HIDE_DISABLE=('FIDO2',)     # Can the user disable his key (Added in 1.2.0).
+   MFA_OWNED_BY_ENTERPRISE = FALSE  # Who owns security keys   
+   PASSWORD_HASHERS = DEFAULT_PASSWORD_HASHERS # Comment if PASSWORD_HASHER already set in your settings.py
+   PASSWORD_HASHERS += ['mfa.recovery.Hash'] 
+   RECOVERY_ITERATION = 350000 #Number of iteration for recovery code, higher is more secure, but uses more resources for generation and check...
+
+   TOKEN_ISSUER_NAME="PROJECT_NAME"      #TOTP Issuer name
+
+   U2F_APPID="https://localhost"    #URL For U2F
+   FIDO_SERVER_ID=u"localehost"      # Server rp id for FIDO2, it is the full domain of your project
+   FIDO_SERVER_NAME=u"PROJECT_NAME"
+   ```
+   **Method Names**
+   * U2F
+   * FIDO2
+   * TOTP
+   * Trusted_Devices
+   * Email
+   * RECOVERY
+   
+   **Notes**:
+    * Starting version 1.1, ~~FIDO_LOGIN_URL~~ isn't required for FIDO2 anymore.
+    * Starting version 1.7.0, Key owners can be specified.
+    * Starting version 2.2.0
+        * Added: `MFA_SUCCESS_REGISTRATION_MSG` & `MFA_REDIRECT_AFTER_REGISTRATION`
+    Start version 2.6.0
+        * Added: `MFA_ALWAYS_GO_TO_LAST_METHOD`, `MFA_RENAME_METHODS`, `MFA_ENFORCE_RECOVERY_METHOD` & `RECOVERY_ITERATION`
+4. Break your login function
+
+   Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support mfa, this has to change
+   
+      * authenticate the user
+      * if username and password are correct , check if the user has mfa or not
+          * if user has mfa then redirect to mfa page
+          * if user doesn't have mfa then call your function to create the user session
+
+   ```python
+    def login(request): # this function handles the login form POST
+       user = auth.authenticate(username=username, password=password)  
+       if user is not None: # if the user object exist
+            from mfa.helpers import has_mfa
+            res =  has_mfa(username = username,request=request) # has_mfa returns false or HttpResponseRedirect
+            if res:
+                return res
+            return log_user_in(request,username=user.username) 
+            #log_user_in is a function that handles creatung user session, it should be in the setting file as MFA_CALLBACK
+     ```
+5. Add mfa to urls.py
+   ```python 
+   import mfa
+   import mfa.TrustedDevice
+   urls_patterns= [
+   '...',
+   url(r'^mfa/', include('mfa.urls')),
+   url(r'devices/add$', mfa.TrustedDevice.add,name="mfa_add_new_trusted_device"), # This short link to add new trusted device
+   '....',
+    ]
+    ```
+6. Provide `mfa_auth_base.html` in your templates with block called 'head' and 'content', The template will be included during the user login, the template shall be close to the login template.
+    If you will use Email Token method, then you have to provide template named `mfa_email_token_template.html` that will content the format of the email with parameter named `user` and `otp`.
+7. To match the look and feel of your project, MFA includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
+   **Note:** Starting v2.3.0, a new template `mfa_base.html` is introduced, this template is used by `MFA.html` so you can control the styling better and current `mfa_base.html` extends `base.html`
+8. Somewhere in your app, add a link to 'mfa_home'
+```<li><a href="{% url 'mfa_home' %}">Security</a> </li>```
+
+
+For Example, See 'example' app and look at EXAMPLE.md to see how to set it up.
+
+# Going Passwordless
+
+To be able to go passwordless for returning users, create a cookie  named 'base_username' containing username as shown in snippet below
+```python
+    response = render(request, 'Dashboard.html', context))
+    if request.session.get("mfa",{}).get("verified",False)  and getattr(settings,"MFA_QUICKLOGIN",False):
+        if request.session["mfa"]["method"]!="Trusted Device":
+            response.set_cookie("base_username", request.user.username, path="/",max_age = 15*24*60*60)
+    return response
+```
+
+Second, update the GET part of your login view
+```python
+    if "mfa" in settings.INSTALLED_APPS and getattr(settings,"MFA_QUICKLOGIN",False) and request.COOKIES.get('base_username'):
+        username=request.COOKIES.get('base_username')
+        from mfa.helpers import has_mfa
+        res =  has_mfa(username = username,request=request,)
+        if res: return res
+        ## continue and return the form.
+```
+# Checking MFA on Client Side
+
+Sometimes you like to verify that the user is still there so simple you can ask django-mfa2 to check that for you
+
+```html
+    {% include 'mfa_check.html' %}
+```
+````js
+function success_func() {
+  //logic if mfa check succeeds
+}
+function fail_func() {
+  //logic if mfa check fails
+}
+function some_func() {
+    recheck_mfa(success_func,fail_func,MUST_BE_MFA)
+    //MUST_BE_MFA true or false, if the user must has with MFA
+  }
+
+````
+
+# Contributors
+* [mahmoodnasr](https://github.com/mahmoodnasr)
+* [d3cline](https://github.com/d3cline)
+* [swainn](https://github.com/swainn)
+* [unramk](https://github.com/unramk)
+* [willingham](https://github.com/willingham)
+* [AndreasDickow](https://github.com/AndreasDickow)
+* [mnelson4](https://github.com/mnelson4)
+* [ezrajrice](https://github.com/ezrajrice)
+* [Spitfireap](https://github.com/Spitfireap)
+* [peterthomassen](https://github.com/peterthomassen)
+
+
+ # Security contact information
+To report a security vulnerability, please use the [Tidelift security contact](https://tidelift.com/security). Tidelift will coordinate the fix and disclosure.
```

### Comparing `django-mfa2-2.8.0/django_mfa2.egg-info/SOURCES.txt` & `django-mfa2-2.9.0b1/django_mfa2.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_mfa2.egg-info/PKG-INFO
 django_mfa2.egg-info/SOURCES.txt
 django_mfa2.egg-info/dependency_links.txt
@@ -32,19 +33,22 @@
 mfa/migrations/0005_auto_20181115_2014.py
 mfa/migrations/0006_trusted_devices.py
 mfa/migrations/0007_auto_20181230_1549.py
 mfa/migrations/0008_user_keys_last_used.py
 mfa/migrations/0009_user_keys_owned_by_enterprise.py
 mfa/migrations/0010_auto_20201110_0557.py
 mfa/migrations/0011_auto_20210530_0622.py
+mfa/migrations/0012_alter_user_keys_id.py
 mfa/migrations/__init__.py
 mfa/static/mfa/css/bootstrap-toggle.min.css
 mfa/static/mfa/js/bootstrap-toggle.min.js
+mfa/static/mfa/js/bootstrap-toggle.min.js.map
 mfa/static/mfa/js/cbor.js
 mfa/static/mfa/js/qrious.min.js
+mfa/static/mfa/js/qrious.min.js.map
 mfa/static/mfa/js/u2f-api.js
 mfa/static/mfa/js/ua-parser.min.js
 mfa/templates/MFA.html
 mfa/templates/mfa_base.html
 mfa/templates/mfa_check.html
 mfa/templates/modal.html
 mfa/templates/select_mfa_method.html
```

### Comparing `django-mfa2-2.8.0/mfa/Email.py` & `django-mfa2-2.9.0b1/mfa/Email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,109 @@
+import datetime
+from random import randint
 from django.shortcuts import render
 from django.views.decorators.cache import never_cache
 from django.template.context_processors import csrf
-import datetime,random
-from random import randint
-from .models import *
-#from django.template.context import RequestContext
+from django.contrib.auth import get_user_model
+from django.http import HttpResponseRedirect
+from django.conf import settings
+
+from .models import User_Keys
+
 from .views import login
 from .Common import send
 
-def sendEmail(request,username,secret):
+
+def sendEmail(request, username, secret):
     """Send Email to the user after rendering `mfa_email_token_template`"""
-    from django.contrib.auth import get_user_model
+
     User = get_user_model()
-    key = getattr(User, 'USERNAME_FIELD', 'username')
+    key = getattr(User, "USERNAME_FIELD", "username")
     kwargs = {key: username}
     user = User.objects.get(**kwargs)
-    res=render(request,"mfa_email_token_template.html",{"request":request,"user":user,'otp':secret})
-    return send([user.email],"OTP", res.content.decode())
+    res = render(
+        request,
+        "mfa_email_token_template.html",
+        {"request": request, "user": user, "otp": secret},
+    )
+    return send([user.email], "OTP", res.content.decode())
+
 
 @never_cache
 def start(request):
     """Start adding email as a 2nd factor"""
     context = csrf(request)
     if request.method == "POST":
-        if request.session["email_secret"] == request.POST["otp"]:  #if successful
-            uk=User_Keys()
-            uk.username=request.user.username
-            uk.key_type="Email"
-            uk.enabled=1
+        if request.session["email_secret"] == request.POST["otp"]:  # if successful
+            uk = User_Keys()
+            uk.username = request.user.username
+            uk.key_type = "Email"
+            uk.enabled = 1
             uk.save()
-            from django.http import HttpResponseRedirect
+
             try:
-                from django.core.urlresolvers import reverse
+                from django.core.urlresolvers import reverse  # pyre-ignore[21]
             except:
                 from django.urls import reverse
-            if getattr(settings, 'MFA_ENFORCE_RECOVERY_METHOD', False) and not User_Keys.objects.filter(
-                    key_type="RECOVERY", username=request.user.username).exists():
-                request.session["mfa_reg"] = {"method": "Email",
-                                              "name": getattr(settings, "MFA_RENAME_METHODS", {}).get("Email", "Email")}
+            if (
+                getattr(settings, "MFA_ENFORCE_RECOVERY_METHOD", False)
+                and not User_Keys.objects.filter(
+                    key_type="RECOVERY", username=request.user.username
+                ).exists()
+            ):
+                request.session["mfa_reg"] = {
+                    "method": "Email",
+                    "name": getattr(settings, "MFA_RENAME_METHODS", {}).get(
+                        "Email", "Email"
+                    ),
+                }
             else:
-                return HttpResponseRedirect(reverse(getattr(settings,'MFA_REDIRECT_AFTER_REGISTRATION','mfa_home')))
+                return HttpResponseRedirect(
+                    reverse(
+                        getattr(settings, "MFA_REDIRECT_AFTER_REGISTRATION", "mfa_home")
+                    )
+                )
         context["invalid"] = True
     else:
-        request.session["email_secret"] = str(randint(0,100000))  #generate a random integer
+        request.session["email_secret"] = str(
+            randint(0, 100000)
+        )  # generate a random integer
 
         if sendEmail(request, request.user.username, request.session["email_secret"]):
             context["sent"] = True
-    return render(request,"Email/Add.html", context)
+    return render(request, "Email/Add.html", context)
+
+
 @never_cache
 def auth(request):
     """Authenticating the user by email."""
-    context=csrf(request)
-    if request.method=="POST":
-        if request.session["email_secret"]==request.POST["otp"].strip():
-            uk = User_Keys.objects.get(username=request.session["base_username"], key_type="Email")
-            mfa = {"verified": True, "method": "Email","id":uk.id}
+    context = csrf(request)
+    if request.method == "POST":
+        if request.session["email_secret"] == request.POST["otp"].strip():
+            uk = User_Keys.objects.get(
+                username=request.session["base_username"], key_type="Email"
+            )
+            mfa = {"verified": True, "method": "Email", "id": uk.id}
             if getattr(settings, "MFA_RECHECK", False):
-                mfa["next_check"] = datetime.datetime.timestamp(datetime.datetime.now() + datetime.timedelta(
-                    seconds = random.randint(settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX)))
+                mfa["next_check"] = datetime.datetime.timestamp(
+                    datetime.datetime.now()
+                    + datetime.timedelta(
+                        seconds=random.randint(
+                            settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX
+                        )
+                    )
+                )
             request.session["mfa"] = mfa
 
             from django.utils import timezone
-            uk.last_used=timezone.now()
+
+            uk.last_used = timezone.now()
             uk.save()
             return login(request)
-        context["invalid"]=True
+        context["invalid"] = True
     else:
         request.session["email_secret"] = str(randint(0, 100000))
-        if sendEmail(request, request.session["base_username"], request.session["email_secret"]):
+        if sendEmail(
+            request, request.session["base_username"], request.session["email_secret"]
+        ):
             context["sent"] = True
-    return render(request,"Email/Auth.html", context)
+    return render(request, "Email/Auth.html", context)
```

### Comparing `django-mfa2-2.8.0/mfa/FIDO2.py` & `django-mfa2-2.9.0b1/mfa/FIDO2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,181 +1,254 @@
-from fido2.client import Fido2Client
 from fido2.server import Fido2Server, PublicKeyCredentialRpEntity
 from fido2.webauthn import AttestationObject, AuthenticatorData, CollectedClientData
 from django.template.context_processors import csrf
 from django.views.decorators.csrf import csrf_exempt
 from django.shortcuts import render
-# from django.template.context import RequestContext
+
 import simplejson
 from fido2 import cbor
 from django.http import HttpResponse
 from django.conf import settings
-from .models import *
 from fido2.utils import websafe_decode, websafe_encode
 from fido2.webauthn import AttestedCredentialData
 from .views import login, reset_cookie
+from .models import User_Keys
 import datetime
 from .Common import get_redirect_url
 from django.utils import timezone
 from django.http import JsonResponse
 
+
 def recheck(request):
     """Starts FIDO2 recheck"""
     context = csrf(request)
     context["mode"] = "recheck"
     request.session["mfa_recheck"] = True
     return render(request, "FIDO2/recheck.html", context)
 
 
 def getServer():
     """Get Server Info from settings and returns a Fido2Server"""
-    rp = PublicKeyCredentialRpEntity(id=settings.FIDO_SERVER_ID, name=settings.FIDO_SERVER_NAME)
+    rp = PublicKeyCredentialRpEntity(
+        id=settings.FIDO_SERVER_ID, name=settings.FIDO_SERVER_NAME
+    )
     return Fido2Server(rp)
 
 
 def begin_registeration(request):
     """Starts registering a new FIDO Device, called from API"""
     server = getServer()
-    registration_data, state = server.register_begin({
-        u'id': request.user.username.encode("utf8"),
-        u'name': (request.user.first_name + " " + request.user.last_name),
-        u'displayName': request.user.username,
-    }, getUserCredentials(request.user.username))
-    request.session['fido_state'] = state
-
-    return HttpResponse(cbor.encode(registration_data), content_type = 'application/octet-stream')
+    registration_data, state = server.register_begin(
+        {
+            "id": request.user.username.encode("utf8"),
+            "name": (request.user.first_name + " " + request.user.last_name),
+            "displayName": request.user.username,
+        },
+        getUserCredentials(request.user.username),
+    )
+    request.session["fido_state"] = state
+
+    return HttpResponse(
+        cbor.encode(registration_data), content_type="application/octet-stream"
+    )
 
 
 @csrf_exempt
 def complete_reg(request):
     """Completes the registeration, called by API"""
     try:
         if not "fido_state" in request.session:
-            return JsonResponse({'status': 'ERR', "message": "FIDO Status can't be found, please try again"})
+            return JsonResponse(
+                {
+                    "status": "ERR",
+                    "message": "FIDO Status can't be found, please try again",
+                }
+            )
         data = cbor.decode(request.body)
 
-        client_data = CollectedClientData(data['clientDataJSON'])
-        att_obj = AttestationObject((data['attestationObject']))
+        client_data = CollectedClientData(data["clientDataJSON"])
+        att_obj = AttestationObject((data["attestationObject"]))
         server = getServer()
         auth_data = server.register_complete(
-            request.session.pop('fido_state'),
-            client_data,
-            att_obj
+            request.session.pop("fido_state"), client_data, att_obj
         )
         encoded = websafe_encode(auth_data.credential_data)
         uk = User_Keys()
         uk.username = request.user.username
-        uk.properties = {"device": encoded, "type": att_obj.fmt, }
+        uk.properties = {
+            "device": encoded,
+            "type": att_obj.fmt,
+        }
         uk.owned_by_enterprise = getattr(settings, "MFA_OWNED_BY_ENTERPRISE", False)
         uk.key_type = "FIDO2"
         uk.save()
-        if getattr(settings, 'MFA_ENFORCE_RECOVERY_METHOD', False) and not User_Keys.objects.filter(key_type = "RECOVERY", username=request.user.username).exists():
-            request.session["mfa_reg"] = {"method":"FIDO2","name": getattr(settings, "MFA_RENAME_METHODS", {}).get("FIDO2", "FIDO2")}
-            return HttpResponse(simplejson.dumps({'status': 'RECOVERY'}))
+        if (
+            getattr(settings, "MFA_ENFORCE_RECOVERY_METHOD", False)
+            and not User_Keys.objects.filter(
+                key_type="RECOVERY", username=request.user.username
+            ).exists()
+        ):
+            request.session["mfa_reg"] = {
+                "method": "FIDO2",
+                "name": getattr(settings, "MFA_RENAME_METHODS", {}).get(
+                    "FIDO2", "FIDO2"
+                ),
+            }
+            return HttpResponse(simplejson.dumps({"status": "RECOVERY"}))
         else:
-            return HttpResponse(simplejson.dumps({'status': 'OK'}))
+            return HttpResponse(simplejson.dumps({"status": "OK"}))
     except Exception as exp:
         import traceback
+
         print(traceback.format_exc())
         try:
             from raven.contrib.django.raven_compat.models import client
+
             client.captureException()
         except:
             pass
-        return JsonResponse({'status': 'ERR', "message": "Error on server, please try again later"})
+        return JsonResponse(
+            {"status": "ERR", "message": "Error on server, please try again later"}
+        )
 
 
 def start(request):
     """Start Registration a new FIDO Token"""
     context = csrf(request)
     context.update(get_redirect_url())
-    context["method"] = {"name":getattr(settings,"MFA_RENAME_METHODS",{}).get("FIDO2","FIDO2 Security Key")}
-    context["RECOVERY_METHOD"]=getattr(settings,"MFA_RENAME_METHODS",{}).get("RECOVERY","Recovery codes")
+    context["method"] = {
+        "name": getattr(settings, "MFA_RENAME_METHODS", {}).get(
+            "FIDO2", "FIDO2 Security Key"
+        )
+    }
+    context["RECOVERY_METHOD"] = getattr(settings, "MFA_RENAME_METHODS", {}).get(
+        "RECOVERY", "Recovery codes"
+    )
     return render(request, "FIDO2/Add.html", context)
 
 
 def getUserCredentials(username):
     credentials = []
-    for uk in User_Keys.objects.filter(username = username, key_type = "FIDO2"):
-        credentials.append(AttestedCredentialData(websafe_decode(uk.properties["device"])))
+    for uk in User_Keys.objects.filter(username=username, key_type="FIDO2"):
+        credentials.append(
+            AttestedCredentialData(websafe_decode(uk.properties["device"]))
+        )
     return credentials
 
 
 def auth(request):
     context = csrf(request)
     return render(request, "FIDO2/Auth.html", context)
 
 
 def authenticate_begin(request):
     server = getServer()
-    credentials = getUserCredentials(request.session.get("base_username", request.user.username))
+    credentials = getUserCredentials(
+        request.session.get("base_username", request.user.username)
+    )
     auth_data, state = server.authenticate_begin(credentials)
-    request.session['fido_state'] = state
-    return HttpResponse(cbor.encode(auth_data), content_type = "application/octet-stream")
+    request.session["fido_state"] = state
+    return HttpResponse(cbor.encode(auth_data), content_type="application/octet-stream")
 
 
 @csrf_exempt
 def authenticate_complete(request):
     try:
         credentials = []
         username = request.session.get("base_username", request.user.username)
         server = getServer()
         credentials = getUserCredentials(username)
         data = cbor.decode(request.body)
-        credential_id = data['credentialId']
-        client_data = CollectedClientData(data['clientDataJSON'])
-        auth_data = AuthenticatorData(data['authenticatorData'])
-        signature = data['signature']
+        credential_id = data["credentialId"]
+        client_data = CollectedClientData(data["clientDataJSON"])
+        auth_data = AuthenticatorData(data["authenticatorData"])
+        signature = data["signature"]
         try:
             cred = server.authenticate_complete(
-                request.session.pop('fido_state'),
+                request.session.pop("fido_state"),
                 credentials,
                 credential_id,
                 client_data,
                 auth_data,
-                signature
+                signature,
             )
         except ValueError:
-            return HttpResponse(simplejson.dumps({'status': "ERR",
-                                                  "message": "Wrong challenge received, make sure that this is your security and try again."}),
-                                content_type = "application/json")
+            return HttpResponse(
+                simplejson.dumps(
+                    {
+                        "status": "ERR",
+                        "message": "Wrong challenge received, make sure that this is your security and try again.",
+                    }
+                ),
+                content_type="application/json",
+            )
         except Exception as excep:
             try:
                 from raven.contrib.django.raven_compat.models import client
+
                 client.captureException()
             except:
                 pass
-            return HttpResponse(simplejson.dumps({'status': "ERR",
-                                                  "message": str(excep)}),
-                                content_type = "application/json")
+            return HttpResponse(
+                simplejson.dumps({"status": "ERR", "message": str(excep)}),
+                content_type="application/json",
+            )
 
         if request.session.get("mfa_recheck", False):
             import time
+
             request.session["mfa"]["rechecked_at"] = time.time()
-            return HttpResponse(simplejson.dumps({'status': "OK"}),
-                                content_type = "application/json")
+            return HttpResponse(
+                simplejson.dumps({"status": "OK"}), content_type="application/json"
+            )
         else:
             import random
-            keys = User_Keys.objects.filter(username = username, key_type = "FIDO2", enabled = 1)
+
+            keys = User_Keys.objects.filter(
+                username=username, key_type="FIDO2", enabled=1
+            )
             for k in keys:
-                if AttestedCredentialData(websafe_decode(k.properties["device"])).credential_id == cred.credential_id:
+                if (
+                    AttestedCredentialData(
+                        websafe_decode(k.properties["device"])
+                    ).credential_id
+                    == cred.credential_id
+                ):
                     k.last_used = timezone.now()
                     k.save()
-                    mfa = {"verified": True, "method": "FIDO2", 'id': k.id}
+                    mfa = {"verified": True, "method": "FIDO2", "id": k.id}
                     if getattr(settings, "MFA_RECHECK", False):
-                        mfa["next_check"] = datetime.datetime.timestamp((datetime.datetime.now() + datetime.timedelta(
-                            seconds = random.randint(settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX))))
+                        mfa["next_check"] = datetime.datetime.timestamp(
+                            (
+                                datetime.datetime.now()
+                                + datetime.timedelta(
+                                    seconds=random.randint(
+                                        settings.MFA_RECHECK_MIN,
+                                        settings.MFA_RECHECK_MAX,
+                                    )
+                                )
+                            )
+                        )
                     request.session["mfa"] = mfa
                     try:
                         authenticated = request.user.is_authenticated
                     except:
                         authenticated = request.user.is_authenticated()
                     if not authenticated:
                         res = login(request)
-                        if not "location" in res: return reset_cookie(request)
-                        return HttpResponse(simplejson.dumps({'status': "OK", "redirect": res["location"]}),
-                                            content_type = "application/json")
-                    return HttpResponse(simplejson.dumps({'status': "OK"}),
-                                        content_type = "application/json")
+                        if not "location" in res:
+                            return reset_cookie(request)
+                        return HttpResponse(
+                            simplejson.dumps(
+                                {"status": "OK", "redirect": res["location"]}
+                            ),
+                            content_type="application/json",
+                        )
+                    return HttpResponse(
+                        simplejson.dumps({"status": "OK"}),
+                        content_type="application/json",
+                    )
     except Exception as exp:
-        return HttpResponse(simplejson.dumps({'status': "ERR", "message": exp.message}),
-                            content_type = "application/json")
+        return HttpResponse(
+            simplejson.dumps({"status": "ERR", "message": exp.message}),
+            content_type="application/json",
+        )
```

### Comparing `django-mfa2-2.8.0/mfa/TrustedDevice.py` & `django-mfa2-2.9.0b1/mfa/TrustedDevice.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,177 @@
 import string
 import random
+from datetime import datetime, timedelta
 from django.shortcuts import render
 from django.http import HttpResponse
-from django.template.context import RequestContext
 from django.template.context_processors import csrf
-from .models import *
 import user_agents
 from django.utils import timezone
 from django.urls import reverse
 
+from .models import User_Keys
+
 def id_generator(size=6, chars=string.ascii_uppercase + string.digits):
-    x=''.join(random.choice(chars) for _ in range(size))
-    if not User_Keys.objects.filter(properties__icontains='"key": "%s"'%x).exists(): return x
-    else: return id_generator(size,chars)
+    x = "".join(random.choice(chars) for _ in range(size))
+    if not User_Keys.objects.filter(properties__icontains='"key": "%s"' % x).exists():
+        return x
+    return id_generator(size, chars)
+
 
 def getUserAgent(request):
-    id=id=request.session.get("td_id",None)
-    if id:
-        tk=User_Keys.objects.get(id=id)
-        if tk.properties.get("user_agent","")!="":
+    device_id = request.session.get("td_id", None)
+    if device_id:
+        tk = User_Keys.objects.get(id=device_id)
+        if tk.properties.get("user_agent", "") != "":
             ua = user_agents.parse(tk.properties["user_agent"])
-            res = render(None, "TrustedDevices/user-agent.html", context={"ua":ua})
+            res = render(None, "TrustedDevices/user-agent.html", context={"ua": ua})
             return HttpResponse(res)
-    return HttpResponse("")
+    return HttpResponse("No Device provide", status=401)
+
 
 def trust_device(request):
     tk = User_Keys.objects.get(id=request.session["td_id"])
-    tk.properties["status"]="trusted"
+    tk.properties["status"] = "trusted"
     tk.save()
     del request.session["td_id"]
     return HttpResponse("OK")
 
+
 def checkTrusted(request):
     res = ""
-    id=request.session.get("td_id","")
-    if id!="":
+    id = request.session.get("td_id", "")
+    if id != "":
         try:
             tk = User_Keys.objects.get(id=id)
-            if tk.properties["status"] == "trusted": res = "OK"
+            if tk.properties["status"] == "trusted":
+                res = "OK"
         except:
             pass
     return HttpResponse(res)
 
+
 def getCookie(request):
     tk = User_Keys.objects.get(id=request.session["td_id"])
 
     if tk.properties["status"] == "trusted":
-        context={"added":True}
-        response = render(request,"TrustedDevices/Done.html", context)
-        from datetime import datetime, timedelta
+        context = {"added": True}
+        response = render(request, "TrustedDevices/Done.html", context)
+
         expires = datetime.now() + timedelta(days=180)
-        tk.expires=expires
+        tk.expires = expires
         tk.save()
         response.set_cookie("deviceid", tk.properties["signature"], expires=expires)
         return response
 
+
 def add(request):
-    context=csrf(request)
-    if request.method=="GET":
-        context.update({"username":request.GET.get('u',''),"key":request.GET.get('k','')})
-        return render(request,"TrustedDevices/Add.html",context)
+    context = csrf(request)
+    if request.method == "GET":
+        context.update(
+            {"username": request.GET.get("u", ""), "key": request.GET.get("k", "")}
+        )
+        return render(request, "TrustedDevices/Add.html", context)
     else:
-        key=request.POST["key"].replace("-","").replace(" ","").upper()
+        key = request.POST["key"].replace("-", "").replace(" ", "").upper()
         context["username"] = request.POST["username"]
         context["key"] = request.POST["key"]
-        trusted_keys=User_Keys.objects.filter(username=request.POST["username"],properties__icontains='"key": "%s"'%key)
-        cookie=False
+        trusted_keys = User_Keys.objects.filter(
+            username=request.POST["username"], properties__icontains='"key": "%s"' % key
+        )
+        cookie = False
         if trusted_keys.exists():
-            tk=trusted_keys[0]
-            request.session["td_id"]=tk.id
-            ua=request.META['HTTP_USER_AGENT']
-            agent=user_agents.parse(ua)
+            tk = trusted_keys[0]
+            request.session["td_id"] = tk.id
+            ua = request.META["HTTP_USER_AGENT"]
+            agent = user_agents.parse(ua)
             if agent.is_pc:
-                context["invalid"]="This is a PC, it can't used as a trusted device."
+                context["invalid"] = "This is a PC, it can't used as a trusted device."
             else:
-                tk.properties["user_agent"]=ua
+                tk.properties["user_agent"] = ua
                 tk.save()
-                context["success"]=True
+                context["success"] = True
             # tk.properties["user_agent"]=ua
             # tk.save()
             # context["success"]=True
 
         else:
-            context["invalid"]="The username or key is wrong, please check and try again."
+            context[
+                "invalid"
+            ] = "The username or key is wrong, please check and try again."
+
+        return render(request, "TrustedDevices/Add.html", context)
 
-        return  render(request,"TrustedDevices/Add.html", context)
 
 def start(request):
-    if User_Keys.objects.filter(username=request.user.username,key_type="Trusted Device").count()>= 2:
-        return render(request,"TrustedDevices/start.html",{"not_allowed":True})
-    td=None
-    if not request.session.get("td_id",None):
-        td=User_Keys()
-        td.username=request.user.username
-        td.properties={"key":id_generator(),"status":"adding"}
-        td.key_type="Trusted Device"
+    if (
+        User_Keys.objects.filter(
+            username=request.user.username, key_type="Trusted Device"
+        ).count()
+        >= 2
+    ):
+        return render(request, "TrustedDevices/start.html", {"not_allowed": True})
+    td = None
+    if not request.session.get("td_id", None):
+        td = User_Keys()
+        td.username = request.user.username
+        td.properties = {"key": id_generator(), "status": "adding"}
+        td.key_type = "Trusted Device"
         td.save()
-        request.session["td_id"]=td.id
+        request.session["td_id"] = td.id
     try:
-        if td==None: td=User_Keys.objects.get(id=request.session["td_id"])
-        context={"key":td.properties["key"],"url":request.scheme+"://"+request.get_host() + reverse('add_trusted_device')}
+        if td == None:
+            td = User_Keys.objects.get(id=request.session["td_id"])
+        context = {
+            "key": td.properties["key"],
+            "url": request.scheme
+            + "://"
+            + request.get_host()
+            + reverse("add_trusted_device"),
+        }
     except:
         del request.session["td_id"]
         return start(request)
-    return render(request,"TrustedDevices/start.html",context)
+    return render(request, "TrustedDevices/start.html", context)
+
 
 def send_email(request):
-    body=render(request,"TrustedDevices/email.html",{}).content
+    body = render(request, "TrustedDevices/email.html", {}).content
     from .Common import send
-    e=request.user.email
-    if e=="":
-        e=request.session.get("user",{}).get("email","")
-    if e=="":
+
+    e = request.user.email
+    if e == "":
+        e = request.session.get("user", {}).get("email", "")
+    if e == "":
         res = "User has no email on the system."
-    elif send([e],"Add Trusted Device Link",body):
-        res="Sent Successfully"
+    elif send([e], "Add Trusted Device Link", body):
+        res = "Sent Successfully"
     else:
-        res="Error occured, please try again later."
+        res = "Error occured, please try again later."
     return HttpResponse(res)
 
 
 def verify(request):
-    if request.COOKIES.get('deviceid',None):
+    if request.COOKIES.get("deviceid", None):
         from jose import jwt
-        json= jwt.decode(request.COOKIES.get('deviceid'),settings.SECRET_KEY)
-        if json["username"].lower()== request.session['base_username'].lower():
+
+        json = jwt.decode(request.COOKIES.get("deviceid"), settings.SECRET_KEY)
+        if json["username"].lower() == request.session["base_username"].lower():
             try:
-                uk = User_Keys.objects.get(username=request.POST["username"].lower(), properties__icontains='"key": "%s"'%json["key"])
+                uk = User_Keys.objects.get(
+                    username=request.POST["username"].lower(),
+                    properties__icontains='"key": "%s"' % json["key"],
+                )
                 if uk.enabled and uk.properties["status"] == "trusted":
-                    uk.last_used=timezone.now()
+                    uk.last_used = timezone.now()
                     uk.save()
-                    request.session["mfa"] = {"verified": True, "method": "Trusted Device","id":uk.id}
+                    request.session["mfa"] = {
+                        "verified": True,
+                        "method": "Trusted Device",
+                        "id": uk.id,
+                    }
                     return True
             except:
                 import traceback
+
                 print(traceback.format_exc())
                 return False
     return False
```

### Comparing `django-mfa2-2.8.0/mfa/U2F.py` & `django-mfa2-2.9.0b1/mfa/U2F.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,171 @@
-
-from u2flib_server.u2f import (begin_registration, begin_authentication,
-                               complete_registration, complete_authentication)
+from u2flib_server.u2f import (
+    begin_registration,
+    begin_authentication,
+    complete_registration,
+    complete_authentication,
+)
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.serialization import Encoding
 from django.shortcuts import render
 import simplejson
-#from django.template.context import RequestContext
+
 from django.template.context_processors import csrf
-from django.conf import settings
 from django.http import HttpResponse
-from .models import *
+from django.conf import settings
+from .models import User_Keys
 from .views import login
 from .Common import get_redirect_url
-import datetime
 from django.utils import timezone
 
+
 def recheck(request):
     context = csrf(request)
-    context["mode"]="recheck"
+    context["mode"] = "recheck"
     s = sign(request.user.username)
     request.session["_u2f_challenge_"] = s[0]
     context["token"] = s[1]
-    request.session["mfa_recheck"]=True
-    return render(request,"U2F/recheck.html", context)
+    request.session["mfa_recheck"] = True
+    return render(request, "U2F/recheck.html", context)
+
 
 def process_recheck(request):
-    x=validate(request,request.user.username)
-    if x==True:
+    x = validate(request, request.user.username)
+    if x == True:
         import time
+
         request.session["mfa"]["rechecked_at"] = time.time()
-        return HttpResponse(simplejson.dumps({"recheck":True}),content_type="application/json")
+        return HttpResponse(
+            simplejson.dumps({"recheck": True}), content_type="application/json"
+        )
     return x
 
+
 def check_errors(request, data):
     if "errorCode" in data:
-        if data["errorCode"] == 0: return True
+        if data["errorCode"] == 0:
+            return True
         if data["errorCode"] == 4:
             return HttpResponse("Invalid Security Key")
         if data["errorCode"] == 1:
             return auth(request)
     return True
-def validate(request,username):
+
+
+def validate(request, username):
     import datetime, random
 
     data = simplejson.loads(request.POST["response"])
 
-    res= check_errors(request,data)
-    if res!=True:
+    res = check_errors(request, data)
+    if res != True:
         return res
 
-    challenge = request.session.pop('_u2f_challenge_')
+    challenge = request.session.pop("_u2f_challenge_")
     device, c, t = complete_authentication(challenge, data, [settings.U2F_APPID])
     try:
-        key=User_Keys.objects.get(username=username,properties__icontains='"publicKey": "%s"'%device["publicKey"])
-        key.last_used=timezone.now()
+        key = User_Keys.objects.get(
+            username=username,
+            properties__icontains='"publicKey": "%s"' % device["publicKey"],
+        )
+        key.last_used = timezone.now()
         key.save()
-        mfa = {"verified": True, "method": "U2F","id":key.id}
+        mfa = {"verified": True, "method": "U2F", "id": key.id}
         if getattr(settings, "MFA_RECHECK", False):
-            mfa["next_check"] = datetime.datetime.timestamp((datetime.datetime.now()
-                                     + datetime.timedelta(
-                        seconds=random.randint(settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX))))
+            mfa["next_check"] = datetime.datetime.timestamp(
+                (
+                    datetime.datetime.now()
+                    + datetime.timedelta(
+                        seconds=random.randint(
+                            settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX
+                        )
+                    )
+                )
+            )
         request.session["mfa"] = mfa
         return True
     except:
         return False
 
 
-
 def auth(request):
-    context=csrf(request)
-    s=sign(request.session["base_username"])
-    request.session["_u2f_challenge_"]=s[0]
-    context["token"]=s[1]
-    context["method"] = {"name": getattr(settings, "MFA_RENAME_METHODS", {}).get("U2F", "Classical Security Key")}
-    return render(request,"U2F/Auth.html",context)
+    context = csrf(request)
+    s = sign(request.session["base_username"])
+    request.session["_u2f_challenge_"] = s[0]
+    context["token"] = s[1]
+    context["method"] = {
+        "name": getattr(settings, "MFA_RENAME_METHODS", {}).get(
+            "U2F", "Classical Security Key"
+        )
+    }
+    return render(request, "U2F/Auth.html", context)
+
 
 def start(request):
     enroll = begin_registration(settings.U2F_APPID, [])
-    request.session['_u2f_enroll_'] = enroll.json
-    context=csrf(request)
-    context["token"]=simplejson.dumps(enroll.data_for_client)
+    request.session["_u2f_enroll_"] = enroll.json
+    context = csrf(request)
+    context["token"] = simplejson.dumps(enroll.data_for_client)
     context.update(get_redirect_url())
-    context["method"] = {"name": getattr(settings, "MFA_RENAME_METHODS", {}).get("U2F", "Classical Security Key")}
-    context["RECOVERY_METHOD"] = getattr(settings, "MFA_RENAME_METHODS", {}).get("RECOVERY", "Recovery codes")
-    return render(request,"U2F/Add.html",context)
+    context["method"] = {
+        "name": getattr(settings, "MFA_RENAME_METHODS", {}).get(
+            "U2F", "Classical Security Key"
+        )
+    }
+    context["RECOVERY_METHOD"] = getattr(settings, "MFA_RENAME_METHODS", {}).get(
+        "RECOVERY", "Recovery codes"
+    )
+    return render(request, "U2F/Add.html", context)
 
 
 def bind(request):
     import hashlib
-    enroll = request.session['_u2f_enroll_']
-    data=simplejson.loads(request.POST["response"])
+
+    enroll = request.session["_u2f_enroll_"]
+    data = simplejson.loads(request.POST["response"])
     device, cert = complete_registration(enroll, data, [settings.U2F_APPID])
     cert = x509.load_der_x509_certificate(cert, default_backend())
-    cert_hash=hashlib.md5(cert.public_bytes(Encoding.PEM)).hexdigest()
-    q=User_Keys.objects.filter(key_type="U2F", properties__icontains= cert_hash)
+    cert_hash = hashlib.md5(cert.public_bytes(Encoding.PEM)).hexdigest()
+    q = User_Keys.objects.filter(key_type="U2F", properties__icontains=cert_hash)
     if q.exists():
-        return HttpResponse("This key is registered before, it can't be registered again.")
-    User_Keys.objects.filter(username=request.user.username,key_type="U2F").delete()
+        return HttpResponse(
+            "This key is registered before, it can't be registered again."
+        )
+    User_Keys.objects.filter(username=request.user.username, key_type="U2F").delete()
     uk = User_Keys()
     uk.username = request.user.username
     uk.owned_by_enterprise = getattr(settings, "MFA_OWNED_BY_ENTERPRISE", False)
-    uk.properties = {"device":simplejson.loads(device.json),"cert":cert_hash}
+    uk.properties = {"device": simplejson.loads(device.json), "cert": cert_hash}
     uk.key_type = "U2F"
     uk.save()
-    if getattr(settings, 'MFA_ENFORCE_RECOVERY_METHOD', False) and not User_Keys.objects.filter(key_type="RECOVERY",
-                                                                                                username=request.user.username).exists():
-        request.session["mfa_reg"] = {"method": "U2F",
-                                      "name": getattr(settings, "MFA_RENAME_METHODS", {}).get("U2F", "Classical Security Key")}
-        return HttpResponse('RECOVERY')
+    if (
+        getattr(settings, "MFA_ENFORCE_RECOVERY_METHOD", False)
+        and not User_Keys.objects.filter(
+            key_type="RECOVERY", username=request.user.username
+        ).exists()
+    ):
+        request.session["mfa_reg"] = {
+            "method": "U2F",
+            "name": getattr(settings, "MFA_RENAME_METHODS", {}).get(
+                "U2F", "Classical Security Key"
+            ),
+        }
+        return HttpResponse("RECOVERY")
     return HttpResponse("OK")
 
+
 def sign(username):
-    u2f_devices=[d.properties["device"] for d in User_Keys.objects.filter(username=username,key_type="U2F")]
+    u2f_devices = [
+        d.properties["device"]
+        for d in User_Keys.objects.filter(username=username, key_type="U2F")
+    ]
     challenge = begin_authentication(settings.U2F_APPID, u2f_devices)
-    return [challenge.json,simplejson.dumps(challenge.data_for_client)]
+    return [challenge.json, simplejson.dumps(challenge.data_for_client)]
+
 
 def verify(request):
-    x= validate(request,request.session["base_username"])
-    if x==True:
+    x = validate(request, request.session["base_username"])
+    if x == True:
         return login(request)
-    else: return x
+    else:
+        return x
```

### Comparing `django-mfa2-2.8.0/mfa/helpers.py` & `django-mfa2-2.9.0b1/mfa/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-import pyotp
-from .models import *
-from . import TrustedDevice, U2F, FIDO2, totp
 import simplejson
 from django.shortcuts import HttpResponse
-from mfa.views import verify,goto
-def has_mfa(request,username):
-    if User_Keys.objects.filter(username=username,enabled=1).count()>0:
+from mfa.views import verify
+from . import TrustedDevice, U2F, FIDO2, totp
+from .models import User_Keys
+
+
+def has_mfa(request, username):
+    if User_Keys.objects.filter(username=username, enabled=1).count() > 0:
         return verify(request, username)
     return False
 
-def is_mfa(request,ignore_methods=[]):
-    if request.session.get("mfa",{}).get("verified",False):
-        if not request.session.get("mfa",{}).get("method",None) in ignore_methods:
+
+def is_mfa(request, ignore_methods=[]):
+    if request.session.get("mfa", {}).get("verified", False):
+        if not request.session.get("mfa", {}).get("method", None) in ignore_methods:
             return True
     return False
 
+
 def recheck(request):
-    method=request.session.get("mfa",{}).get("method",None)
+    method = request.session.get("mfa", {}).get("method", None)
     if not method:
-        return HttpResponse(simplejson.dumps({"res":False}),content_type="application/json")
-    if method=="Trusted Device":
-        return HttpResponse(simplejson.dumps({"res":TrustedDevice.verify(request)}),content_type="application/json")
-    elif method=="U2F":
-        return HttpResponse(simplejson.dumps({"html": U2F.recheck(request).content}), content_type="application/json")
+        return HttpResponse(
+            simplejson.dumps({"res": False}), content_type="application/json"
+        )
+    if method == "Trusted Device":
+        return HttpResponse(
+            simplejson.dumps({"res": TrustedDevice.verify(request)}),
+            content_type="application/json",
+        )
+    elif method == "U2F":
+        return HttpResponse(
+            simplejson.dumps({"html": U2F.recheck(request).content}),
+            content_type="application/json",
+        )
     elif method == "FIDO2":
-        return HttpResponse(simplejson.dumps({"html": FIDO2.recheck(request).content}), content_type="application/json")
-    elif method=="TOTP":
-        return HttpResponse(simplejson.dumps({"html": totp.recheck(request).content}), content_type="application/json")
-
-
-
+        return HttpResponse(
+            simplejson.dumps({"html": FIDO2.recheck(request).content}),
+            content_type="application/json",
+        )
+    elif method == "TOTP":
+        return HttpResponse(
+            simplejson.dumps({"html": totp.recheck(request).content}),
+            content_type="application/json",
+        )
```

### Comparing `django-mfa2-2.8.0/mfa/middleware.py` & `django-mfa2-2.9.0b1/mfa/middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 import time
 from django.http import HttpResponseRedirect
-from django.core.urlresolvers import reverse
+
+try:
+    from django.urls import reverse
+except ImportError:
+    from django.core.urlresolvers import reverse  # pyre-ignore[21]
+
+
 from django.conf import settings
+
+
 def process(request):
-    next_check=request.session.get('mfa',{}).get("next_check",False)
-    if not next_check: return None
-    now=int(time.time())
+    next_check = request.session.get("mfa", {}).get("next_check", False)
+    if not next_check:
+        return None
+    now = int(time.time())
     if now >= next_check:
-        method=request.session["mfa"]["method"]
+        method = request.session["mfa"]["method"]
         path = request.META["PATH_INFO"]
-        return HttpResponseRedirect(reverse(method+"_auth")+"?next=%s"%(settings.BASE_URL + path).replace("//", "/"))
-    return None
+        return HttpResponseRedirect(
+            reverse(method + "_auth")
+            + "?next=%s" % (settings.BASE_URL + path).replace("//", "/")
+        )
+    return None
```

### Comparing `django-mfa2-2.8.0/mfa/migrations/0005_auto_20181115_2014.py` & `django-mfa2-2.9.0b1/mfa/migrations/0005_auto_20181115_2014.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 from django.db import models, migrations
+
 try:
     from django.db.models import JSONField
 except ImportError:
     try:
-        from jsonfield.fields import JSONField
+        from jsonfield.fields import JSONField  # pyre-ignore[21]
     except ImportError:
-        raise ImportError("Can't find a JSONField implementation, please install jsonfield if django < 4.0")
-
+        raise ImportError(
+            "Can't find a JSONField implementation, please install jsonfield if django < 4.0"
+        )
 
 
 def modify_json(apps, schema_editor):
     from django.conf import settings
+
     if "mysql" in settings.DATABASES.get("default", {}).get("engine", ""):
         migrations.RunSQL("alter table mfa_user_keys modify column properties json;")
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ('mfa', '0004_user_keys_enabled'),
+        ("mfa", "0004_user_keys_enabled"),
     ]
 
     operations = [
         migrations.RemoveField(
-            model_name='user_keys',
-            name='secret_key',
+            model_name="user_keys",
+            name="secret_key",
         ),
         migrations.AddField(
-            model_name='user_keys',
-            name='properties',
+            model_name="user_keys",
+            name="properties",
             field=JSONField(null=True),
         ),
-        migrations.RunPython(modify_json)
+        migrations.RunPython(modify_json),
     ]
```

### Comparing `django-mfa2-2.8.0/mfa/migrations/0006_trusted_devices.py` & `django-mfa2-2.9.0b1/mfa/migrations/0006_trusted_devices.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 from django.db import models, migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('mfa', '0005_auto_20181115_2014'),
+        ("mfa", "0005_auto_20181115_2014"),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Trusted_Devices',
+            name="Trusted_Devices",
             fields=[
-                ('id', models.AutoField(verbose_name='ID', serialize=False, auto_created=True, primary_key=True)),
-                ('signature', models.CharField(max_length=255)),
-                ('key', models.CharField(max_length=6)),
-                ('username', models.CharField(max_length=50)),
-                ('user_agent', models.CharField(max_length=255)),
-                ('status', models.CharField(default=b'adding', max_length=255)),
-                ('added_on', models.DateTimeField(auto_now_add=True)),
-                ('last_used', models.DateTimeField(default=None, null=True)),
+                (
+                    "id",
+                    models.AutoField(
+                        verbose_name="ID",
+                        serialize=False,
+                        auto_created=True,
+                        primary_key=True,
+                    ),
+                ),
+                ("signature", models.CharField(max_length=255)),
+                ("key", models.CharField(max_length=6)),
+                ("username", models.CharField(max_length=50)),
+                ("user_agent", models.CharField(max_length=255)),
+                ("status", models.CharField(default=b"adding", max_length=255)),
+                ("added_on", models.DateTimeField(auto_now_add=True)),
+                ("last_used", models.DateTimeField(default=None, null=True)),
             ],
         ),
     ]
```

### Comparing `django-mfa2-2.8.0/mfa/migrations/0009_user_keys_owned_by_enterprise.py` & `django-mfa2-2.9.0b1/mfa/migrations/0009_user_keys_owned_by_enterprise.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from __future__ import unicode_literals
 
 from django.db import models, migrations
 from django.conf import settings
 
 
 def update_owned_by_enterprise(apps, schema_editor):
-    user_keys = apps.get_model('mfa', 'user_keys')
-    user_keys.objects.filter(key_type='FIDO2').update(owned_by_enterprise=getattr(settings,"MFA_OWNED_BY_ENTERPRISE",False))
+    user_keys = apps.get_model("mfa", "user_keys")
+    user_keys.objects.filter(key_type="FIDO2").update(
+        owned_by_enterprise=getattr(settings, "MFA_OWNED_BY_ENTERPRISE", False)
+    )
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('mfa', '0008_user_keys_last_used'),
+        ("mfa", "0008_user_keys_last_used"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='user_keys',
-            name='owned_by_enterprise',
+            model_name="user_keys",
+            name="owned_by_enterprise",
             field=models.NullBooleanField(default=None),
         ),
-        migrations.RunPython(update_owned_by_enterprise)
+        migrations.RunPython(update_owned_by_enterprise),
     ]
```

### Comparing `django-mfa2-2.8.0/mfa/models.py` & `django-mfa2-2.9.0b1/mfa/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 from django.db import models
+from jose import jwt
+from django.conf import settings
+
 try:
     from django.db.models import JSONField
 except ModuleNotFoundError:
     try:
-        from jsonfield import JSONField
-    except ModuleNotFoundError:
-        raise ModuleNotFoundError("Can't find a JSONField implementation, please install jsonfield if django < 4.0")
+        from jsonfield import JSONField  # pyre-ignore[21]
+    except ModuleNotFoundError as exc:
+        raise ModuleNotFoundError(
+            "Can't find a JSONField implementation, please install jsonfield if django < 4.0"
+        )
 
-from jose import jwt
-from django.conf import settings
-#from jsonLookup import shasLookup, hasLookup
-# JSONField.register_lookup(shasLookup)
-# JSONField.register_lookup(hasLookup)
 
 
 class User_Keys(models.Model):
-    username=models.CharField(max_length = 50)
-    properties=JSONField(null = True)
-    added_on=models.DateTimeField(auto_now_add = True)
-    key_type=models.CharField(max_length = 25,default = "TOTP")
-    enabled=models.BooleanField(default=True)
-    expires=models.DateTimeField(null=True,default=None,blank=True)
-    last_used=models.DateTimeField(null=True,default=None,blank=True)
-    owned_by_enterprise=models.BooleanField(default=None,null=True,blank=True)
-
-    def save(self, force_insert=False, force_update=False, using=None, update_fields=None):
-        if self.key_type == "Trusted Device" and self.properties.get("signature","") == "":
-            self.properties["signature"]= jwt.encode({"username": self.username, "key": self.properties["key"]}, settings.SECRET_KEY)
-        super(User_Keys, self).save(force_insert=force_insert, force_update=force_update, using=using, update_fields=update_fields)
+    username = models.CharField(max_length=50)
+    properties = JSONField(null=True)
+    added_on = models.DateTimeField(auto_now_add=True)
+    key_type = models.CharField(max_length=25, default="TOTP")
+    enabled = models.BooleanField(default=True)
+    expires = models.DateTimeField(null=True, default=None, blank=True)
+    last_used = models.DateTimeField(null=True, default=None, blank=True)
+    owned_by_enterprise = models.BooleanField(default=None, null=True, blank=True)
+
+    def save(
+        self, force_insert=False, force_update=False, using=None, update_fields=None
+    ):
+        if (
+            self.key_type == "Trusted Device"
+            and self.properties.get("signature", "") == ""
+        ):
+            self.properties["signature"] = jwt.encode(
+                {"username": self.username, "key": self.properties["key"]},
+                settings.SECRET_KEY,
+            )
+        super(User_Keys, self).save(
+            force_insert=force_insert,
+            force_update=force_update,
+            using=using,
+            update_fields=update_fields,
+        )
 
     def __unicode__(self):
-        return "%s -- %s"%(self.username,self.key_type)
+        return "%s -- %s" % (self.username, self.key_type)
 
     def __str__(self):
         return self.__unicode__()
 
     class Meta:
-        app_label='mfa'
+        app_label = "mfa"
```

### Comparing `django-mfa2-2.8.0/mfa/recovery.py` & `django-mfa2-2.9.0b1/mfa/recovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,153 @@
+import time
+import random
+import string
+import simplejson
+
 from django.shortcuts import render
 from django.views.decorators.cache import never_cache
 from django.template.context_processors import csrf
+from django.utils import timezone
 from django.contrib.auth.hashers import make_password, PBKDF2PasswordHasher
 from django.http import HttpResponse
+from django.conf import settings
 from .Common import get_redirect_url
-from .models import *
-import simplejson
-import random
-import string
-import datetime
-from django.utils import timezone
+from .models import User_Keys
 
 USER_FRIENDLY_NAME = "Recovery Codes"
 
+
 class Hash(PBKDF2PasswordHasher):
-    algorithm = 'pbkdf2_sha256_custom'
-    iterations = getattr(settings,"RECOVERY_ITERATION",1)
+    algorithm = "pbkdf2_sha256_custom"
+    iterations = getattr(settings, "RECOVERY_ITERATION", 1)
+
 
 def delTokens(request):
-    #Only when all MFA have been deactivated, or to generate new !
-    #We iterate only to clean if any error happend and multiple entry of RECOVERY created for one user
-    for key in User_Keys.objects.filter(username=request.user.username, key_type = "RECOVERY"):
+    # Only when all MFA have been deactivated, or to generate new !
+    # We iterate only to clean if any error happend and multiple entry of RECOVERY created for one user
+    for key in User_Keys.objects.filter(
+        username=request.user.username, key_type="RECOVERY"
+    ):
         if key.username == request.user.username:
             key.delete()
 
+
 def randomGen(n):
-    return ''.join(random.choice(string.ascii_uppercase + string.ascii_lowercase + string.digits) for _ in range(n))
+    return "".join(
+        random.choice(string.ascii_uppercase + string.ascii_lowercase + string.digits)
+        for _ in range(n)
+    )
+
 
 @never_cache
 def genTokens(request):
-    #Delete old ones
+    # Delete old ones
     delTokens(request)
-    #Then generate new one
+    # Then generate new one
     salt = randomGen(15)
     hashedKeys = []
     clearKeys = []
     for i in range(5):
-            token = randomGen(5) + "-" + randomGen(5)
-            hashedToken = make_password(token, salt, 'pbkdf2_sha256_custom')
-            hashedKeys.append(hashedToken)
-            clearKeys.append(token)
-    uk=User_Keys()
+        token = randomGen(5) + "-" + randomGen(5)
+        hashedToken = make_password(token, salt, "pbkdf2_sha256_custom")
+        hashedKeys.append(hashedToken)
+        clearKeys.append(token)
+    uk = User_Keys()
 
     uk.username = request.user.username
-    uk.properties={"secret_keys":hashedKeys, "salt":salt}
-    uk.key_type="RECOVERY"
+    uk.properties = {"secret_keys": hashedKeys, "salt": salt}
+    uk.key_type = "RECOVERY"
     uk.enabled = True
     uk.save()
-    return HttpResponse(simplejson.dumps({"keys":clearKeys}))
+    return HttpResponse(simplejson.dumps({"keys": clearKeys}))
 
 
 def verify_login(request, username, token):
-    for key in User_Keys.objects.filter(username=username, key_type = "RECOVERY"):
+    for key in User_Keys.objects.filter(username=username, key_type="RECOVERY"):
         secret_keys = key.properties["secret_keys"]
         salt = key.properties["salt"]
         hashedToken = make_password(token, salt, "pbkdf2_sha256_custom")
-        for i,token in enumerate(secret_keys):
+        for i, token in enumerate(secret_keys):
             if hashedToken == token:
                 secret_keys.pop(i)
                 key.properties["secret_keys"] = secret_keys
-                key.last_used= timezone.now()
+                key.last_used = timezone.now()
                 key.save()
                 return [True, key.id, len(secret_keys) == 0]
     return [False]
 
+
 def getTokenLeft(request):
-    uk = User_Keys.objects.filter(username=request.user.username, key_type = "RECOVERY")
-    keyLeft=0
+    uk = User_Keys.objects.filter(username=request.user.username, key_type="RECOVERY")
+    keyLeft = 0
     for key in uk:
         keyLeft += len(key.properties["secret_keys"])
-    return HttpResponse(simplejson.dumps({"left":keyLeft}))
+    return HttpResponse(simplejson.dumps({"left": keyLeft}))
+
 
 def recheck(request):
     context = csrf(request)
-    context["mode"]="recheck"
+    context["mode"] = "recheck"
     if request.method == "POST":
-        if verify_login(request,request.user.username, token=request.POST["recovery"])[0]:
-            import time
+        if verify_login(request, request.user.username, token=request.POST["recovery"])[
+            0
+        ]:
+
             request.session["mfa"]["rechecked_at"] = time.time()
-            return HttpResponse(simplejson.dumps({"recheck": True}), content_type="application/json")
+            return HttpResponse(
+                simplejson.dumps({"recheck": True}), content_type="application/json"
+            )
         else:
-            return HttpResponse(simplejson.dumps({"recheck": False}), content_type="application/json")
-    return render(request,"RECOVERY/recheck.html", context)
+            return HttpResponse(
+                simplejson.dumps({"recheck": False}), content_type="application/json"
+            )
+    return render(request, "RECOVERY/recheck.html", context)
+
 
 @never_cache
 def auth(request):
     from .views import login
-    context=csrf(request)
-    if request.method=="POST":
+
+    context = csrf(request)
+    if request.method == "POST":
         tokenLength = len(request.POST["recovery"])
         if tokenLength == 11 and "RECOVERY" not in settings.MFA_UNALLOWED_METHODS:
-            #Backup code check
-            resBackup=verify_login(request, request.session["base_username"], token=request.POST["recovery"])
+            # Backup code check
+            resBackup = verify_login(
+                request,
+                request.session["base_username"],
+                token=request.POST["recovery"],
+            )
             if resBackup[0]:
-                mfa = {"verified": True, "method": "RECOVERY","id":resBackup[1], "lastBackup":resBackup[2]}
+                mfa = {
+                    "verified": True,
+                    "method": "RECOVERY",
+                    "id": resBackup[1],
+                    "lastBackup": resBackup[2],
+                }
                 # if getattr(settings, "MFA_RECHECK", False):
                 #     mfa["next_check"] = datetime.datetime.timestamp((datetime.datetime.now()
                 #                             + datetime.timedelta(
                 #                 seconds=random.randint(settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX))))
                 request.session["mfa"] = mfa
                 if resBackup[2]:
-                    #If the last bakup code has just been used, we return a response insead of redirecting to login
+                    # If the last bakup code has just been used, we return a response insead of redirecting to login
                     context["lastBackup"] = True
-                    return render(request,"RECOVERY/Auth.html", context)                
+                    return render(request, "RECOVERY/Auth.html", context)
                 return login(request)
-        context["invalid"]=True
+        context["invalid"] = True
 
-    elif request.method=="GET":
+    elif request.method == "GET":
         mfa = request.session.get("mfa")
         if mfa and mfa["verified"] and mfa["lastBackup"]:
             return login(request)
 
-    return render(request,"RECOVERY/Auth.html", context)
+    return render(request, "RECOVERY/Auth.html", context)
+
 
 @never_cache
 def start(request):
     """Start Managing recovery tokens"""
     context = get_redirect_url()
     if "mfa_reg" in request.session:
         context["mfa_redirect"] = request.session["mfa_reg"]["name"]
-    return render(request,"RECOVERY/Add.html",context)
+    return render(request, "RECOVERY/Add.html", context)
```

### Comparing `django-mfa2-2.8.0/mfa/static/mfa/css/bootstrap-toggle.min.css` & `django-mfa2-2.9.0b1/mfa/static/mfa/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/static/mfa/js/bootstrap-toggle.min.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/static/mfa/js/cbor.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/cbor.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/static/mfa/js/qrious.min.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/static/mfa/js/u2f-api.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/u2f-api.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/static/mfa/js/ua-parser.min.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/ua-parser.min.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/Email/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/Email/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/Email/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/Email/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/FIDO2/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/FIDO2/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/FIDO2/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/FIDO2/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/MFA.html` & `django-mfa2-2.9.0b1/mfa/templates/MFA.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/RECOVERY/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/RECOVERY/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/RECOVERY/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/RECOVERY/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/TOTP/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/TOTP/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/TOTP/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/TOTP/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/TrustedDevices/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/TrustedDevices/Done.html` & `django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Done.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/TrustedDevices/start.html` & `django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/start.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/U2F/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/U2F/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/U2F/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/U2F/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/mfa_check.html` & `django-mfa2-2.9.0b1/mfa/templates/mfa_check.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/modal.html` & `django-mfa2-2.9.0b1/mfa/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/templates/select_mfa_method.html` & `django-mfa2-2.9.0b1/mfa/templates/select_mfa_method.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.8.0/mfa/totp.py` & `django-mfa2-2.9.0b1/mfa/totp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,125 @@
+import random
+import datetime
+import simplejson
+import pyotp
 from django.shortcuts import render
 from django.views.decorators.cache import never_cache
 from django.http import HttpResponse
-from .Common import get_redirect_url
-from .models import *
 from django.template.context_processors import csrf
-import simplejson
 from django.conf import settings
-import pyotp
-from .views import login
-import datetime
 from django.utils import timezone
-import random
+from .views import login
+from .Common import get_redirect_url
+from .models import User_Keys
 
 
-def verify_login(request,username,token):
-    for key in User_Keys.objects.filter(username=username,key_type = "TOTP"):
+def verify_login(request, username, token):
+    for key in User_Keys.objects.filter(username=username, key_type="TOTP"):
         totp = pyotp.TOTP(key.properties["secret_key"])
-        if  totp.verify(token,valid_window = 30):
-            key.last_used=timezone.now()
+        if totp.verify(token, valid_window=30):
+            key.last_used = timezone.now()
             key.save()
-            return [True,key.id]
+            return [True, key.id]
     return [False]
 
+
 def recheck(request):
     context = csrf(request)
-    context["mode"]="recheck"
+    context["mode"] = "recheck"
     if request.method == "POST":
-        if verify_login(request,request.user.username, token=request.POST["otp"])[0]:
-            import time
+        if verify_login(request, request.user.username, token=request.POST["otp"])[0]:
             request.session["mfa"]["rechecked_at"] = time.time()
-            return HttpResponse(simplejson.dumps({"recheck": True}), content_type="application/json")
+            return HttpResponse(
+                simplejson.dumps({"recheck": True}), content_type="application/json"
+            )
         else:
-            return HttpResponse(simplejson.dumps({"recheck": False}), content_type="application/json")
-    return render(request,"TOTP/recheck.html", context)
+            return HttpResponse(
+                simplejson.dumps({"recheck": False}), content_type="application/json"
+            )
+    return render(request, "TOTP/recheck.html", context)
+
 
 @never_cache
 def auth(request):
-    context=csrf(request)
-    if request.method=="POST":
+    context = csrf(request)
+    if request.method == "POST":
         tokenLength = len(request.POST["otp"])
         if tokenLength == 6:
-            #TOTO code check
-            res=verify_login(request,request.session["base_username"],token = request.POST["otp"])
+            # TOTO code check
+            res = verify_login(
+                request, request.session["base_username"], token=request.POST["otp"]
+            )
             if res[0]:
-                mfa = {"verified": True, "method": "TOTP","id":res[1]}
+                mfa = {"verified": True, "method": "TOTP", "id": res[1]}
                 if getattr(settings, "MFA_RECHECK", False):
-                    mfa["next_check"] = datetime.datetime.timestamp((datetime.datetime.now()
-                                            + datetime.timedelta(
-                                seconds=random.randint(settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX))))
+                    mfa["next_check"] = datetime.datetime.timestamp(
+                        (
+                            datetime.datetime.now()
+                            + datetime.timedelta(
+                                seconds=random.randint(
+                                    settings.MFA_RECHECK_MIN, settings.MFA_RECHECK_MAX
+                                )
+                            )
+                        )
+                    )
                 request.session["mfa"] = mfa
                 return login(request)
-        context["invalid"]=True
-    return render(request,"TOTP/Auth.html", context)
-
+        context["invalid"] = True
+    return render(request, "TOTP/Auth.html", context)
 
 
 def getToken(request):
-    secret_key=pyotp.random_base32()
+    secret_key = pyotp.random_base32()
     totp = pyotp.TOTP(secret_key)
-    request.session["new_mfa_answer"]=totp.now()
-    return HttpResponse(simplejson.dumps({"qr":pyotp.totp.TOTP(secret_key).provisioning_uri(str(request.user.username), issuer_name = settings.TOKEN_ISSUER_NAME),
-                         "secret_key": secret_key}))
+    request.session["new_mfa_answer"] = totp.now()
+    return HttpResponse(
+        simplejson.dumps(
+            {
+                "qr": pyotp.totp.TOTP(secret_key).provisioning_uri(
+                    str(request.user.username), issuer_name=settings.TOKEN_ISSUER_NAME
+                ),
+                "secret_key": secret_key,
+            }
+        )
+    )
+
+
 def verify(request):
-    answer=request.GET["answer"]
-    secret_key=request.GET["key"]
+    answer = request.GET["answer"]
+    secret_key = request.GET["key"]
     totp = pyotp.TOTP(secret_key)
-    if totp.verify(answer,valid_window = 60):
-        uk=User_Keys()
-        uk.username=request.user.username
-        uk.properties={"secret_key":secret_key}
-        #uk.name="Authenticatior #%s"%User_Keys.objects.filter(username=user.username,type="TOTP")
-        uk.key_type="TOTP"
+    if totp.verify(answer, valid_window=60):
+        uk = User_Keys()
+        uk.username = request.user.username
+        uk.properties = {"secret_key": secret_key}
+        # uk.name="Authenticatior #%s"%User_Keys.objects.filter(username=user.username,type="TOTP")
+        uk.key_type = "TOTP"
         uk.save()
-        if getattr(settings, 'MFA_ENFORCE_RECOVERY_METHOD', False) and not User_Keys.objects.filter(key_type="RECOVERY",
-                                                                                                    username=request.user.username).exists():
-            request.session["mfa_reg"] = {"method": "TOTP",
-                                          "name": getattr(settings, "MFA_RENAME_METHODS", {}).get("TOTP", "TOTP")}
+        if (
+            getattr(settings, "MFA_ENFORCE_RECOVERY_METHOD", False)
+            and not User_Keys.objects.filter(
+                key_type="RECOVERY", username=request.user.username
+            ).exists()
+        ):
+            request.session["mfa_reg"] = {
+                "method": "TOTP",
+                "name": getattr(settings, "MFA_RENAME_METHODS", {}).get("TOTP", "TOTP"),
+            }
             return HttpResponse("RECOVERY")
         else:
             return HttpResponse("Success")
-    else: return HttpResponse("Error")
+    else:
+        return HttpResponse("Error")
+
 
 @never_cache
 def start(request):
     """Start Adding Time One Time Password (TOTP)"""
     context = get_redirect_url()
-    context["RECOVERY_METHOD"] = getattr(settings, "MFA_RENAME_METHODS", {}).get("RECOVERY", "Recovery codes")
-    context["method"] = {"name":getattr(settings,"MFA_RENAME_METHODS",{}).get("TOTP","Authenticator")}
-    return render(request,"TOTP/Add.html",context)
+    context["RECOVERY_METHOD"] = getattr(settings, "MFA_RENAME_METHODS", {}).get(
+        "RECOVERY", "Recovery codes"
+    )
+    context["method"] = {
+        "name": getattr(settings, "MFA_RENAME_METHODS", {}).get("TOTP", "Authenticator")
+    }
+    return render(request, "TOTP/Add.html", context)
```

### Comparing `django-mfa2-2.8.0/mfa/urls.py` & `django-mfa2-2.9.0b1/mfa/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-from . import views,totp,U2F,TrustedDevice,helpers,FIDO2,Email,recovery
-#app_name='mfa'
+from . import views, totp, U2F, TrustedDevice, helpers, FIDO2, Email, recovery
 
-try:
-    from django.urls import  re_path as url
-except:
-     from django.conf.urls import  url
-urlpatterns = [
-    url(r'totp/start/', totp.start , name="start_new_otop"),
-    url(r'totp/getToken', totp.getToken , name="get_new_otop"),
-    url(r'totp/verify', totp.verify, name="verify_otop"),
-    url(r'totp/auth', totp.auth, name="totp_auth"),
-    url(r'totp/recheck', totp.recheck, name="totp_recheck"),
-
-    url(r'recovery/start', recovery.start, name="manage_recovery_codes"),
-    url(r'recovery/getTokenLeft', recovery.getTokenLeft, name="get_recovery_token_left"),
-    url(r'recovery/genTokens', recovery.genTokens, name="regen_recovery_tokens"),
-    url(r'recovery/auth', recovery.auth, name="recovery_auth"),
-    url(r'recovery/recheck', recovery.recheck, name="recovery_recheck"),
-
-    url(r'email/start/', Email.start , name="start_email"),
-    url(r'email/auth/', Email.auth , name="email_auth"),
-
-    url(r'u2f/$', U2F.start, name="start_u2f"),
-    url(r'u2f/bind', U2F.bind, name="bind_u2f"),
-    url(r'u2f/auth', U2F.auth, name="u2f_auth"),
-    url(r'u2f/process_recheck', U2F.process_recheck, name="u2f_recheck"),
-    url(r'u2f/verify', U2F.verify, name="u2f_verify"),
+# app_name='mfa'
 
-    url(r'fido2/$', FIDO2.start, name="start_fido2"),
-    url(r'fido2/auth', FIDO2.auth, name="fido2_auth"),
-    url(r'fido2/begin_auth', FIDO2.authenticate_begin, name="fido2_begin_auth"),
-    url(r'fido2/complete_auth', FIDO2.authenticate_complete, name="fido2_complete_auth"),
-    url(r'fido2/begin_reg', FIDO2.begin_registeration, name="fido2_begin_reg"),
-    url(r'fido2/complete_reg', FIDO2.complete_reg, name="fido2_complete_reg"),
-    url(r'fido2/recheck', FIDO2.recheck, name="fido2_recheck"),
-
-
-    url(r'td/$', TrustedDevice.start, name="start_td"),
-    url(r'td/add', TrustedDevice.add, name="add_td"),
-    url(r'td/send_link', TrustedDevice.send_email, name="td_sendemail"),
-    url(r'td/get-ua', TrustedDevice.getUserAgent, name="td_get_useragent"),
-    url(r'td/trust', TrustedDevice.trust_device, name="td_trust_device"),
-    url(r'u2f/checkTrusted', TrustedDevice.checkTrusted, name="td_checkTrusted"),
-    url(r'u2f/secure_device', TrustedDevice.getCookie, name="td_securedevice"),
+try:
+    from django.urls import re_path as url
+except ImportError:
+    from django.conf.urls import url
 
-    url(r'^$', views.index, name="mfa_home"),
-    url(r'goto/(.*)', views.goto, name="mfa_goto"),
-    url(r'selct_method', views.show_methods, name="mfa_methods_list"),
-    url(r'recheck', helpers.recheck, name="mfa_recheck"),
-    url(r'toggleKey', views.toggleKey, name="toggle_key"),
-    url(r'delete', views.delKey, name="mfa_delKey"),
-    url(r'reset', views.reset_cookie, name="mfa_reset_cookie"),
 
-            ]
-# print(urlpatterns)
+urlpatterns = [
+    url(r"totp/start/", totp.start, name="start_new_otop"),
+    url(r"totp/getToken", totp.getToken, name="get_new_otop"),
+    url(r"totp/verify", totp.verify, name="verify_otop"),
+    url(r"totp/auth", totp.auth, name="totp_auth"),
+    url(r"totp/recheck", totp.recheck, name="totp_recheck"),
+    url(r"recovery/start", recovery.start, name="manage_recovery_codes"),
+    url(
+        r"recovery/getTokenLeft", recovery.getTokenLeft, name="get_recovery_token_left"
+    ),
+    url(r"recovery/genTokens", recovery.genTokens, name="regen_recovery_tokens"),
+    url(r"recovery/auth", recovery.auth, name="recovery_auth"),
+    url(r"recovery/recheck", recovery.recheck, name="recovery_recheck"),
+    url(r"email/start/", Email.start, name="start_email"),
+    url(r"email/auth/", Email.auth, name="email_auth"),
+    url(r"u2f/$", U2F.start, name="start_u2f"),
+    url(r"u2f/bind", U2F.bind, name="bind_u2f"),
+    url(r"u2f/auth", U2F.auth, name="u2f_auth"),
+    url(r"u2f/process_recheck", U2F.process_recheck, name="u2f_recheck"),
+    url(r"u2f/verify", U2F.verify, name="u2f_verify"),
+    url(r"fido2/$", FIDO2.start, name="start_fido2"),
+    url(r"fido2/auth", FIDO2.auth, name="fido2_auth"),
+    url(r"fido2/begin_auth", FIDO2.authenticate_begin, name="fido2_begin_auth"),
+    url(
+        r"fido2/complete_auth", FIDO2.authenticate_complete, name="fido2_complete_auth"
+    ),
+    url(r"fido2/begin_reg", FIDO2.begin_registeration, name="fido2_begin_reg"),
+    url(r"fido2/complete_reg", FIDO2.complete_reg, name="fido2_complete_reg"),
+    url(r"fido2/recheck", FIDO2.recheck, name="fido2_recheck"),
+    url(r"td/$", TrustedDevice.start, name="start_td"),
+    url(r"td/add", TrustedDevice.add, name="add_td"),
+    url(r"td/send_link", TrustedDevice.send_email, name="td_sendemail"),
+    url(r"td/get-ua", TrustedDevice.getUserAgent, name="td_get_useragent"),
+    url(r"td/trust", TrustedDevice.trust_device, name="td_trust_device"),
+    url(r"u2f/checkTrusted", TrustedDevice.checkTrusted, name="td_checkTrusted"),
+    url(r"u2f/secure_device", TrustedDevice.getCookie, name="td_securedevice"),
+    url(r"^$", views.index, name="mfa_home"),
+    url(r"goto/(.*)", views.goto, name="mfa_goto"),
+    url(r"selct_method", views.show_methods, name="mfa_methods_list"),
+    url(r"recheck", helpers.recheck, name="mfa_recheck"),
+    url(r"toggleKey", views.toggleKey, name="toggle_key"),
+    url(r"delete", views.delKey, name="mfa_delKey"),
+    url(r"reset", views.reset_cookie, name="mfa_reset_cookie"),
+]
+# print(urlpatterns)
```

### Comparing `django-mfa2-2.8.0/mfa/views.py` & `django-mfa2-2.9.0b1/mfa/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,124 @@
 import importlib
 
 from django.shortcuts import render
-from django.http import HttpResponse,HttpResponseRedirect
-from .models import *
+from django.http import HttpResponse, HttpResponseRedirect
+
+
 try:
     from django.urls import reverse
 except:
-    from django.core.urlresolvers import reverse
-from django.template.context_processors import csrf
-from django.template.context import RequestContext
-from django.conf import settings
-from . import TrustedDevice
+    from django.core.urlresolvers import reverse  # pyre-ignore[21]
 from django.contrib.auth.decorators import login_required
+from django.conf import settings
 from user_agents import parse
+from . import TrustedDevice
+from .models import User_Keys
+
 
 @login_required
 def index(request):
-    keys=[]
-    context={"keys":User_Keys.objects.filter(username=request.user.username),"UNALLOWED_AUTHEN_METHODS":settings.MFA_UNALLOWED_METHODS
-             ,"HIDE_DISABLE":getattr(settings,"MFA_HIDE_DISABLE",[]),'RENAME_METHODS':getattr(settings,'MFA_RENAME_METHODS',{})}
+    keys = []
+    context = {
+        "keys": User_Keys.objects.filter(username=request.user.username),
+        "UNALLOWED_AUTHEN_METHODS": settings.MFA_UNALLOWED_METHODS,
+        "HIDE_DISABLE": getattr(settings, "MFA_HIDE_DISABLE", []),
+        "RENAME_METHODS": getattr(settings, "MFA_RENAME_METHODS", {}),
+    }
     for k in context["keys"]:
-        k.name = getattr(settings,'MFA_RENAME_METHODS',{}).get(k.key_type,k.key_type)
-        if k.key_type =="Trusted Device":
-            setattr(k,"device",parse(k.properties.get("user_agent","-----")))
+        k.name = getattr(settings, "MFA_RENAME_METHODS", {}).get(k.key_type, k.key_type)
+        if k.key_type == "Trusted Device":
+            setattr(k, "device", parse(k.properties.get("user_agent", "-----")))
         elif k.key_type == "FIDO2":
-            setattr(k,"device",k.properties.get("type","----"))
+            setattr(k, "device", k.properties.get("type", "----"))
         elif k.key_type == "RECOVERY":
             context["recovery"] = k
             continue
         keys.append(k)
-    context["keys"]=keys
-    return render(request,"MFA.html",context)
+    context["keys"] = keys
+    return render(request, "MFA.html", context)
 
-def verify(request,username):
-    request.session["base_username"] = username
-    #request.session["base_password"] = password
-    keys=User_Keys.objects.filter(username=username,enabled=1)
-    methods=list(set([k.key_type for k in keys]))
 
-    if "Trusted Device" in methods and not request.session.get("checked_trusted_device",False):
+def verify(request, username):
+    request.session["base_username"] = username
+    # request.session["base_password"] = password
+    keys = User_Keys.objects.filter(username=username, enabled=1)
+    methods = list(set([k.key_type for k in keys]))
+
+    if "Trusted Device" in methods and not request.session.get(
+        "checked_trusted_device", False
+    ):
         if TrustedDevice.verify(request):
             return login(request)
         methods.remove("Trusted Device")
     request.session["mfa_methods"] = methods
 
-    if len(methods)==1:
-        return HttpResponseRedirect(reverse(methods[0].lower()+"_auth"))
-    if getattr(settings,"MFA_ALWAYS_GO_TO_LAST_METHOD",False):
+    if len(methods) == 1:
+        return HttpResponseRedirect(reverse(methods[0].lower() + "_auth"))
+    if getattr(settings, "MFA_ALWAYS_GO_TO_LAST_METHOD", False):
         keys = keys.exclude(last_used__isnull=True).order_by("last_used")
-        if keys.count()>0:
+        if keys.count() > 0:
             return HttpResponseRedirect(reverse(keys[0].key_type.lower() + "_auth"))
     return show_methods(request)
 
+
 def show_methods(request):
-    return render(request,"select_mfa_method.html", {'RENAME_METHODS':getattr(settings,'MFA_RENAME_METHODS',{})})
+    return render(
+        request,
+        "select_mfa_method.html",
+        {"RENAME_METHODS": getattr(settings, "MFA_RENAME_METHODS", {})},
+    )
+
 
 def reset_cookie(request):
-    response=HttpResponseRedirect(settings.LOGIN_URL)
+    response = HttpResponseRedirect(settings.LOGIN_URL)
     response.delete_cookie("base_username")
     return response
 
+
 def login(request):
-    from django.contrib import auth
-    from django.conf import settings
     callable_func = __get_callable_function__(settings.MFA_LOGIN_CALLBACK)
-    return callable_func(request,username=request.session["base_username"])
+    return callable_func(request, username=request.session["base_username"])
 
 
 @login_required
 def delKey(request):
-    key=User_Keys.objects.get(id=request.GET["id"])
+    key = User_Keys.objects.get(id=request.GET["id"])
     if key.username == request.user.username:
         key.delete()
         return HttpResponse("Deleted Successfully")
     else:
         return HttpResponse("Error: You own this token so you can't delete it")
 
+
 def __get_callable_function__(func_path):
-    import importlib
-    if not '.' in func_path:
+
+    if not "." in func_path:
         raise Exception("class Name should include modulename.classname")
 
     parsed_str = func_path.split(".")
-    module_name , func_name = ".".join(parsed_str[:-1]) , parsed_str[-1]
+    module_name, func_name = ".".join(parsed_str[:-1]), parsed_str[-1]
     imported_module = importlib.import_module(module_name)
-    callable_func = getattr(imported_module,func_name)
+    callable_func = getattr(imported_module, func_name)
     if not callable_func:
         raise Exception("Module does not have requested function")
     return callable_func
 
+
 @login_required
 def toggleKey(request):
-    id=request.GET["id"]
-    q=User_Keys.objects.filter(username=request.user.username, id=id)
-    if q.count()==1:
-        key=q[0]
+    id = request.GET["id"]
+    q = User_Keys.objects.filter(username=request.user.username, id=id)
+    if q.count() == 1:
+        key = q[0]
         if not key.key_type in settings.MFA_HIDE_DISABLE:
-            key.enabled=not key.enabled
+            key.enabled = not key.enabled
             key.save()
             return HttpResponse("OK")
         else:
             return HttpResponse("You can't change this method.")
     else:
         return HttpResponse("Error")
 
-def goto(request,method):
-    return HttpResponseRedirect(reverse(method.lower()+"_auth"))
+
+def goto(request, method):
+    return HttpResponseRedirect(reverse(method.lower() + "_auth"))
```

### Comparing `django-mfa2-2.8.0/setup.py` & `django-mfa2-2.9.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-mfa2',
-    version='2.8.0',
+    version='2.9.0b1',
     description='Allows user to add 2FA to their accounts',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
 
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-mfa2/',
@@ -19,22 +19,22 @@
         'django >= 2.0',
         'simplejson',
         'pyotp',
         'python-u2flib-server',
         'ua-parser',
         'user-agents',
         'python-jose',
-        'fido2 == 1.0.0',
+        'fido2 >= 1.1.0',
       ],
     python_requires=">=3.5",
     include_package_data=True,
     zip_safe=False, # because we're including static files
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        #"Development Status :: 4 - Beta",
+        #"Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
```

