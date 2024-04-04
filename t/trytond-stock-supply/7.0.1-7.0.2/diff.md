# Comparing `tmp/trytond_stock_supply-7.0.1.tar.gz` & `tmp/trytond_stock_supply-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply-7.0.1.tar", last modified: Mon Jan 15 23:12:39 2024, max compression
+gzip compressed data, was "trytond_stock_supply-7.0.2.tar", last modified: Thu Apr  4 07:46:25 2024, max compression
```

## Comparing `trytond_stock_supply-7.0.1.tar` & `trytond_stock_supply-7.0.2.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:12:39.871294 trytond_stock_supply-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3971 2024-01-15 23:12:37.000000 trytond_stock_supply-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-01-15 23:12:37.000000 trytond_stock_supply-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-01-15 23:12:39.871294 trytond_stock_supply-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:12:39.864627 trytond_stock_supply-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2813 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:12:39.867960 trytond_stock_supply-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5635 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6000 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5981 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6050 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4704 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6098 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6102 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5766 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4701 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4980 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5820 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5039 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5924 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4611 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5684 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5505 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8358 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/order_point.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4016 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/order_point.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14504 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)      966 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-15 23:12:39.871294 trytond_stock_supply-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4354 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7697 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5026 2024-01-08 10:57:27.000000 trytond_stock_supply-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1279 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:12:39.867960 trytond_stock_supply-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5764 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/scenario_stock_internal_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/scenario_stock_internal_supply_lead_time.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4459 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/scenario_stock_internal_supply_overflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7517 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/scenario_stock_supply_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:55:12.000000 trytond_stock_supply-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:12:39.871294 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-01-15 23:12:39.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2024-01-15 23:12:39.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-15 23:12:39.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-01-15 23:12:39.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:19.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-01-15 23:12:39.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-15 23:12:39.000000 trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:12:39.871294 trytond_stock_supply-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1076 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/view/order_point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      486 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/view/order_point_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.1/view/supply_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.184930 trytond_stock_supply-7.0.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4072 2024-04-04 07:46:22.000000 trytond_stock_supply-7.0.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-04-04 07:46:22.000000 trytond_stock_supply-7.0.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.178263 trytond_stock_supply-7.0.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2791 2024-03-03 16:24:20.000000 trytond_stock_supply-7.0.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5635 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5981 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6050 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4704 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6098 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6102 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5766 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4701 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4980 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5820 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5039 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5924 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4611 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5684 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5505 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8358 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/order_point.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4016 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/order_point.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14550 2024-03-25 21:49:01.000000 trytond_stock_supply-7.0.2/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      966 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:46:25.184930 trytond_stock_supply-7.0.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4354 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7697 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5026 2024-01-08 10:57:27.000000 trytond_stock_supply-7.0.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1279 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5764 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_lead_time.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4459 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_overflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7517 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_supply_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2365 2024-04-04 07:46:25.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:19.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1076 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/order_point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      486 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/order_point_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/supply_start_form.xml
```

### Comparing `trytond_stock_supply-7.0.1/CHANGELOG` & `trytond_stock_supply-7.0.2/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.2 - 2024-04-04
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.1 - 2024-01-15
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_stock_supply-7.0.1/COPYRIGHT` & `trytond_stock_supply-7.0.2/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Copyright (C) 2013-2019 NaN-tic.
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_supply-7.0.1/LICENSE` & `trytond_stock_supply-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/PKG-INFO` & `trytond_stock_supply-7.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
```

### Comparing `trytond_stock_supply-7.0.1/README.rst` & `trytond_stock_supply-7.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/__init__.py` & `trytond_stock_supply-7.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/doc/conf.py` & `trytond_stock_supply-7.0.2/doc/conf.py`

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

### Comparing `trytond_stock_supply-7.0.1/doc/index.rst` & `trytond_stock_supply-7.0.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/bg.po` & `trytond_stock_supply-7.0.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/ca.po` & `trytond_stock_supply-7.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/cs.po` & `trytond_stock_supply-7.0.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/de.po` & `trytond_stock_supply-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/es.po` & `trytond_stock_supply-7.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/es_419.po` & `trytond_stock_supply-7.0.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/et.po` & `trytond_stock_supply-7.0.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/fa.po` & `trytond_stock_supply-7.0.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/fi.po` & `trytond_stock_supply-7.0.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/fr.po` & `trytond_stock_supply-7.0.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/hu.po` & `trytond_stock_supply-7.0.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/id.po` & `trytond_stock_supply-7.0.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/it.po` & `trytond_stock_supply-7.0.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/lo.po` & `trytond_stock_supply-7.0.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/lt.po` & `trytond_stock_supply-7.0.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/nl.po` & `trytond_stock_supply-7.0.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/pl.po` & `trytond_stock_supply-7.0.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/pt.po` & `trytond_stock_supply-7.0.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/ro.po` & `trytond_stock_supply-7.0.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/ru.po` & `trytond_stock_supply-7.0.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/sl.po` & `trytond_stock_supply-7.0.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/tr.po` & `trytond_stock_supply-7.0.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/uk.po` & `trytond_stock_supply-7.0.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/locale/zh_CN.po` & `trytond_stock_supply-7.0.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/location.py` & `trytond_stock_supply-7.0.2/location.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/message.xml` & `trytond_stock_supply-7.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/order_point.py` & `trytond_stock_supply-7.0.2/order_point.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/order_point.xml` & `trytond_stock_supply-7.0.2/order_point.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/product.py` & `trytond_stock_supply-7.0.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/product.xml` & `trytond_stock_supply-7.0.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/purchase_request.py` & `trytond_stock_supply-7.0.2/purchase_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
                             company, order_point)
                         new_requests.append(request)
 
         # delete purchase requests without a purchase line
         products = set(products)
         reqs = cls.search([
                 ('state', '=', 'draft'),
+                ('purchase_line', '=', None),
                 ('company', '=', company.id),
                 ('origin', 'like', 'stock.order_point,%'),
                 ])
         reqs = [r for r in reqs
             if r.product in products and r.warehouse in warehouses]
         cls.delete(reqs)
         new_requests = cls.compare_requests(new_requests, company)
```

### Comparing `trytond_stock_supply-7.0.1/purchase_request.xml` & `trytond_stock_supply-7.0.2/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/setup.py` & `trytond_stock_supply-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/shipment.py` & `trytond_stock_supply-7.0.2/shipment.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/stock.py` & `trytond_stock_supply-7.0.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/stock.xml` & `trytond_stock_supply-7.0.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/tests/scenario_stock_internal_supply.rst` & `trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/tests/scenario_stock_internal_supply_lead_time.rst` & `trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_lead_time.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/tests/scenario_stock_internal_supply_overflow.rst` & `trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_overflow.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/tests/scenario_stock_supply_purchase_request.rst` & `trytond_stock_supply-7.0.2/tests/scenario_stock_supply_purchase_request.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/tests/test_module.py` & `trytond_stock_supply-7.0.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/tox.ini` & `trytond_stock_supply-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/PKG-INFO` & `trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trytond-stock-supply
-Version: 7.0.1
+Name: trytond_stock_supply
+Version: 7.0.2
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
```

### Comparing `trytond_stock_supply-7.0.1/trytond_stock_supply.egg-info/SOURCES.txt` & `trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_stock_supply-7.0.1/view/order_point_form.xml` & `trytond_stock_supply-7.0.2/view/order_point_form.xml`

 * *Files identical despite different names*

