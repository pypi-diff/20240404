# Comparing `tmp/imio.webspellchecker-1.0b5.tar.gz` & `tmp/imio.webspellchecker-1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.webspellchecker-1.0b5.tar", last modified: Fri Mar 29 14:08:50 2024, max compression
+gzip compressed data, was "imio.webspellchecker-1.0b6.tar", last modified: Thu Apr  4 12:49:42 2024, max compression
```

## Comparing `imio.webspellchecker-1.0b5.tar` & `imio.webspellchecker-1.0b6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/
--rw-rw-r--   0 adu       (1000) adu       (1000)      751 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/CHANGES.md
--rw-rw-r--   0 adu       (1000) adu       (1000)       49 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/CONTRIBUTORS.md
--rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/LICENSE.GPL
--rw-rw-r--   0 adu       (1000) adu       (1000)      655 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/LICENSE.md
--rw-rw-r--   0 adu       (1000) adu       (1000)       60 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/MANIFEST.in
--rw-rw-r--   0 adu       (1000) adu       (1000)     4276 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)     2231 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/README.md
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.531714 imio.webspellchecker-1.0b5/docs/
--rw-rw-r--   0 adu       (1000) adu       (1000)     7909 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/docs/conf.py
--rw-rw-r--   0 adu       (1000) adu       (1000)       83 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/docs/index.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)      321 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/setup.cfg
--rw-rw-r--   0 adu       (1000) adu       (1000)     2181 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/setup.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.511714 imio.webspellchecker-1.0b5/src/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.531714 imio.webspellchecker-1.0b5/src/imio/
--rw-rw-r--   0 adu       (1000) adu       (1000)       80 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.535714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/
--rw-rw-r--   0 adu       (1000) adu       (1000)      137 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.535714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1420 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     5144 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/controlpanel.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.535714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/
--rw-rw-r--   0 adu       (1000) adu       (1000)      608 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/controlpanel-icon.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      626 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     2587 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/plone_spinner.svg
--rw-rw-r--   0 adu       (1000) adu       (1000)     5890 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/wsctheme.css
--rw-rw-r--   0 adu       (1000) adu       (1000)     1781 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/viewlet.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2474 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/webspellchecker.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1028 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      417 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/interfaces.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.535714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/
--rw-rw-r--   0 adu       (1000) adu       (1000)      611 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/README.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.511714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/en/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.535714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/en/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3725 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.511714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/fr/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5838 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3900 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/imio.webspellchecker.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)     1756 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/update.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      497 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/update.sh
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.511714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/base/
--rw-rw-r--   0 adu       (1000) adu       (1000)      186 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/base/browserlayer.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)       88 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/base/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      573 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/base/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone4/
--rw-rw-r--   0 adu       (1000) adu       (1000)      682 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone4/controlpanel.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      339 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone4/cssregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone4/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      240 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone4/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone6/
--rw-rw-r--   0 adu       (1000) adu       (1000)      679 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone6/controlpanel.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone6/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      544 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone6/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/testing/
--rw-rw-r--   0 adu       (1000) adu       (1000)      189 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/testing/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      726 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/testing/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/uninstall/
--rw-rw-r--   0 adu       (1000) adu       (1000)      112 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1430 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      661 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/setuphandlers.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1913 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/testing.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      445 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/testing.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.539714 imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/
--rw-rw-r--   0 adu       (1000) adu       (1000)      745 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2789 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/test_setup.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     6504 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/test_view.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      212 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/upgrades.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      389 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/upgrades.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      738 2024-03-29 14:08:49.000000 imio.webspellchecker-1.0b5/src/imio/webspellchecker/vocabularies.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-03-29 14:08:50.531714 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/
--rw-rw-r--   0 adu       (1000) adu       (1000)     4276 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)     2626 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)      145 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/entry_points.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/namespace_packages.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/not-zip-safe
--rw-rw-r--   0 adu       (1000) adu       (1000)      131 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/requires.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-03-29 14:08:50.000000 imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/top_level.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      826 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/CHANGES.md
+-rw-rw-r--   0 adu       (1000) adu       (1000)       49 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/CONTRIBUTORS.md
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/LICENSE.GPL
+-rw-rw-r--   0 adu       (1000) adu       (1000)      655 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/LICENSE.md
+-rw-rw-r--   0 adu       (1000) adu       (1000)       60 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/MANIFEST.in
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4351 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2231 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/README.md
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/docs/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7909 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/docs/conf.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)       83 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/docs/index.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)      321 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/setup.cfg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2181 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/setup.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       80 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      137 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1420 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5144 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/controlpanel.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      608 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/controlpanel-icon.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      626 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2587 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/plone_spinner.svg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5890 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/wsctheme.css
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1841 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/viewlet.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2474 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/webspellchecker.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1028 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      417 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/interfaces.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      611 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/README.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3725 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5838 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3900 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/imio.webspellchecker.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1756 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/update.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      497 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/update.sh
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      186 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/browserlayer.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)       88 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      573 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      682 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/controlpanel.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      339 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/cssregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      240 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      679 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/controlpanel.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      544 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      189 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      726 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/uninstall/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      112 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1430 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      661 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/setuphandlers.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1913 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/testing.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      445 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/testing.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      745 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2789 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_setup.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     6504 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_view.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      212 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/upgrades.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      389 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/upgrades.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      738 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/vocabularies.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4351 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2626 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)      145 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/entry_points.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/namespace_packages.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/not-zip-safe
+-rw-rw-r--   0 adu       (1000) adu       (1000)      131 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/requires.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/top_level.txt
```

### Comparing `imio.webspellchecker-1.0b5/CHANGES.md` & `imio.webspellchecker-1.0b6/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 
-1.0b5 (2024-03-29)
+1.0b6 (2024-04-04)
+
+- Use proper type on the script tags.
+  [aduchene]
+
+## 1.0b5 (2024-03-29)
 
 - Use unicode for default values.
   [aduchene]
 
 
 ## 1.0b4 (2024-03-28)
