# Comparing `tmp/koalix-crm-1.13.dev6.tar.gz` & `tmp/koalix-crm-1.13.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/koalix-crm-1.13.dev6.tar", last modified: Mon Dec 30 22:11:17 2019, max compression
+gzip compressed data, was "dist/koalix-crm-1.13.dev9.tar", last modified: Sat Mar 28 17:08:48 2020, max compression
```

## Comparing `koalix-crm-1.13.dev6.tar` & `koalix-crm-1.13.dev9.tar`

### file list

```diff
@@ -1,448 +1,453 @@
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1039 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/global_support_functions.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2326 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/plugin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/
--rw-r--r--   0 jenkins    (112) jenkins    (116)       26 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/views.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3449 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/admin.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4326 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6490 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3715 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3603 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3604 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5735 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      175 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/const/events.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/pt_BR/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2910 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1648 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/de/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/de/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2873 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1507 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/en/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10746 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11838 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/de/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10401 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10486 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)      663 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/exceptions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/management/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/management/commands/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/management/commands/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/management/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3550 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/views.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      623 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/admin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/factories/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      330 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/factories/factory_product_category.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/factories/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      374 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1524 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/account_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2866 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/product_categorie_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2650 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/restinterface.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5414 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/booking_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      720 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/rest/accounting_period_rest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1664 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/product_category.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11316 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/accounting_period.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     8768 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/account.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3405 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/booking.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      780 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4451 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1633 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1285 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3463 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6726 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6786 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      404 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0003_remove_account_originalamount.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2146 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1030 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/tests/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/tests/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11707 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/tests/test_accountingModelTest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      207 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/const/accountTypeChoices.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/pt_BR/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7519 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4242 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/de/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/de/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6010 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2778 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      943 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/exceptions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4427 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/document_template.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7364 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/user_extension.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1042 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5285 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/template_set.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/management/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/management/commands/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/management/commands/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/management/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1838 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/admin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3347 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/factory_document_template.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      696 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/factory_user_extension.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      258 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/factory_template_set.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      325 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    16815 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/template_set_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      695 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/user_extension_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      356 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/user_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3975 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/document_template_rest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     9678 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7474 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1230 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10481 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      637 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6874 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2212 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      229 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/const/purpose.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4568 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/test_support_functions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6075 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/time_reporting.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      842 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/create_work_report.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      983 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/register_payment.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      647 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/exception.html
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    54101 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/logo.jpg
--rw-r--r--   0 jenkins    (112) jenkins    (116)   122303 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5699 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/fontconfig.xml
--rw-r--r--   0 jenkins    (112) jenkins    (116)   704128 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf
--rw-r--r--   0 jenkins    (112) jenkins    (116)   756072 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf
--rw-r--r--   0 jenkins    (112) jenkins    (116)   156738 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/dejavusans.xml
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50534 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50508 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50599 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/invoice.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50630 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/quote.xsl
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/
--rwxr-xr-x   0 jenkins    (112) jenkins    (116)    27411 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/work_report.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50534 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50507 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50540 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/invoice.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    30645 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/project_report.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/quote.xsl
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1232 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/task_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2183 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/generic_task_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2782 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/generic_project_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7885 2019-12-29 17:52:35.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/work.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1001 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1458 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/estimation_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1440 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/agreement_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    26869 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/project.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3037 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1543 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/reporting_period_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1032 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource_price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      861 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/agreement_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1416 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/project_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7245 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/estimation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      744 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/urls.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    27663 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1023 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      614 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource_manager.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      870 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/project_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    13725 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      855 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/task_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11426 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/reporting/reporting_period.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2183 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/exceptions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/management/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/management/commands/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4865 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/management/commands/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/management/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5279 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/customer.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      384 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/email_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1149 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/customer_billing_cycle.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1988 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/person.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2629 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/postal_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1313 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/supplier.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      380 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/phone_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      574 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/customer_group.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     9916 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/contact.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4282 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/contact/call.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1844 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/tax.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2101 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/currency_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1035 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/product_price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2131 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/unit_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5867 2019-12-29 19:53:45.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/product_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      455 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/product.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1809 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/unit.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2971 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/customer_group_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1933 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/currency.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6455 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/product/price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4447 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/admin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      915 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_reporting_period_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      488 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_project_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      848 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_agreement_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      346 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_delivery_note.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1072 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_project.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      689 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_sales_document_position.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      552 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_currency.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      297 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_purchase_confirmation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      751 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_customer_group_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      377 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_resource_manager.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      496 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_customer_group.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      657 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_unit_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      422 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_payment_reminder.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      313 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_resource_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      691 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1398 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_sales_document.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      790 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_customer.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      965 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_contract.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1173 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_generic_project_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1979 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      723 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_currency_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      321 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_tax.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      538 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_project_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      443 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_purchase_order.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      594 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_task_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      453 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_contact.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      512 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1668 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_estimation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1170 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_generic_task_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      457 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_postal_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      383 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_customer_billing_cycle.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      371 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_invoice.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1499 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_resource_price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      868 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_estimation_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      239 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_product.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      951 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_work.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      788 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_task_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      677 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      299 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_quote.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      972 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_product_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      649 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_reporting_period.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      318 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_agreement_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1133 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_user.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      655 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_unit.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1827 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_product_price.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4600 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/pdfexport.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4103 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/time_tracking.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2129 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/user_extension_missing.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6431 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/work_entry_form.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2132 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/create_work_report.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2120 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/template_set_missing.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1948 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/user_is_not_human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5633 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/create_task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2140 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/reporting_period_missing.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1964 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/range_selection_form.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3001 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/newdocument.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2635 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/renderer.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3996 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/views/work_entry_formset.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2885 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1592 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_manager_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2894 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/unit_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      383 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/currency_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      728 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_type_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5586 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/project_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2739 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7180 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/contact_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3417 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/customer_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      944 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/agreement_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4701 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/work_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3711 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/estimation_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2987 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/tax_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      906 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/customer_billing_cycle_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      555 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/customer_group_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      644 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/task_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      662 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/project_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3801 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/product_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10754 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/restinterface.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3623 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/task_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5956 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/agreement_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      734 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/agreement_type_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      962 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/estimation_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4073 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/human_resource_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4438 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_price_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      969 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/reporting_period_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3607 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/rest/reporting_period_rest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1332 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0036_auto_20180626_2059.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      605 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0029_auto_20180611_1903.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      858 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0008_auto_20180104_2042.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      616 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0044_reportingperiod_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      600 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0039_auto_20180702_1635.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      521 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0047_work_worked_hours.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      457 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0010_auto_20180104_2138.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7581 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0015_auto_20180111_2043.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6072 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0025_auto_20180413_1937.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1428 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0048_auto_20181012_2056.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    53282 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5968 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0027_auto_20180606_2034.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2448 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0011_auto_20180104_2152.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      403 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0058_auto_20190401_2009.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1791 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0007_auto_20171210_2126.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2269 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0038_auto_20180702_1628.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      705 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0024_auto_20180122_2121.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3366 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0032_auto_20180612_1925.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2741 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0051_auto_20181014_2302.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      547 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0002_auto_20170927_2042.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1150 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0021_purchaseorder.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      574 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0041_auto_20180724_1657.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      766 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0020_auto_20180116_2056.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2217 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0018_auto_20180111_2031.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1854 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0017_auto_20180111_2022.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4572 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0056_auto_20181216_2224.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      989 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0028_auto_20180611_1835.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      751 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0022_auto_20180117_2020.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      473 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0037_auto_20180701_2128.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    41477 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0005_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      624 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0012_auto_20180105_1840.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2741 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0052_auto_20181014_2304.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4850 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0006_auto_20171210_1805.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2753 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0004_auto_20171009_2008.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2407 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0050_auto_20181014_2300.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      389 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0046_auto_20180805_2051.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1316 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0016_auto_20180111_2011.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1557 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0045_auto_20180805_2047.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      600 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0035_auto_20180619_1924.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1095 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0026_auto_20180507_1957.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      575 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0040_auto_20180724_1657.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      698 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0014_auto_20180108_2048.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1149 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0055_auto_20181022_1937.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      265 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0057_merge_20190106_1510.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    17512 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0053_auto_20181014_2305.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      496 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0054_auto_20181020_1845.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6285 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0009_auto_20180104_2111.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      576 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0056_auto_20190102_2230.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2144 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0013_auto_20180105_2159.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1685 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0034_genericprojectlink.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    42385 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0003_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1542 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0049_auto_20181014_2258.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      732 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0033_auto_20180612_1936.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      576 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0042_auto_20180724_1816.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      486 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0023_auto_20180119_2102.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1955 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0019_auto_20180112_2020.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      514 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0031_auto_20180612_1924.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1085 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0030_auto_20180611_1930.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      981 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0043_reportingperiodstatus.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2510 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_poject_admin_view.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6015 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_work_delete.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5602 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_user_is_not_human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3500 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_planned_costs.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6237 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_view_work_entry_form.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3624 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_update_last_status_update.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3350 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_supplier_admin_view.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5090 2019-12-29 17:52:35.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_sales_document_from_contract.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3754 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_time_tracking_add_row.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4361 2019-12-29 19:53:45.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_incomplete_sales_document_position.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5118 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_effort.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    16624 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_calculations_document.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5669 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_project_planned_costs.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5645 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_duration.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2045 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5232 2019-12-29 17:52:35.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_sales_document_from_quote.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6508 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6969 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_delete_of_empty_row.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6337 2019-12-29 17:52:35.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5665 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5984 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_project_effective_costs.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1105 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_version_increase.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4337 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_planned_effort.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2991 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_constructor.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3258 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_planned_duration.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      188 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/const/postaladdressprefix.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10650 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/const/country.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      955 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/const/status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      935 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/const/purpose.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2152 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/inlinemixin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    13462 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/contract.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    21404 2019-12-29 19:53:45.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/sales_document.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3204 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/payment_reminder.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1326 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/purchase_confirmation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5225 2019-12-29 19:53:45.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/calculations.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     9519 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/invoice.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3578 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/quote.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5038 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/pdf_export.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1983 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/purchase_order.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5730 2019-12-29 19:53:45.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/sales_document_position.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1627 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/documents/delivery_note.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/pt_BR/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    62091 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)    30449 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/de/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/de/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    45333 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)    20733 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jenkins    (112) jenkins    (116)       55 2019-12-29 19:53:45.000000 koalix-crm-1.13.dev6/koalixcrm/version.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      492 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/MANIFEST.in
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3123 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/README.md
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      271 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/requires.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)        1 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)      480 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (112) jenkins    (116)        1 2019-12-29 20:01:31.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (112) jenkins    (116)    17941 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)       26 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/koalix_crm.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)      480 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/PKG-INFO
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:16.000000 koalix-crm-1.13.dev6/projectsettings/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/projectsettings/settings/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      469 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/development_sqlite_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      451 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/development_sqlite_settings_linux.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3985 2019-12-29 17:52:35.000000 koalix-crm-1.13.dev6/projectsettings/settings/base_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      508 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/production_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      676 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/heroku_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      589 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/docker_production_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      509 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/docker_development_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      461 2019-12-27 14:28:09.000000 koalix-crm-1.13.dev6/projectsettings/settings/development_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       38 2019-12-30 22:11:17.000000 koalix-crm-1.13.dev6/setup.cfg
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1433 2019-12-29 17:52:35.000000 koalix-crm-1.13.dev6/setup.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1181 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/global_support_functions.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2326 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/plugin.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       26 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/views.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3449 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/admin.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4326 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/models.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/__init__.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6490 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3715 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3603 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3604 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5735 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/const/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/const/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      175 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/const/events.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2910 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1648 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2873 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1507 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/__init__.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    10746 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    11838 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    10401 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    10486 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      663 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/exceptions.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/commands/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/commands/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3550 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/views.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      623 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/admin.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/factories/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      330 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/factories/factory_product_category.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/factories/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      374 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/models.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/__init__.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1524 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/account_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2866 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/product_categorie_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2650 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/restinterface.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5414 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/booking_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      720 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/accounting_period_rest.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1664 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/product_category.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    11316 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/accounting_period.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     8768 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/account.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3405 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/booking.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      780 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4451 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1633 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1285 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3463 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6726 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6786 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      404 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0003_remove_account_originalamount.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2146 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1030 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/tests/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/tests/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    11709 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/tests/test_accountingModelTest.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/const/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/const/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      207 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/const/accountTypeChoices.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7519 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4242 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6010 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2778 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      943 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/exceptions.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4427 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/document_template.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7364 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/user_extension.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1042 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5285 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/template_set.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/commands/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/commands/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1838 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/admin.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3347 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_document_template.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      696 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_user_extension.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      258 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_template_set.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      325 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/models.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/__init__.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    16815 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/template_set_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      695 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/user_extension_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      356 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/user_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3975 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/document_template_rest.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     9678 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7474 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1230 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    10481 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      637 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6874 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2212 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/const/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/const/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      229 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/const/purpose.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4427 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/test_support_functions.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5940 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/time_reporting.html
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      579 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/set_timezone.html
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      842 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/create_work_report.html
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      983 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/register_payment.html
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      647 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/exception.html
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    54101 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/logo.jpg
+-rw-r--r--   0 jenkins    (112) jenkins    (116)   122303 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5699 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/fontconfig.xml
+-rw-r--r--   0 jenkins    (112) jenkins    (116)   704128 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf
+-rw-r--r--   0 jenkins    (112) jenkins    (116)   756072 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf
+-rw-r--r--   0 jenkins    (112) jenkins    (116)   156738 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans.xml
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50534 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50508 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50599 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/invoice.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50630 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/quote.xsl
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/
+-rwxr-xr-x   0 jenkins    (112) jenkins    (116)    27411 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/work_report.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50534 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50507 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50540 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/invoice.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    30645 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/project_report.xsl
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/quote.xsl
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1232 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2183 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_task_link.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2782 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_project_link.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7885 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/work.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1001 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1458 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1440 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    26869 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3037 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1543 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1032 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_price.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      861 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1416 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7245 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      864 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/urls.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    27663 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1023 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      614 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_manager.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      870 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_link_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    13725 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/human_resource.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      855 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_link_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    11426 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2183 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/exceptions.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4865 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/__init__.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5279 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      384 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/email_address.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1149 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_billing_cycle.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1988 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/person.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/postal_address.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1313 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/supplier.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      380 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/phone_address.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      574 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_group.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     9916 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/contact.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4282 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/call.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1844 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/tax.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2101 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/currency_transform.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1035 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/product_price.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2131 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/unit_transform.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5867 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/product_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      455 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/product.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1809 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/unit.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2971 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/customer_group_transform.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1933 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/currency.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6455 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/price.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4447 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/admin.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/middleware/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/middleware/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      428 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/middleware/timezoneMiddleware.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      915 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      488 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      848 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      346 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_delivery_note.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1072 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      689 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document_position.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      552 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      297 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_purchase_confirmation.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      751 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_group_transform.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      377 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_manager.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      496 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_group.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      657 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit_transform.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      422 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_payment_reminder.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      313 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      691 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_human_resource.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1658 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      790 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      965 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_contract.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1173 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_project_link.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1981 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      723 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency_transform.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      321 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_tax.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      538 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project_link_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      443 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_purchase_order.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      594 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_link_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      453 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_contact.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      512 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1670 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1170 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_task_link.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      457 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_postal_address.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      383 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_billing_cycle.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      371 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_invoice.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1501 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_price.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      868 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      239 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      953 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_work.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      788 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      679 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      299 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_quote.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      974 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      649 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      318 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement_type.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1133 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_user.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      655 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1829 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_price.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4600 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/pdfexport.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      354 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/set_timezone.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4103 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/time_tracking.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2129 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/user_extension_missing.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6226 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_form.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2132 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/create_work_report.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2120 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/template_set_missing.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1948 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/user_is_not_human_resource.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5633 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/create_task.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2140 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/reporting_period_missing.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1964 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/range_selection_form.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3001 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/newdocument.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2635 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/renderer.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3957 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_formset.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2885 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/models.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/__init__.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1592 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_manager_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2894 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/unit_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      383 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/currency_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      728 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_type_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5586 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2739 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7180 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/contact_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3417 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      944 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_status_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4701 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/work_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3711 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2987 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/tax_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      906 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_billing_cycle_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      555 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_group_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      644 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_status_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      662 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_status_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3801 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/product_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    10754 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/restinterface.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3623 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5956 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      734 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_type_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      962 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_status_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4073 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/human_resource_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4438 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_price_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      969 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_status_rest.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3607 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_rest.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1332 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0036_auto_20180626_2059.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      605 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0029_auto_20180611_1903.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      858 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0008_auto_20180104_2042.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      616 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0044_reportingperiod_status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      600 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0039_auto_20180702_1635.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      521 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0047_work_worked_hours.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      457 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0010_auto_20180104_2138.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7581 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0015_auto_20180111_2043.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6072 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0025_auto_20180413_1937.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1428 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0048_auto_20181012_2056.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    53282 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5968 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0027_auto_20180606_2034.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2448 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0011_auto_20180104_2152.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      403 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0058_auto_20190401_2009.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1791 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0007_auto_20171210_2126.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2269 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0038_auto_20180702_1628.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      705 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0024_auto_20180122_2121.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3366 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0032_auto_20180612_1925.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2741 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0051_auto_20181014_2302.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      547 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0002_auto_20170927_2042.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1150 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0021_purchaseorder.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      574 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0041_auto_20180724_1657.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      766 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0020_auto_20180116_2056.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2217 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0018_auto_20180111_2031.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1854 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0017_auto_20180111_2022.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4572 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20181216_2224.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      989 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0028_auto_20180611_1835.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      751 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0022_auto_20180117_2020.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      473 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0037_auto_20180701_2128.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    41477 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0005_auto_20171110_1732.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      624 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0012_auto_20180105_1840.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2741 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0052_auto_20181014_2304.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4850 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0006_auto_20171210_1805.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2753 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0004_auto_20171009_2008.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2407 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0050_auto_20181014_2300.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      389 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0046_auto_20180805_2051.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1316 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0016_auto_20180111_2011.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1557 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0045_auto_20180805_2047.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      600 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0035_auto_20180619_1924.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1095 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0026_auto_20180507_1957.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      575 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0040_auto_20180724_1657.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      698 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0014_auto_20180108_2048.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1149 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0055_auto_20181022_1937.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      265 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0057_merge_20190106_1510.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    17512 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0053_auto_20181014_2305.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      496 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0054_auto_20181020_1845.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6285 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0009_auto_20180104_2111.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      576 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20190102_2230.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2144 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0013_auto_20180105_2159.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1685 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0034_genericprojectlink.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    42385 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0003_auto_20171009_1949.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1542 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0049_auto_20181014_2258.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      732 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0033_auto_20180612_1936.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      576 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0042_auto_20180724_1816.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      486 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0023_auto_20180119_2102.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1955 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0019_auto_20180112_2020.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      514 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0031_auto_20180612_1924.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1085 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0030_auto_20180611_1930.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      981 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0043_reportingperiodstatus.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2510 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_poject_admin_view.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6017 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_work_delete.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5602 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_user_is_not_human_resource.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3500 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_costs.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6608 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_view_work_entry_form.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3624 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_update_last_status_update.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3350 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_supplier_admin_view.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5090 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_contract.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3754 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_time_tracking_add_row.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4363 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_incomplete_sales_document_position.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5120 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_effort.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    16626 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_calculations_document.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5670 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_planned_costs.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5647 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_duration.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2045 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_task.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5232 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_quote.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6510 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     7340 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_delete_of_empty_row.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     6337 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5667 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5986 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_effective_costs.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1105 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_version_increase.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3864 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_effort.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2991 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_constructor.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3260 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_duration.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      188 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/postaladdressprefix.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    10650 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/country.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      955 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/status.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      935 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/purpose.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     2152 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/inlinemixin.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    13462 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/contract.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    21434 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3204 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/payment_reminder.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1326 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_confirmation.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5232 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/calculations.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     9519 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/invoice.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3578 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/quote.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5038 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/pdf_export.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1983 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_order.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     5730 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document_position.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1627 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/delivery_note.py
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    62091 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    30449 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    45333 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    20733 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       55 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/version.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      492 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/MANIFEST.in
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     3123 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/README.md
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      271 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        1 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      480 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        1 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (112) jenkins    (116)    18113 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       26 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      480 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/PKG-INFO
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/projectsettings/
+drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/projectsettings/settings/
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      469 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/development_sqlite_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      451 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/development_sqlite_settings_linux.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/__init__.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     4055 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/base_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      508 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/production_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      676 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/heroku_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      589 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/docker_production_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      509 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/docker_development_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)      461 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/development_settings.py
+-rw-r--r--   0 jenkins    (112) jenkins    (116)       38 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/setup.cfg
+-rw-r--r--   0 jenkins    (112) jenkins    (116)     1433 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/setup.py
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/global_support_functions.py` & `koalix-crm-1.13.dev9/koalixcrm/global_support_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import datetime
 
