# Comparing `tmp/rer.block.iframembed-1.0.2.tar.gz` & `tmp/rer.block.iframembed-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.block.iframembed-1.0.2.tar", last modified: Wed Mar 27 15:04:05 2024, max compression
+gzip compressed data, was "rer.block.iframembed-1.0.3.tar", last modified: Thu Apr  4 14:44:47 2024, max compression
```

## Comparing `rer.block.iframembed-1.0.2.tar` & `rer.block.iframembed-1.0.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.177329 rer.block.iframembed-1.0.2/
--rw-r--r--   0 cekk       (501) staff       (20)      297 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       78 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      671 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      118 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     2128 2024-03-27 15:04:05.177389 rer.block.iframembed-1.0.2/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)      740 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.170980 rer.block.iframembed-1.0.2/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7923 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       83 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       42 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      518 2024-03-27 15:04:05.177662 rer.block.iframembed-1.0.2/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2443 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.167939 rer.block.iframembed-1.0.2/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.171110 rer.block.iframembed-1.0.2/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.172216 rer.block.iframembed-1.0.2/src/rer/block/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.172786 rer.block.iframembed-1.0.2/src/rer/block/iframembed/
--rw-r--r--   0 cekk       (501) staff       (20)      137 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.173112 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      883 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      486 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/controlpanel.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.173239 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/overrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/overrides/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.173349 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/static/.gitkeep
--rw-r--r--   0 cekk       (501) staff       (20)     1261 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.173697 rer.block.iframembed-1.0.2/src/rer/block/iframembed/interfaces/
--rw-r--r--   0 cekk       (501) staff       (20)      296 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/interfaces/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      268 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/interfaces/layer.py
--rw-r--r--   0 cekk       (501) staff       (20)      712 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/interfaces/settings.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.174254 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.168489 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.174492 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/en/LC_MESSAGES/rer.block.iframembed.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1566 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/en/LC_MESSAGES/rer.block.iframembed.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.168597 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.174733 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1133 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1867 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.po
--rw-r--r--   0 cekk       (501) staff       (20)     1689 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/rer.block.iframembed.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1587 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      497 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.168843 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.175332 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      185 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      590 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      182 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.175472 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      275 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.175598 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      130 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.175839 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      233 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.176159 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/deserializers/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/deserializers/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2669 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/deserializers/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      423 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/deserializers/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.176367 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      148 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.176735 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/controlpanel/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/controlpanel/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      665 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/controlpanel/adapters.py
--rw-r--r--   0 cekk       (501) staff       (20)      400 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/controlpanel/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      621 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1523 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.177093 rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.177212 rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/robot/
--rw-r--r--   0 cekk       (501) staff       (20)     2011 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/robot/test_example.robot
--rw-r--r--   0 cekk       (501) staff       (20)      905 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/test_robot.py
--rw-r--r--   0 cekk       (501) staff       (20)     2496 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/test_setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-27 15:04:05.172102 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     2128 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2942 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      125 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       14 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      173 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2024-03-27 15:04:05.000000 rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)     3563 2024-03-27 15:04:04.000000 rer.block.iframembed-1.0.2/tox.ini
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.930629 rer.block.iframembed-1.0.3/
+-rw-r--r--   0 cekk       (501) staff       (20)      420 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       78 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      671 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     2251 2024-04-04 14:44:47.930688 rer.block.iframembed-1.0.3/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)      740 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.923367 rer.block.iframembed-1.0.3/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7923 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       83 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       42 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      518 2024-04-04 14:44:47.930981 rer.block.iframembed-1.0.3/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2443 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.920041 rer.block.iframembed-1.0.3/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.923496 rer.block.iframembed-1.0.3/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.924669 rer.block.iframembed-1.0.3/src/rer/block/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.925397 rer.block.iframembed-1.0.3/src/rer/block/iframembed/
+-rw-r--r--   0 cekk       (501) staff       (20)      137 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.925845 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      883 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      486 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.925995 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/overrides/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.926123 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/static/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     1261 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.926638 rer.block.iframembed-1.0.3/src/rer/block/iframembed/interfaces/
+-rw-r--r--   0 cekk       (501) staff       (20)      296 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/interfaces/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      268 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/interfaces/layer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      712 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/interfaces/settings.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.927330 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.920681 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.927623 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/en/LC_MESSAGES/rer.block.iframembed.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1566 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/en/LC_MESSAGES/rer.block.iframembed.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.920797 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.927888 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1133 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1867 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1689 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/rer.block.iframembed.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1587 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      497 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      260 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.921049 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.928519 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      185 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      590 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      182 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.928643 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      275 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.928772 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.929015 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      233 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.929388 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/deserializers/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/deserializers/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2780 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/deserializers/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      423 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/deserializers/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.929628 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      148 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.930018 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/controlpanel/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/controlpanel/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      665 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/controlpanel/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)      400 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/controlpanel/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      621 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1523 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.930375 rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.930500 rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     2011 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)      905 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/test_robot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2496 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-04 14:44:47.924537 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     2251 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2942 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      125 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       14 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      173 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     3563 2024-04-04 14:44:47.000000 rer.block.iframembed-1.0.3/tox.ini
```

### Comparing `rer.block.iframembed-1.0.2/DEVELOP.rst` & `rer.block.iframembed-1.0.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/LICENSE.GPL` & `rer.block.iframembed-1.0.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/LICENSE.rst` & `rer.block.iframembed-1.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/PKG-INFO` & `rer.block.iframembed-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.block.iframembed
-Version: 1.0.2
+Version: 1.0.3
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/rer.block.iframembed
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.block.iframembed
 Project-URL: Source, https://github.com/RegioneER/rer.block.iframembed
