# Comparing `tmp/trytond_stock-7.0.3.tar.gz` & `tmp/trytond_stock-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock-7.0.3.tar", last modified: Sat Feb  3 11:07:29 2024, max compression
+gzip compressed data, was "trytond_stock-7.0.4.tar", last modified: Thu Apr  4 07:47:41 2024, max compression
```

## Comparing `trytond_stock-7.0.3.tar` & `trytond_stock-7.0.4.tar`

### file list

```diff
@@ -1,198 +1,197 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.200479 trytond_stock-7.0.3/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)    11290 2024-02-03 11:07:21.000000 trytond_stock-7.0.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      826 2024-02-03 11:07:20.000000 trytond_stock-7.0.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3045 2024-02-03 11:07:29.200479 trytond_stock-7.0.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2614 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8338 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2011 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52930 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/customer_return_restocking_list.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    52628 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/delivery_note.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.147148 trytond_stock-7.0.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2806 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/conf.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.150481 trytond_stock-7.0.3/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/inventory.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/location.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2037 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1102 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/period.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3305 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7779 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/design/shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2311 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.153814 trytond_stock-7.0.3/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/usage/period.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4193 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/usage/quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4669 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/usage/shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2344 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/doc/usage/value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      885 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.157147 trytond_stock-7.0.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/icons/tryton-shipment-in.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/icons/tryton-shipment-out.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/icons/tryton-stock.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    52341 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/internal_shipment.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    23339 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/inventory.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8485 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/inventory.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.167147 trytond_stock-7.0.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    91376 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96258 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82480 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98123 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97127 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81190 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    89915 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   101859 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82454 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97707 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92412 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    80682 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    84575 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    89594 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86771 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96425 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    85282 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87205 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    94071 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    91586 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86207 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82400 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    77357 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90721 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    28680 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11878 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9292 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    68816 2024-01-26 18:06:23.000000 trytond_stock-7.0.3/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8316 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5665 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4044 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6992 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5532 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    53034 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/picking_list.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    50768 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22458 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:07:29.200479 trytond_stock-7.0.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4569 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   116164 2024-01-13 00:01:20.000000 trytond_stock-7.0.3/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47119 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2918 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22634 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    32870 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/stock_reporting_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52114 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/supplier_restocking_list.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.177147 trytond_stock-7.0.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8312 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_average_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7877 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_inventory.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3365 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_inventory_count.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_inventory_empty_quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_move_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3845 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_product_quantities_by_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5199 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_recompute_average_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_recompute_average_cost_price_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5080 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7934 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_reporting_margin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3430 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_in.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2377 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_in_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_in_same_storage_input.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4638 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_internal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3350 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_internal_transit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     9151 2024-01-13 00:01:20.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_out.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2677 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_out_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2488 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_out_return_same_storage_input.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2529 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/scenario_stock_shipment_out_same_storage_output.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    70406 2024-01-26 18:06:23.000000 trytond_stock-7.0.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-01-15 23:14:00.000000 trytond_stock-7.0.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.197146 trytond_stock-7.0.3/trytond_stock.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3045 2024-02-03 11:07:28.000000 trytond_stock-7.0.3/trytond_stock.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     9816 2024-02-03 11:07:28.000000 trytond_stock-7.0.3/trytond_stock.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:07:28.000000 trytond_stock-7.0.3/trytond_stock.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2024-02-03 11:07:28.000000 trytond_stock-7.0.3/trytond_stock.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:12.000000 trytond_stock-7.0.3/trytond_stock.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-02-03 11:07:28.000000 trytond_stock-7.0.3/trytond_stock.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:07:28.000000 trytond_stock-7.0.3/trytond_stock.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:07:29.197146 trytond_stock-7.0.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1128 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_count_quantity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_count_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_line_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/inventory_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_quantity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_quantity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/location_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1623 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/move_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/party_address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/party_address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/party_contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/party_contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      903 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/period_cache_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/period_cache_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_by_location_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_cost_price_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_cost_price_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_modify_cost_price_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_quantities_warehouse_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_quantities_warehouse_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_quantities_warehouse_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/product_quantities_warehouse_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/products_by_locations_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/products_by_locations_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/recompute_cost_price_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_category_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_category_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_category_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_time_series_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_time_series_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_product_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_product_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_product_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/reporting_margin_product_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_assign_partial_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      650 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_in_return_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_in_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_internal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_internal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1763 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_out_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_out_return_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      646 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/shipment_out_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-10-30 17:06:38.000000 trytond_stock-7.0.3/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.299605 trytond_stock-7.0.4/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11391 2024-04-04 07:47:38.000000 trytond_stock-7.0.4/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      826 2024-04-04 07:47:38.000000 trytond_stock-7.0.4/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-04 07:47:41.299605 trytond_stock-7.0.4/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2614 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8338 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2011 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52930 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/customer_return_restocking_list.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    52628 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/delivery_note.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.279606 trytond_stock-7.0.4/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2784 2024-03-03 16:24:20.000000 trytond_stock-7.0.4/doc/conf.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.282939 trytond_stock-7.0.4/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/inventory.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/location.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2037 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1102 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/period.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3305 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7779 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/design/shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2311 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.286273 trytond_stock-7.0.4/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/usage/period.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4193 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/usage/quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4669 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/usage/shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/doc/usage/value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      885 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.286273 trytond_stock-7.0.4/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/icons/tryton-shipment-in.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/icons/tryton-shipment-out.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/icons/tryton-stock.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    52341 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/internal_shipment.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    23339 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/inventory.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8485 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/inventory.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.289606 trytond_stock-7.0.4/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    91376 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96258 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82480 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    98123 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97127 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81190 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    89915 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   101859 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82454 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97707 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92412 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    80682 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    84575 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    89594 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86771 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96425 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85282 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87205 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    94071 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    91586 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86207 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82400 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    77357 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90721 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    28680 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11878 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9292 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    68816 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8316 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5665 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4044 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6992 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5532 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    53034 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/picking_list.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    50848 2024-03-25 21:41:30.000000 trytond_stock-7.0.4/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22458 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:47:41.299605 trytond_stock-7.0.4/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4560 2024-03-03 16:24:03.000000 trytond_stock-7.0.4/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   116165 2024-03-25 21:22:17.000000 trytond_stock-7.0.4/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    47119 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2918 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22634 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    32870 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/stock_reporting_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52114 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/supplier_restocking_list.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.289606 trytond_stock-7.0.4/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8312 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_average_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7877 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_inventory.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3365 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_inventory_count.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_inventory_empty_quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_move_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3845 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_product_quantities_by_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5199 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_recompute_average_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3123 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_recompute_average_cost_price_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5080 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7934 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_reporting_margin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3430 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_in.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2377 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_in_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_in_same_storage_input.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4638 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_internal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3350 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_internal_transit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     9151 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_out.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2677 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_out_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2488 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_out_return_same_storage_input.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2529 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tests/scenario_stock_shipment_out_same_storage_output.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    70406 2024-01-26 18:06:23.000000 trytond_stock-7.0.4/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.299605 trytond_stock-7.0.4/trytond_stock.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-04 07:47:40.000000 trytond_stock-7.0.4/trytond_stock.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     9798 2024-04-04 07:47:41.000000 trytond_stock-7.0.4/trytond_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:47:40.000000 trytond_stock-7.0.4/trytond_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2024-04-04 07:47:40.000000 trytond_stock-7.0.4/trytond_stock.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:12.000000 trytond_stock-7.0.4/trytond_stock.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-04-04 07:47:40.000000 trytond_stock-7.0.4/trytond_stock.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:47:40.000000 trytond_stock-7.0.4/trytond_stock.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:47:41.299605 trytond_stock-7.0.4/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1128 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_count_quantity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_count_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_line_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/inventory_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/location_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/location_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/view/location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/location_quantity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/location_quantity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-02-05 16:24:27.000000 trytond_stock-7.0.4/view/location_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1623 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/move_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/party_address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/party_address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/party_contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/party_contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      903 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/period_cache_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/period_cache_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_by_location_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_cost_price_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_cost_price_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_modify_cost_price_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_quantities_warehouse_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_quantities_warehouse_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_quantities_warehouse_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/product_quantities_warehouse_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/products_by_locations_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/products_by_locations_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/recompute_cost_price_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_category_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_category_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_category_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_time_series_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_time_series_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_product_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_product_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_product_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/reporting_margin_product_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_assign_partial_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      650 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_in_return_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_in_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_internal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_internal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1763 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_out_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_out_return_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      646 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/shipment_out_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-10-30 17:06:38.000000 trytond_stock-7.0.4/view/user_form_preferences.xml
```

### Comparing `trytond_stock-7.0.3/CHANGELOG` & `trytond_stock-7.0.4/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.4 - 2024-04-04
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.3 - 2024-02-03
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.2 - 2024-01-15
 --------------------------
