# Comparing `tmp/trytond_account_es-7.0.0.tar.gz` & `tmp/trytond_account_es-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es-7.0.0.tar", last modified: Mon Oct 30 17:19:54 2023, max compression
+gzip compressed data, was "trytond_account_es-7.0.1.tar", last modified: Thu Apr  4 07:52:47 2024, max compression
```

## Comparing `trytond_account_es-7.0.0.tar` & `trytond_account_es-7.0.1.tar`

### file list

```diff
@@ -1,105 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:54.005922 trytond_account_es-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-22 17:22:50.000000 trytond_account_es-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2157 2023-10-30 17:01:32.000000 trytond_account_es-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-10-30 17:01:32.000000 trytond_account_es-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3106 2023-10-30 17:19:54.005922 trytond_account_es-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)   454723 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   417678 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/account_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1356 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/account_payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:14.000000 trytond_account_es-7.0.0/account_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   311313 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/account_pyme.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1186 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/aeat111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/aeat115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/aeat303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1087 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/aeat347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/aeat349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/create_chart.xsl
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:54.005922 trytond_account_es-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-22 17:22:50.000000 trytond_account_es-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:50.000000 trytond_account_es-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_es-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:53.999256 trytond_account_es-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10593 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10727 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10656 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10242 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9321 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10537 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9119 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9682 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10407 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9020 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-28 12:11:19.000000 trytond_account_es-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36721 2023-08-13 15:26:13.000000 trytond_account_es-7.0.0/reporting_tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12080 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/reporting_tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:19:54.005922 trytond_account_es-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3912 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   151042 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tax_groups.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   158875 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/tax_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   156637 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/tax_pyme.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:54.002589 trytond_account_es-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/tests/111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/tests/115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/303_compensate.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4589 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/scenario_ec_operation_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8625 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/tests/scenario_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4268 2023-06-10 11:39:56.000000 trytond_account_es-7.0.0/tests/scenario_reporting_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5349 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/scenario_reporting_cancelled_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4400 2023-06-10 11:39:56.000000 trytond_account_es-7.0.0/tests/scenario_reporting_compensate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4672 2023-06-10 11:39:56.000000 trytond_account_es-7.0.0/tests/scenario_reporting_surcharge_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/tests/vat_book.csv
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_es-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-10-30 17:01:29.000000 trytond_account_es-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:54.005922 trytond_account_es-7.0.0/trytond_account_es.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3106 2023-10-30 17:19:53.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3448 2023-10-30 17:19:53.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:19:53.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-10-30 17:19:53.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:19:53.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:19:53.000000 trytond_account_es-7.0.0/trytond_account_es.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:54.002589 trytond_account_es-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/es_ec_operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/es_ec_operation_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-01-16 14:00:20.000000 trytond_account_es-7.0.0/view/print_aeat_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/vat_book_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/vat_book_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/vat_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view/vat_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_account_es-7.0.0/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.274936 trytond_account_es-7.0.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2258 2024-04-04 07:52:44.000000 trytond_account_es-7.0.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2024-04-04 07:52:44.000000 trytond_account_es-7.0.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-04 07:52:47.271603 trytond_account_es-7.0.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   454723 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   417678 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1356 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   311313 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_pyme.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1186 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1087 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-03-25 21:39:48.000000 trytond_account_es-7.0.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/create_chart.xsl
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.264937 trytond_account_es-7.0.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2789 2024-03-03 16:24:20.000000 trytond_account_es-7.0.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.268270 trytond_account_es-7.0.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10593 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10727 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10656 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10242 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9321 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10537 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9119 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9682 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10407 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9020 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36721 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/reporting_tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12080 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/reporting_tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:52:47.274936 trytond_account_es-7.0.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3912 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   151042 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax_groups.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   158875 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   156637 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax_pyme.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.268270 trytond_account_es-7.0.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/303_compensate.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4589 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_ec_operation_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8625 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5349 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_cancelled_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4400 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_compensate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4672 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_surcharge_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/vat_book.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.271603 trytond_account_es-7.0.1/trytond_account_es.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3430 2024-04-04 07:52:47.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:32.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.271603 trytond_account_es-7.0.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/es_ec_operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/es_ec_operation_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/print_aeat_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_book_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_book_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view.xml
```

### Comparing `trytond_account_es-7.0.0/CHANGELOG` & `trytond_account_es-7.0.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.1 - 2024-04-04
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_account_es-7.0.0/COPYRIGHT` & `trytond_account_es-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/LICENSE` & `trytond_account_es-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/PKG-INFO` & `trytond_account_es-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_es
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton with Spanish chart of accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_es-7.0.0/README.rst` & `trytond_account_es-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/__init__.py` & `trytond_account_es-7.0.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/account.py` & `trytond_account_es-7.0.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/account.xml` & `trytond_account_es-7.0.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/account_normal.xml` & `trytond_account_es-7.0.1/account_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/account_payment.py` & `trytond_account_es-7.0.1/account_payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/account_payment.xml` & `trytond_account_es-7.0.1/account_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/account_pyme.xml` & `trytond_account_es-7.0.1/account_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/aeat111.txt` & `trytond_account_es-7.0.1/aeat111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/aeat303.txt` & `trytond_account_es-7.0.1/aeat303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/aeat347.txt` & `trytond_account_es-7.0.1/aeat347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/aeat349.txt` & `trytond_account_es-7.0.1/aeat349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/company.py` & `trytond_account_es-7.0.1/company.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,11 +15,11 @@
         for contact_mechanism in self.party.contact_mechanisms:
             if contact_mechanism.type in {'phone', 'mobile'}:
                 try:
                     phonenumber = phonenumbers.parse(
                         contact_mechanism.value, None)
                 except NumberParseException:
                     continue
