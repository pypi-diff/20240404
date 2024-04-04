# Comparing `tmp/pubtools-pulplib-2.8.0.tar.gz` & `tmp/pubtools-pulplib-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pubtools-pulplib-2.8.0.tar", last modified: Wed Mar 17 12:11:46 2021, max compression
+gzip compressed data, was "dist/pubtools-pulplib-2.9.0.tar", last modified: Tue Jun 15 11:58:52 2021, max compression
```

## Comparing `pubtools-pulplib-2.8.0.tar` & `pubtools-pulplib-2.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/tests/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2879 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/tests/model/test_model_assertions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/tests/model/test_model_invariants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/tests/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4289 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/tests/model/assertions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3425 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2069 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3425 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      619 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7535 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/maintenance.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/yum.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16910 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1792 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/container.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      225 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4277 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6225 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/task.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/convert.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4868 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3324 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/rpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1810 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/modulemd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/modulemd_defaults.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      242 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1520 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2679 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/distributor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      505 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2009 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/attr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1116 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/frozenlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9446 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/criteria.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2607 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/retry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7042 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23300 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7384 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/repository.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/unit.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2101 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/task.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/maintenance.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:46.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5193 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/match.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14159 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5336 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4104 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/page.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/compat_attr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7788 2021-03-17 12:11:02.000000 pubtools-pulplib-2.8.0/CHANGELOG.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/tests/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/tests/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2879 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/tests/model/test_model_assertions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/tests/model/test_model_invariants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/tests/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4289 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/tests/model/assertions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2916 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2069 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2916 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      619 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7535 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/maintenance.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4877 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/yum.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17067 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1792 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/container.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      225 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4277 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6225 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/task.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/convert.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4868 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3324 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/rpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2905 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/modulemd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/modulemd_defaults.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      242 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1520 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2679 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/distributor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      505 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2009 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/attr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1116 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/frozenlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9446 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/criteria.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      777 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2607 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/retry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7042 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/search.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23300 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7384 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3201 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/repository.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3688 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/unit.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2101 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/task.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/maintenance.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:52.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5193 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/match.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14159 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5336 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/controller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       39 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4104 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/page.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/compat_attr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8128 2021-06-15 11:58:07.000000 pubtools-pulplib-2.9.0/CHANGELOG.md
```

### Comparing `pubtools-pulplib-2.8.0/setup.py` & `pubtools-pulplib-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_requirements():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="pubtools-pulplib",
-    version="2.8.0",
+    version="2.9.0",
     packages=find_packages(exclude=["tests"]),
     package_data={"pubtools.pulplib._impl.schema": ["*.yaml"]},
     url="https://github.com/release-engineering/pubtools-pulplib",
     license="GNU General Public License",
     description=get_description(),
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
```

### Comparing `pubtools-pulplib-2.8.0/tests/model/test_model_assertions.py` & `pubtools-pulplib-2.9.0/tests/model/test_model_assertions.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/tests/model/test_model_invariants.py` & `pubtools-pulplib-2.9.0/tests/model/test_model_invariants.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/tests/model/assertions.py` & `pubtools-pulplib-2.9.0/tests/model/assertions.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/PKG-INFO` & `pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 Metadata-Version: 2.1
 Name: pubtools-pulplib
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Pulp library for publishing tools
 Home-page: https://github.com/release-engineering/pubtools-pulplib
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-pulplib/
 Project-URL: Changelog, https://github.com/release-engineering/pubtools-pulplib/blob/master/CHANGELOG.md