```

### Comparing `trytond_stock-7.0.3/COPYRIGHT` & `trytond_stock-7.0.4/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/LICENSE` & `trytond_stock-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/PKG-INFO` & `trytond_stock-7.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock
-Version: 7.0.3
+Version: 7.0.4
 Summary: Tryton module for stock and inventory
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock/
+Project-URL: Documentation, https://docs.tryton.org/modules-stock/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_stock-7.0.3/__init__.py` & `trytond_stock-7.0.4/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/configuration.py` & `trytond_stock-7.0.4/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/configuration.xml` & `trytond_stock-7.0.4/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/customer_return_restocking_list.fodt` & `trytond_stock-7.0.4/customer_return_restocking_list.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/delivery_note.fodt` & `trytond_stock-7.0.4/delivery_note.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/conf.py` & `trytond_stock-7.0.4/doc/conf.py`

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

### Comparing `trytond_stock-7.0.3/doc/design/configuration.rst` & `trytond_stock-7.0.4/doc/design/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/design/inventory.rst` & `trytond_stock-7.0.4/doc/design/inventory.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/design/location.rst` & `trytond_stock-7.0.4/doc/design/location.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/design/move.rst` & `trytond_stock-7.0.4/doc/design/move.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/design/period.rst` & `trytond_stock-7.0.4/doc/design/period.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/design/product.rst` & `trytond_stock-7.0.4/doc/design/product.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/design/shipment.rst` & `trytond_stock-7.0.4/doc/design/shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/setup.rst` & `trytond_stock-7.0.4/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/usage/period.rst` & `trytond_stock-7.0.4/doc/usage/period.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/usage/quantity.rst` & `trytond_stock-7.0.4/doc/usage/quantity.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/usage/shipment.rst` & `trytond_stock-7.0.4/doc/usage/shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/doc/usage/value.rst` & `trytond_stock-7.0.4/doc/usage/value.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/exceptions.py` & `trytond_stock-7.0.4/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/icons/LICENSE` & `trytond_stock-7.0.4/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/internal_shipment.fodt` & `trytond_stock-7.0.4/internal_shipment.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/inventory.py` & `trytond_stock-7.0.4/inventory.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/inventory.xml` & `trytond_stock-7.0.4/inventory.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/ir.py` & `trytond_stock-7.0.4/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/bg.po` & `trytond_stock-7.0.4/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/ca.po` & `trytond_stock-7.0.4/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/cs.po` & `trytond_stock-7.0.4/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/de.po` & `trytond_stock-7.0.4/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/es.po` & `trytond_stock-7.0.4/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/es_419.po` & `trytond_stock-7.0.4/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/et.po` & `trytond_stock-7.0.4/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/fa.po` & `trytond_stock-7.0.4/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/fi.po` & `trytond_stock-7.0.4/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/fr.po` & `trytond_stock-7.0.4/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/hu.po` & `trytond_stock-7.0.4/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/id.po` & `trytond_stock-7.0.4/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/it.po` & `trytond_stock-7.0.4/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/lo.po` & `trytond_stock-7.0.4/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/lt.po` & `trytond_stock-7.0.4/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/nl.po` & `trytond_stock-7.0.4/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/pl.po` & `trytond_stock-7.0.4/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/pt.po` & `trytond_stock-7.0.4/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/ro.po` & `trytond_stock-7.0.4/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/ru.po` & `trytond_stock-7.0.4/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/sl.po` & `trytond_stock-7.0.4/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/tr.po` & `trytond_stock-7.0.4/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/uk.po` & `trytond_stock-7.0.4/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/locale/zh_CN.po` & `trytond_stock-7.0.4/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/location.py` & `trytond_stock-7.0.4/location.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/location.xml` & `trytond_stock-7.0.4/location.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/message.xml` & `trytond_stock-7.0.4/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/move.py` & `trytond_stock-7.0.4/move.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/move.xml` & `trytond_stock-7.0.4/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/party.py` & `trytond_stock-7.0.4/party.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/party.xml` & `trytond_stock-7.0.4/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/period.py` & `trytond_stock-7.0.4/period.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/period.xml` & `trytond_stock-7.0.4/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/picking_list.fodt` & `trytond_stock-7.0.4/picking_list.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/product.py` & `trytond_stock-7.0.4/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1154,29 +1154,31 @@
                 revision.product = product
                 revision.template = product.template
                 revisions.append(revision)
                 if ((
                             product.cost_price_method == 'fixed'
                             and revision.date == today)
                         or product.type == 'service'):