+import pytz
+
 
 def limit_string_length(input_string, maximum_length):
     if len(input_string) > maximum_length:
         output_string = input_string[:maximum_length]
     else:
         output_string = input_string
     return output_string
@@ -39,7 +41,12 @@
         self.condition = condition
 
     def __call__(self, func):
         if not self.condition:
             # Return the function unchanged, not decorated.
             return func
         return self.decorator(func)
+
+
+def make_date_utc(input_date):
+    output_date = pytz.timezone("UTC").localize(input_date, is_dst=None)
+    return output_date
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/plugin.py` & `koalix-crm-1.13.dev9/koalixcrm/plugin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/admin.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/models.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/models.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0001_initial.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl` & `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl` & `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl` & `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl` & `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/exceptions.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/views.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/views.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/admin.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/rest/account_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/account_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/rest/product_categorie_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/product_categorie_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/rest/restinterface.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/restinterface.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/rest/booking_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/booking_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/rest/accounting_period_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/accounting_period_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/product_category.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/product_category.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/accounting_period.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/accounting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/account.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/account.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/accounting/booking.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/booking.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0001_initial.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/tests/test_accountingModelTest.py` & `koalix-crm-1.13.dev9/koalixcrm/accounting/tests/test_accountingModelTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from django.test import TestCase
 from django.contrib.auth.models import User
 from koalixcrm.accounting.models import Account
 from koalixcrm.accounting.models import AccountingPeriod
 from koalixcrm.accounting.models import Booking
 from koalixcrm.crm.documents.pdf_export import PDFExport
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class AccountingModelTest(TestCase):
     def setUp(self):
         user = User.objects.create(username='Username',
                                    password="Userone")
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/exceptions.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/document_template.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/document_template.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/user_extension.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/user_extension.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/user_extension/template_set.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/template_set.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/admin.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/factory_document_template.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_document_template.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/factories/factory_user_extension.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_user_extension.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/template_set_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/template_set_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/user_extension_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/user_extension_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/rest/document_template_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/document_template_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0001_initial.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py` & `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/test_support_functions.py` & `koalix-crm-1.13.dev9/koalixcrm/test_support_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 
-import pytz
 from selenium.common.exceptions import NoSuchElementException
 import time
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
@@ -29,19 +28,14 @@
         element = testcase.selenium.find_element_by_xpath(xpath)
         if element.text != string:
             print("issue")
     except NoSuchElementException:
         return
 
 
