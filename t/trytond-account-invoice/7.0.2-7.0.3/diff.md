# Comparing `tmp/trytond_account_invoice-7.0.2.tar.gz` & `tmp/trytond_account_invoice-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice-7.0.2.tar", last modified: Thu Feb 15 18:39:50 2024, max compression
+gzip compressed data, was "trytond_account_invoice-7.0.3.tar", last modified: Thu Apr  4 07:51:26 2024, max compression
```

## Comparing `trytond_account_invoice-7.0.2.tar` & `trytond_account_invoice-7.0.3.tar`

### file list

```diff
@@ -1,141 +1,140 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.268972 trytond_account_invoice-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     8119 2024-02-15 18:39:47.000000 trytond_account_invoice-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-02-15 18:39:47.000000 trytond_account_invoice-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3045 2024-02-15 18:39:50.268972 trytond_account_invoice-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1977 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14844 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4994 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.255638 trytond_account_invoice-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.258972 trytond_account_invoice-7.0.2/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/doc/usage/amend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/doc/usage/prepare.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3685 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.258972 trytond_account_invoice-7.0.2/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/icons/tryton-invoice.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    93989 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/invoice.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)   135485 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24229 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.258972 trytond_account_invoice-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37836 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38969 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32667 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39531 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38699 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33590 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36710 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40759 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32628 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39437 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35285 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35155 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35914 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38488 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36664 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38646 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33293 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36237 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37024 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38499 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37347 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32610 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31192 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37385 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6174 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3274 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2389 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-02-12 10:16:44.000000 trytond_account_invoice-7.0.2/payment_term.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/payment_term.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-15 18:39:50.268972 trytond_account_invoice-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4644 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.262305 trytond_account_invoice-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3188 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_cancelling_invoice_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4029 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_credit_note.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    13194 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5700 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2856 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_alternate_currency_lower_rate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3472 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_alternate_currency_rate_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_alternative_payee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_customer_sequential.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_group_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1868 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2606 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_manual_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3521 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_overpayment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2506 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_report_revision.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_reschedule_lines.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3480 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_supplier_post_paid.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3585 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_tax_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3408 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_invoice_with_credit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.265638 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3045 2024-02-15 18:39:49.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-02-15 18:39:50.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-15 18:39:49.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-02-15 18:39:49.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:33.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-02-15 18:39:49.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-15 18:39:49.000000 trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:39:50.265638 trytond_account_invoice-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4672 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_report_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_report_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_sequence_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_tax_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_tax_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/invoice_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/move_line_list_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/pay_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_method_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/view/payment_term_line_relativedelta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/view/payment_term_line_relativedelta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.2/view/payment_term_line_relativedelta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.2/view/payment_term_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.297054 trytond_account_invoice-7.0.3/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8220 2024-04-04 07:51:23.000000 trytond_account_invoice-7.0.3/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-04 07:51:23.000000 trytond_account_invoice-7.0.3/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-04 07:51:26.297054 trytond_account_invoice-7.0.3/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1977 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14844 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4994 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.287054 trytond_account_invoice-7.0.3/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-03-03 16:24:20.000000 trytond_account_invoice-7.0.3/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.287054 trytond_account_invoice-7.0.3/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/doc/usage/amend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/doc/usage/prepare.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3685 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.290388 trytond_account_invoice-7.0.3/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/icons/tryton-invoice.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    93989 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/invoice.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)   135623 2024-03-25 21:52:17.000000 trytond_account_invoice-7.0.3/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24229 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.290388 trytond_account_invoice-7.0.3/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37836 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38969 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32667 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39531 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38699 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33590 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36710 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40759 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32628 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39437 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35285 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35155 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35914 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38488 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36664 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38646 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33293 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36237 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37024 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38499 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37347 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32610 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31192 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37385 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6174 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3274 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2389 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-02-12 10:16:44.000000 trytond_account_invoice-7.0.3/payment_term.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/payment_term.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:51:26.297054 trytond_account_invoice-7.0.3/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-03-03 16:24:03.000000 trytond_account_invoice-7.0.3/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.293721 trytond_account_invoice-7.0.3/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3188 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_cancelling_invoice_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4029 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_credit_note.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    13194 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5700 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2856 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_alternate_currency_lower_rate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3472 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_alternate_currency_rate_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_alternative_payee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_customer_sequential.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_group_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1868 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2606 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_manual_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3521 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_overpayment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2506 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_report_revision.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_reschedule_lines.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3480 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_supplier_post_paid.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3585 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_tax_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3408 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_invoice_with_credit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-02-15 18:39:58.000000 trytond_account_invoice-7.0.3/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.297054 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-04 07:51:25.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     6188 2024-04-04 07:51:26.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:51:25.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-04 07:51:25.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:33.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-04 07:51:25.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:51:25.000000 trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:51:26.297054 trytond_account_invoice-7.0.3/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4672 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_report_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_report_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_sequence_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_tax_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_tax_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/invoice_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/move_line_list_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/pay_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_method_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/view/payment_term_line_relativedelta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/view/payment_term_line_relativedelta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.3/view/payment_term_line_relativedelta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.3/view/payment_term_tree.xml
```

### Comparing `trytond_account_invoice-7.0.2/CHANGELOG` & `trytond_account_invoice-7.0.3/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.3 - 2024-04-04
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.2 - 2024-02-15
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.1 - 2024-01-15
 --------------------------
