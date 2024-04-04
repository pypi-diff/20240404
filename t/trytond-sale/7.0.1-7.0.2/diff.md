# Comparing `tmp/trytond_sale-7.0.1.tar.gz` & `tmp/trytond_sale-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-7.0.1.tar", last modified: Sat Feb  3 11:24:44 2024, max compression
+gzip compressed data, was "trytond_sale-7.0.2.tar", last modified: Thu Apr  4 07:49:38 2024, max compression
```

## Comparing `trytond_sale-7.0.1.tar` & `trytond_sale-7.0.2.tar`

### file list

```diff
@@ -1,127 +1,126 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.461337 trytond_sale-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     6633 2024-02-03 11:24:40.000000 trytond_sale-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-02-03 11:24:39.000000 trytond_sale-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3341 2024-02-03 11:24:44.461337 trytond_sale-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.448004 trytond_sale-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2805 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9118 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.448004 trytond_sale-7.0.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/usage/presales.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4006 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/usage/reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.451337 trytond_sale-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/icons/tryton-sale.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5255 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.454670 trytond_sale-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    41487 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42300 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36585 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43026 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42500 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34894 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39826 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    44547 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36546 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42901 2024-01-26 17:57:52.000000 trytond_sale-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40842 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37767 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39110 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40549 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40909 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42387 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38023 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39321 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42391 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41566 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39026 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36537 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34330 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36845 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4617 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4574 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8949 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2740 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    76266 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/sale.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    84404 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24435 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36553 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:24:44.461337 trytond_sale-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4565 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7657 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3013 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.454670 trytond_sale-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20146 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_default_methods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1500 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_manual_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3028 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12999 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/scenario_sale_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2524 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:55:12.000000 trytond_sale-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.458003 trytond_sale-7.0.1/trytond_sale.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3341 2024-02-03 11:24:43.000000 trytond_sale-7.0.1/trytond_sale.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5204 2024-02-03 11:24:44.000000 trytond_sale-7.0.1/trytond_sale.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:24:43.000000 trytond_sale-7.0.1/trytond_sale.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-02-03 11:24:43.000000 trytond_sale-7.0.1/trytond_sale.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale-7.0.1/trytond_sale.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-02-03 11:24:43.000000 trytond_sale-7.0.1/trytond_sale.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:24:43.000000 trytond_sale-7.0.1/trytond_sale.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:24:44.458003 trytond_sale-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/product_list_sale_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/return_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3846 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1554 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_customer_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_customer_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_customer_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_customer_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_main_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_main_time_series_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_product_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_product_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_product_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_product_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_reporting_region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/sale_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_sale-7.0.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.976528 trytond_sale-7.0.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6734 2024-04-04 07:49:35.000000 trytond_sale-7.0.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-04 07:49:35.000000 trytond_sale-7.0.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-04 07:49:38.976528 trytond_sale-7.0.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.959862 trytond_sale-7.0.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2783 2024-03-03 16:24:20.000000 trytond_sale-7.0.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9118 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.966528 trytond_sale-7.0.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/doc/usage/presales.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4006 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/doc/usage/reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.969861 trytond_sale-7.0.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/icons/tryton-sale.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5255 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.969861 trytond_sale-7.0.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41487 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42300 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36585 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43026 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42500 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34894 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39826 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    44547 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36546 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42901 2024-01-26 17:57:52.000000 trytond_sale-7.0.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40842 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37767 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39110 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40549 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40909 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42387 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38023 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39321 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42391 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41566 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39026 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36537 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34330 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36845 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4617 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4574 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8949 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2740 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    76266 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/sale.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    84662 2024-04-04 07:37:13.000000 trytond_sale-7.0.2/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24435 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36553 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:49:38.976528 trytond_sale-7.0.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-03-03 16:24:03.000000 trytond_sale-7.0.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7657 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3013 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.973194 trytond_sale-7.0.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20146 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_default_methods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2359 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_manual_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3028 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12999 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tests/scenario_sale_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2524 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-02-05 16:24:27.000000 trytond_sale-7.0.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.976528 trytond_sale-7.0.2/trytond_sale.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-04 07:49:38.000000 trytond_sale-7.0.2/trytond_sale.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-04 07:49:38.000000 trytond_sale-7.0.2/trytond_sale.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:49:38.000000 trytond_sale-7.0.2/trytond_sale.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-04-04 07:49:38.000000 trytond_sale-7.0.2/trytond_sale.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale-7.0.2/trytond_sale.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-04 07:49:38.000000 trytond_sale-7.0.2/trytond_sale.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:49:38.000000 trytond_sale-7.0.2/trytond_sale.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:49:38.976528 trytond_sale-7.0.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/product_list_sale_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/return_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3846 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1554 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_customer_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_customer_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_customer_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_customer_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_main_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_main_time_series_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_product_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_product_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_product_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_product_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_reporting_region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/sale_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_sale-7.0.2/view/template_tree.xml
```

### Comparing `trytond_sale-7.0.1/CHANGELOG` & `trytond_sale-7.0.2/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.2 - 2024-04-04
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.1 - 2024-02-03
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_sale-7.0.1/COPYRIGHT` & `trytond_sale-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/LICENSE` & `trytond_sale-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/PKG-INFO` & `trytond_sale-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale/
+Project-URL: Documentation, https://docs.tryton.org/modules-sale/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_sale-7.0.1/__init__.py` & `trytond_sale-7.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/configuration.py` & `trytond_sale-7.0.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/configuration.xml` & `trytond_sale-7.0.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/doc/conf.py` & `trytond_sale-7.0.2/doc/conf.py`

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