-def make_date_utc(input_date):
-    output_date = pytz.timezone("UTC").localize(input_date, is_dst=None)
-    return output_date
-
-
 def create_sales_document_from_reference(test_case,
                                          timeout,
                                          reference_type,
                                          reference_id,
                                          document_type,
                                          action_name,
                                          template_name,
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/time_reporting.html` & `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/time_reporting.html`

 * *Files 4% similar despite different names*

```diff
@@ -71,29 +71,29 @@
 </script>
 {% endblock %}
 {% block title %}
 Reporting
 {% endblock %}
 
 {% block content %}
+{% load tz %}
 <form action="" method="post">{% csrf_token %}
     {{ formset.management_form }}
     <div style="font-weight: bold;">Selected Range</div>
     <table style="border: none;">
     {{ range_selection_form}}
     </table>
     <br/>
     <div>
         <table cellspacing="0" class="grp-table">
             {% for form in formset.forms %}
             {% if forloop.first %}
             <tr>
                 <th>{{form.project.label}}, {{form.task.label}} </th>
-                <th>{{form.date.label}}</th>
-                <th>{{form.start_time.label}}, {{form.stop_time.label}}</th>
+                <th>{{form.datetime_start.label}}<br/>{{form.datetime_stop.label}}</th>
                 <th>{{form.worked_hours.label}}</th>
                 <th>{{form.description.label}}</th>
                 <th>{{form.DELETE.label}}</th>
             </tr>
             {% endif %}
             {% if form.non_field_errors %}
             <tr class="alert alert-danger">
@@ -105,23 +105,19 @@
                     {{ form.project }}
                     {{ form.project.errors }}
                     <br/><br/>
                     {{ form.task }}
                     {{ form.task.errors }}
                 </td>
                 <td>
-                    {{ form.date }}
-                    {{ form.date.errors }}
-                </td>
-                <td>
-                    {{ form.start_time }}
-                    {{ form.start_time.errors }}
-                    <br/><br/>
-                    {{ form.stop_time }}
-                    {{ form.stop_time.errors }}
+                    {{ form.datetime_start }}
+                    {{ form.datetime_start.errors }}
+                <br/>
+                    {{ form.datetime_stop }}
+                    {{ form.datetime_stop.errors }}
                 </td>
                 <td>
                     {{ form.worked_hours }}
                     {{ form.worked_hours.errors }}
                 </td>
                 <td>
                     {{ form.description }}
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/create_work_report.html` & `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/create_work_report.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/register_payment.html` & `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/register_payment.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/templates/crm/admin/exception.html` & `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/exception.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/logo.jpg` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/logo.jpg`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/fontconfig.xml` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/fontconfig.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/generic/dejavusans.xml` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/invoice.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/invoice.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/en/quote.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/quote.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/work_report.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/work_report.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/invoice.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/invoice.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/project_report.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/project_report.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/static/default_templates/de/quote.xsl` & `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/quote.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/task_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/generic_task_link.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_task_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/generic_project_link.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_project_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/work.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/work.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/estimation_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/agreement_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/project.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/agreement.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/reporting_period_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource_price.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/agreement_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/project_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/estimation.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/urls.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # DJANGO IMPORTS
 from django.urls import path
 
 from koalixcrm.crm.views.time_tracking import work_report
 from koalixcrm.crm.views.user_extension_missing import user_extension_missing
 from koalixcrm.crm.views.reporting_period_missing import reporting_period_missing
 from koalixcrm.crm.views.user_is_not_human_resource import user_is_not_human_resource
+from koalixcrm.crm.views.set_timezone import set_timezone
 
 urlpatterns = [
     path('time_tracking/', work_report, name="monthly_report"),
     path('user_extension_missing/', user_extension_missing, name="user_extension_missing"),
     path('reporting_period_missing/', reporting_period_missing, name="reporting_period_missing"),
     path('user_is_not_human_resource/', user_is_not_human_resource, name="user_is_not_human_resource"),
+    path('set_timezone/', set_timezone, name="set_timezone"),
 ]
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/task.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/resource_manager.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_manager.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/project_link_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/human_resource.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/task_link_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/reporting/reporting_period.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/exceptions.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/customer.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/customer_billing_cycle.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_billing_cycle.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/person.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/person.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/postal_address.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/postal_address.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/supplier.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/supplier.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/customer_group.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_group.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/contact.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/contact.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/contact/call.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/contact/call.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/tax.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/tax.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/currency_transform.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/currency_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/product_price.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/product_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/unit_transform.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/unit_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/product_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/product_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/unit.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/unit.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/customer_group_transform.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/customer_group_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/currency.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/currency.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/product/price.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/product/price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/admin.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_reporting_period_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_agreement_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_project.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_sales_document_position.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_currency.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_customer_group_transform.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_group_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_unit_transform.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_human_resource.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_sales_document.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_contract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 # -*- coding: utf-8 -*-
 
 import factory
-from koalixcrm.crm.models import SalesDocument
+from koalixcrm.crm.models import Contract
 from koalixcrm.crm.factories.factory_user import StaffUserFactory
-from koalixcrm.crm.factories.factory_contract import StandardContractFactory
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
-from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardQuoteTemplateFactory
+from koalixcrm.djangoUserExtension.factories.factory_template_set import StandardTemplateSetFactory
 
 
-class StandardSalesDocumentFactory(factory.django.DjangoModelFactory):
+class StandardContractFactory(factory.django.DjangoModelFactory):
     class Meta:
-        model = SalesDocument
+        model = Contract
 
-    contract = factory.SubFactory(StandardContractFactory)
-    external_reference = "This is an external Reference"
-    discount = "0"
-    description = "This is the description of a sales document"
-    last_pricing_date = "2018-05-01"
-    last_calculated_price = "220.00"
-    last_calculated_tax = "10.00"
-    customer = factory.SubFactory(StandardCustomerFactory)
     staff = factory.SubFactory(StaffUserFactory)
-    currency = factory.SubFactory(StandardCurrencyFactory)
+    description = "This is the description to a test contract"
+    default_customer = factory.SubFactory(StandardCustomerFactory)
+    default_currency = factory.SubFactory(StandardCurrencyFactory)
+    default_template_set = factory.SubFactory(StandardTemplateSetFactory)
     date_of_creation = "2018-05-01"
-    custom_date_field = "2018-05-20"
-    last_modification = "2018-05-25"
+    last_modification = "2018-05-03"
     last_modified_by = factory.SubFactory(StaffUserFactory)
-    template_set = factory.SubFactory(StandardQuoteTemplateFactory)
-    derived_from_sales_document = None
-    last_print_date = "2018-05-26"
-
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_customer.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_contract.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_work.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import factory
-from koalixcrm.crm.models import Contract
-from koalixcrm.crm.factories.factory_user import StaffUserFactory
-from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
-from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
-from koalixcrm.djangoUserExtension.factories.factory_template_set import StandardTemplateSetFactory
+import datetime
+from koalixcrm.crm.models import Work
+from koalixcrm.crm.factories.factory_task import StandardTaskFactory
+from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
+from koalixcrm.crm.factories.factory_human_resource import StandardUserExtensionFactory
+from koalixcrm.global_support_functions import make_date_utc
 
 
-class StandardContractFactory(factory.django.DjangoModelFactory):
+class StandardWorkFactory(factory.django.DjangoModelFactory):
     class Meta:
-        model = Contract
+        model = Work
 
-    staff = factory.SubFactory(StaffUserFactory)
-    description = "This is the description to a test contract"
-    default_customer = factory.SubFactory(StandardCustomerFactory)
-    default_currency = factory.SubFactory(StandardCurrencyFactory)
-    default_template_set = factory.SubFactory(StandardTemplateSetFactory)
-    date_of_creation = "2018-05-01"
-    last_modification = "2018-05-03"
-    last_modified_by = factory.SubFactory(StaffUserFactory)
+    human_resource = factory.SubFactory(StandardUserExtensionFactory)
+    date = make_date_utc(datetime.datetime(2018, 5, 1, 0, 00))
+    start_time = None
+    stop_time = None
+    worked_hours = "1.50"
+    short_description = "The employee did some work"
+    description = "And here he describes some more about his work"
+    task = factory.SubFactory(StandardTaskFactory)
+    reporting_period = factory.SubFactory(StandardReportingPeriodFactory)
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_generic_project_link.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_project_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_agreement.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from koalixcrm.crm.factories.factory_resource import StandardResourceFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_unit import StandardUnitFactory
 from koalixcrm.crm.factories.factory_resource_price import StandardResourcePriceFactory
 from koalixcrm.crm.factories.factory_agreement_type import StandardAgreementTypeFactory
 from koalixcrm.crm.factories.factory_agreement_status import AgreedAgreementStatusFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class StandardAgreementToTaskFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = Agreement
 
     date_from = make_date_utc(datetime.datetime(2018, 6, 15, 00))
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_currency_transform.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_project_link_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_task_link_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_resource.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_estimation.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 from koalixcrm.crm.models import Estimation
 from koalixcrm.crm.factories.factory_resource import StandardResourceFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_estimation_status import StartedEstimationStatusFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class StandardEstimationToTaskFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = Estimation
 
     amount = "112.50"
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_generic_task_link.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_task_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_resource_price.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import factory
 import datetime
 from koalixcrm.crm.models import ResourcePrice
 from koalixcrm.crm.factories.factory_resource import StandardResourceFactory
 from koalixcrm.crm.factories.factory_unit import StandardUnitFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class StandardResourcePriceFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = ResourcePrice
 
     resource = factory.SubFactory(StandardResourceFactory)
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_estimation_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_work.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import factory
 import datetime
-from koalixcrm.crm.models import Work
-from koalixcrm.crm.factories.factory_task import StandardTaskFactory
-from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
-from koalixcrm.crm.factories.factory_human_resource import StandardUserExtensionFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.crm.models import ProductType
+from koalixcrm.crm.factories.factory_unit import StandardUnitFactory
+from koalixcrm.crm.factories.factory_user import StaffUserFactory
+from koalixcrm.crm.factories.factory_tax import StandardTaxFactory
+from koalixcrm.global_support_functions import make_date_utc
 
 
-class StandardWorkFactory(factory.django.DjangoModelFactory):
+class StandardProductTypeFactory(factory.django.DjangoModelFactory):
     class Meta:
-        model = Work
+        model = ProductType
+        django_get_or_create = ('product_type_identifier',)
 
-    human_resource = factory.SubFactory(StandardUserExtensionFactory)
-    date = make_date_utc(datetime.datetime(2018, 5, 1, 0, 00))
-    start_time = None
-    stop_time = None
-    worked_hours = "1.50"
-    short_description = "The employee did some work"
-    description = "And here he describes some more about his work"
-    task = factory.SubFactory(StandardTaskFactory)
-    reporting_period = factory.SubFactory(StandardReportingPeriodFactory)
+    title = "This is a test Product"
+    description = "This is a test Product"
+    product_type_identifier = "123456"
+    default_unit = factory.SubFactory(StandardUnitFactory)
+    date_of_creation = make_date_utc(datetime.datetime(2018, 6, 15, 00))
+    last_modification = make_date_utc(datetime.datetime(2018, 6, 15, 00))
+    last_modified_by = factory.SubFactory(StaffUserFactory)
+    tax = factory.SubFactory(StandardTaxFactory)
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_task_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_task.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import factory
 import datetime
 from koalixcrm.crm.models import Task
 from koalixcrm.crm.factories.factory_project import StandardProjectFactory
 from koalixcrm.crm.factories.factory_task_status import StartedTaskStatusFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class StandardTaskFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = Task
 
     title = 'This is a test Task'
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_product_type.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 # -*- coding: utf-8 -*-
 
 import factory
 import datetime
-from koalixcrm.crm.models import ProductType
-from koalixcrm.crm.factories.factory_unit import StandardUnitFactory
+from koalixcrm.global_support_functions import make_date_utc
+from koalixcrm.crm.models import SalesDocument
 from koalixcrm.crm.factories.factory_user import StaffUserFactory
-from koalixcrm.crm.factories.factory_tax import StandardTaxFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.crm.factories.factory_contract import StandardContractFactory
+from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
+from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
+from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardQuoteTemplateFactory
 
 
-class StandardProductTypeFactory(factory.django.DjangoModelFactory):
+class StandardSalesDocumentFactory(factory.django.DjangoModelFactory):
     class Meta:
-        model = ProductType
-        django_get_or_create = ('product_type_identifier',)
+        model = SalesDocument
 
-    title = "This is a test Product"
-    description = "This is a test Product"
-    product_type_identifier = "123456"
-    default_unit = factory.SubFactory(StandardUnitFactory)
-    date_of_creation = make_date_utc(datetime.datetime(2018, 6, 15, 00))
-    last_modification = make_date_utc(datetime.datetime(2018, 6, 15, 00))
+    contract = factory.SubFactory(StandardContractFactory)
+    external_reference = "This is an external Reference"
+    discount = "0"
+    description = "This is the description of a sales document"
+    last_pricing_date = make_date_utc(datetime.datetime(2018, 5, 1, 00))
+    last_calculated_price = "220.00"
+    last_calculated_tax = "10.00"
+    customer = factory.SubFactory(StandardCustomerFactory)
+    staff = factory.SubFactory(StaffUserFactory)
+    currency = factory.SubFactory(StandardCurrencyFactory)
+    date_of_creation = make_date_utc(datetime.datetime(2018, 5, 1, 00))
+    custom_date_field = make_date_utc(datetime.datetime(2018, 5, 20, 00))
+    last_modification = make_date_utc(datetime.datetime(2018, 5, 25, 00))
     last_modified_by = factory.SubFactory(StaffUserFactory)
-    tax = factory.SubFactory(StandardTaxFactory)
+    template_set = factory.SubFactory(StandardQuoteTemplateFactory)
+    derived_from_sales_document = None
+    last_print_date = make_date_utc(datetime.datetime(2018, 5, 26, 00))
+
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_reporting_period.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_user.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_user.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_unit.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/factories/factory_product_price.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import factory
 import datetime
 from koalixcrm.crm.models import ProductPrice
 from koalixcrm.crm.factories.factory_product import StandardProductFactory
 from koalixcrm.crm.factories.factory_unit import StandardUnitFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class StandardPriceFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = ProductPrice
         django_get_or_create = ('product_type',
                                 'unit',
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/pdfexport.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/pdfexport.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/time_tracking.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/time_tracking.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/user_extension_missing.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/user_extension_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/work_entry_form.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_form.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 
-import datetime
 from django.forms import NumberInput
 from koalixcrm.crm.reporting.task import Task
 from koalixcrm.crm.reporting.project import Project
 from django.contrib.admin.widgets import *
 from koalixcrm.global_support_functions import limit_string_length
 from koalixcrm.djangoUserExtension.models import UserExtension
 from koalixcrm.crm.reporting.reporting_period import ReportingPeriod
@@ -16,20 +15,18 @@
     Form which allows to fill out a full Work. Instead of only showing the task, it is possible
     to select the task based on the input from the project
     """
     project = forms.ModelChoiceField(queryset=Project.objects.filter(reportingperiod__status__is_done=False).distinct(),
                                      required=True)
     task = forms.ModelChoiceField(queryset=Task.objects.filter(status__is_done=False),
                                   required=True)
-    date = forms.DateField(widget=AdminDateWidget,
-                           required=True)
-    start_time = forms.TimeField(widget=AdminTimeWidget,
-                                 required=False)
-    stop_time = forms.TimeField(widget=AdminTimeWidget,
-                                required=False)
+    datetime_start = forms.SplitDateTimeField(widget=AdminSplitDateTime,
+                                              required=True)
+    datetime_stop = forms.SplitDateTimeField(widget=AdminSplitDateTime,
+                                             required=False)
     worked_hours = forms.DecimalField(widget=NumberInput(attrs={'step': 0.1,
                                                                 'min': 0,
                                                                 'max': 24}),
                                       required=False)
     description = forms.CharField(widget=AdminTextareaWidget,
                                   required=True)
     work_id = forms.IntegerField(widget=forms.HiddenInput(),
@@ -52,18 +49,18 @@
           The django built in form validation must already have been passed
 
         Returns:
           True when no ValidationError was raised
 
         Raises:
           may raise ValidationError exception"""
-        if ("start_time" in cleaned_data) & ("stop_time" in cleaned_data) & ("worked_hours" in cleaned_data):
-            start_stop_pattern_complete = bool(cleaned_data["start_time"]) & bool(cleaned_data["stop_time"])
-            start_stop_pattern_stop_missing = bool(cleaned_data["start_time"]) & (not bool(cleaned_data["stop_time"]))
-            start_stop_pattern_start_missing = (not bool(cleaned_data["start_time"])) & bool(cleaned_data["stop_time"])
+        if ("datetime_start" in cleaned_data) & ("datetime_stop" in cleaned_data) & ("worked_hours" in cleaned_data):
+            start_stop_pattern_complete = bool(cleaned_data["datetime_start"]) & bool(cleaned_data["datetime_stop"])
+            start_stop_pattern_stop_missing = bool(cleaned_data["datetime_start"]) & (not bool(cleaned_data["datetime_stop"]))
+            start_stop_pattern_start_missing = (not bool(cleaned_data["datetime_start"])) & bool(cleaned_data["datetime_stop"])
             worked_hours_pattern = bool(cleaned_data["worked_hours"])
         else:
             raise forms.ValidationError('Programming error', code='invalid')
         if start_stop_pattern_complete & worked_hours_pattern:
             raise forms.ValidationError('Please either set the start, stop time or worked hours (not both)',
                                         code='invalid')
         elif start_stop_pattern_start_missing or start_stop_pattern_stop_missing:
@@ -100,20 +97,18 @@
                 else:
                     return
             if self.cleaned_data['DELETE']:
                 work.delete()
             else:
                 work.task = self.cleaned_data['task']
                 work.reporting_period = ReportingPeriod.get_reporting_period(project=self.cleaned_data['task'].project,
-                                                                             search_date=self.cleaned_data['date'])
+                                                                             search_date=self.cleaned_data['datetime_start'].date())
                 work.human_resource = HumanResource.objects.get(user=UserExtension.get_user_extension(request.user))
-                work.date = self.cleaned_data['date']
-                if bool(self.cleaned_data['start_time']) & bool(self.cleaned_data['stop_time']):
-                    work.start_time = datetime.datetime.combine(self.cleaned_data['date'],
-                                                                self.cleaned_data['start_time'])
-                    work.stop_time = datetime.datetime.combine(self.cleaned_data['date'],
-                                                               self.cleaned_data['stop_time'])
+                work.date = self.cleaned_data['datetime_start'].date()
+                if bool(self.cleaned_data['datetime_start']) & bool(self.cleaned_data['datetime_stop']):
+                    work.start_time = self.cleaned_data['datetime_start']
+                    work.stop_time = self.cleaned_data['datetime_stop']
                 else:
                     work.worked_hours = self.cleaned_data['worked_hours']
                 work.description = self.cleaned_data['description']
                 work.short_description = limit_string_length(work.description, 100)
                 work.save()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/create_work_report.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/create_work_report.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/template_set_missing.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/template_set_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/user_is_not_human_resource.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/user_is_not_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/create_task.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/create_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/reporting_period_missing.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/reporting_period_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/range_selection_form.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/range_selection_form.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/newdocument.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/newdocument.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/renderer.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/renderer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/views/work_entry_formset.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_formset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,16 @@
         from koalixcrm.crm.reporting.work import Work
         list_of_work = Work.objects.filter(human_resource=human_resource, date__lte=stop_date, date__gte=start_date).order_by("date")
         initial = []
         for work in list_of_work:
             initial.append({'work_id': work.id,
                             'task': work.task,
                             'project': work.task.project,
-                            'date': work.date,
-                            'start_time': work.start_time,
-                            'stop_time': work.stop_time,
+                            'datetime_start': work.start_time,
+                            'datetime_stop': work.stop_time,
                             'worked_hours': work.worked_hours,
                             'description': work.description})
         return initial
 
     @staticmethod
     def load_formset(range_selection_form, request):
         WorkEntryFormSet = forms.formset_factory(WorkEntry,
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/models.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/models.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_manager_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_manager_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/unit_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/unit_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_type_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_type_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/project_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/contact_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/contact_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/customer_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/agreement_status_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/work_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/work_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/estimation_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/tax_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/tax_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/customer_billing_cycle_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_billing_cycle_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/customer_group_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_group_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/task_status_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/project_status_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/product_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/product_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/restinterface.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/restinterface.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/task_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/agreement_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/agreement_type_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_type_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/estimation_status_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/human_resource_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/human_resource_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/resource_price_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_price_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/reporting_period_status_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/rest/reporting_period_rest.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0036_auto_20180626_2059.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0036_auto_20180626_2059.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0029_auto_20180611_1903.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0029_auto_20180611_1903.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0008_auto_20180104_2042.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0008_auto_20180104_2042.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0044_reportingperiod_status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0044_reportingperiod_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0039_auto_20180702_1635.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0039_auto_20180702_1635.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0047_work_worked_hours.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0047_work_worked_hours.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0015_auto_20180111_2043.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0015_auto_20180111_2043.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0025_auto_20180413_1937.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0025_auto_20180413_1937.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0048_auto_20181012_2056.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0048_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0001_initial.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0027_auto_20180606_2034.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0027_auto_20180606_2034.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0011_auto_20180104_2152.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0011_auto_20180104_2152.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0007_auto_20171210_2126.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0007_auto_20171210_2126.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0038_auto_20180702_1628.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0038_auto_20180702_1628.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0024_auto_20180122_2121.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0024_auto_20180122_2121.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0032_auto_20180612_1925.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0032_auto_20180612_1925.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0051_auto_20181014_2302.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0051_auto_20181014_2302.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0002_auto_20170927_2042.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0002_auto_20170927_2042.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0021_purchaseorder.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0021_purchaseorder.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0041_auto_20180724_1657.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0041_auto_20180724_1657.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0020_auto_20180116_2056.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0020_auto_20180116_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0018_auto_20180111_2031.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0018_auto_20180111_2031.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0017_auto_20180111_2022.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0017_auto_20180111_2022.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0056_auto_20181216_2224.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20181216_2224.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0028_auto_20180611_1835.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0028_auto_20180611_1835.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0022_auto_20180117_2020.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0022_auto_20180117_2020.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0005_auto_20171110_1732.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0005_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0012_auto_20180105_1840.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0012_auto_20180105_1840.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0052_auto_20181014_2304.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0052_auto_20181014_2304.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0006_auto_20171210_1805.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0006_auto_20171210_1805.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0004_auto_20171009_2008.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0004_auto_20171009_2008.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0050_auto_20181014_2300.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0050_auto_20181014_2300.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0016_auto_20180111_2011.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0016_auto_20180111_2011.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0045_auto_20180805_2047.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0045_auto_20180805_2047.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0035_auto_20180619_1924.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0035_auto_20180619_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0026_auto_20180507_1957.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0026_auto_20180507_1957.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0040_auto_20180724_1657.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0040_auto_20180724_1657.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0014_auto_20180108_2048.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0014_auto_20180108_2048.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0055_auto_20181022_1937.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0055_auto_20181022_1937.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0053_auto_20181014_2305.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0053_auto_20181014_2305.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0009_auto_20180104_2111.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0009_auto_20180104_2111.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0056_auto_20190102_2230.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20190102_2230.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0013_auto_20180105_2159.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0013_auto_20180105_2159.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0034_genericprojectlink.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0034_genericprojectlink.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0003_auto_20171009_1949.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0003_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0049_auto_20181014_2258.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0049_auto_20181014_2258.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0033_auto_20180612_1936.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0033_auto_20180612_1936.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0042_auto_20180724_1816.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0042_auto_20180724_1816.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0019_auto_20180112_2020.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0019_auto_20180112_2020.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0031_auto_20180612_1924.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0031_auto_20180612_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0030_auto_20180611_1930.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0030_auto_20180611_1930.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/migrations/0043_reportingperiodstatus.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0043_reportingperiodstatus.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_poject_admin_view.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_poject_admin_view.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_work_delete.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_work_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_work import StandardWorkFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_reporting_period_status import DoneReportingPeriodStatusFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 from koalixcrm.crm.exceptions import ReportingPeriodDoneDeleteNotPossible
 
 
 class TestWorkDelete(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_user_is_not_human_resource.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_user_is_not_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_planned_costs.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_view_work_entry_form.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_view_work_entry_form.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,29 +72,32 @@
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-0-project'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         # find the form element
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-project"]')
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-task"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-date"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-start_time"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-stop_time"]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_0]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_0"]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_1]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_1"]')
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-worked_hours"]')
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-description"]')
         assert_when_element_does_not_exist(self, 'save')
         project = selenium.find_element_by_xpath('//*[@id="id_form-0-project"]')