```

### Comparing `trytond_account_invoice-7.0.2/COPYRIGHT` & `trytond_account_invoice-7.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/LICENSE` & `trytond_account_invoice-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/PKG-INFO` & `trytond_account_invoice-7.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice/
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account_invoice-7.0.2/__init__.py` & `trytond_account_invoice-7.0.3/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/account.py` & `trytond_account_invoice-7.0.3/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/account.xml` & `trytond_account_invoice-7.0.3/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/company.py` & `trytond_account_invoice-7.0.3/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/doc/conf.py` & `trytond_account_invoice-7.0.3/doc/conf.py`

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

### Comparing `trytond_account_invoice-7.0.2/doc/configuration.rst` & `trytond_account_invoice-7.0.3/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/doc/design.rst` & `trytond_account_invoice-7.0.3/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/doc/usage/amend.rst` & `trytond_account_invoice-7.0.3/doc/usage/amend.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/doc/usage/prepare.rst` & `trytond_account_invoice-7.0.3/doc/usage/prepare.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/doc/usage/process.rst` & `trytond_account_invoice-7.0.3/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/exceptions.py` & `trytond_account_invoice-7.0.3/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/icons/LICENSE` & `trytond_account_invoice-7.0.3/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/invoice.fodt` & `trytond_account_invoice-7.0.3/invoice.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/invoice.py` & `trytond_account_invoice-7.0.3/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2366,16 +2366,20 @@
         pool = Pool()
         Invoice = pool.get('account.invoice')
         return Invoice.fields_get(['state'])['state']['selection']
 
     @fields.depends('invoice', '_parent_invoice.state')
     def on_change_with_invoice_state(self, name=None):
         if self.invoice:
-            return self.invoice.state
-        return 'draft'
+            state = self.invoice.state
+            if state == 'cancelled' and self.invoice.cancel_move:
+                state = 'paid'
+        else:
+            state = 'draft'
+        return state
 
     @fields.depends('invoice', '_parent_invoice.party', 'party')
     def on_change_with_party_lang(self, name=None):
         Config = Pool().get('ir.configuration')
         if self.invoice and self.invoice.party:
             party = self.invoice.party
         else:
```

### Comparing `trytond_account_invoice-7.0.2/invoice.xml` & `trytond_account_invoice-7.0.3/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/bg.po` & `trytond_account_invoice-7.0.3/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/ca.po` & `trytond_account_invoice-7.0.3/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/cs.po` & `trytond_account_invoice-7.0.3/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/de.po` & `trytond_account_invoice-7.0.3/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/es.po` & `trytond_account_invoice-7.0.3/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/es_419.po` & `trytond_account_invoice-7.0.3/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/et.po` & `trytond_account_invoice-7.0.3/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/fa.po` & `trytond_account_invoice-7.0.3/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/fi.po` & `trytond_account_invoice-7.0.3/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/fr.po` & `trytond_account_invoice-7.0.3/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/hu.po` & `trytond_account_invoice-7.0.3/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/id.po` & `trytond_account_invoice-7.0.3/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/it.po` & `trytond_account_invoice-7.0.3/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/lo.po` & `trytond_account_invoice-7.0.3/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/lt.po` & `trytond_account_invoice-7.0.3/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/nl.po` & `trytond_account_invoice-7.0.3/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/pl.po` & `trytond_account_invoice-7.0.3/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/pt.po` & `trytond_account_invoice-7.0.3/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/ro.po` & `trytond_account_invoice-7.0.3/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/ru.po` & `trytond_account_invoice-7.0.3/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/sl.po` & `trytond_account_invoice-7.0.3/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/tr.po` & `trytond_account_invoice-7.0.3/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/uk.po` & `trytond_account_invoice-7.0.3/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/locale/zh_CN.po` & `trytond_account_invoice-7.0.3/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/message.xml` & `trytond_account_invoice-7.0.3/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/party.py` & `trytond_account_invoice-7.0.3/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/party.xml` & `trytond_account_invoice-7.0.3/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/payment_term.py` & `trytond_account_invoice-7.0.3/payment_term.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/payment_term.xml` & `trytond_account_invoice-7.0.3/payment_term.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/setup.py` & `trytond_account_invoice-7.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
-        'https://docs.tryton.org/projects/modules-account-invoice/',
+        'https://docs.tryton.org/modules-account-invoice/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice',
     package_dir={'trytond.modules.account_invoice': '.'},
     packages=(
         ['trytond.modules.account_invoice']
```

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_cancelling_invoice_move.rst` & `trytond_account_invoice-7.0.3/tests/scenario_cancelling_invoice_move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_credit_note.rst` & `trytond_account_invoice-7.0.3/tests/scenario_credit_note.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_alternate_currency.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_alternate_currency_lower_rate.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_alternate_currency_lower_rate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_alternate_currency_rate_change.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_alternate_currency_rate_change.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_alternative_payee.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_alternative_payee.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_customer_sequential.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_customer_sequential.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_group_line.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_group_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_in_future.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_in_future.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_manual_tax.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_manual_tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_overpayment.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_overpayment.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_report_revision.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_report_revision.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_reschedule_lines.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_reschedule_lines.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_supplier.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_supplier.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_supplier_post_paid.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_supplier_post_paid.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_tax_deductible.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_tax_deductible.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_invoice_with_credit.rst` & `trytond_account_invoice-7.0.3/tests/scenario_invoice_with_credit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/scenario_renew_fiscalyear.rst` & `trytond_account_invoice-7.0.3/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/test_module.py` & `trytond_account_invoice-7.0.3/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tests/tools.py` & `trytond_account_invoice-7.0.3/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/tox.ini` & `trytond_account_invoice-7.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/PKG-INFO` & `trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice/
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account_invoice-7.0.2/trytond_account_invoice.egg-info/SOURCES.txt` & `trytond_account_invoice-7.0.3/trytond_account_invoice.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_account_invoice-7.0.2/view/credit_start_form.xml` & `trytond_account_invoice-7.0.3/view/credit_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_form.xml` & `trytond_account_invoice-7.0.3/view/invoice_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_line_form.xml` & `trytond_account_invoice-7.0.3/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_line_tree.xml` & `trytond_account_invoice-7.0.3/view/invoice_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_line_tree_sequence.xml` & `trytond_account_invoice-7.0.3/view/invoice_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_sequence_form.xml` & `trytond_account_invoice-7.0.3/view/invoice_sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_tax_form.xml` & `trytond_account_invoice-7.0.3/view/invoice_tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_tax_tree_sequence.xml` & `trytond_account_invoice-7.0.3/view/invoice_tax_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/invoice_tree.xml` & `trytond_account_invoice-7.0.3/view/invoice_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/move_line_list_payment.xml` & `trytond_account_invoice-7.0.3/view/move_line_list_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/party_form.xml` & `trytond_account_invoice-7.0.3/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/pay_ask_form.xml` & `trytond_account_invoice-7.0.3/view/pay_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/pay_start_form.xml` & `trytond_account_invoice-7.0.3/view/pay_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/payment_method_form.xml` & `trytond_account_invoice-7.0.3/view/payment_method_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/payment_term_form.xml` & `trytond_account_invoice-7.0.3/view/payment_term_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/payment_term_line_form.xml` & `trytond_account_invoice-7.0.3/view/payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.2/view/payment_term_line_relativedelta_form.xml` & `trytond_account_invoice-7.0.3/view/payment_term_line_relativedelta_form.xml`

 * *Files identical despite different names*