-                    cost = revision.get_cost_price(product.cost_price)
+                    cost = round_price(
+                        revision.get_cost_price(product.cost_price))
                     costs[cost].append(product)
                     records.remove(product)
         elif self.model.__name__ == 'product.template':
             records = list(self.records)
             for template in list(records):
                 revision = self.get_revision(Revision)
                 revision.template = template
                 revisions.append(revision)
                 if ((
                             template.cost_price_method == 'fixed'
                             and revision.date == today)
                         or template.type == 'service'):
                     for product in template.products:
-                        cost = revision.get_cost_price(product.cost_price)
+                        cost = round_price(
+                            revision.get_cost_price(product.cost_price))
                         costs[cost].append(product)
                     records.remove(template)
         Revision.save(revisions)
         if costs:
             Product.update_cost_price(costs)
         if records:
             start = min((r.date for r in revisions), default=None)
```

### Comparing `trytond_stock-7.0.3/product.xml` & `trytond_stock-7.0.4/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/res.py` & `trytond_stock-7.0.4/res.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/res.xml` & `trytond_stock-7.0.4/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/setup.py` & `trytond_stock-7.0.4/setup.py`

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
-        "Documentation": 'https://docs.tryton.org/projects/modules-stock/',
+        "Documentation": 'https://docs.tryton.org/modules-stock/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock',
     package_dir={'trytond.modules.stock': '.'},
     packages=(
         ['trytond.modules.stock']
```