-        date = selenium.find_element_by_xpath('//*[@id="id_form-0-date"]')
-        start_time = selenium.find_element_by_xpath('//*[@id="id_form-0-start_time"]')
-        stop_time = selenium.find_element_by_xpath('//*[@id="id_form-0-stop_time"]')
+        datetime_start_date = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_start_0"]')
+        datetime_start_time = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_start_1"]')
+        datetime_stop_date = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_stop_0"]')
+        datetime_stop_time = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_stop_1"]')
         description = selenium.find_element_by_xpath('//*[@id="id_form-0-description"]')
         project.send_keys(self.test_reporting_period.project.id.__str__())
-        date.send_keys(datetime.date.today().__str__())
-        start_time.send_keys(datetime.time(11, 55).__str__())
-        stop_time.send_keys(datetime.time(12, 55).__str__())
+        datetime_start_date.send_keys(datetime.date.today().__str__())
+        datetime_stop_date.send_keys(datetime.date.today().__str__())
+        datetime_start_time.send_keys(datetime.time(11, 55).__str__())
+        datetime_stop_time.send_keys(datetime.time(12, 55).__str__())
         description.send_keys("This is a test work entered through the front-end")
         task = selenium.find_element_by_xpath('//*[@id="id_form-0-task"]/option[text()="'+self.test_1st_task.title+'"]')
         task.click()
         save_button = selenium.find_element_by_name('save')
         save_button.send_keys(Keys.RETURN)
         time.sleep(1)
         try:
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_update_last_status_update.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_update_last_status_update.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_supplier_admin_view.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_supplier_admin_view.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_sales_document_from_contract.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_contract.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_time_tracking_add_row.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_time_tracking_add_row.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_incomplete_sales_document_position.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_incomplete_sales_document_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from koalixcrm.crm.factories.factory_sales_document_position import StandardSalesDocumentPositionFactory
 from koalixcrm.crm.factories.factory_product_type import StandardProductTypeFactory
 from koalixcrm.crm.factories.factory_product_price import StandardPriceFactory
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory, AdvancedCustomerGroupFactory
 from koalixcrm.crm.factories.factory_tax import StandardTaxFactory
 from koalixcrm.crm.factories.factory_unit import StandardUnitFactory, SmallUnitFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 from koalixcrm.crm.models import SalesDocumentPosition
 
 
 class DocumentSalesDocumentPosition(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_effort.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_effort.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_work import StandardWorkFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class TaskEffectiveEffort(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
         end_date_first_task = (datetime_now + datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_calculations_document.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_calculations_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory, AdvancedCustomerGroupFactory
 from koalixcrm.crm.factories.factory_tax import StandardTaxFactory
 from koalixcrm.crm.factories.factory_unit import StandardUnitFactory, SmallUnitFactory
 from koalixcrm.crm.factories.factory_customer_group_transform import StandardCustomerGroupTransformFactory
 from koalixcrm.crm.factories.factory_unit_transform import StandardUnitTransformFactory
 from koalixcrm.crm.factories.factory_currency_transform import StandardCurrencyTransformFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class DocumentCalculationsTest(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
         end_date = (datetime_now + datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_project_planned_costs.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_planned_costs.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_estimation import StandardEstimationToTaskFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_resource_price import StandardResourcePriceFactory
 from koalixcrm.crm.factories.factory_project import StandardProjectFactory
 from koalixcrm.crm.factories.factory_unit import StandardUnitFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class TaskPlannedEffort(TestCase):
     def setUp(self):
-
         self.test_billing_cycle = StandardCustomerBillingCycleFactory.create()
         self.test_user = AdminUserFactory.create()
         self.test_customer_group = StandardCustomerGroupFactory.create()
         self.test_unit = StandardUnitFactory.create()
         self.test_customer = StandardCustomerFactory.create(is_member_of=(self.test_customer_group,))
         self.test_currency = StandardCurrencyFactory.create()
         self.test_user_extension = StandardUserExtensionFactory.create(user=self.test_user)
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_duration.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_duration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_work import StandardWorkFactory
 from koalixcrm.crm.factories.factory_task_status import DoneTaskStatusFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
 
 
 class TaskEffectiveDuration(TestCase):
 
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime.now())
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_task.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_sales_document_from_quote.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_quote.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_work import StandardWorkFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_resource_price import StandardResourcePriceFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
 from koalixcrm.crm.factories.factory_agreement import StandardAgreementToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class TaskEffectiveCostsWithAgreement(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
         end_date_first_task = (datetime_now + datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_delete_of_empty_row.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_delete_of_empty_row.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,17 +68,18 @@
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-0-project'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         # find the form element
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-project"]')
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-task"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-date"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-start_time"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-stop_time"]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_0]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_0"]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_1]')
+        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_1"]')
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-worked_hours"]')
         assert_when_element_does_not_exist(self, '//*[@id="id_form-0-description"]')
         assert_when_element_does_not_exist(self, 'save')
         # check existence of a second form before pressing add more
         assert_when_element_exists(self, '//*[@id="id_form-1-project"]')
         add_more_button = selenium.find_element_by_xpath('//*[@id="add_more"]')
         add_more_button.send_keys(Keys.RETURN)
@@ -89,22 +90,24 @@
         add_more_button.send_keys(Keys.RETURN)
         delete_form = selenium.find_element_by_id('id_form-1-DELETE')
         if not delete_form.is_selected():
             delete_form.send_keys(Keys.SPACE)
         # check existence of a second form after pressing add more
         assert_when_element_does_not_exist(self, '//*[@id="id_form-2-project"]')
         project = selenium.find_element_by_xpath('//*[@id="id_form-2-project"]')
-        date = selenium.find_element_by_xpath('//*[@id="id_form-2-date"]')
-        start_time = selenium.find_element_by_xpath('//*[@id="id_form-2-start_time"]')
-        stop_time = selenium.find_element_by_xpath('//*[@id="id_form-2-stop_time"]')
+        datetime_start_date = selenium.find_element_by_xpath('//*[@id="id_form-2-datetime_start_0"]')
+        datetime_start_time = selenium.find_element_by_xpath('//*[@id="id_form-2-datetime_start_1"]')
+        datetime_stop_date = selenium.find_element_by_xpath('//*[@id="id_form-2-datetime_stop_0"]')
+        datetime_stop_time = selenium.find_element_by_xpath('//*[@id="id_form-2-datetime_stop_1"]')
         description = selenium.find_element_by_xpath('//*[@id="id_form-2-description"]')
         project.send_keys(self.test_reporting_period.project.id.__str__())
-        date.send_keys(datetime.date.today().__str__())
-        start_time.send_keys(datetime.time(11, 55).__str__())
-        stop_time.send_keys(datetime.time(12, 55).__str__())
+        datetime_start_date.send_keys(datetime.date.today().__str__())
+        datetime_stop_date.send_keys(datetime.date.today().__str__())
+        datetime_start_time.send_keys(datetime.time(11, 55).__str__())
+        datetime_stop_time.send_keys(datetime.time(12, 55).__str__())
         description.send_keys("This is a test work entered through the front-end")
         task = selenium.find_element_by_xpath('//*[@id="id_form-2-task"]/option[text()="'+self.test_1st_task.title+'"]')
         task.click()
         save_button = selenium.find_element_by_name('save')
         save_button.send_keys(Keys.RETURN)
         time.sleep(1)
         try:
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_work import StandardWorkFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_resource_price import StandardResourcePriceFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class TaskEffectiveCostsWithoutAgreement(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
         end_date_first_task = (datetime_now + datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_project_effective_costs.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_effective_costs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.crm.factories.factory_work import StandardWorkFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_resource_price import StandardResourcePriceFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
 from koalixcrm.crm.factories.factory_agreement import StandardAgreementToTaskFactory
 from koalixcrm.crm.factories.factory_project import StandardProjectFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class TaskEffectiveCostsWithAgreement(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
         end_date_first_task = (datetime_now + datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_version_increase.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_version_increase.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_planned_effort.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_effort.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,18 @@
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.djangoUserExtension.factories.factory_user_extension import StandardUserExtensionFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_estimation import StandardEstimationToTaskFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
-from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
 
 
 class TaskPlannedEffort(TestCase):
     def setUp(self):
-        datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
-        start_date = (datetime_now - datetime.timedelta(days=30)).date()
-        end_date_first_task = (datetime_now + datetime.timedelta(days=30)).date()
-        end_date_second_task = (datetime_now + datetime.timedelta(days=60)).date()
-
         self.test_billing_cycle = StandardCustomerBillingCycleFactory.create()
         self.test_user = AdminUserFactory.create()
         self.test_customer_group = StandardCustomerGroupFactory.create()
         self.test_customer = StandardCustomerFactory.create(is_member_of=(self.test_customer_group,))
         self.test_currency = StandardCurrencyFactory.create()
         self.test_user_extension = StandardUserExtensionFactory.create(user=self.test_user)
         self.test_reporting_period = StandardReportingPeriodFactory.create()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_constructor.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_constructor.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/tests/test_task_planned_duration.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_duration.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.djangoUserExtension.factories.factory_user_extension import StandardUserExtensionFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.factories.factory_estimation import StandardHumanResourceEstimationToTaskFactory
-from koalixcrm.test_support_functions import make_date_utc
+from koalixcrm.global_support_functions import make_date_utc
 
 
 class TaskPlannedDuration(TestCase):
     def setUp(self):
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         start_date = (datetime_now - datetime.timedelta(days=30)).date()
         end_date_first_task = (datetime_now + datetime.timedelta(days=30)).date()
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/const/country.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/const/country.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/const/status.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/const/status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/const/purpose.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/const/purpose.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/inlinemixin.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/inlinemixin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/contract.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/contract.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/sales_document.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
 from django.contrib import admin, messages
 from django.utils.translation import ugettext as _
 from koalixcrm.crm.const.purpose import *
-from koalixcrm.global_support_functions import xstr
+from koalixcrm.global_support_functions import xstr, make_date_utc
 from koalixcrm.crm.contact.phone_address import PhoneAddress
 from koalixcrm.crm.contact.email_address import EmailAddress
 from koalixcrm.crm.contact.postal_address import PostalAddress
 from koalixcrm.crm.documents.sales_document_position import SalesDocumentPosition, SalesDocumentInlinePosition
 from koalixcrm.djangoUserExtension.models import TextParagraphInDocumentTemplate, UserExtension
 from koalixcrm.crm.product.product_type import ProductType
 from koalixcrm.crm.exceptions import TemplateSetMissingInContract
@@ -174,15 +174,15 @@
         if isinstance(calling_model, SalesDocument):
             sales_document_positions = SalesDocumentPosition.objects.filter(sales_document=calling_model.id)
             for sales_document_position in list(sales_document_positions):
                 new_position = SalesDocumentPosition()
                 new_position.create_position(sales_document_position, self)
 
     def create_pdf(self, template_set, printed_by):
-        self.last_print_date = datetime.now()
+        self.last_print_date = make_date_utc(datetime.now())
         self.save()
         return koalixcrm.crm.documents.pdf_export.PDFExport.create_pdf(self, template_set, printed_by)
 
     def get_template_set(self):
         if self.template_set:
             return self.template_set
         else:
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/payment_reminder.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/payment_reminder.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/purchase_confirmation.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_confirmation.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/calculations.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/calculations.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,21 +66,22 @@
             calculated price
             or raises exception
 
         Raises:
             Can trow Product.NoPriceFound when Product Price was overwritten but the price was not set
             Can trow Position.NoPriceFound when Position Price has no value but overwrite price is set """
 
-        if not position.position_price_per_unit:
-            raise SalesDocumentPosition.NoPriceFound
+
         if not position.overwrite_product_price:
             position.position_price_per_unit = position.product_type.get_price(pricing_date,
                                                                                position.unit,
                                                                                contact,
                                                                                currency)
+        elif position.position_price_per_unit is None:
+            raise SalesDocumentPosition.NoPriceFound
         nominal_total = position.position_price_per_unit * position.quantity
         if isinstance(position.discount, Decimal):
             nominal_minus_discount = nominal_total * (1 - position.discount / 100)
         else:
             nominal_minus_discount = nominal_total
         total_with_tax = Decimal(nominal_minus_discount)
         position.last_calculated_price = currency.round(total_with_tax)
```

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/invoice.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/invoice.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/quote.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/quote.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/pdf_export.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/pdf_export.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/purchase_order.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_order.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/sales_document_position.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/documents/delivery_note.py` & `koalix-crm-1.13.dev9/koalixcrm/crm/documents/delivery_note.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/README.md` & `koalix-crm-1.13.dev9/README.md`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/koalix_crm.egg-info/SOURCES.txt` & `koalix-crm-1.13.dev9/koalix_crm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,16 @@
 koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
 koalixcrm/crm/locale/de/LC_MESSAGES/django.po
 koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
 koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
 koalixcrm/crm/management/__init__.py
 koalixcrm/crm/management/commands/__init__.py
 koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
+koalixcrm/crm/middleware/__init__.py
+koalixcrm/crm/middleware/timezoneMiddleware.py
 koalixcrm/crm/migrations/0001_initial.py
 koalixcrm/crm/migrations/0002_auto_20170927_2042.py
 koalixcrm/crm/migrations/0003_auto_20171009_1949.py
 koalixcrm/crm/migrations/0004_auto_20171009_2008.py
 koalixcrm/crm/migrations/0005_auto_20171110_1732.py
 koalixcrm/crm/migrations/0006_auto_20171210_1805.py
 koalixcrm/crm/migrations/0007_auto_20171210_2126.py
@@ -279,14 +281,15 @@
 koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
 koalixcrm/crm/static/default_templates/generic/dejavusans.xml
 koalixcrm/crm/static/default_templates/generic/fontconfig.xml
 koalixcrm/crm/static/default_templates/generic/logo.jpg
 koalixcrm/crm/templates/crm/admin/create_work_report.html
 koalixcrm/crm/templates/crm/admin/exception.html
 koalixcrm/crm/templates/crm/admin/register_payment.html
+koalixcrm/crm/templates/crm/admin/set_timezone.html
 koalixcrm/crm/templates/crm/admin/time_reporting.html
 koalixcrm/crm/tests/__init__.py
 koalixcrm/crm/tests/test_calculations_document.py
 koalixcrm/crm/tests/test_create_sales_document_from_contract.py
 koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
 koalixcrm/crm/tests/test_create_sales_document_from_quote.py
 koalixcrm/crm/tests/test_create_task.py
@@ -314,14 +317,15 @@
 koalixcrm/crm/views/create_task.py
 koalixcrm/crm/views/create_work_report.py
 koalixcrm/crm/views/newdocument.py
 koalixcrm/crm/views/pdfexport.py
 koalixcrm/crm/views/range_selection_form.py
 koalixcrm/crm/views/renderer.py
 koalixcrm/crm/views/reporting_period_missing.py
+koalixcrm/crm/views/set_timezone.py
 koalixcrm/crm/views/template_set_missing.py
 koalixcrm/crm/views/time_tracking.py
 koalixcrm/crm/views/user_extension_missing.py
 koalixcrm/crm/views/user_is_not_human_resource.py
 koalixcrm/crm/views/work_entry_form.py
 koalixcrm/crm/views/work_entry_formset.py
 koalixcrm/djangoUserExtension/__init__.py
```

### Comparing `koalix-crm-1.13.dev6/projectsettings/settings/base_settings.py` & `koalix-crm-1.13.dev9/projectsettings/settings/base_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    'koalixcrm.crm.middleware.timezoneMiddleware.TimezoneMiddleware',
 ]
 
 ROOT_URLCONF = 'projectsettings.urls'
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
```

### Comparing `koalix-crm-1.13.dev6/projectsettings/settings/heroku_settings.py` & `koalix-crm-1.13.dev9/projectsettings/settings/heroku_settings.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/projectsettings/settings/docker_production_settings.py` & `koalix-crm-1.13.dev9/projectsettings/settings/docker_production_settings.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev6/setup.py` & `koalix-crm-1.13.dev9/setup.py`

 * *Files identical despite different names*