-                if phonenumber and phonenumber.country_code == '34':
+                if phonenumber and phonenumber.country_code == 34:
                     phone = contact_mechanism.value
                     break
         return phone
```

### Comparing `trytond_account_es-7.0.0/create_chart.xsl` & `trytond_account_es-7.0.1/create_chart.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/doc/conf.py` & `trytond_account_es-7.0.1/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
```

### Comparing `trytond_account_es-7.0.0/doc/index.rst` & `trytond_account_es-7.0.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/bg.po` & `trytond_account_es-7.0.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/ca.po` & `trytond_account_es-7.0.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/cs.po` & `trytond_account_es-7.0.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/de.po` & `trytond_account_es-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/es.po` & `trytond_account_es-7.0.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/es_419.po` & `trytond_account_es-7.0.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/et.po` & `trytond_account_es-7.0.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/fa.po` & `trytond_account_es-7.0.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/fi.po` & `trytond_account_es-7.0.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/fr.po` & `trytond_account_es-7.0.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/hu.po` & `trytond_account_es-7.0.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/id.po` & `trytond_account_es-7.0.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/it.po` & `trytond_account_es-7.0.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/lo.po` & `trytond_account_es-7.0.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/lt.po` & `trytond_account_es-7.0.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/nl.po` & `trytond_account_es-7.0.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/pl.po` & `trytond_account_es-7.0.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/pt.po` & `trytond_account_es-7.0.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/ro.po` & `trytond_account_es-7.0.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/ru.po` & `trytond_account_es-7.0.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/sl.po` & `trytond_account_es-7.0.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/tr.po` & `trytond_account_es-7.0.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/uk.po` & `trytond_account_es-7.0.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/locale/zh_CN.po` & `trytond_account_es-7.0.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/party.py` & `trytond_account_es-7.0.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/reporting_tax.py` & `trytond_account_es-7.0.1/reporting_tax.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/reporting_tax.xml` & `trytond_account_es-7.0.1/reporting_tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/setup.py` & `trytond_account_es-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tax.xml` & `trytond_account_es-7.0.1/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tax_groups.xml` & `trytond_account_es-7.0.1/tax_groups.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tax_normal.xml` & `trytond_account_es-7.0.1/tax_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tax_pyme.xml` & `trytond_account_es-7.0.1/tax_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/111.txt` & `trytond_account_es-7.0.1/tests/111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/115.txt` & `trytond_account_es-7.0.1/tests/115.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/303.txt` & `trytond_account_es-7.0.1/tests/303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/303_compensate.txt` & `trytond_account_es-7.0.1/tests/303_compensate.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/347.txt` & `trytond_account_es-7.0.1/tests/347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/349.txt` & `trytond_account_es-7.0.1/tests/349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/scenario_ec_operation_list.rst` & `trytond_account_es-7.0.1/tests/scenario_ec_operation_list.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/scenario_reporting.rst` & `trytond_account_es-7.0.1/tests/scenario_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/scenario_reporting_alternate_currency.rst` & `trytond_account_es-7.0.1/tests/scenario_reporting_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/scenario_reporting_cancelled_invoices.rst` & `trytond_account_es-7.0.1/tests/scenario_reporting_cancelled_invoices.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/scenario_reporting_compensate.rst` & `trytond_account_es-7.0.1/tests/scenario_reporting_compensate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tests/scenario_reporting_surcharge_tax.rst` & `trytond_account_es-7.0.1/tests/scenario_reporting_surcharge_tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/tox.ini` & `trytond_account_es-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/trytond_account_es.egg-info/PKG-INFO` & `trytond_account_es-7.0.1/trytond_account_es.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trytond-account-es
-Version: 7.0.0
+Name: trytond_account_es
+Version: 7.0.1
 Summary: Tryton with Spanish chart of accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_es-7.0.0/trytond_account_es.egg-info/SOURCES.txt` & `trytond_account_es-7.0.1/trytond_account_es.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 account.py
```

### Comparing `trytond_account_es-7.0.0/view/tax_form.xml` & `trytond_account_es-7.0.1/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/view/tax_template_form.xml` & `trytond_account_es-7.0.1/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/view/vat_book_list.xml` & `trytond_account_es-7.0.1/view/vat_book_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/view/vat_list_list.xml` & `trytond_account_es-7.0.1/view/vat_list_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.0/view.xml` & `trytond_account_es-7.0.1/view.xml`

 * *Files identical despite different names*