### Comparing `trytond_stock-7.0.3/shipment.py` & `trytond_stock-7.0.4/shipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     def _get_assign_domain(cls):
         pool = Pool()
         Date = pool.get('ir.date')
         context = Transaction().context
         return [
             ('company', '=', context.get('company')),
             ('state', '=', 'waiting'),
-            ('planned_date', '=', Date.today()),
+            ('planned_date', '<=', Date.today()),
             ]
 
     @classmethod
     def assign_cron(cls):
         shipments = cls.search(cls._get_assign_domain())
         cls.assign_try(shipments)
```

### Comparing `trytond_stock-7.0.3/shipment.xml` & `trytond_stock-7.0.4/shipment.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/stock.xml` & `trytond_stock-7.0.4/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/stock_reporting_margin.py` & `trytond_stock-7.0.4/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/stock_reporting_margin.xml` & `trytond_stock-7.0.4/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/supplier_restocking_list.fodt` & `trytond_stock-7.0.4/supplier_restocking_list.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_average_cost_price.rst` & `trytond_stock-7.0.4/tests/scenario_stock_average_cost_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_inventory.rst` & `trytond_stock-7.0.4/tests/scenario_stock_inventory.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_inventory_count.rst` & `trytond_stock-7.0.4/tests/scenario_stock_inventory_count.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_inventory_empty_quantity.rst` & `trytond_stock-7.0.4/tests/scenario_stock_inventory_empty_quantity.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_move_in_future.rst` & `trytond_stock-7.0.4/tests/scenario_stock_move_in_future.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_product_quantities_by_warehouse.rst` & `trytond_stock-7.0.4/tests/scenario_stock_product_quantities_by_warehouse.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_recompute_average_cost_price.rst` & `trytond_stock-7.0.4/tests/scenario_stock_recompute_average_cost_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_recompute_average_cost_price_production.rst` & `trytond_stock-7.0.4/tests/scenario_stock_recompute_average_cost_price_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_reporting.rst` & `trytond_stock-7.0.4/tests/scenario_stock_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_reporting_margin.rst` & `trytond_stock-7.0.4/tests/scenario_stock_reporting_margin.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_in.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_in.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_in_return.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_in_return.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_in_same_storage_input.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_in_same_storage_input.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_internal.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_internal.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_internal_transit.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_internal_transit.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_out.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_out.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_out_return.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_out_return.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_out_return_same_storage_input.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_out_return_same_storage_input.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/scenario_stock_shipment_out_same_storage_output.rst` & `trytond_stock-7.0.4/tests/scenario_stock_shipment_out_same_storage_output.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tests/test_module.py` & `trytond_stock-7.0.4/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/tox.ini` & `trytond_stock-7.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/trytond_stock.egg-info/PKG-INFO` & `trytond_stock-7.0.4/trytond_stock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock
-Version: 7.0.3
+Version: 7.0.4
 Summary: Tryton module for stock and inventory
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock/
+Project-URL: Documentation, https://docs.tryton.org/modules-stock/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `trytond_stock-7.0.3/trytond_stock.egg-info/SOURCES.txt` & `trytond_stock-7.0.4/trytond_stock.egg-info/SOURCES.txt`

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
 configuration.py
