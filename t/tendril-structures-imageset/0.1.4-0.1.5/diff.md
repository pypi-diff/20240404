# Comparing `tmp/tendril-structures-imageset-0.1.4.tar.gz` & `tmp/tendril-structures-imageset-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-structures-imageset-0.1.4.tar", last modified: Thu Apr  4 06:06:00 2024, max compression
+gzip compressed data, was "tendril-structures-imageset-0.1.5.tar", last modified: Thu Apr  4 14:17:37 2024, max compression
```

## Comparing `tendril-structures-imageset-0.1.4.tar` & `tendril-structures-imageset-0.1.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2384 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-imageset-0.1.4/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13484 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      911 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1608 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3284 2024-04-03 16:32:06.000000 tendril-structures-imageset-0.1.4/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.028524 tendril-structures-imageset-0.1.4/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-imageset-0.1.4/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-imageset-0.1.4/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-imageset-0.1.4/src/tendril/apiserver/routers/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-imageset-0.1.4/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11993 2024-04-04 06:05:41.000000 tendril-structures-imageset-0.1.4/src/tendril/apiserver/templates/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-imageset-0.1.4/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/common/imageset/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-imageset-0.1.4/src/tendril/common/imageset/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1134 2024-04-03 12:57:25.000000 tendril-structures-imageset-0.1.4/src/tendril/common/imageset/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-imageset-0.1.4/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2714 2024-04-03 12:14:02.000000 tendril-structures-imageset-0.1.4/src/tendril/config/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.4/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-imageset-0.1.4/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4551 2024-04-03 09:27:40.000000 tendril-structures-imageset-0.1.4/src/tendril/db/controllers/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.4/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1979 2024-04-03 16:24:17.000000 tendril-structures-imageset-0.1.4/src/tendril/db/models/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-imageset-0.1.4/src/tendril/interests/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.4/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11883 2024-04-03 16:26:18.000000 tendril-structures-imageset-0.1.4/src/tendril/interests/mixins/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-imageset-0.1.4/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.4/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      298 2024-04-03 12:26:14.000000 tendril-structures-imageset-0.1.4/src/tendril/libraries/mixins/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/structures/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-imageset-0.1.4/src/tendril/structures/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril/structures/imageset/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 07:07:26.000000 tendril-structures-imageset-0.1.4/src/tendril/structures/imageset/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-04 06:05:59.000000 tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1570 2024-04-04 06:05:59.000000 tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-04 06:05:59.000000 tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-04 06:05:59.000000 tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-04 06:05:59.000000 tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 06:06:00.032524 tendril-structures-imageset-0.1.4/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.4/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2384 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-imageset-0.1.5/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13484 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      911 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1608 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3284 2024-04-03 16:32:06.000000 tendril-structures-imageset-0.1.5/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.223902 tendril-structures-imageset-0.1.5/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-imageset-0.1.5/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-imageset-0.1.5/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-imageset-0.1.5/src/tendril/apiserver/routers/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-imageset-0.1.5/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11993 2024-04-04 06:05:41.000000 tendril-structures-imageset-0.1.5/src/tendril/apiserver/templates/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-imageset-0.1.5/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/common/imageset/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-imageset-0.1.5/src/tendril/common/imageset/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1134 2024-04-03 12:57:25.000000 tendril-structures-imageset-0.1.5/src/tendril/common/imageset/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-imageset-0.1.5/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2714 2024-04-03 12:14:02.000000 tendril-structures-imageset-0.1.5/src/tendril/config/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.5/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.227902 tendril-structures-imageset-0.1.5/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-imageset-0.1.5/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4551 2024-04-03 09:27:40.000000 tendril-structures-imageset-0.1.5/src/tendril/db/controllers/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.5/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1979 2024-04-03 16:24:17.000000 tendril-structures-imageset-0.1.5/src/tendril/db/models/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-imageset-0.1.5/src/tendril/interests/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.5/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11900 2024-04-04 14:13:42.000000 tendril-structures-imageset-0.1.5/src/tendril/interests/mixins/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-imageset-0.1.5/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.5/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      298 2024-04-03 12:26:14.000000 tendril-structures-imageset-0.1.5/src/tendril/libraries/mixins/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/structures/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-imageset-0.1.5/src/tendril/structures/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril/structures/imageset/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 07:07:26.000000 tendril-structures-imageset-0.1.5/src/tendril/structures/imageset/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-04 14:17:37.000000 tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1570 2024-04-04 14:17:37.000000 tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-04 14:17:37.000000 tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-04 14:17:37.000000 tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-04 14:17:37.000000 tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-04 14:17:37.231902 tendril-structures-imageset-0.1.5/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.5/tox.ini
```

### Comparing `tendril-structures-imageset-0.1.4/.gitignore` & `tendril-structures-imageset-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/.readthedocs.yml` & `tendril-structures-imageset-0.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/.travis.yml` & `tendril-structures-imageset-0.1.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/LICENSE` & `tendril-structures-imageset-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/PKG-INFO` & `tendril-structures-imageset-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-imageset
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple image set structure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-imageset
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-imageset.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-imageset/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-imageset
```

### Comparing `tendril-structures-imageset-0.1.4/README.rst` & `tendril-structures-imageset-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/Makefile` & `tendril-structures-imageset-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/_static/custom.css` & `tendril-structures-imageset-0.1.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/_static/favicon.ico` & `tendril-structures-imageset-0.1.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/_static/logo.png` & `tendril-structures-imageset-0.1.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/_static/logo_packed.png` & `tendril-structures-imageset-0.1.5/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/_templates/about.html` & `tendril-structures-imageset-0.1.5/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/conf.py` & `tendril-structures-imageset-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/index.rst` & `tendril-structures-imageset-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/docs/installation.rst` & `tendril-structures-imageset-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/setup.py` & `tendril-structures-imageset-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/apiserver/templates/imageset.py` & `tendril-structures-imageset-0.1.5/src/tendril/apiserver/templates/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/common/imageset/exceptions.py` & `tendril-structures-imageset-0.1.5/src/tendril/common/imageset/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/config/__init__.py` & `tendril-structures-imageset-0.1.5/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/config/imageset.py` & `tendril-structures-imageset-0.1.5/src/tendril/config/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/db/controllers/imageset.py` & `tendril-structures-imageset-0.1.5/src/tendril/db/controllers/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/db/models/imageset.py` & `tendril-structures-imageset-0.1.5/src/tendril/db/models/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril/interests/mixins/imageset.py` & `tendril-structures-imageset-0.1.5/src/tendril/interests/mixins/imageset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from httpx import HTTPStatusError
 
 from tendril.filestore import buckets
 from tendril.config import IMAGESET_UPLOAD_FILESTORE_BUCKET
 from tendril.config import IMAGESET_PUBLISHING_FILESTORE_BUCKET
 
