# Comparing `tmp/trytond_account-7.0.4.tar.gz` & `tmp/trytond_account-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account-7.0.4.tar", last modified: Sun Mar  3 12:27:00 2024, max compression
+gzip compressed data, was "trytond_account-7.0.5.tar", last modified: Thu Apr  4 07:53:36 2024, max compression
```

## Comparing `trytond_account-7.0.4.tar` & `trytond_account-7.0.5.tar`

### file list

```diff
@@ -1,259 +1,258 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.628730 trytond_account-7.0.4/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-30 17:06:37.000000 trytond_account-7.0.4/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)    10892 2024-03-03 12:26:57.000000 trytond_account-7.0.4/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-03-03 12:26:57.000000 trytond_account-7.0.4/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:37.000000 trytond_account-7.0.4/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:37.000000 trytond_account-7.0.4/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2855 2024-03-03 12:27:00.628730 trytond_account-7.0.4/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.4/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-10-30 17:06:37.000000 trytond_account-7.0.4/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)   126779 2024-02-05 16:24:27.000000 trytond_account-7.0.4/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47195 2023-10-30 17:06:37.000000 trytond_account-7.0.4/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-10-30 17:06:38.000000 trytond_account-7.0.4/aged_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-10-30 17:06:38.000000 trytond_account-7.0.4/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6045 2023-10-30 17:06:37.000000 trytond_account-7.0.4/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2023-10-30 17:06:37.000000 trytond_account-7.0.4/company.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8831 2023-10-30 17:06:37.000000 trytond_account-7.0.4/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-10-30 17:06:37.000000 trytond_account-7.0.4/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.602064 trytond_account-7.0.4/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-10-30 17:06:37.000000 trytond_account-7.0.4/doc/configuration.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.605397 trytond_account-7.0.4/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/fiscal-year.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/journal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/design/template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.4/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-10-30 17:06:38.000000 trytond_account-7.0.4/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:37.000000 trytond_account-7.0.4/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:37.000000 trytond_account-7.0.4/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-10-30 17:06:38.000000 trytond_account-7.0.4/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.608730 trytond_account-7.0.4/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/close.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/create.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/structure.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-02-05 16:24:27.000000 trytond_account-7.0.4/doc/usage/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1764 2024-02-05 16:24:27.000000 trytond_account-7.0.4/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26145 2024-02-05 16:24:27.000000 trytond_account-7.0.4/fiscalyear.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-10-30 17:06:37.000000 trytond_account-7.0.4/fiscalyear.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-10-30 17:06:38.000000 trytond_account-7.0.4/general_journal.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81559 2023-10-30 17:06:38.000000 trytond_account-7.0.4/general_ledger.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.608730 trytond_account-7.0.4/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account-7.0.4/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:37.000000 trytond_account-7.0.4/icons/tryton-account-block.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:06:37.000000 trytond_account-7.0.4/icons/tryton-account-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_account-7.0.4/icons/tryton-account-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-10-30 17:06:37.000000 trytond_account-7.0.4/icons/tryton-account.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13034 2024-02-29 11:37:15.000000 trytond_account-7.0.4/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11585 2023-10-30 17:06:38.000000 trytond_account-7.0.4/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.612064 trytond_account-7.0.4/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   131031 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130273 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)   114028 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   133893 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130589 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118850 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)   126934 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   138509 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)   117820 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132568 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125409 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)   116858 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122752 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)   143136 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)   134636 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130971 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122026 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125322 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   128774 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132947 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122943 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   113860 2023-10-30 17:06:37.000000 trytond_account-7.0.4/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   147904 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125886 2023-10-30 17:06:38.000000 trytond_account-7.0.4/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-10-30 17:06:38.000000 trytond_account-7.0.4/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)    17440 2024-02-05 16:24:27.000000 trytond_account-7.0.4/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22110 2023-10-30 17:06:37.000000 trytond_account-7.0.4/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11303 2023-10-30 17:06:37.000000 trytond_account-7.0.4/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-10-30 17:06:38.000000 trytond_account-7.0.4/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11058 2023-10-30 17:06:37.000000 trytond_account-7.0.4/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11004 2023-10-30 17:06:38.000000 trytond_account-7.0.4/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11069 2023-10-30 17:06:38.000000 trytond_account-7.0.4/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11050 2023-10-30 17:06:38.000000 trytond_account-7.0.4/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11083 2023-10-30 17:06:38.000000 trytond_account-7.0.4/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11090 2023-10-30 17:06:37.000000 trytond_account-7.0.4/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11405 2023-10-30 17:06:37.000000 trytond_account-7.0.4/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11056 2023-10-30 17:06:38.000000 trytond_account-7.0.4/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   116245 2024-02-05 16:24:27.000000 trytond_account-7.0.4/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27018 2023-10-30 17:06:38.000000 trytond_account-7.0.4/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15750 2023-10-30 17:06:38.000000 trytond_account-7.0.4/move_template.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6825 2023-10-30 17:06:38.000000 trytond_account-7.0.4/move_template.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13724 2023-10-30 17:06:38.000000 trytond_account-7.0.4/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-10-30 17:06:37.000000 trytond_account-7.0.4/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16034 2024-02-05 16:24:27.000000 trytond_account-7.0.4/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4175 2023-10-30 17:06:38.000000 trytond_account-7.0.4/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:27:00.628730 trytond_account-7.0.4/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4595 2023-10-30 17:06:38.000000 trytond_account-7.0.4/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    70835 2024-01-08 10:53:54.000000 trytond_account-7.0.4/tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.615397 trytond_account-7.0.4/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4654 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_account_active.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:06:37.000000 trytond_account-7.0.4/tests/scenario_account_reconcile.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3992 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_account_reconcile.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_account_reconcile_automatic.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6220 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_account_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tests/scenario_account_reconciliation_alternate_currency.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3640 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_account_reconciliation_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tests/scenario_account_reconciliation_alternate_currency_write_off.json
--rw-r--r--   0 ced       (1000) ced       (1000)     4369 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4816 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_close_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4337 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_move_cancel.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_move_line_delegate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5034 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_move_line_group.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4919 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_move_line_reschedule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4696 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_move_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2276 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10880 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_reports.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2670 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tests/scenario_tax_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    75953 2024-02-29 15:13:04.000000 trytond_account-7.0.4/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4788 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account-7.0.4/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-10-30 17:06:38.000000 trytond_account-7.0.4/trial_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-02-05 16:24:27.000000 trytond_account-7.0.4/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.628730 trytond_account-7.0.4/trytond_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2855 2024-03-03 12:27:00.000000 trytond_account-7.0.4/trytond_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    12383 2024-03-03 12:27:00.000000 trytond_account-7.0.4/trytond_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:27:00.000000 trytond_account-7.0.4/trytond_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-03-03 12:27:00.000000 trytond_account-7.0.4/trytond_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 trytond_account-7.0.4/trytond_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-03-03 12:27:00.000000 trytond_account-7.0.4/trytond_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:27:00.000000 trytond_account-7.0.4/trytond_account.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-10-30 17:06:38.000000 trytond_account-7.0.4/type_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:27:00.628730 trytond_account-7.0.4/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/account_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_deferral_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_deferral_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_list_balance_sheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/account_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/account_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_type_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/account_type_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/account_type_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/account_type_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/aged_balance_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/aged_balance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/balance_sheet_context_comparison_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1353 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/create_chart_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/create_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/fiscalyear_balance_non_deferral_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/fiscalyear_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/fiscalyear_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/fiscalyear_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/general_ledger_account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/general_ledger_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/general_ledger_account_party_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/general_ledger_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/general_ledger_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/journal_list_cash.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/journal_open_cash_context.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/journal_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/journal_period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/journal_period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-02-29 11:37:15.000000 trytond_account-7.0.4/view/journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_cancel_default_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/move_line_delegate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1753 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_group_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_list_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_list_reconcile.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_receivable_payable_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/move_line_reschedule_preview_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/move_line_reschedule_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_reschedule_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1026 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      636 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_line_tree_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_reconciliation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_reconciliation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/move_template_create_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      857 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_template_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_template_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_template_keyword_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/open_journal_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-10-30 17:06:37.000000 trytond_account-7.0.4/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/reconcile_lines_writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      755 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/reconcile_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/reconcile_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/renew_fiscalyear_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_code_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_group_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_rule_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/tax_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/update_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/update_chart_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account-7.0.4/view/writeoff_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.410318 trytond_account-7.0.5/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10993 2024-04-04 07:53:33.000000 trytond_account-7.0.5/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-04 07:53:33.000000 trytond_account-7.0.5/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:37.000000 trytond_account-7.0.5/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:37.000000 trytond_account-7.0.5/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-04 07:53:36.410318 trytond_account-7.0.5/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.5/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-10-30 17:06:37.000000 trytond_account-7.0.5/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   126779 2024-02-05 16:24:27.000000 trytond_account-7.0.5/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    47195 2023-10-30 17:06:37.000000 trytond_account-7.0.5/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-10-30 17:06:38.000000 trytond_account-7.0.5/aged_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-10-30 17:06:38.000000 trytond_account-7.0.5/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6045 2023-10-30 17:06:37.000000 trytond_account-7.0.5/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2023-10-30 17:06:37.000000 trytond_account-7.0.5/company.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8831 2023-10-30 17:06:37.000000 trytond_account-7.0.5/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-10-30 17:06:37.000000 trytond_account-7.0.5/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.383652 trytond_account-7.0.5/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2786 2024-03-03 16:24:20.000000 trytond_account-7.0.5/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-10-30 17:06:37.000000 trytond_account-7.0.5/doc/configuration.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.386985 trytond_account-7.0.5/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/fiscal-year.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/journal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/design/template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.5/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-10-30 17:06:38.000000 trytond_account-7.0.5/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:37.000000 trytond_account-7.0.5/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:37.000000 trytond_account-7.0.5/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-10-30 17:06:38.000000 trytond_account-7.0.5/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.390318 trytond_account-7.0.5/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/close.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/create.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/structure.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-02-05 16:24:27.000000 trytond_account-7.0.5/doc/usage/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1764 2024-02-05 16:24:27.000000 trytond_account-7.0.5/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26145 2024-02-05 16:24:27.000000 trytond_account-7.0.5/fiscalyear.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-10-30 17:06:37.000000 trytond_account-7.0.5/fiscalyear.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-10-30 17:06:38.000000 trytond_account-7.0.5/general_journal.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81559 2023-10-30 17:06:38.000000 trytond_account-7.0.5/general_ledger.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.393652 trytond_account-7.0.5/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account-7.0.5/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:37.000000 trytond_account-7.0.5/icons/tryton-account-block.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:06:37.000000 trytond_account-7.0.5/icons/tryton-account-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_account-7.0.5/icons/tryton-account-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-10-30 17:06:37.000000 trytond_account-7.0.5/icons/tryton-account.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13034 2024-02-29 11:37:15.000000 trytond_account-7.0.5/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11585 2023-10-30 17:06:38.000000 trytond_account-7.0.5/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.393652 trytond_account-7.0.5/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   131031 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130273 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   114028 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   133893 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130589 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   118850 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   126934 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   138509 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   117820 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132568 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125409 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   116858 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122752 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   143136 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   134636 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130971 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122026 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125322 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   128774 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132947 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122943 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   113860 2023-10-30 17:06:37.000000 trytond_account-7.0.5/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   147904 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125886 2023-10-30 17:06:38.000000 trytond_account-7.0.5/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-10-30 17:06:38.000000 trytond_account-7.0.5/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)    17440 2024-02-05 16:24:27.000000 trytond_account-7.0.5/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22110 2023-10-30 17:06:37.000000 trytond_account-7.0.5/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11303 2023-10-30 17:06:37.000000 trytond_account-7.0.5/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-10-30 17:06:38.000000 trytond_account-7.0.5/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11058 2023-10-30 17:06:37.000000 trytond_account-7.0.5/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11004 2023-10-30 17:06:38.000000 trytond_account-7.0.5/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11069 2023-10-30 17:06:38.000000 trytond_account-7.0.5/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11050 2023-10-30 17:06:38.000000 trytond_account-7.0.5/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11083 2023-10-30 17:06:38.000000 trytond_account-7.0.5/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11090 2023-10-30 17:06:37.000000 trytond_account-7.0.5/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11405 2023-10-30 17:06:37.000000 trytond_account-7.0.5/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11056 2023-10-30 17:06:38.000000 trytond_account-7.0.5/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   116246 2024-03-25 21:44:24.000000 trytond_account-7.0.5/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27018 2023-10-30 17:06:38.000000 trytond_account-7.0.5/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15750 2023-10-30 17:06:38.000000 trytond_account-7.0.5/move_template.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6825 2023-10-30 17:06:38.000000 trytond_account-7.0.5/move_template.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13724 2023-10-30 17:06:38.000000 trytond_account-7.0.5/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-10-30 17:06:37.000000 trytond_account-7.0.5/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16034 2024-02-05 16:24:27.000000 trytond_account-7.0.5/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4175 2023-10-30 17:06:38.000000 trytond_account-7.0.5/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:53:36.410318 trytond_account-7.0.5/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-03-03 16:24:03.000000 trytond_account-7.0.5/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    70835 2024-01-08 10:53:54.000000 trytond_account-7.0.5/tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.396985 trytond_account-7.0.5/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4654 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_account_active.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:06:37.000000 trytond_account-7.0.5/tests/scenario_account_reconcile.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3992 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_account_reconcile.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2456 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_account_reconcile_automatic.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6220 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_account_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tests/scenario_account_reconciliation_alternate_currency.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3640 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_account_reconciliation_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tests/scenario_account_reconciliation_alternate_currency_write_off.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     4369 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4816 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_close_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4337 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_move_cancel.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_move_line_delegate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5034 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_move_line_group.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4919 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_move_line_reschedule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4696 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_move_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2276 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10880 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_reports.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2670 2024-02-05 16:24:27.000000 trytond_account-7.0.5/tests/scenario_tax_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    75953 2024-02-29 15:13:04.000000 trytond_account-7.0.5/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4788 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account-7.0.5/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-10-30 17:06:38.000000 trytond_account-7.0.5/trial_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-03-03 12:27:12.000000 trytond_account-7.0.5/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.410318 trytond_account-7.0.5/trytond_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-04 07:53:35.000000 trytond_account-7.0.5/trytond_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    12365 2024-04-04 07:53:36.000000 trytond_account-7.0.5/trytond_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:53:35.000000 trytond_account-7.0.5/trytond_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-04 07:53:35.000000 trytond_account-7.0.5/trytond_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 trytond_account-7.0.5/trytond_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-04 07:53:35.000000 trytond_account-7.0.5/trytond_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:53:35.000000 trytond_account-7.0.5/trytond_account.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-10-30 17:06:38.000000 trytond_account-7.0.5/type_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:53:36.410318 trytond_account-7.0.5/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/account_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_deferral_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_deferral_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_list_balance_sheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/account_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/account_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_type_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/account_type_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/account_type_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/account_type_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/aged_balance_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/aged_balance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/balance_sheet_context_comparison_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      710 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1353 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/create_chart_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/create_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/fiscalyear_balance_non_deferral_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/fiscalyear_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/fiscalyear_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/fiscalyear_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/general_ledger_account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/general_ledger_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/general_ledger_account_party_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/general_ledger_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/general_ledger_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/journal_list_cash.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/journal_open_cash_context.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/journal_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/journal_period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/journal_period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-02-29 11:37:15.000000 trytond_account-7.0.5/view/journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_cancel_default_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/move_line_delegate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1753 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_group_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_list_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_list_reconcile.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_receivable_payable_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/move_line_reschedule_preview_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/move_line_reschedule_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_reschedule_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1026 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      636 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_line_tree_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_reconciliation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_reconciliation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/move_template_create_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      857 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_template_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_template_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_template_keyword_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/open_journal_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-10-30 17:06:37.000000 trytond_account-7.0.5/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/reconcile_lines_writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      755 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/reconcile_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/reconcile_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/renew_fiscalyear_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_code_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_group_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_rule_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/tax_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/update_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/update_chart_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account-7.0.5/view/writeoff_tree.xml
```

### Comparing `trytond_account-7.0.4/CHANGELOG` & `trytond_account-7.0.5/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.5 - 2024-04-04
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.4 - 2024-03-03
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.3 - 2024-01-15
 --------------------------