@@ -79,14 +79,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.3 (2024-04-04)
+------------------
+
+- Use env variable "disable_iframe_domains" to force disable validation.
+  [cekk]
+
+
 1.0.2 (2024-03-27)
 ------------------
 
 - If no domains are set, everything is invalid.
   [cekk]
```

### Comparing `rer.block.iframembed-1.0.2/README.rst` & `rer.block.iframembed-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/docs/conf.py` & `rer.block.iframembed-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/setup.cfg` & `rer.block.iframembed-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/setup.py` & `rer.block.iframembed-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.block.iframembed",
-    version="1.0.2",
+    version="1.0.3",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/browser/configure.zcml` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/configure.zcml` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/interfaces/settings.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/README.rst` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/en/LC_MESSAGES/rer.block.iframembed.po` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/en/LC_MESSAGES/rer.block.iframembed.po`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.mo` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.mo`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.po` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/it/LC_MESSAGES/rer.block.iframembed.po`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/rer.block.iframembed.pot` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/rer.block.iframembed.pot`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/locales/update.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/profiles/default/controlpanel.xml` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/deserializers/blocks.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/deserializers/blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     )
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def is_allowed_url(self, url):
+        disabled = os.environ.get("disable_iframe_domains", "False").lower() in (
+            "1",
+            "true",
+        )
+        if disabled:
+            return True
         valid_domains = api.portal.get_registry_record(
             "available_domains", interface=IRerBlockIframembedSettings
         )
         if not valid_domains:
             return False
         for domain in valid_domains:
             if url.startswith(domain):
@@ -42,15 +48,14 @@
         if not self.is_allowed_url(block.get("iframe_href", "")):
             raise BadRequest(api.portal.translate(self.msg))
         return block
 
 
 class HTMLBlockDeserializerBase(DeserializerBase):
     block_type = "html"
-    disabled = os.environ.get("disable_transform_html", False)
 
     def __call__(self, block):
         portal_transforms = api.portal.get_tool(name="portal_transforms")
         html_text = block.get("html", "")
 
         doc = lxml.html.fromstring(html_text)
         if doc.xpath("//iframe"):
```

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/restapi/services/controlpanel/adapters.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/restapi/services/controlpanel/adapters.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/setuphandlers.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/testing.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/testing.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/robot/test_example.robot` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/test_robot.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer/block/iframembed/tests/test_setup.py` & `rer.block.iframembed-1.0.3/src/rer/block/iframembed/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/PKG-INFO` & `rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.block.iframembed
-Version: 1.0.2
+Version: 1.0.3
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/rer.block.iframembed
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.block.iframembed
 Project-URL: Source, https://github.com/RegioneER/rer.block.iframembed
@@ -79,14 +79,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.3 (2024-04-04)
+------------------
+
+- Use env variable "disable_iframe_domains" to force disable validation.
+  [cekk]
+
+
 1.0.2 (2024-03-27)
 ------------------
 
 - If no domains are set, everything is invalid.
   [cekk]
```

### Comparing `rer.block.iframembed-1.0.2/src/rer.block.iframembed.egg-info/SOURCES.txt` & `rer.block.iframembed-1.0.3/src/rer.block.iframembed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rer.block.iframembed-1.0.2/tox.ini` & `rer.block.iframembed-1.0.3/tox.ini`

 * *Files identical despite different names*