```

### Comparing `trytond_stock-7.0.3/view/configuration_form.xml` & `trytond_stock-7.0.4/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/inventory_form.xml` & `trytond_stock-7.0.4/view/inventory_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/inventory_line_form.xml` & `trytond_stock-7.0.4/view/inventory_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/location_form.xml` & `trytond_stock-7.0.4/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/location_quantity_form.xml` & `trytond_stock-7.0.4/view/location_quantity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/move_form.xml` & `trytond_stock-7.0.4/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/move_tree.xml` & `trytond_stock-7.0.4/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/party_form.xml` & `trytond_stock-7.0.4/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/reporting_margin_category_list.xml` & `trytond_stock-7.0.4/view/reporting_margin_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/reporting_margin_context_form.xml` & `trytond_stock-7.0.4/view/reporting_margin_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_in_form.xml` & `trytond_stock-7.0.4/view/shipment_in_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_in_return_form.xml` & `trytond_stock-7.0.4/view/shipment_in_return_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_in_return_tree.xml` & `trytond_stock-7.0.4/view/shipment_in_return_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_in_tree.xml` & `trytond_stock-7.0.4/view/shipment_in_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_internal_form.xml` & `trytond_stock-7.0.4/view/shipment_internal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_internal_tree.xml` & `trytond_stock-7.0.4/view/shipment_internal_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_out_form.xml` & `trytond_stock-7.0.4/view/shipment_out_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_out_return_form.xml` & `trytond_stock-7.0.4/view/shipment_out_return_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_out_return_tree.xml` & `trytond_stock-7.0.4/view/shipment_out_return_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-7.0.3/view/shipment_out_tree.xml` & `trytond_stock-7.0.4/view/shipment_out_tree.xml`

 * *Files identical despite different names*