```

### Comparing `imio.webspellchecker-1.0b5/LICENSE.GPL` & `imio.webspellchecker-1.0b6/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/LICENSE.md` & `imio.webspellchecker-1.0b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/PKG-INFO` & `imio.webspellchecker-1.0b6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.webspellchecker
-Version: 1.0b5
+Version: 1.0b6
 Summary: Integration of Webspellchecker's WProofReader with Plone, providing real-time spellchecking for various WYSIWYG editors.
 Home-page: https://github.com/collective/imio.webspellchecker
 Author: iMio
 Author-email: antoine.duchene@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.webspellchecker
 Project-URL: Source, https://github.com/imio/imio.webspellchecker
@@ -89,15 +89,20 @@
 
 - Antoine Duchêne, (iMio, scrl)
 
 
 # Changelog
 
 
-1.0b5 (2024-03-29)
+1.0b6 (2024-04-04)
+
+- Use proper type on the script tags.
+  [aduchene]
+
+## 1.0b5 (2024-03-29)
 
 - Use unicode for default values.
   [aduchene]
 
 
 ## 1.0b4 (2024-03-28)
```

### Comparing `imio.webspellchecker-1.0b5/README.md` & `imio.webspellchecker-1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/docs/conf.py` & `imio.webspellchecker-1.0b6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/setup.py` & `imio.webspellchecker-1.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.md").read(),
     ]
 )
 
 
 setup(
     name="imio.webspellchecker",
-    version="1.0b5",
+    version="1.0b6",
     description="Integration of Webspellchecker's WProofReader with Plone, "
     "providing real-time spellchecking for various WYSIWYG editors.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/configure.zcml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/controlpanel.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/controlpanel-icon.png` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/controlpanel-icon.png`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/plone_spinner.svg` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/plone_spinner.svg`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/static/wsctheme.css` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/wsctheme.css`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/viewlet.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/viewlet.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from plone import api
 from plone.app.layout.viewlets import ViewletBase
 from plone.registry.interfaces import IRegistry
 from zope.component import getUtility
 
 
 WSC_SCRIPTS_TEMPLATE = """
-<script src="{plonesite}/wscinit.js?t={timestamp}"></script>
-<script crossorigin="anonymous" src="{bundle}?t={timestamp}"></script>
+<script type="application/javascript" src="{plonesite}/wscinit.js?t={timestamp}"></script>
+<script type="application/javascript" crossorigin="anonymous" src="{bundle}?t={timestamp}"></script>
 """
 
 
 class WscJsViewlet(ViewletBase):
     def is_allowed_portal_type(self, settings):
         """
         Check if the portal type of the current context is allowed.
```

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/browser/webspellchecker.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/webspellchecker.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/configure.zcml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/README.rst` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/README.rst`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/imio.webspellchecker.pot` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/imio.webspellchecker.pot`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/locales/update.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/update.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/base/registry.xml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone4/controlpanel.xml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone6/controlpanel.xml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/plone6/registry.xml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles/testing/registry.xml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/profiles.zcml` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/setuphandlers.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/testing.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/testing.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/__init__.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/test_setup.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/tests/test_view.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio/webspellchecker/vocabularies.py` & `imio.webspellchecker-1.0b6/src/imio/webspellchecker/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/PKG-INFO` & `imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.webspellchecker
-Version: 1.0b5
+Version: 1.0b6
 Summary: Integration of Webspellchecker's WProofReader with Plone, providing real-time spellchecking for various WYSIWYG editors.
 Home-page: https://github.com/collective/imio.webspellchecker
 Author: iMio
 Author-email: antoine.duchene@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.webspellchecker
 Project-URL: Source, https://github.com/imio/imio.webspellchecker
@@ -89,15 +89,20 @@
 
 - Antoine Duchêne, (iMio, scrl)
 
 
 # Changelog
 
 
-1.0b5 (2024-03-29)
+1.0b6 (2024-04-04)
+
+- Use proper type on the script tags.
+  [aduchene]
+
+## 1.0b5 (2024-03-29)
 
 - Use unicode for default values.
   [aduchene]
 
 
 ## 1.0b4 (2024-03-28)
```

### Comparing `imio.webspellchecker-1.0b5/src/imio.webspellchecker.egg-info/SOURCES.txt` & `imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