-from tendril.interests.base import InterestBase
+from tendril.interests.mixins.base import InterestMixinBase
 from tendril.common.states import LifecycleStatus
 from tendril.authz.roles.interests import require_state
 from tendril.authz.roles.interests import require_permission
 
 from tendril.caching import tokens
 from tendril.caching.tokens import TokenStatus
 
@@ -27,15 +27,15 @@
 from tendril.utils.parsers.media.info import get_media_info
 
 from tendril.utils.db import with_db
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
-class InterestImageSetMixin(InterestBase):
+class InterestImageSetMixin(InterestMixinBase):
     token_namespace = 'isu'
     upload_bucket_name = IMAGESET_UPLOAD_FILESTORE_BUCKET
     publish_bucket_name = IMAGESET_PUBLISHING_FILESTORE_BUCKET
     additional_export_fields = ['imageset']
 
     def __init__(self, *args, **kwargs):
         super(InterestImageSetMixin, self).__init__(*args, **kwargs)
```

### Comparing `tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/PKG-INFO` & `tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-imageset
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple image set structure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-imageset
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-imageset.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-imageset/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-imageset
```

### Comparing `tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/SOURCES.txt` & `tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/src/tendril_structures_imageset.egg-info/requires.txt` & `tendril-structures-imageset-0.1.5/src/tendril_structures_imageset.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/tests/coveralls.py` & `tendril-structures-imageset-0.1.5/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.4/tox.ini` & `tendril-structures-imageset-0.1.5/tox.ini`

 * *Files identical despite different names*