### Comparing `trytond_sale-7.0.1/doc/design.rst` & `trytond_sale-7.0.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/doc/usage/presales.rst` & `trytond_sale-7.0.2/doc/usage/presales.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/doc/usage/process.rst` & `trytond_sale-7.0.2/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/doc/usage/reporting.rst` & `trytond_sale-7.0.2/doc/usage/reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/doc/usage/returns.rst` & `trytond_sale-7.0.2/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/icons/LICENSE` & `trytond_sale-7.0.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/invoice.py` & `trytond_sale-7.0.2/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/invoice.xml` & `trytond_sale-7.0.2/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/bg.po` & `trytond_sale-7.0.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/ca.po` & `trytond_sale-7.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/cs.po` & `trytond_sale-7.0.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/de.po` & `trytond_sale-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/es.po` & `trytond_sale-7.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/es_419.po` & `trytond_sale-7.0.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/et.po` & `trytond_sale-7.0.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/fa.po` & `trytond_sale-7.0.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/fi.po` & `trytond_sale-7.0.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/fr.po` & `trytond_sale-7.0.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/hu.po` & `trytond_sale-7.0.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/id.po` & `trytond_sale-7.0.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/it.po` & `trytond_sale-7.0.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/lo.po` & `trytond_sale-7.0.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/lt.po` & `trytond_sale-7.0.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/nl.po` & `trytond_sale-7.0.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/pl.po` & `trytond_sale-7.0.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/pt.po` & `trytond_sale-7.0.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/ro.po` & `trytond_sale-7.0.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/ru.po` & `trytond_sale-7.0.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/sl.po` & `trytond_sale-7.0.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/tr.po` & `trytond_sale-7.0.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/uk.po` & `trytond_sale-7.0.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/locale/zh_CN.po` & `trytond_sale-7.0.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/message.xml` & `trytond_sale-7.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/party.py` & `trytond_sale-7.0.2/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/party.xml` & `trytond_sale-7.0.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/product.py` & `trytond_sale-7.0.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/product.xml` & `trytond_sale-7.0.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/sale.fodt` & `trytond_sale-7.0.2/sale.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/sale.py` & `trytond_sale-7.0.2/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,20 +617,28 @@
     def get_invoice_state(self):
         '''
         Return the invoice state for the sale.
         '''
         skips = set(self.invoices_ignored)
         skips.update(self.invoices_recreated)
         invoices = [i for i in self._invoices_for_state if i not in skips]