```

### Comparing `trytond_account-7.0.4/COPYRIGHT` & `trytond_account-7.0.5/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/LICENSE` & `trytond_account-7.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/PKG-INFO` & `trytond_account-7.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.0.4
+Version: 7.0.5
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account/
+Project-URL: Documentation, https://docs.tryton.org/modules-account/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account-7.0.4/__init__.py` & `trytond_account-7.0.5/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/account.py` & `trytond_account-7.0.5/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/account.xml` & `trytond_account-7.0.5/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/aged_balance.fodt` & `trytond_account-7.0.5/aged_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/common.py` & `trytond_account-7.0.5/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/company.py` & `trytond_account-7.0.5/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/company.xml` & `trytond_account-7.0.5/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/configuration.py` & `trytond_account-7.0.5/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/configuration.xml` & `trytond_account-7.0.5/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/conf.py` & `trytond_account-7.0.5/doc/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_account-7.0.4/doc/configuration.rst` & `trytond_account-7.0.5/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/account.rst` & `trytond_account-7.0.5/doc/design/account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/configuration.rst` & `trytond_account-7.0.5/doc/design/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/fiscal-year.rst` & `trytond_account-7.0.5/doc/design/fiscal-year.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/journal.rst` & `trytond_account-7.0.5/doc/design/journal.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/move.rst` & `trytond_account-7.0.5/doc/design/move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/tax.rst` & `trytond_account-7.0.5/doc/design/tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/design/template.rst` & `trytond_account-7.0.5/doc/design/template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/reference.rst` & `trytond_account-7.0.5/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/setup.rst` & `trytond_account-7.0.5/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/usage/close.rst` & `trytond_account-7.0.5/doc/usage/close.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/usage/create.rst` & `trytond_account-7.0.5/doc/usage/create.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/usage/process.rst` & `trytond_account-7.0.5/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/usage/report.rst` & `trytond_account-7.0.5/doc/usage/report.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/usage/structure.rst` & `trytond_account-7.0.5/doc/usage/structure.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/doc/usage/view.rst` & `trytond_account-7.0.5/doc/usage/view.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/exceptions.py` & `trytond_account-7.0.5/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/fiscalyear.py` & `trytond_account-7.0.5/fiscalyear.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/fiscalyear.xml` & `trytond_account-7.0.5/fiscalyear.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/general_journal.fodt` & `trytond_account-7.0.5/general_journal.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/general_ledger.fodt` & `trytond_account-7.0.5/general_ledger.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/icons/LICENSE` & `trytond_account-7.0.5/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/journal.py` & `trytond_account-7.0.5/journal.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/journal.xml` & `trytond_account-7.0.5/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/bg.po` & `trytond_account-7.0.5/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/ca.po` & `trytond_account-7.0.5/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/cs.po` & `trytond_account-7.0.5/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/de.po` & `trytond_account-7.0.5/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/es.po` & `trytond_account-7.0.5/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/es_419.po` & `trytond_account-7.0.5/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/et.po` & `trytond_account-7.0.5/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/fa.po` & `trytond_account-7.0.5/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/fi.po` & `trytond_account-7.0.5/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/fr.po` & `trytond_account-7.0.5/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/hu.po` & `trytond_account-7.0.5/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/id.po` & `trytond_account-7.0.5/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/it.po` & `trytond_account-7.0.5/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/lo.po` & `trytond_account-7.0.5/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/lt.po` & `trytond_account-7.0.5/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/nl.po` & `trytond_account-7.0.5/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/pl.po` & `trytond_account-7.0.5/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/pt.po` & `trytond_account-7.0.5/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/ro.po` & `trytond_account-7.0.5/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/ru.po` & `trytond_account-7.0.5/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/sl.po` & `trytond_account-7.0.5/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/tr.po` & `trytond_account-7.0.5/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/uk.po` & `trytond_account-7.0.5/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/locale/zh_CN.po` & `trytond_account-7.0.5/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/localize.xsl` & `trytond_account-7.0.5/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/message.xml` & `trytond_account-7.0.5/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart.xml` & `trytond_account-7.0.5/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_bg.xml` & `trytond_account-7.0.5/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_ca.xml` & `trytond_account-7.0.5/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_de.xml` & `trytond_account-7.0.5/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_en.xml` & `trytond_account-7.0.5/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_es.xml` & `trytond_account-7.0.5/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_fr.xml` & `trytond_account-7.0.5/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_nl.xml` & `trytond_account-7.0.5/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_pt.xml` & `trytond_account-7.0.5/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_ru.xml` & `trytond_account-7.0.5/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/minimal_chart_sl.xml` & `trytond_account-7.0.5/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/move.py` & `trytond_account-7.0.5/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -1985,34 +1985,33 @@
                         'ir.msg_access_wizard_model_error',
                         wizard=cls.__name__,
                         model=model))
         super().check_access()
 
     def get_writeoff(self):
         "Return writeoff amount and company"