-Description: 
-        
-        A Python client for [Pulp 2.x](https://pulpproject.org/), used by
-        [release-engineering](https://github.com/release-engineering) publishing tools.
-        
-        [![Build Status](https://travis-ci.org/release-engineering/pubtools-pulplib.svg?branch=master)](https://travis-ci.org/release-engineering/pubtools-pulplib)
-        [![Coverage Status](https://coveralls.io/repos/github/release-engineering/pubtools-pulplib/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/pubtools-pulplib?branch=master)
-        
-        - [Source](https://github.com/release-engineering/pubtools-pulplib)
-        - [Documentation](https://release-engineering.github.io/pubtools-pulplib/)
-        - [PyPI](https://pypi.org/project/pubtools-pulplib)
-        
-        
-        Installation
-        ------------
-        
-        Install the `pubtools-pulplib` package from PyPI.
-        
-        ```
-        pip install pubtools-pulplib
-        ```
-        
-        
-        Usage Example
-        -------------
-        
-        ```python
-        from pubtools.pulplib import Client
-        
-        # Make a client pointing at this Pulp server
-        client = Client(url='https://pulp.example.com/', auth=('admin', 'some-password'))
-        
-        # Get a particular repo by ID.
-        # All methods return Future instances; .result() blocks
-        repo = client.get_repository('zoo').result()
-        
-        # Pulp objects have relevant methods, e.g. publish().
-        # Returned future may encapsulate one or more Pulp tasks.
-        publish = repo.publish().result()
-        ```
-        
-        Development
-        -----------
-        
-        Patches may be contributed via pull requests to
-        https://github.com/release-engineering/pubtools-pulplib.
-        
-        All changes must pass the automated test suite, along with various static
-        checks.
-        
-        The [Black](https://black.readthedocs.io/) code style is enforced.
-        Enabling autoformatting via a pre-commit hook is recommended:
-        
-        ```
-        pip install -r requirements-dev.txt
-        pre-commit install
-        ```
-        
-        License
-        -------
-        
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU General Public License as published by
-        the Free Software Foundation, either version 3 of the License, or
-        (at your option) any later version.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+A Python client for [Pulp 2.x](https://pulpproject.org/), used by
+[release-engineering](https://github.com/release-engineering) publishing tools.
+
+[![Build Status](https://travis-ci.org/release-engineering/pubtools-pulplib.svg?branch=master)](https://travis-ci.org/release-engineering/pubtools-pulplib)
+[![Coverage Status](https://coveralls.io/repos/github/release-engineering/pubtools-pulplib/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/pubtools-pulplib?branch=master)
+
+- [Source](https://github.com/release-engineering/pubtools-pulplib)
+- [Documentation](https://release-engineering.github.io/pubtools-pulplib/)
+- [PyPI](https://pypi.org/project/pubtools-pulplib)
+
+
+Installation
+------------
+
+Install the `pubtools-pulplib` package from PyPI.
+
+```
+pip install pubtools-pulplib
+```
+
+
+Usage Example
+-------------
+
+```python
+from pubtools.pulplib import Client
+
+# Make a client pointing at this Pulp server
+client = Client(url='https://pulp.example.com/', auth=('admin', 'some-password'))
+
+# Get a particular repo by ID.
+# All methods return Future instances; .result() blocks
+repo = client.get_repository('zoo').result()
+
+# Pulp objects have relevant methods, e.g. publish().
+# Returned future may encapsulate one or more Pulp tasks.
+publish = repo.publish().result()
+```
+
+Development
+-----------
+
+Patches may be contributed via pull requests to
+https://github.com/release-engineering/pubtools-pulplib.
+
+All changes must pass the automated test suite, along with various static
+checks.
+
+The [Black](https://black.readthedocs.io/) code style is enforced.
+Enabling autoformatting via a pre-commit hook is recommended:
+
+```
+pip install -r requirements-dev.txt
+pre-commit install
+```
+
+License
+-------
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+
```

### Comparing `pubtools-pulplib-2.8.0/pubtools_pulplib.egg-info/SOURCES.txt` & `pubtools-pulplib-2.9.0/pubtools_pulplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/PKG-INFO` & `pubtools-pulplib-2.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 Metadata-Version: 2.1
 Name: pubtools-pulplib
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Pulp library for publishing tools
 Home-page: https://github.com/release-engineering/pubtools-pulplib
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-pulplib/
 Project-URL: Changelog, https://github.com/release-engineering/pubtools-pulplib/blob/master/CHANGELOG.md
-Description: 
-        
-        A Python client for [Pulp 2.x](https://pulpproject.org/), used by
-        [release-engineering](https://github.com/release-engineering) publishing tools.
-        
-        [![Build Status](https://travis-ci.org/release-engineering/pubtools-pulplib.svg?branch=master)](https://travis-ci.org/release-engineering/pubtools-pulplib)
-        [![Coverage Status](https://coveralls.io/repos/github/release-engineering/pubtools-pulplib/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/pubtools-pulplib?branch=master)
-        
-        - [Source](https://github.com/release-engineering/pubtools-pulplib)
-        - [Documentation](https://release-engineering.github.io/pubtools-pulplib/)
-        - [PyPI](https://pypi.org/project/pubtools-pulplib)
-        
-        
-        Installation
-        ------------
-        
-        Install the `pubtools-pulplib` package from PyPI.
-        
-        ```
-        pip install pubtools-pulplib
-        ```
-        
-        
-        Usage Example
-        -------------
-        
-        ```python
-        from pubtools.pulplib import Client
-        
-        # Make a client pointing at this Pulp server
-        client = Client(url='https://pulp.example.com/', auth=('admin', 'some-password'))
-        
-        # Get a particular repo by ID.
-        # All methods return Future instances; .result() blocks
-        repo = client.get_repository('zoo').result()
-        
-        # Pulp objects have relevant methods, e.g. publish().
-        # Returned future may encapsulate one or more Pulp tasks.
-        publish = repo.publish().result()
-        ```
-        
-        Development
-        -----------
-        
-        Patches may be contributed via pull requests to
-        https://github.com/release-engineering/pubtools-pulplib.
-        
-        All changes must pass the automated test suite, along with various static
-        checks.
-        
-        The [Black](https://black.readthedocs.io/) code style is enforced.
-        Enabling autoformatting via a pre-commit hook is recommended:
-        
-        ```
-        pip install -r requirements-dev.txt
-        pre-commit install
-        ```
-        
-        License
-        -------
-        
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU General Public License as published by
-        the Free Software Foundation, either version 3 of the License, or
-        (at your option) any later version.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+A Python client for [Pulp 2.x](https://pulpproject.org/), used by
+[release-engineering](https://github.com/release-engineering) publishing tools.
+
+[![Build Status](https://travis-ci.org/release-engineering/pubtools-pulplib.svg?branch=master)](https://travis-ci.org/release-engineering/pubtools-pulplib)
+[![Coverage Status](https://coveralls.io/repos/github/release-engineering/pubtools-pulplib/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/pubtools-pulplib?branch=master)
+
+- [Source](https://github.com/release-engineering/pubtools-pulplib)
+- [Documentation](https://release-engineering.github.io/pubtools-pulplib/)
+- [PyPI](https://pypi.org/project/pubtools-pulplib)
+
+
+Installation
+------------
+
+Install the `pubtools-pulplib` package from PyPI.
+
+```
+pip install pubtools-pulplib
+```
+
+
+Usage Example
+-------------
+
+```python
+from pubtools.pulplib import Client
+
+# Make a client pointing at this Pulp server
+client = Client(url='https://pulp.example.com/', auth=('admin', 'some-password'))
+
+# Get a particular repo by ID.
+# All methods return Future instances; .result() blocks
+repo = client.get_repository('zoo').result()
+
+# Pulp objects have relevant methods, e.g. publish().
+# Returned future may encapsulate one or more Pulp tasks.
+publish = repo.publish().result()
+```
+
+Development
+-----------
+
+Patches may be contributed via pull requests to
+https://github.com/release-engineering/pubtools-pulplib.
+
+All changes must pass the automated test suite, along with various static
+checks.
+
+The [Black](https://black.readthedocs.io/) code style is enforced.
+Enabling autoformatting via a pre-commit hook is recommended:
+
+```
+pip install -r requirements-dev.txt
+pre-commit install
+```
+
+License
+-------
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+
```

### Comparing `pubtools-pulplib-2.8.0/LICENSE` & `pubtools-pulplib-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/README.md` & `pubtools-pulplib-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/__init__.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/__init__.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/maintenance.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/maintenance.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/base.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,17 @@
     """A list of GPG signing key IDs used to sign content in this repository."""
 
     skip_rsync_repodata = pulp_attrib(default=False, type=bool)
     """True if this repository is explicitly configured such that a publish of
     this repository will not publish repository metadata to remote hosts.
     """
 
+    content_set = pulp_attrib(default=None, type=str, pulp_field="notes.content_set")
+    """Name of content set that is associated with this repository"""
+
     @distributors.validator
     def _check_repo_id(self, _, value):
         # checks if distributor's repository id is same as the repository it
         # is attached to
         for distributor in value:
             if not distributor.repo_id:
                 return
```

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/container.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/container.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/repository/file.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/repository/file.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/task.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/task.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/convert.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/convert.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/common.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/common.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/rpm.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/rpm.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/base.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/base.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/modulemd.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/modulemd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from .base import Unit, unit_type
 
 from ..attr import pulp_attrib
 from ... import compat_attr as attr
 from ..frozenlist import frozenlist_or_none_converter
 
 
@@ -58,7 +60,39 @@
         converter=frozenlist_or_none_converter,
         pulp_field="repository_memberships",
     )
     """IDs of repositories containing the unit, or ``None`` if this information is unavailable.
 
     .. versionadded:: 2.6.0
     """
+    artifacts = pulp_attrib(
+        default=None,
+        type=list,
+        converter=frozenlist_or_none_converter,
+        pulp_field="artifacts",
+    )
+    """List of artifacts related to the given module, usually it's a list
+    rpms in nevra format without '.rpm' extension and consist of binary, debug and source
+    rpms as well.
+
+    Example:
+    ["perl-version-7:0.99.24-441.module+el8.3.0+6718+7f269185.src",
+     "perl-version-7:0.99.24-441.module+el8.3.0+6718+7f269185.x86_64",
+    ]
+    """
+
+    profiles = pulp_attrib(type=dict, pulp_field="profiles", default=None)
+    """The profiles of this modulemd unit."""
+
+    @property
+    def artifacts_filenames(self):
+        """
+        Artifacts are typically stored as a list of rpms of nevra format without '.rpm' extension,
+        this method removes the epoch and returns set of actual rpm filenames.
+        """
+        regex = r"\d+:"
+        reg = re.compile(regex)
+
+        out = set()
+        for rpm_nevra in self.artifacts or []:
+            out.add(reg.sub("", rpm_nevra, count=1) + ".rpm")
+        return out
```

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/modulemd_defaults.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/modulemd_defaults.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/unit/file.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/unit/file.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/distributor.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/distributor.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/attr.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/attr.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/model/frozenlist.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/model/frozenlist.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/criteria.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/criteria.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/util.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/util.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/errors.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/errors.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/retry.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/retry.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/search.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/search.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/client.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/client.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/client/poller.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/client/poller.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/repository.yaml` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/repository.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,22 @@
 
       # List of repositories used for populating the repository
       population_sources:
         type: array
         items:
           type: string
 
+      # Name of content set that is associated with this repository
+      content_set:
+        type: string
+
+      # Version of ubi config that should be used for population of this repository
+      ubi_config_version:
+        type: string
+
   # List of repository distributors.
   # Note that order matters in this list.
   distributors:
     type: array
     items:
       $ref: "#/definitions/distributor"
```

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/unit.yaml` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/unit.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -126,14 +126,22 @@
         type: string
 
       repository_memberships:
         type: array
         items:
           type: string
 
+      artifacts:
+        type: array
+        items:
+          type: string
+      
+      profiles:
+        type: object
+
     required:
     - _content_type_id
     - name
     - stream
     - version
     - context
     - arch
```

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/task.yaml` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/task.yaml`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/maintenance.yaml` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/maintenance.yaml`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/schema/__init__.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/match.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/match.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/client.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/client.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/fake/controller.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/fake/controller.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/page.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/page.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/pubtools/pulplib/_impl/compat_attr.py` & `pubtools-pulplib-2.9.0/pubtools/pulplib/_impl/compat_attr.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulplib-2.8.0/CHANGELOG.md` & `pubtools-pulplib-2.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-- n/a
+### n/a
+
+## [2.9.0] - 2021-06-15
+### Added
+- Support for various repo notes for Repository model
+- Support for various fields of ModuleMd unit
+- Introduced YumRepository.get_x_repository methods that can retrieve
+  related binary, debug and source repository
 
 ## [2.8.0] - 2021-03-17
 
 ### Added
 - Maximum number of queued or running Pulp tasks can be customized by callers
 
 ## [2.7.0] - 2020-06-11
@@ -197,15 +204,16 @@
 ### Fixed
 - Fixed missing schema files from distribution
 
 ## 0.1.0 - 2019-06-13
 
 - Initial release to PyPI
 
-[Unreleased]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.8.0...HEAD
+[Unreleased]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.9.0...HEAD
+[2.9.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.9.0...HEAD
 [2.8.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.7.0...v2.8.0
 [2.7.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.6.0...v2.7.0
 [2.6.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.5.0...v2.6.0
 [2.5.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.4.0...v2.5.0
 [2.4.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.3.1...v2.4.0
 [2.3.1]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.3.0...v2.3.1
 [2.3.0]: https://github.com/release-engineering/pubtools-pulplib/compare/v2.2.0...v2.3.0
```