+
+        def is_cancelled(invoice):
+            return invoice.state == 'cancelled' and not invoice.cancel_move
+
+        def is_paid(invoice):
+            return (
+                invoice.state == 'paid'
+                or (invoice.state == 'cancelled' and invoice.cancel_move))
         if invoices:
-            if any(i.state == 'cancelled' for i in invoices):
+            if any(is_cancelled(i) for i in invoices):
                 return 'exception'
-            elif all(i.state == 'paid' for i in invoices):
+            elif all(is_paid(i) for i in invoices):
                 return 'paid'
-            elif any(i.state == 'paid' for i in invoices):
+            elif any(is_paid(i) for i in invoices):
                 return 'partially paid'
             elif any(i.state == 'posted' for i in invoices):
                 return 'awaiting payment'
             else:
                 return 'pending'
         return 'none'
```

### Comparing `trytond_sale-7.0.1/sale.xml` & `trytond_sale-7.0.2/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/sale_reporting.py` & `trytond_sale-7.0.2/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/sale_reporting.xml` & `trytond_sale-7.0.2/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/setup.py` & `trytond_sale-7.0.2/setup.py`

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
-        "Documentation": 'https://docs.tryton.org/projects/modules-sale/',
+        "Documentation": 'https://docs.tryton.org/modules-sale/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale',
     package_dir={'trytond.modules.sale': '.'},
     packages=(
         ['trytond.modules.sale']
```

### Comparing `trytond_sale-7.0.1/stock.py` & `trytond_sale-7.0.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/stock.xml` & `trytond_sale-7.0.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale.rst` & `trytond_sale-7.0.2/tests/scenario_sale.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_default_methods.rst` & `trytond_sale-7.0.2/tests/scenario_sale_default_methods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_default_taxes.rst` & `trytond_sale-7.0.2/tests/scenario_sale_default_taxes.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_empty.rst` & `trytond_sale-7.0.2/tests/scenario_sale_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_manual_invoice.rst` & `trytond_sale-7.0.2/tests/scenario_sale_manual_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_manual_shipment.rst` & `trytond_sale-7.0.2/tests/scenario_sale_manual_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_modify_header.rst` & `trytond_sale-7.0.2/tests/scenario_sale_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/scenario_sale_reporting.rst` & `trytond_sale-7.0.2/tests/scenario_sale_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tests/test_module.py` & `trytond_sale-7.0.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/tox.ini` & `trytond_sale-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/trytond_sale.egg-info/PKG-INFO` & `trytond_sale-7.0.2/trytond_sale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale/
+Project-URL: Documentation, https://docs.tryton.org/modules-sale/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_sale-7.0.1/trytond_sale.egg-info/SOURCES.txt` & `trytond_sale-7.0.2/trytond_sale.egg-info/SOURCES.txt`

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
 configuration.py
```

### Comparing `trytond_sale-7.0.1/view/configuration_form.xml` & `trytond_sale-7.0.2/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/party_form.xml` & `trytond_sale-7.0.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/product_list_sale_line.xml` & `trytond_sale-7.0.2/view/product_list_sale_line.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/product_sale_context_form.xml` & `trytond_sale-7.0.2/view/product_sale_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_form.xml` & `trytond_sale-7.0.2/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_line_form.xml` & `trytond_sale-7.0.2/view/sale_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_line_tree.xml` & `trytond_sale-7.0.2/view/sale_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_line_tree_sequence.xml` & `trytond_sale-7.0.2/view/sale_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_reporting_context_form.xml` & `trytond_sale-7.0.2/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_reporting_customer_category_list.xml` & `trytond_sale-7.0.2/view/sale_reporting_customer_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_reporting_product_category_list.xml` & `trytond_sale-7.0.2/view/sale_reporting_product_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/sale_tree.xml` & `trytond_sale-7.0.2/view/sale_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.1/view/template_form.xml` & `trytond_sale-7.0.2/view/template_form.xml`

 * *Files identical despite different names*