-        company = None
+        company = currency = None
         amount = Decimal('0.0')
         amount_second_currency = Decimal('0.0')
         second_currencies = set()
         for line in self.records:
             amount += line.debit - line.credit
             if line.amount_second_currency is not None:
                 amount_second_currency += line.amount_second_currency
             second_currencies.add(line.second_currency)
             if not company:
                 company = line.account.company
+                currency = company.currency
         try:
             second_currency, = second_currencies
         except ValueError:
             second_currency = None
         if second_currency:
             amount = amount_second_currency
             currency = second_currency
-        else:
-            currency = company.currency
         return amount, currency, company
 
     def transition_start(self):
         amount, currency, company = self.get_writeoff()
         if not company:
             return 'end'
         if currency.is_zero(amount):
```

### Comparing `trytond_account-7.0.4/move.xml` & `trytond_account-7.0.5/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/move_template.py` & `trytond_account-7.0.5/move_template.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/move_template.xml` & `trytond_account-7.0.5/move_template.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/party.py` & `trytond_account-7.0.5/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/party.xml` & `trytond_account-7.0.5/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/period.py` & `trytond_account-7.0.5/period.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/period.xml` & `trytond_account-7.0.5/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/setup.py` & `trytond_account-7.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-account/',
+        "Documentation": 'https://docs.tryton.org/modules-account/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account',
     package_dir={'trytond.modules.account': '.'},
     packages=(
         ['trytond.modules.account']
```

### Comparing `trytond_account-7.0.4/tax.py` & `trytond_account-7.0.5/tax.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tax.xml` & `trytond_account-7.0.5/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_account_active.rst` & `trytond_account-7.0.5/tests/scenario_account_active.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_account_reconcile.rst` & `trytond_account-7.0.5/tests/scenario_account_reconcile.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_account_reconcile_automatic.rst` & `trytond_account-7.0.5/tests/scenario_account_reconcile_automatic.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_account_reconciliation.rst` & `trytond_account-7.0.5/tests/scenario_account_reconciliation.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_account_reconciliation_alternate_currency.rst` & `trytond_account-7.0.5/tests/scenario_account_reconciliation_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_account_reconciliation_alternate_currency_write_off.rst` & `trytond_account-7.0.5/tests/scenario_account_reconciliation_alternate_currency_write_off.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_close_fiscalyear.rst` & `trytond_account-7.0.5/tests/scenario_close_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_move_cancel.rst` & `trytond_account-7.0.5/tests/scenario_move_cancel.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_move_line_delegate.rst` & `trytond_account-7.0.5/tests/scenario_move_line_delegate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_move_line_group.rst` & `trytond_account-7.0.5/tests/scenario_move_line_group.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_move_line_reschedule.rst` & `trytond_account-7.0.5/tests/scenario_move_line_reschedule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_move_template.rst` & `trytond_account-7.0.5/tests/scenario_move_template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_renew_fiscalyear.rst` & `trytond_account-7.0.5/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_reports.rst` & `trytond_account-7.0.5/tests/scenario_reports.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/scenario_tax_code.rst` & `trytond_account-7.0.5/tests/scenario_tax_code.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/test_module.py` & `trytond_account-7.0.5/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tests/tools.py` & `trytond_account-7.0.5/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tox.ini` & `trytond_account-7.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/trial_balance.fodt` & `trytond_account-7.0.5/trial_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/tryton.cfg` & `trytond_account-7.0.5/tryton.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tryton]
-version=7.0.4
+version=7.0.5
 depends:
     company
     currency
     ir
     party
     res
 xml:
```

### Comparing `trytond_account-7.0.4/trytond_account.egg-info/PKG-INFO` & `trytond_account-7.0.5/trytond_account.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.0.4
+Version: 7.0.5
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account/
+Project-URL: Documentation, https://docs.tryton.org/modules-account/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_account-7.0.4/trytond_account.egg-info/SOURCES.txt` & `trytond_account-7.0.5/trytond_account.egg-info/SOURCES.txt`

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

### Comparing `trytond_account-7.0.4/type_statement.fodt` & `trytond_account-7.0.5/type_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/account_deferral_form.xml` & `trytond_account-7.0.5/view/account_deferral_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/account_form.xml` & `trytond_account-7.0.5/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/account_template_form.xml` & `trytond_account-7.0.5/view/account_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/account_type_form.xml` & `trytond_account-7.0.5/view/account_type_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/account_type_template_form.xml` & `trytond_account-7.0.5/view/account_type_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/aged_balance_context_form.xml` & `trytond_account-7.0.5/view/aged_balance_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/company_form.xml` & `trytond_account-7.0.5/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/configuration_form.xml` & `trytond_account-7.0.5/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/fiscalyear_balance_non_deferral_start_form.xml` & `trytond_account-7.0.5/view/fiscalyear_balance_non_deferral_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/fiscalyear_create_periods_start_form.xml` & `trytond_account-7.0.5/view/fiscalyear_create_periods_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/fiscalyear_form.xml` & `trytond_account-7.0.5/view/fiscalyear_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/general_ledger_account_context_form.xml` & `trytond_account-7.0.5/view/general_ledger_account_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/general_ledger_line_list.xml` & `trytond_account-7.0.5/view/general_ledger_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/income_statement_context_form.xml` & `trytond_account-7.0.5/view/income_statement_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/journal_form.xml` & `trytond_account-7.0.5/view/journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_form.xml` & `trytond_account-7.0.5/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_form.xml` & `trytond_account-7.0.5/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_form_move.xml` & `trytond_account-7.0.5/view/move_line_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_list_payable_receivable.xml` & `trytond_account-7.0.5/view/move_line_list_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_reschedule_start_form.xml` & `trytond_account-7.0.5/view/move_line_reschedule_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_template_form.xml` & `trytond_account-7.0.5/view/move_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_tree.xml` & `trytond_account-7.0.5/view/move_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_line_tree_move.xml` & `trytond_account-7.0.5/view/move_line_tree_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_template_form.xml` & `trytond_account-7.0.5/view/move_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_template_keyword_form.xml` & `trytond_account-7.0.5/view/move_template_keyword_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/move_tree.xml` & `trytond_account-7.0.5/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/party_form.xml` & `trytond_account-7.0.5/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/period_form.xml` & `trytond_account-7.0.5/view/period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/reconcile_show_form.xml` & `trytond_account-7.0.5/view/reconcile_show_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/renew_fiscalyear_start_form.xml` & `trytond_account-7.0.5/view/renew_fiscalyear_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_code_context_form.xml` & `trytond_account-7.0.5/view/tax_code_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_code_form.xml` & `trytond_account-7.0.5/view/tax_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_code_template_form.xml` & `trytond_account-7.0.5/view/tax_code_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_form.xml` & `trytond_account-7.0.5/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_rule_form.xml` & `trytond_account-7.0.5/view/tax_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_rule_line_form.xml` & `trytond_account-7.0.5/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_rule_line_template_form.xml` & `trytond_account-7.0.5/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_template_form.xml` & `trytond_account-7.0.5/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/tax_test_form.xml` & `trytond_account-7.0.5/view/tax_test_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.4/view/writeoff_form.xml` & `trytond_account-7.0.5/view/writeoff_form.xml`

 * *Files identical despite different names*

